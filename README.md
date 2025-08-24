<!DOCTYPE html>
<html lang="km" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CHOMRONG • CV Website</title>
  <meta name="description" content="Perfect personal CV website for CHOMRONG — modern, responsive, fast." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet" />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          container: { center: true, padding: '1rem' },
          colors: {
            brand: {
              50: '#eff6ff', 100: '#dbeafe', 200: '#bfdbfe', 300: '#93c5fd', 400: '#60a5fa', 500: '#3b82f6',
              600: '#2563eb', 700: '#1d4ed8', 800: '#1e40af', 900: '#1e3a8a'
            },
          },
          boxShadow: { soft: '0 10px 30px rgba(0,0,0,0.08)' },
          keyframes: {
            fadeUp: { '0%': { opacity: 0, transform: 'translateY(20px)'}, '100%': { opacity: 1, transform: 'translateY(0)'} },
            shimmer: { '0%': { backgroundPosition: '-700px 0'}, '100%': { backgroundPosition: '700px 0'} }
          },
          animation: { fadeUp: 'fadeUp .8s ease-out forwards', shimmer: 'shimmer 1.4s linear infinite' }
        }
      },
      darkMode: 'class'
    }
  </script>
  <style>
    :root { --ring: 0 0 0 3px rgba(59,130,246,.35); }
    html, body { font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Arial, Noto Sans, 'Khmer OS Battambang', sans-serif; }
    .bar { height: 10px; border-radius: 9999px; background: rgba(0,0,0,.08); }
    .bar>span { display:block; height:100%; border-radius:9999px; background: linear-gradient(90deg,#3b82f6,#60a5fa); width:0; transition: width 1.2s ease; }
    .dark .bar{ background: rgba(255,255,255,.12);}
    .timeline:before { content: ""; position:absolute; left:0.875rem; top:0; bottom:0; width:2px; background: linear-gradient(#93c5fd,#3b82f6); opacity:.35; }
    .timeline-item { position:relative; padding-left:3rem; }
    .timeline-item:before { content:""; position:absolute; left:0.5rem; top:.35rem; width:10px; height:10px; background:#3b82f6; border:2px solid white; border-radius:9999px; box-shadow:0 0 0 3px rgba(59,130,246,.25); }
    .glass { background: rgba(255,255,255,.6); backdrop-filter: blur(8px); }
    .dark .glass { background: rgba(17,24,39,.5); }
    .shimmer { background: linear-gradient(90deg, rgba(0,0,0,.04) 25%, rgba(0,0,0,.08) 37%, rgba(0,0,0,.04) 63%); background-size: 1400px 100%; }
    .dark .shimmer { background: linear-gradient(90deg, rgba(255,255,255,.04) 25%, rgba(255,255,255,.08) 37%, rgba(255,255,255,.04) 63%); }
    ::-webkit-scrollbar { width: 10px; height: 10px; }
    ::-webkit-scrollbar-thumb { background: #9ca3af; border-radius: 9999px; }
    .dark ::-webkit-scrollbar-thumb { background: #4b5563; }
    .star-btn { transition: transform .08s ease; }
    .star-btn:active { transform: scale(0.92); }
  </style>
</head>
<body class="bg-white text-gray-800 dark:bg-gray-950 dark:text-gray-100">
  <header class="sticky top-0 z-50 bg-white/80 dark:bg-gray-950/70 backdrop-blur border-b border-gray-100 dark:border-gray-900">
    <div class="container flex items-center justify-between py-3">
      <a href="#home" class="flex items-center gap-2 group">
        <div class="w-9 h-9 rounded-2xl bg-gradient-to-br from-brand-500 to-brand-700 grid place-items-center text-white font-extrabold shadow-soft">C</div>
        <div>
          <div class="font-extrabold leading-4">CHOMRONG</div>
          <div class="text-xs text-gray-500 dark:text-gray-400 leading-3">CV • InfoSec • Builder</div>
        </div>
      </a>
      <nav class="hidden md:flex items-center gap-6 text-sm">
        <a href="#home" class="nav-link hover:text-brand-600">Home</a>
        <a href="#about" class="nav-link hover:text-brand-600">About</a>
        <a href="#skills" class="nav-link hover:text-brand-600">Skills</a>
        <a href="#experience" class="nav-link hover:text-brand-600">Experience</a>
        <a href="#projects" class="nav-link hover:text-brand-600">Projects</a>
        <a href="#contact" class="nav-link hover:text-brand-600">Contact</a>
      </nav>
      <div class="flex items-center gap-2">
        <button id="themeToggle" class="p-2 rounded-xl hover:bg-gray-100 dark:hover:bg-gray-900 focus:outline-none focus:ring-2 focus:ring-brand-500" aria-label="Toggle theme">
          <svg id="sun" xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 hidden" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="4"/><path d="M12 2v2m0 16v2M4.93 4.93l1.41 1.41M17.66 17.66l1.41 1.41M2 12h2m16 0h2M4.93 19.07l1.41-1.41M17.66 6.34l1.41-1.41"/></svg>
          <svg id="moon" xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 hidden" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg>
        </button>
        <button id="mobileMenuBtn" class="md:hidden p-2 rounded-xl hover:bg-gray-100 dark:hover:bg-gray-900" aria-label="Open menu">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" /></svg>
        </button>
      </div>
    </div>
    <div id="mobileMenu" class="md:hidden hidden border-t border-gray-100 dark:border-gray-900">
      <div class="container py-3 grid gap-2 text-sm">
        <a href="#home" class="py-2">Home</a>
        <a href="#about" class="py-2">About</a>
        <a href="#skills" class="py-2">Skills</a>
        <a href="#experience" class="py-2">Experience</a>
        <a href="#projects" class="py-2">Projects</a>
        <a href="#contact" class="py-2">Contact</a>
      </div>
    </div>
  </header>

  <section id="home" class="relative overflow-hidden">
    <div class="absolute inset-0 -z-10 opacity-[0.08] dark:opacity-[0.12]" aria-hidden="true">
      <svg class="w-full h-full" xmlns="http://www.w3.org/2000/svg"><defs><linearGradient id="g" x1="0" x2="1"><stop stop-color="#3b82f6"/><stop offset="1" stop-color="#1e40af"/></linearGradient></defs><circle cx="20%" cy="20%" r="180" fill="url(#g)"/><circle cx="80%" cy="40%" r="240" fill="url(#g)"/><circle cx="60%" cy="90%" r="160" fill="url(#g)"/></svg>
    </div>
    <div class="container grid md:grid-cols-2 gap-10 items-center py-16 md:py-24">
      <div class="order-2 md:order-1 animate-fadeUp">
        <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-medium bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300">ស្វាគមន៍! — CV របស់ CHOMRONG</div>
        <h1 class="mt-4 text-3xl md:text-5xl font-extrabold leading-tight tracking-tight">Hello, I'm <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-500 to-brand-700">CHOMRONG</span><br/>Student • Cybersecurity • Builder</h1>
        <p class="mt-4 text-gray-600 dark:text-gray-300 max-w-xl">សិស្សថ្នាក់ទី 10 ពី Preah Vihear — ស្រលាញ់វិទ្យាសាស្ត្រ, Coding, និងបង្កើតផលិតផលឌីជីថល។ គោលបំណង៖ ក្លាយជាអ្នកដឹកនាំ IT និងស្ថាបនិកសហគ្រាស។</p>
        <div class="mt-6 flex flex-wrap items-center gap-3">
          <a href="#projects" class="px-5 py-2.5 rounded-2xl bg-brand-600 text-white font-semibold shadow-soft hover:bg-brand-700 focus:outline-none focus:ring-[var(--ring)]">មើលគម្រោង</a>
          <a href="#contact" class="px-5 py-2.5 rounded-2xl bg-gray-900/5 dark:bg-white/10 font-semibold hover:bg-gray-900/10 dark:hover:bg白/20">ទាក់ទងខ្ញុំ</a>
          <a href="#resume" class="px-5 py-2.5 rounded-2xl bg-gray-900/5 dark:bg-white/10 font-semibold hover:bg-gray-900/10 dark:hover:bg-white/20">ទាញយក Resume</a>
        </div>
      </div>
      <div class="order-1 md:order-2 flex justify-center animate-fadeUp">
        <div class="relative w-64 h-64 md:w-80 md:h-80 rounded-[2rem] overflow-hidden shadow-soft ring-1 ring-black/5 dark:ring-white/10 glass">
          <img src="https://picsum.photos/640/640" alt="CHOMRONG portrait" class="w-full h-full object-cover" />
          <div class="absolute bottom-0 left-0 right-0 p-4 bg-gradient-to-t from-black/50 to-transparent text-white">
            <div class="text-lg font-semibold">Yat Chomrong</div>
            <div class="text-xs opacity-90">Student • Cybersecurity • Builder</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="about" class="py-16 md:py-24">
    <div class="container">
      <div class="grid md:grid-cols-3 gap-8 items-start">
        <div class="md:col-span-2">
          <h2 class="text-2xl md:text-3xl font-extrabold">អំពីខ្ញុំ</h2>
          <p class="mt-4 text-gray-600 dark:text-gray-300">ខ្ញុំឈ្មោះ <strong>Yat Chomrong</strong> (CHOMRONG) — កំពុងរៀននៅថ្នាក់ទី 10 នៅ Preah Vihear។ ខ្ញុំស្រលាញ់វិទ្យាសាស្ត្រ, Coding, Networking & Security, និងស្វែងរកគំនិតថ្មីៗ ដើម្បីបង្កើតសេវាកម្មឌីជីថលដែលមានតម្លៃសម្រាប់សង្គម។ គោលបំណងរយៈពេលវែង៖ បង្កើតក្រុមហ៊ុន IT ដ៏រឹងមាំ និងចូលរួមការពារទិន្នន័យសាធារណៈ។</p>
          <div class="mt-6 grid sm:grid-cols-2 gap-4">
            <div class="p-5 rounded-2xl border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5">
              <div class="text-xs uppercase tracking-wider text-gray-500">មុខច្បាស់</div>
              <div class="mt-1 font-semibold">Cybersecurity, Web Dev, AI Tools</div>
            </div>
            <div class="p-5 rounded-2xl border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5">
              <div class="text-xs uppercase tracking-wider text-gray-500">ទីតាំង</div>
              <div class="mt-1 font-semibold">Preah Vihear, Cambodia</div>
            </div>
          </div>
        </div>
        <aside class="space-y-4">
          <div class="p-5 rounded-2xl bg-gradient-to-br from-brand-500 to-brand-700 text-white shadow-soft">
            <div class="text-sm opacity-90">ស្លោក</div>
            <div class="text-lg font-bold leading-tight">"ស្វែងរកចំណេះដឹងរៀងរាល់ថ្ងៃ—ស្ថាបនាជីវិតរៀងរាល់ឆ្នាំ"</div>
          </div>
          <ul class="grid gap-3 text-sm">
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> អាយុ 16 ឆ្នាំ</li>
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> សិស្សថ្នាក់ទី 10</li>
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> ចូលចិត្ត Coding និង Security</li>
          </ul>
        </aside>
      </div>
    </div>
  </section>

  <section id="skills" class="py-16 md:py-24 bg-gray-50 dark:bg-gray-900/30">
    <div class="container">
      <h2 class="text-2xl md:text-3xl font-extrabold">ជំនាញ</h2>
      <p class="mt-2 text-gray-600 dark:text-gray-300">កំពុងអភិវឌ្ឍជំនាញតាមផែនការរៀនជំហានៗ — ខាងក្រោមនេះជាមាត្រដ្ឋានបច្ចុប្បន្ន (អាប់ដេតដោយដៃ)។</p>
      <div class="mt-8 grid md:grid-cols-2 gap-6">
        <div class="space-y-5">
          <div><div class="flex justify-between text-sm"><span>HTML • CSS (Tailwind)</span><span class="text-gray-500">80%</span></div><div class="bar"><span data-width="80%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>JavaScript (ES6+)</span><span class="text-gray-500">70%</span></div><div class="bar"><span data-width="70%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>React Basics</span><span class="text-gray-500">60%</span></div><div class="bar"><span data-width="60%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>Node.js Fundamentals</span><span class="text-gray-500">45%</span></div><div class="bar"><span data-width="45%"></span></div></div>
        </div>
        <div class="space-y-5">
          <div><div class="flex justify-between text-sm"><span>Networking Basics</span><span class="text-gray-500">50%</span></div><div class="bar"><span data-width="50%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>Linux • CLI</span><span class="text-gray-500">55%</span></div><div class="bar"><span data-width="55%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>Cybersecurity (Intro)</span><span class="text-gray-500">40%</span></div><div class="bar"><span data-width="40%"></span></div></div>
          <div><div class="flex justify-between text-sm"><span>English Communication</span><span class="text-gray-500">65%</span></div><div class="bar"><span data-width="65%"></span></div></div>
        </div>
      </div>
    </div>
  </section>

  <section id="experience" class="py-16 md:py-24">
    <div class="container">
      <h2 class="text-2xl md:text-3xl font-extrabold">បទពិសោធន៍ និងសមិទ្ធផល</h2>
      <div class="mt-8 relative timeline">
        <div class="grid gap-8">
          <article class="timeline-item p-5 rounded-2xl border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5">
            <header class="flex items-center justify-between"><h3 class="font-bold">FF DIAMOND.Shop — Top-up Landing</h3><span class="text-xs text-gray-500">2025</span></header>
            <p class="mt-2 text-gray-600 dark:text-gray-300">រចនាទំព័រទិញពេជ្រ Free Fire ដោយមាន UI ស្អាត, ស្លាកតម្លៃ និងការទូទាត់ងាយ។</p>
          </article>
          <article class="timeline-item p-5 rounded-2xl border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5">
            <header class="flex items-center justify-between"><h3 class="font-bold">Telegram Bot — NBOTN_BOT</h3><span class="text-xs text-gray-500">2025</span></header>
            <p class="mt-2 text-gray-600 dark:text-gray-300">ធ្វើ Bot ផ្ទាល់ខ្លួនសម្រាប់ការគ្រប់គ្រងឧបករណ៍ និងការងារប្រចាំថ្ងៃ។</p>
          </article>
        </div>
      </div>
    </div>
  </section>

  <section id="projects" class="py-16 md:py-24 bg-gray-50 dark:bg-gray-900/30">
    <div class="container">
      <div class="flex flex-wrap items-end justify_between gap-4">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">គម្រោង</h2>
          <p class="mt-2 text-gray-600 dark:text-gray-300">សូមមើលគម្រោងលួកកាលពីម្សិលមិញ និងកំពុងធ្វើ។ អាចច្រោះតាមប្រភេទខាងក្រោម។</p>
        </div>
        <div class="flex flex-wrap gap-2 text-sm" role="tablist" aria-label="Project filters">
          <button class="filter px-4 py-2 rounded-xl bg-brand-600 text-white" data-type="all">All</button>
          <button class="filter px-4 py-2 rounded-xl bg-gray-900/5 dark:bg-white/10" data-type="web">Web</button>
          <button class="filter px-4 py-2 rounded-xl bg-gray-900/5 dark:bg-white/10" data-type="bot">Bot</button>
          <button class="filter px-4 py-2 rounded-xl bg-gray-900/5 dark:bg-white/10" data-type="security">Security</button>
        </div>
      </div>

      <div class="mt-8 grid sm:grid-cols-2 lg:grid-cols-3 gap-6" id="projectGrid">
        <article class="card group rounded-2xl overflow-hidden border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5" data-type="web">
          <div class="relative aspect-video shimmer"></div>
          <div class="p-5">
            <h3 class="font-semibold group-hover:text-brand-600">Top-Up Landing</h3>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">Landing Page សម្រាប់ Free Fire — ឆ្លាតវៃ និងលឿន។</p>
            <div class="mt-3 flex items-center gap-2 text-xs text-gray-500">
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Tailwind</span>
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Vanilla JS</span>
            </div>
            <div class="mt-4 flex justify-between items-center">
              <button class="px-3 py-1.5 rounded-lg bg-gray-900/5 dark:bg-white/10 text-sm view-btn" data-title="Top-Up Landing" data-img="https://picsum.photos/1200/800">Preview</button>
              <a href="#" class="text-brand-600 text-sm">Source</a>
            </div>
          </div>
        </article>

        <article class="card group rounded-2xl overflow-hidden border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5" data-type="bot">
          <div class="relative aspect-video shimmer"></div>
          <div class="p-5">
            <h3 class="font-semibold group-hover:text-brand-600">Telegram NBOTN_BOT</h3>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">Bot សម្រាប់ការងារប្រចាំថ្ងៃ និងអូតូម៉ាត។</p>
            <div class="mt-3 flex items-center gap-2 text-xs text-gray-500">
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Telegram API</span>
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Node</span>
            </div>
            <div class="mt-4 flex justify-between items-center">
              <button class="px-3 py-1.5 rounded-lg bg-gray-900/5 dark:bg-white/10 text-sm view-btn" data-title="NBOTN_BOT" data-img="https://picsum.photos/seed/bot/1200/800">Preview</button>
              <a href="#" class="text-brand-600 text-sm">Source</a>
            </div>
          </div>
        </article>

        <article class="card group rounded-2xl overflow-hidden border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5" data-type="security">
          <div class="relative aspect-video shimmer"></div>
          <div class="p-5">
            <h3 class="font-semibold group-hover:text-brand-600">Security Notes</h3>
            <p class="mt-1 text-sm text-gray-600 dark:text-gray-300">សង្ខេប note សុវត្ថិភាព បណ្តាញ និង Linux hardening។</p>
            <div class="mt-3 flex items-center gap-2 text-xs text-gray-500">
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Linux</span>
              <span class="px-2 py-1 rounded-full bg-gray-100 dark:bg-white/10">Net</span>
            </div>
            <div class="mt-4 flex justify-between items-center">
              <button class="px-3 py-1.5 rounded-lg bg-gray-900/5 dark:bg-white/10 text-sm view-btn" data-title="Security Notes" data-img="https://picsum.photos/seed/sec/1200/800">Preview</button>
              <a href="#" class="text-brand-600 text-sm">Source</a>
            </div>
          </div>
        </article>
      </div>
    </div>
  </section>

  <section id="resume" class="py-16 md:py-24">
    <div class="container">
      <div class="grid md:grid-cols-2 gap-8 items-center">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">Resume & សមិទ្ធផល</h2>
          <p class="mt-2 text-gray-600 dark:text-gray-300">ទាញយក Resume ជា TXT និងមើលសមិទ្ធផលសំខាន់ៗរបស់ខ្ញុំខាងក្រោម។</p>
          <div class="mt-4 flex gap-3">
            <button id="downloadResume" class="px-5 py-2.5 rounded-2xl bg-brand-600 text-white font-semibold shadow-soft hover:bg-brand-700">Download TXT</button>
            <a href="#contact" class="px-5 py-2.5 rounded-2xl bg-gray-900/5 dark:bg-white/10 font-semibold">Hire Me</a>
          </div>
          <ul class="mt-6 grid gap-3 text-sm text-gray-700 dark:text-gray-200">
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> Winner — School Coding Mini Hackathon (2025)</li>
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> Built 3+ real projects with users</li>
            <li class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-brand-500"></span> Active community helper & tutor</li>
          </ul>
        </div>
        <div class="rounded-2xl overflow-hidden border border-gray-100 dark:border-gray-800 bg-white/50 dark:bg-white/5 p-6 grid gap-4">
          <div class="h-4 w-2/3 shimmer rounded"></div>
          <div class="h-4 w-1/2 shimmer rounded"></div>
          <div class="h-40 shimmer rounded-2xl"></div>
          <div class="grid grid-cols-3 gap-3">
            <div class="h-14 shimmer rounded-xl"></div>
            <div class="h-14 shimmer rounded-xl"></div>
            <div class="h-14 shimmer rounded-xl"></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact" class="py-16 md:py-24 bg-gray-50 dark:bg-gray-900/30">
    <div class="container">
      <div class="grid md:grid-cols-2 gap-8">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">ទាក់ទង</h2>
          <p class="mt-2 text-gray-600 dark:text-gray-300">មានគម្រោង ឬការងារចូលចិត្ត? បញ្ជូនសារ ឬទំនាក់ទំនងតាមបណ្តាញខាងក្រោម។</p>
          <div class="mt-4 grid gap-2 text-sm">
            <a href="mailto:chomrong@example.com" class="inline-flex items-center gap-2 hover:text-brand-600">chomrong@example.com</a>
            <a href="https://t.me/Blackcyber_Kh" class="inline-flex items-center gap-2 hover:text-brand-600">Telegram</a>
            <a href="#" class="inline-flex items-center gap-2 hover:text-brand-600">GitHub</a>
          </div>
        </div>
        <form id="contactForm" class="p-6 rounded-2xl border border-gray-100 dark:border-gray-800 bg-white/70 dark:bg-white/5 space-y-4">
          <div><label class="text-sm">ឈ្មោះ</label><input type="text" name="name" required class="mt-1 w-full px-4 py-2.5 rounded-xl border border-gray-200 dark:border-gray-800 bg-white/80 dark:bg-gray-950/60 focus:outline-none focus:ring-2 focus:ring-brand-500" placeholder="ឈ្មោះរបស់អ្នក" /></div>
          <div><label class="text-sm">អ៊ីមែល</label><input type="email" name="email" required class="mt-1 w-full px-4 py-2.5 rounded-xl border border-gray-200 dark:border-gray-800 bg-white/80 dark:bg-gray-950/60 focus:outline-none focus:ring-2 focus:ring-brand-500" placeholder="you@mail.com" /></div>
          <div><label class="text-sm">សារ</label><textarea name="message" rows="5" required class="mt-1 w-full px-4 py-2.5 rounded-xl border border-gray-200 dark:border-gray-800 bg-white/80 dark:bg-gray-950/60 focus:outline-none focus:ring-2 focus:ring-brand-500" placeholder="សូមសរសេរ..."></textarea></div>
          <div class="flex items-center justify-between"><div id="formStatus" class="text-sm"></div><button class="px-5 py-2.5 rounded-2xl bg-brand-600 text-white font-semibold shadow-soft hover:bg-brand-700">Send Message</button></div>
        </form>
      </div>
    </div>
  </section>

  <!-- Rating Section -->
  <section id="rating" class="py-16 md:py-20 bg-white/60 dark:bg-white/5">
    <div class="container text-center">
      <h2 class="text-2xl md:text-3xl font-extrabold">⭐ Rate My CV</h2>
      <p class="mt-2 text-gray-600 dark:text-gray-300">ចូលចិត្ត CV នេះប៉ុណ្ណា? ចុចផ្កាយដើម្បីវាយតម្លៃ ហើយយើងនឹងបញ្ជូនអ្នកទៅ Bot របស់ខ្ញុំ</p>
      <div class="mt-6 flex justify-center gap-2" id="starRow" aria-label="Star rating">
        <button class="star-btn px-4 py-2 rounded-2xl bg-gray-100 dark:bg-white/10 text-2xl" data-star="1">⭐</button>
        <button class="star-btn px-4 py-2 rounded-2xl bg-gray-100 dark:bg-white/10 text-2xl" data-star="2">⭐</button>
        <button class="star-btn px-4 py-2 rounded-2xl bg-gray-100 dark:bg-white/10 text-2xl" data-star="3">⭐</button>
        <button class="star-btn px-4 py-2 rounded-2xl bg-gray-100 dark:bg-white/10 text-2xl" data-star="4">⭐</button>
        <button class="star-btn px-4 py-2 rounded-2xl bg-gray-100 dark:bg-white/10 text-2xl" data-star="5">⭐</button>
      </div>
      <div id="ratingStats" class="mt-4 text-sm text-gray-600 dark:text-gray-300">Average: 0.0 (0 ratings)</div>
    </div>
  </section>

  <footer class="py-10 border-t border-gray-100 dark:border-gray-900">
    <div class="container flex flex-col md:flex-row items-center justify-between gap-4 text-sm text-gray-500">
      <div>© <span id="year"></span> CHOMRONG • All rights reserved.</div>
      <div class="flex items-center gap-3">
        <a href="#home" class="hover:text-brand-600">Back to top</a>
        <span>•</span>
        <a href="#contact" class="hover:text-brand-600">Contact</a>
      </div>
    </div>
  </footer>

  <!-- Modal -->
  <div id="modal" class="fixed inset-0 hidden items-center justify-center p-6 z-[60]">
    <div class="absolute inset-0 bg-black/60" data-close="true"></div>
    <div class="relative max-w-4xl w-full bg-white dark:bg-gray-950 rounded-2xl overflow-hidden shadow-soft">
      <div class="flex items-center justify-between p-4 border-b border-gray-100 dark:border-gray-800">
        <h3 id="modalTitle" class="font-semibold"></h3>
        <button class="p-2 rounded-lg hover:bg-gray-100 dark:hover:bg-gray-900" data-close="true" aria-label="Close">
          <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" /></svg>
        </button>
      </div>
      <img id="modalImg" alt="Project preview" class="w-full max-h-[70vh] object-cover" />
    </div>
  </div>

  <script>
    const root = document.documentElement;
    const themeToggle = document.getElementById('themeToggle');
    const sun = document.getElementById('sun');
    const moon = document.getElementById('moon');
    const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
    const savedTheme = localStorage.getItem('theme');
    function applyTheme(mode){
      const isDark = mode === 'dark';
      root.classList.toggle('dark', isDark);
      sun?.classList.toggle('hidden', !isDark);
      moon?.classList.toggle('hidden', isDark);
      localStorage.setItem('theme', isDark ? 'dark' : 'light');
    }
    applyTheme(savedTheme || (prefersDark ? 'dark' : 'light'));
    themeToggle?.addEventListener('click', ()=>{
      applyTheme(root.classList.contains('dark') ? 'light' : 'dark');
    });

    const mobileBtn = document.getElementById('mobileMenuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    mobileBtn?.addEventListener('click', ()=> mobileMenu.classList.toggle('hidden'));

    const bars = document.querySelectorAll('.bar>span');
    const io = new IntersectionObserver((entries)=>{
      entries.forEach(e=>{ if(e.isIntersecting){ e.target.style.width = e.target.dataset.width; } });
    },{ threshold:.35 });
    bars.forEach(b=> io.observe(b));

    const filterBtns = document.querySelectorAll('.filter');
    const cards = document.querySelectorAll('#projectGrid .card');
    filterBtns.forEach(btn=>{
      btn.addEventListener('click', ()=>{
        filterBtns.forEach(b=> b.classList.remove('bg-brand-600','text-white'));
        filterBtns.forEach(b=> b.classList.add('bg-gray-900/5','dark:bg-white/10'));
        btn.classList.add('bg-brand-600','text-white');
        btn.classList.remove('bg-gray-900/5','dark:bg-white/10');
        const type = btn.dataset.type;
        cards.forEach(c=>{
          const show = type === 'all' || c.dataset.type === type;
          c.classList.toggle('hidden', !show);
        });
      })
    });

    const modal = document.getElementById('modal');
    const modalImg = document.getElementById('modalImg');
    const modalTitle = document.getElementById('modalTitle');
    document.querySelectorAll('.view-btn').forEach(b=>{
      b.addEventListener('click', ()=>{
        modalTitle.textContent = b.dataset.title || 'Preview';
        modalImg.src = b.dataset.img;
        modal.classList.remove('hidden'); modal.classList.add('flex');
      })
    });
    modal?.addEventListener('click', (e)=>{
      if(e.target.dataset.close !== undefined){
        modal.classList.add('hidden'); modal.classList.remove('flex'); modalImg.src = '';
      }
    });

    document.getElementById('downloadResume')?.addEventListener('click', ()=>{
      const content = `CHOMRONG — Resume\n\nSkills: HTML/CSS, JS, React, Linux, Networking, Cybersecurity.\nProjects: FF DIAMOND.Shop, NBOTN_BOT, Security Notes.\nContact: chomrong@example.com`;
      const blob = new Blob([content], {type:'text/plain'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'CHOMRONG-Resume.txt'; a.click();
      URL.revokeObjectURL(url);
    });

    const form = document.getElementById('contactForm');
    const status = document.getElementById('formStatus');
    form?.addEventListener('submit', (e)=>{
      e.preventDefault();
      const fd = new FormData(form);
      const name = (fd.get('name')||'').toString().trim();
      const email = (fd.get('email')||'').toString().trim();
      const message = (fd.get('message')||'').toString().trim();
      if(!name || !email || !message){
        status.textContent = 'សូមបំពេញទាំងអស់'; status.className = 'text-sm text-red-600'; return;
      }
      status.textContent = 'បានផ្ញើសារ (Demo) — អ្នកអាចភ្ជាប់ API ពិតនៅទីនេះ'; status.className = 'text-sm text-green-600'; form.reset();
    });

    document.getElementById('year').textContent = new Date().getFullYear();

    // Rating logic + redirect to Telegram bot
    const starRow = document.getElementById('starRow');
    const ratingStats = document.getElementById('ratingStats');
    const store = JSON.parse(localStorage.getItem('ratings') || '[]');
    function updateStats(){
      const n = store.length;
      const avg = n ? (store.reduce((a,b)=>a+b,0)/n).toFixed(1) : '0.0';
      ratingStats.textContent = `Average: ${avg} (${n} ratings)`;
    }
    updateStats();
    starRow?.addEventListener('click', (e)=>{
      const btn = e.target.closest('[data-star]');
      if(!btn) return;
      const value = Number(btn.dataset.star);
      store.push(value);
      localStorage.setItem('ratings', JSON.stringify(store));
      updateStats();
      // small visual feedback then jump
      btn.classList.add('ring-2','ring-brand-500');
      setTimeout(()=>{
        window.location.href = 'https://t.me/yatchomrongios_bot';
      }, 650);
    });
  </script>
</body>
</html>
