<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Mening Saytim</title>

<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Shriftlar -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;600;700;800&display=swap" rel="stylesheet">

<style>
  :root{
    --bg:#0a0a0b;
    --surface:rgba(255,255,255,0.03);
    --border:rgba(255,255,255,0.08);
    --text:#ffffff;
    --accent:#7C3AED;
  }

  body{
    background:
      radial-gradient(ellipse 80% 60% at 50% 0%, rgba(124,58,237,0.18), transparent 110%),
      var(--bg);
    color: var(--text);
    font-family:'Sora', system-ui, sans-serif;
    margin: 0;
    padding: 0;
    min-height:100vh;
    overflow-x:hidden;
  }

  .glass{
    background: var(--surface);
    border: 1px solid var(--border);
    backdrop-filter: blur(16px);
    -webkit-backdrop-filter: blur(16px);
  }

  .gradient-text{
    background: linear-gradient(135deg, #fff 0%, #A78BFA 60%, #7C3AED 100%);
    -webkit-background-clip:text;
    background-clip:text;
    -webkit-text-fill-color:transparent;
  }

  .btn-primary{
    background: linear-gradient(135deg, #7C3AED, #6D28D9);
    transition: all .25s ease;
  }
  .btn-primary:hover{
    transform: translateY(-2px);
    box-shadow: 0 8px 30px rgba(124,58,237,0.55);
  }
</style>
</head>

<body>

  <!-- NAVBAR -->
  <header class="sticky top-0 z-50 backdrop-blur-xl bg-[#0a0a0b]/70 border-b border-white/[0.06]">
    <nav class="max-w-[1320px] mx-auto px-6 h-[64px] flex items-center justify-between">
      <a href="#" class="flex items-center gap-2.5">
        <div class="w-9 h-9 rounded-[12px] bg-gradient-to-br from-[#7C3AED] to-[#3B82F6] grid place-items-center">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none"><path d="M13 2L3 14h7l-1 8 10-12h-7l1-8z" fill="#fff"/></svg>
        </div>
        <span class="text-[16px] font-bold">Mening Saytim</span>
      </a>
      <div class="hidden md:flex items-center gap-8 text-[14px] text-white/60">
        <a href="#features" class="hover:text-white transition">Imkoniyatlar</a>
        <a href="#pricing" class="hover:text-white transition">Narxlar</a>
      </div>
      <div class="flex items-center gap-3">
        <button class="btn-primary text-[14px] font-semibold px-4 py-2 rounded-[10px] text-white">Boshlash</button>
      </div>
    </nav>
  </header>

  <!-- HERO -->
  <main class="relative z-10">
    <section class="max-w-[1320px] mx-auto px-6 pt-20 pb-24 text-center">
      <h1 class="text-[42px] md:text-[64px] leading-[1.05] font-extrabold tracking-tighter max-w-[900px] mx-auto">
        <span class="gradient-text">Mukammal</span> mahsulotlar<br>yarating — <span class="gradient-text">tezroq</span>
      </h1>
      <p class="mt-6 text-[16px] md:text-[18px] text-white/60 leading-[1.7] max-w-[560px] mx-auto">
        Zamonaviy dizayn, kuchli funksiyalar va cheksiz imkoniyatlar bir joyda.
      </p>
      <div class="mt-10 flex flex-wrap items-center justify-center gap-4">
        <button class="btn-primary text-[15px] font-semibold px-6 h-[52px] rounded-[14px] text-white">Bepul boshlash</button>
      </div>
    </section>

    <!-- FEATURES -->
    <section id="features" class="max-w-[1320px] mx-auto px-6 py-20">
      <div class="grid md:grid-cols-3 gap-6">
        <div class="glass p-6 rounded-[20px]">
          <div class="w-12 h-12 rounded-[14px] bg-[#7C3AED]/15 grid place-items-center mb-5">
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#A78BFA" stroke-width="2"><path d="M13 2L3 14h7l-1 8 10-12h-7l1-8z"/></svg>
          </div>
          <h3 class="text-[18px] font-bold mb-2">Tezkor ishlash</h3>
          <p class="text-[14px] text-white/50">Eng zamonaviy texnologiyalar bilan qurilgan.</p>
        </div>
        <div class="glass p-6 rounded-[20px]">
          <div class="w-12 h-12 rounded-[14px] bg-[#3B82F6]/10 grid place-items-center mb-5">
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#60A5FA" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="3"/><path d="M9 9h6v6H9z"/></svg>
          </div>
          <h3 class="text-[18px] font-bold mb-2">Xavfsizlik</h3>
          <p class="text-[14px] text-white/50">Ma'lumotlaringiz to'liq himoyalangan holda saqlanadi.</p>
        </div>
        <div class="glass p-6 rounded-[20px]">
          <div class="w-12 h-12 rounded-[14px] bg-emerald-500/10 grid place-items-center mb-5">
            <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#34D399" stroke-width="2"><path d="M12 2v20M2 12h20"/></svg>
          </div>
          <h3 class="text-[18px] font-bold mb-2">Cheksiz imkoniyat</h3>
          <p class="text-[14px] text-white/50">Har qanday loyihaga moslasha oladigan platforma.</p>
        </div>
      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer class="border-t border-white/[0.06] mt-10 py-6 text-center text-white/40 text-[13px]">
    © 2026 Mening Saytim — Barcha huquqlar himoyalangan
  </footer>

</body>
</html>
