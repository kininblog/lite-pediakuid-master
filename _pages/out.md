---
layout: page
title: Out
description: 
permalink: /out.html
---
<div class="max-w-md mx-auto bg-white shadow rounded-lg p-6 text-center">
  <h1 class="text-2xl font-semibold mb-4 text-gray-800">Anda akan dialihkan</h1>
  <p class="text-gray-600 mb-6">Klik tombol di bawah setelah proses selesai.</p>
  <div id="countdown" class="text-4xl font-bold text-blue-600 mb-6">5</div>
  <button id="continue-btn" disabled
          class="w-full bg-gray-400 text-white font-semibold rounded px-4 py-2 cursor-not-allowed transition">
    Menunggu...
  </button>
</div>
<script>
  window.addEventListener('DOMContentLoaded', () => {
    const params = new URLSearchParams(window.location.search);
    const go = params.get('go');
    const countdownEl = document.getElementById('countdown');
    const btn = document.getElementById('continue-btn');

    if (!go) {
      countdownEl.textContent = '';
      btn.textContent = 'Error: parameter go tidak ditemukan';
      return;
    }

    let decoded;
    try {
      decoded = atob(decodeURIComponent(go));
    } catch {
      countdownEl.textContent = '';
      btn.textContent = 'Error: parameter go tidak valid';
      return;
    }

    let count = 5;
    const timer = setInterval(() => {
      count--;
      countdownEl.textContent = count;
      if (count <= 0) {
        clearInterval(timer);
        btn.disabled = false;
        btn.textContent = 'Lanjutkan';
        btn.classList.replace('bg-gray-400', 'bg-blue-600');
        btn.classList.replace('cursor-not-allowed', 'cursor-pointer');
        btn.addEventListener('click', () => {
          window.location.href = decoded;
        });
      }
    }, 1000);
  });
</script>
