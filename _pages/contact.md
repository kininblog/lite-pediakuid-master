---
layout: page
title: Contact Us
description: 
permalink: /contact/
---


  <div class="max-w-2xl mx-auto">
    <div class="bg-white py-8 px-6 shadow rounded-lg sm:px-10">
      <div class="mb-10 text-center">
        <h2 class="text-3xl font-extrabold text-gray-900">Hubungi Kami</h2>
        <p class="mt-2 text-gray-600">Isi form berikut dan kami akan segera membalas pesan Anda</p>
      </div>

      <form id="contactForm" class="space-y-6">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div>
            <label for="name" class="block text-sm font-medium text-gray-700">Nama Lengkap</label>
            <div class="mt-1">
              <input type="text" id="name" name="name" required 
                     class="w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all">
            </div>
          </div>

          <div>
            <label for="email" class="block text-sm font-medium text-gray-700">Alamat Email</label>
            <div class="mt-1">
              <input type="email" id="email" name="email" required 
                     class="w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all">
            </div>
          </div>
        </div>

        <div>
          <label for="subject" class="block text-sm font-medium text-gray-700">Subjek</label>
          <div class="mt-1">
            <input type="text" id="subject" name="subject" required 
                   class="w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all">
          </div>
        </div>

        <div>
          <label for="message" class="block text-sm font-medium text-gray-700">Pesan</label>
          <div class="mt-1">
            <textarea id="message" name="message" rows="4" required 
                      class="w-full px-4 py-2 border border-gray-300 rounded-md shadow-sm focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all"></textarea>
          </div>
        </div>

        <div>
          <button type="submit" 
                  class="w-full flex justify-center py-2 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition-all">
            Kirim Pesan
          </button>
        </div>
      </form>
    </div>
  </div>

  <script>
    document.getElementById('contactForm').addEventListener('submit', function(e) {
      e.preventDefault();
      
      const name = document.getElementById('name').value;
      const email = document.getElementById('email').value;
      const subject = document.getElementById('subject').value;
      const message = document.getElementById('message').value;
      
      const mailtoLink = `mailto:nandafransiska.mail@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(
        `Nama: ${name}\nEmail: ${email}\n\nPesan:\n${message}`
      )}`;
      
      window.location.href = mailtoLink;
      this.reset();
      
      // Tambahkan notifikasi pengiriman sukses
      alert('Pesan berhasil dikirim! Kami akan segera membalas ke email Anda.');
    });
  </script>
