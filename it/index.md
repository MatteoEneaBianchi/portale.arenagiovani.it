---
layout: login
title: Login
description: Ciao
lang: it
ref: homepage
permalink: /
order: 1
---

<style>
  <style>
    .centrato {text-align: center;}
  </style>
</style>
<div class="centrato"><h1><div id="clock">00:00:00</div></h1></div>


    <script>
        function updateClock() {
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            document.getElementById('clock').textContent = `${hours}:${minutes}:${seconds}`;
        }
        
        setInterval(updateClock, 1000);
        updateClock();
    </script>
