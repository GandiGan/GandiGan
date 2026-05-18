<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Preview Profil GitHub Gandi - Tema Eksklusif</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;700&family=Orbitron:wght@400;700;900&family=Inter:wght@300;400;600;700&family=VT323&family=DM+Sans:wght@400;700&display=swap" rel="stylesheet">
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <style>
    body {
      font-family: 'Inter', sans-serif;
      transition: background-color 0.5s ease;
    }
    .font-mono-cyber {
      font-family: 'Fira Code', monospace;
    }
    .font-orbitron {
      font-family: 'Orbitron', sans-serif;
    }
    .font-pixel {
      font-family: 'VT323', monospace;
    }
    .font-minimal {
      font-family: 'DM Sans', sans-serif;
    }

    /* Animasi Mengetik */
    @keyframes blink {
      50% { border-color: transparent }
    }
    .typing-cursor::after {
      content: '|';
      animation: blink 0.8s infinite;
      font-weight: bold;
    }

    /* Transisi Halus untuk Tema */
    .theme-transition {
      transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
    }

    /* Dekorasi Latar Belakang Grid */
    .cyber-grid {
      background-size: 24px 24px;
      transition: background-image 0.5s ease;
    }

    /* Tema Variabel Style */
    /* 1. Neon Green */
    .theme-green {
      --primary: #00FF66;
      --primary-rgb: 0, 255, 102;
      --bg-dark: #0d1117;
      --bg-card: #161b22;
      --bg-terminal: #05080e;
      --accent: #00ffcc;
      --font-header: 'Orbitron', sans-serif;
    }
    /* 2. Synthwave Purple */
    .theme-purple {
      --primary: #ff007f;
      --primary-rgb: 255, 0, 127;
      --bg-dark: #0b0518;
      --bg-card: #140d24;
      --bg-terminal: #07030f;
      --accent: #7b2cbf;
      --font-header: 'Orbitron', sans-serif;
    }
    /* 3. Amber Matrix */
    .theme-amber {
      --primary: #ffb703;
      --primary-rgb: 255, 183, 3;
      --bg-dark: #0f0c05;
      --bg-card: #1a1408;
      --bg-terminal: #080602;
      --accent: #fb8500;
      --font-header: 'Orbitron', sans-serif;
    }
    /* 4. Arctic Ice */
    .theme-ice {
      --primary: #00d2ff;
      --primary-rgb: 0, 210, 255;
      --bg-dark: #050c12;
      --bg-card: #0b1520;
      --bg-terminal: #02070c;
      --accent: #0066cc;
      --font-header: 'Orbitron', sans-serif;
    }
    /* 5. Pixel RPG */
    .theme-pixel {
      --primary: #ff5722;
      --primary-rgb: 255, 87, 34;
      --bg-dark: #140d0a;
      --bg-card: #20140e;
      --bg-terminal: #0c0805;
      --accent: #ffc107;
      --font-header: 'VT323', monospace;
    }
    /* 6. Minimalist Premium */
    .theme-minimal {
      --primary: #818cf8;
      --primary-rgb: 129, 140, 248;
      --bg-dark: #090d16;
      --bg-card: #111827;
      --bg-terminal: #030712;
      --accent: #f43f5e;
      --font-header: 'DM Sans', sans-serif;
    }

    /* Apply Dynamic Theme Variable Styles */
    body {
      background-color: var(--bg-dark);
    }
    .glow-text {
      text-shadow: 0 0 10px rgba(var(--primary-rgb), 0.6), 0 0 25px rgba(var(--primary-rgb), 0.2);
    }
    .neon-border {
      border: 1px solid rgba(var(--primary-rgb), 0.3);
      box-shadow: 0 0 12px rgba(var(--primary-rgb), 0.1);
    }
    .neon-border:hover {
      border: 1px solid rgba(var(--primary-rgb), 0.6);
      box-shadow: 0 0 18px rgba(var(--primary-rgb), 0.2);
    }
    .btn-primary-custom {
      background-color: var(--primary);
      color: #000000;
    }
    .btn-primary-custom:hover {
      box-shadow: 0 0 20px rgba(var(--primary-rgb), 0.6);
      background-color: var(--accent);
    }
    .border-primary-custom {
      border-color: var(--primary);
      color: var(--primary);
    }
    .border-primary-custom:hover {
      background-color: var(--primary);
      color: #000000;
      box-shadow: 0 0 20px rgba(var(--primary-rgb), 0.4);
    }
  </style>
</head>
<body class="theme-green min-h-screen text-gray-300 pb-16 theme-transition">

  <!-- TOP BAR CONTROL PANEL (KUSTOM SIMULATOR) -->
  <div class="bg-gray-900 border-b border-gray-800 px-6 py-4 sticky top-0 z-50 shadow-md">
    <div class="max-w-7xl mx-auto flex flex-col xl:flex-row items-center justify-between gap-4">
      <div class="flex items-center space-x-3">
        <div class="w-3 h-3 bg-red-500 rounded-full animate-ping"></div>
        <span class="font-orbitron font-bold text-white tracking-widest text-sm md:text-base">[ CONFIGURATOR TEMA GANDI ]</span>
      </div>

      <!-- Theme Controls -->
      <div class="flex flex-wrap items-center justify-center gap-2">
        <span class="text-xs text-gray-400 font-mono-cyber mr-2">TEMA UTAMA:</span>
        <button onclick="changeTheme('green')" class="px-2.5 py-1 bg-[#00FF66] text-black font-orbitron font-bold text-[11px] rounded hover:scale-105 transition">NEON GREEN</button>
        <button onclick="changeTheme('purple')" class="px-2.5 py-1 bg-[#ff007f] text-white font-orbitron font-bold text-[11px] rounded hover:scale-105 transition">SYNTHWAVE</button>
        <button onclick="changeTheme('amber')" class="px-2.5 py-1 bg-[#ffb703] text-black font-orbitron font-bold text-[11px] rounded hover:scale-105 transition">AMBER</button>
        <button onclick="changeTheme('ice')" class="px-2.5 py-1 bg-[#00d2ff] text-black font-orbitron font-bold text-[11px] rounded hover:scale-105 transition">ARCTIC ICE</button>
        
        <span class="text-gray-600 px-1 hidden sm:inline">|</span>
        <span class="text-xs text-gray-400 font-mono-cyber mr-2 hidden sm:inline">TEMA BARU:</span>
        <button onclick="changeTheme('pixel')" class="px-2.5 py-1 bg-[#ff5722] text-white font-mono-cyber font-bold text-[11px] rounded hover:scale-105 transition">👾 PIXEL RPG</button>
        <button onclick="changeTheme('minimal')" class="px-2.5 py-1 bg-[#818cf8] text-white font-minimal font-bold text-[11px] rounded hover:scale-105 transition">✨ MINIMALIST</button>
      </div>
    </div>
  </div>

  <!-- MAIN AREA (MOCKUP GITHUB) -->
  <div class="max-w-7xl mx-auto px-4 mt-8">
    <div class="grid grid-cols-1 lg:grid-cols-4 gap-8">
      
      <!-- KOLOM KIRI: INFO USER (MOCKUP GITHUB SIDEBAR) -->
      <div class="lg:col-span-1 flex flex-col items-center lg:items-start">
        
        <!-- Foto Profil Avatar -->
        <div class="relative group w-full max-w-[260px] lg:max-w-full">
          <div class="absolute -inset-1 bg-gradient-to-r from-indigo-500 to-rose-500 rounded-2xl blur opacity-30 group-hover:opacity-75 transition duration-500"></div>
          <div class="relative w-full aspect-square bg-gray-800 rounded-2xl border-2 border-gray-700 overflow-hidden flex flex-col items-center justify-center p-6 text-center">
            <div id="avatar-icon-box" class="w-24 h-24 bg-gradient-to-tr from-indigo-500 to-pink-500 rounded-full flex items-center justify-center text-4xl text-white font-bold mb-4 font-orbitron shadow-lg">
              GA
            </div>
            <span id="role-tag" class="font-orbitron text-xs tracking-wider font-bold mb-1" style="color: var(--primary)">SECURE_ID: 105841</span>
            <span class="text-[10px] text-gray-400 font-mono-cyber">UNISMUH MAKASSAR</span>
          </div>
        </div>

        <!-- Nama User -->
        <div class="mt-4 text-center lg:text-left w-full">
          <h1 class="text-2xl font-bold text-white">Gandi Afriyadi</h1>
          <h2 class="text-lg font-light text-gray-400 font-mono-cyber">@GandiGan</h2>
        </div>

        <button class="w-full mt-4 bg-gray-800 hover:bg-gray-700 text-sm text-gray-300 font-medium py-1.5 px-4 rounded-md border border-gray-700 transition">
          Followers (12) • Following (28)
        </button>

        <!-- Informasi Akademik / Kontak -->
        <div class="mt-6 space-y-4 text-xs text-gray-400 w-full border-t border-gray-800 pt-4 font-mono-cyber">
          <div class="flex items-start space-x-2">
            <i class="fa-solid fa-graduation-cap text-gray-500 mt-0.5"></i>
            <span>Informatics Engineering<br><span class="text-gray-500 text-[10px]">Universitas Muhammadiyah Makassar</span></span>
          </div>
          <div class="flex items-center space-x-2">
            <i class="fa-solid fa-location-dot text-gray-500"></i>
            <span>Makassar, Indonesia</span>
          </div>
          <div class="flex items-center space-x-2">
            <i class="fa-regular fa-envelope text-gray-500"></i>
            <span class="truncate hover:text-white cursor-pointer">105841106624@student.unismuh.ac.id</span>
          </div>
          <div class="flex items-center space-x-2">
            <i class="fa-brands fa-instagram text-gray-500"></i>
            <span class="hover:text-white cursor-pointer">@gandiafriy._</span>
          </div>
        </div>
      </div>

      <!-- KOLOM KANAN: PREVIEW UTAMA GITHUB README -->
      <div class="lg:col-span-3">
        
        <!-- Tab Simulator File GitHub -->
        <div class="bg-gray-900 border border-gray-800 rounded-t-xl px-4 py-3 flex items-center justify-between">
          <div class="flex items-center space-x-2 text-xs font-mono-cyber text-gray-400">
            <i class="fa-regular fa-file-code" style="color: var(--primary)"></i>
            <span class="font-bold text-gray-200">GandiGan / README.md</span>
          </div>
          <span class="text-[10px] font-orbitron px-2 py-0.5 rounded bg-black border border-gray-700 tracking-wider" style="color: var(--primary)">LIVE SIMULATION</span>
        </div>

        <!-- AREA UTAMA RENDERING MARKDOWN (BINGKAI HITAM) -->
        <div class="border-x border-b border-gray-800 p-6 sm:p-10 space-y-10 relative overflow-hidden theme-transition" style="background-color: var(--bg-terminal)">
          
          <!-- Pola Grid Halus Cyber -->
          <div id="bg-grid-overlay" class="absolute inset-0 opacity-10 pointer-events-none" style="background-image: linear-gradient(rgba(255,255,255,0.05) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,0.05) 1px, transparent 1px); background-size: 20px 20px;"></div>

          <div class="relative z-10 space-y-8">
            
            <!-- 1. HEADER TYPING ANIMATION -->
            <div id="typing-border-box" class="text-center py-6 bg-black/50 border rounded-xl p-4 theme-transition" style="border-color: rgba(var(--primary-rgb), 0.2)">
              <span id="live-typing" class="text-lg sm:text-2xl tracking-widest glow-text typing-cursor font-bold" style="color: var(--primary)"></span>
            </div>

            <!-- 2. CAPSULE RENDER (WAVE OR BLOCK HEADER) -->
            <div id="capsule-container" class="relative w-full h-32 overflow-hidden rounded-xl border flex flex-col justify-between p-6 theme-transition" style="border-color: rgba(var(--primary-rgb), 0.2)">
              <div class="absolute inset-0 opacity-20 bg-gradient-to-r" style="background-image: linear-gradient(to right, var(--accent), transparent, var(--accent))"></div>
              
              <!-- Wave Vector -->
              <div id="wave-vector-container" class="absolute bottom-0 left-0 right-0 h-10 overflow-hidden opacity-30">
                <svg class="w-full h-full" viewBox="0 0 1440 74" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M0 12C120 12 240 62 360 62C480 62 600 12 720 12C840 12 960 62 1080 62C1200 62 1320 12 1440 12V74H0V12Z" fill="var(--primary)" />
                </svg>
              </div>
              
              <div class="relative z-10 flex justify-between items-center w-full">
                <div>
                  <span id="capsule-sub-badge" class="text-black text-[9px] font-bold px-2 py-0.5 rounded-full" style="background-color: var(--primary)">TERMINAL SECURE</span>
                  <h2 id="capsule-title" class="text-xl sm:text-2xl font-black tracking-widest mt-1.5" style="color: var(--primary)">WELCOME TO MY SPACE</h2>
                </div>
                <i id="capsule-icon" class="fa-solid fa-microchip text-3xl animate-pulse hidden sm:block" style="color: var(--primary)"></i>
              </div>
              
              <div class="relative z-10 text-[9px] font-mono-cyber flex items-center space-x-2" style="color: var(--primary)">
                <span class="w-1.5 h-1.5 rounded-full animate-ping" style="background-color: var(--primary)"></span>
                <span id="capsule-status-text" class="opacity-80">STABLE CONNECTION RECOGNIZED</span>
              </div>
            </div>

            <!-- 3. TERMINAL INFO / OVERVIEW BOX -->
            <div id="overview-border-box" class="border rounded-lg overflow-hidden theme-transition" style="border-color: rgba(var(--primary-rgb), 0.15)">
              <div id="terminal-bar" class="bg-gray-900/80 px-4 py-2 flex items-center space-x-2 border-b border-gray-800">
                <span class="w-2.5 h-2.5 rounded-full bg-red-500"></span>
                <span class="w-2.5 h-2.5 rounded-full bg-yellow-500"></span>
                <span class="w-2.5 h-2.5 rounded-full bg-green-500"></span>
                <span id="terminal-path" class="text-[10px] font-mono-cyber text-gray-500 ml-2">GandiGan@root:~</span>
              </div>
              <div class="bg-black/60 p-5 sm:p-6 text-xs sm:text-sm space-y-4">
                <div>
                  <span id="terminal-prompt" class="text-emerald-400 font-mono-cyber">GandiGan@root:~$</span> <span class="text-white font-mono-cyber">cat about_me.md</span>
                </div>
                <div id="overview-text" class="text-gray-300 pl-4 border-l-2 leading-relaxed" style="border-color: var(--primary)">
                  Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.
                </div>
                <div id="terminal-grid" class="grid grid-cols-1 sm:grid-cols-3 gap-3 pt-3 text-xs border-t border-gray-900">
                  <div>
                    <span class="block text-gray-500">// Misi Aktif</span>
                    <span class="text-white font-bold">Proyek Kuliah</span>
                  </div>
                  <div>
                    <span class="block text-gray-500">// Eksplorasi</span>
                    <span class="text-white font-bold">JS & Python Advanced</span>
                  </div>
                  <div>
                    <span class="block text-gray-500">// Keunikan</span>
                    <span class="text-white font-bold">Coffee to Code</span>
                  </div>
                </div>
              </div>
            </div>

            <!-- 4. TECH STACK & ACCESSORIES -->
            <div class="space-y-4">
              <div class="flex items-center space-x-3">
                <span id="tech-prefix" class="font-orbitron text-xs tracking-wider" style="color: var(--primary)">01 //</span>
                <h3 id="tech-title" class="text-sm sm:text-base font-black text-white tracking-widest">[ TECH STACK & ACCESSORIES ]</h3>
              </div>
              
              <div class="bg-black/30 border p-5 rounded-xl theme-transition" style="border-color: rgba(var(--primary-rgb), 0.1)">
                <div class="flex flex-wrap gap-3 justify-start">
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-orange-500 transition">
                    <i class="fa-brands fa-html5 text-orange-500"></i>
                    <span>HTML5</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-blue-500 transition">
                    <i class="fa-brands fa-css3-alt text-blue-500"></i>
                    <span>CSS3</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-yellow-500 transition">
                    <i class="fa-brands fa-js text-yellow-500"></i>
                    <span>JavaScript</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-cyan-400 transition">
                    <i class="fa-brands fa-react text-cyan-400"></i>
                    <span>React</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-green-500 transition">
                    <i class="fa-brands fa-node-js text-green-500"></i>
                    <span>NodeJS</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-blue-400 transition">
                    <i class="fa-brands fa-python text-blue-400"></i>
                    <span>Python</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-teal-500 transition">
                    <i class="fa-solid fa-database text-teal-500"></i>
                    <span>MySQL</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-red-500 transition">
                    <i class="fa-brands fa-git-alt text-red-500"></i>
                    <span>Git</span>
                  </span>
                  <span class="px-3 py-1.5 bg-gray-900 border border-gray-800 rounded text-xs font-mono-cyber text-gray-300 flex items-center space-x-1.5 hover:border-blue-600 transition">
                    <i class="fa-solid fa-cube text-blue-600"></i>
                    <span>VSCode</span>
                  </span>
                </div>
              </div>
            </div>

            <!-- 5. STATS LAB -->
            <div class="space-y-4">
              <div class="flex items-center space-x-3">
                <span id="stats-prefix" class="font-orbitron text-xs tracking-wider" style="color: var(--primary)">02 //</span>
                <h3 id="stats-title" class="text-sm sm:text-base font-black text-white tracking-widest">[ DATACENTER STATS ]</h3>
              </div>

              <!-- Simulator Kartu Statistik Unik Anti-Broken -->
              <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Stat Card -->
                <div class="bg-black/40 border rounded-xl p-5 space-y-3 relative overflow-hidden neon-border theme-transition">
                  <h4 id="stat-card-title" class="text-xs font-orbitron tracking-wider border-b border-gray-800 pb-2" style="color: var(--primary)">GANDI'S STATUS ENGINE</h4>
                  <div class="space-y-2 text-xs text-gray-300">
                    <div class="flex justify-between">
                      <span id="stat-label-1" class="text-gray-500">Stars Earned</span>
                      <span class="font-bold text-white">12</span>
                    </div>
                    <div class="flex justify-between">
                      <span id="stat-label-2" class="text-gray-500">Total Commits</span>
                      <span class="font-bold text-white">186</span>
                    </div>
                    <div class="flex justify-between">
                      <span id="stat-label-3" class="text-gray-500">PRs Merged</span>
                      <span class="font-bold text-white">4</span>
                    </div>
                    <div class="flex justify-between">
                      <span id="stat-label-4" class="text-gray-500">Issues Solved</span>
                      <span class="font-bold text-white">2</span>
                    </div>
                  </div>
                </div>

                <!-- Languages Card -->
                <div class="bg-black/40 border rounded-xl p-5 space-y-4 relative overflow-hidden neon-border theme-transition">
                  <h4 id="lang-card-title" class="text-xs font-orbitron tracking-wider border-b border-gray-800 pb-2" style="color: var(--primary)">LANGUAGE DISTRIBUTION</h4>
                  <div class="space-y-2.5">
                    <div class="space-y-1">
                      <div class="flex justify-between text-[11px]">
                        <span class="text-white">JavaScript</span>
                        <span style="color: var(--primary)">42%</span>
                      </div>
                      <div class="w-full h-1 bg-gray-900 rounded-full overflow-hidden">
                        <div class="h-full rounded-full" style="background-color: var(--primary); width: 42%;"></div>
                      </div>
                    </div>
                    <div class="space-y-1">
                      <div class="flex justify-between text-[11px]">
                        <span class="text-white">Python</span>
                        <span style="color: var(--primary)">30%</span>
                      </div>
                      <div class="w-full h-1 bg-gray-900 rounded-full overflow-hidden">
                        <div class="h-full rounded-full" style="background-color: var(--primary); width: 30%;"></div>
                      </div>
                    </div>
                    <div class="space-y-1">
                      <div class="flex justify-between text-[11px]">
                        <span class="text-white">HTML/CSS</span>
                        <span style="color: var(--primary)">28%</span>
                      </div>
                      <div class="w-full h-1 bg-gray-900 rounded-full overflow-hidden">
                        <div class="h-full rounded-full" style="background-color: var(--primary); width: 28%;"></div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!-- 6. HUBUNGI SAYA -->
            <div class="space-y-4">
              <div class="flex items-center space-x-3">
                <span id="connect-prefix" class="font-orbitron text-xs tracking-wider" style="color: var(--primary)">03 //</span>
                <h3 id="connect-title" class="text-sm sm:text-base font-black text-white tracking-widest">[ ESTABLISH CONNECTION ]</h3>
              </div>
              <div class="flex flex-wrap gap-4">
                <a href="mailto:105841106624@student.unismuh.ac.id" class="px-5 py-2.5 bg-gray-900 border-2 font-orbitron font-bold text-xs tracking-wider rounded-lg transition duration-300 flex items-center space-x-2 border-primary-custom">
                  <i class="fa-solid fa-envelope"></i>
                  <span id="mail-btn-text">TERMINAL MAIL</span>
                </a>
                <a href="https://instagram.com/gandiafriy._" target="_blank" class="px-5 py-2.5 bg-gray-900 border-2 font-orbitron font-bold text-xs tracking-wider rounded-lg transition duration-300 flex items-center space-x-2 border-primary-custom">
                  <i class="fa-brands fa-instagram"></i>
                  <span id="ig-btn-text">CYBER INSTAGRAM</span>
                </a>
              </div>
            </div>

            <!-- FOOTER AKHIR -->
            <div id="footer-text-element" class="text-center pt-8 border-t border-gray-900 text-xs text-gray-500 font-mono-cyber">
              <code>// End of file. Copyright © 2026 GandiGan</code>
            </div>

          </div>
        </div>

        <!-- GENERATOR MARKDOWN DISPLAY (TINDAKAN NYATA) -->
        <div class="mt-8 bg-gray-900 border border-gray-800 rounded-xl p-6">
          <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-4 mb-4">
            <div>
              <h4 class="font-orbitron text-sm font-bold text-white tracking-widest">KODE MARKDOWN BISA LANGSUNG DI-COPY:</h4>
              <p class="text-xs text-gray-400 mt-1">Salin kode di bawah ini lalu tempel ke file README.md utama profil GitHub-mu.</p>
            </div>
            <button onclick="copyToClipboard()" class="px-4 py-2 text-xs font-orbitron font-bold rounded flex items-center space-x-2 self-start sm:self-auto btn-primary-custom transition">
              <i class="fa-regular fa-copy"></i>
              <span id="copy-btn-text">SALIN KODE MARKDOWN</span>
            </button>
          </div>
          
          <div class="relative">
            <pre class="bg-black/50 border border-gray-800 rounded-lg p-4 overflow-x-auto text-xs font-mono-cyber text-[#00FF66] max-h-60 overflow-y-auto" id="markdown-code-box">
<!-- Memuat Kode Markdown... -->
            </pre>
          </div>
        </div>

      </div>

    </div>
  </div>

  <script>
    // Database Template Tema Markdown
    const markdownTemplates = {
      green: `<!-- HEADER ANIMASI CYBERPUNK -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=26&duration=2500&pause=500&color=00FF66&center=true&vCenter=true&width=800&lines=%5B%3E%5D+GANDI+AFRIYADI+%3A%3A+DEVELOPER%3B%5B%3E%5D+INITIALIZING+PROFILE...%3B%5B%3E%5D+STATUS%3A+STUDENT+%40UNISMUH" alt="Cyber Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=waving&color=00FF66&height=120&section=header&text=WELCOME%20TO%20MY%20SPACE&fontSize=30&animation=twinkling&fontColor=000000" alt="Banner Wave" />
</p>

---

### 🌐 [ SYSTEM OVERVIEW ]

\`\`\`📋 Root:/GandiGan $ cat about_me.md\`\`\`
> Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.

* 🚀 **Current Mission:** Menyelesaikan proyek kuliah & ngulik hal baru
* 🧠 **Core Upgrade:** Sedang memperdalam ekosistem JavaScript & Python
* ⚡ **Fun Function:** Menghasilkan baris kode yang berjalan lancar (kadang dibantu kopi)

---

### 🛠️ [ TECH STACK & ACCESSORIES ]

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="My Skills" />
  </a>
</p>

---

### 📊 [ DATACENTER STATS ]

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=neon&count_private=true&border_radius=20" alt="Gandi's Stats" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=neon&border_radius=20" alt="Gandi's Languages" />
</p>

---

### 📬 [ ESTABLISH CONNECTION ]

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/TERMINAL_MAIL-00FF66?style=flat-square&logo=gmail&logoColor=black" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/CYBER_IG-00FF66?style=flat-square&logo=instagram&logoColor=black" alt="Instagram" />
  </a>
</p>

---

<div align="center">
  <code>// End of file. Copyright © 2026 GandiGan</code>
</div>`,

      purple: `<!-- HEADER ANIMASI SYNTHWAVE -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=26&duration=2500&pause=500&color=FF007F&center=true&vCenter=true&width=800&lines=%5B%3E%5D+GANDI+AFRIYADI+%3A%3A+SYNTH_DEV%3B%5B%3E%5D+BOOTING+SYSTEM...%3B%5B%3E%5D+RETRO_WAVE_ONLINE" alt="Cyber Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=waving&color=FF007F&height=120&section=header&text=WELCOME%20TO%20MY%20SPACE&fontSize=30&animation=twinkling&fontColor=ffffff" alt="Banner Wave" />
</p>

---

### 🌐 [ SYSTEM OVERVIEW ]

\`\`\`📋 Root:/GandiGan $ cat about_me.md\`\`\`
> Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.

* 🚀 **Current Mission:** Menyelesaikan proyek kuliah & ngulik hal baru
* 🧠 **Core Upgrade:** Sedang memperdalam ekosistem JavaScript & Python
* ⚡ **Fun Function:** Menghasilkan baris kode yang berjalan lancar (kadang dibantu kopi)

---

### 🛠️ [ TECH STACK & ACCESSORIES ]

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="My Skills" />
  </a>
</p>

---

### 📊 [ DATACENTER STATS ]

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=synthwave&count_private=true&border_radius=20" alt="Gandi's Stats" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=synthwave&border_radius=20" alt="Gandi's Languages" />
</p>

---

### 📬 [ ESTABLISH CONNECTION ]

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/RETRO_MAIL-FF007F?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/RETRO_IG-FF007F?style=flat-square&logo=instagram&logoColor=white" alt="Instagram" />
  </a>
</p>

---

<div align="center">
  <code>// End of file. Copyright © 2026 GandiGan</code>
</div>`,

      amber: `<!-- HEADER ANIMASI AMBER -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=26&duration=2500&pause=500&color=FFB703&center=true&vCenter=true&width=800&lines=%5B%3E%5D+GANDI+AFRIYADI+%3A%3A+AMBER_NET%3B%5B%3E%5D+DECRYPTING+DATABASE...%3B%5B%3E%5D+ACCESS+GRANTED" alt="Cyber Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=waving&color=FFB703&height=120&section=header&text=WELCOME%20TO%20MY%20SPACE&fontSize=30&animation=twinkling&fontColor=000000" alt="Banner Wave" />
</p>

---

### 🌐 [ SYSTEM OVERVIEW ]

\`\`\`📋 Root:/GandiGan $ cat about_me.md\`\`\`
> Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.

* 🚀 **Current Mission:** Menyelesaikan proyek kuliah & ngulik hal baru
* 🧠 **Core Upgrade:** Sedang memperdalam ekosistem JavaScript & Python
* ⚡ **Fun Function:** Menghasilkan baris kode yang berjalan lancar (kadang dibantu kopi)

---

### 🛠️ [ TECH STACK & ACCESSORIES ]

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="My Skills" />
  </a>
</p>

---

### 📊 [ DATACENTER STATS ]

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=juicyfresh&count_private=true&border_radius=20" alt="Gandi's Stats" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=juicyfresh&border_radius=20" alt="Gandi's Languages" />
</p>

---

### 📬 [ ESTABLISH CONNECTION ]

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/AMBER_MAIL-FFB703?style=flat-square&logo=gmail&logoColor=black" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/AMBER_IG-FFB703?style=flat-square&logo=instagram&logoColor=black" alt="Instagram" />
  </a>
</p>

---

<div align="center">
  <code>// End of file. Copyright © 2026 GandiGan</code>
</div>`,

      ice: `<!-- HEADER ANIMASI ICE ARCTIC -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&size=26&duration=2500&pause=500&color=00D2FF&center=true&vCenter=true&width=800&lines=%5B%3E%5D+GANDI+AFRIYADI+%3A%3A+ARCTIC_NODE%3B%5B%3E%5D+COOLING+CPU...%3B%5B%3E%5D+TEMPERATURE+OPTIMIZED" alt="Cyber Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=waving&color=00D2FF&height=120&section=header&text=WELCOME%20TO%20MY%20SPACE&fontSize=30&animation=twinkling&fontColor=000000" alt="Banner Wave" />
</p>

---

### 🌐 [ SYSTEM OVERVIEW ]

\`\`\`📋 Root:/GandiGan $ cat about_me.md\`\`\`
> Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.

* 🚀 **Current Mission:** Menyelesaikan proyek kuliah & ngulik hal baru
* 🧠 **Core Upgrade:** Sedang memperdalam ekosistem JavaScript & Python
* ⚡ **Fun Function:** Menghasilkan baris kode yang berjalan lancar (kadang dibantu kopi)

---

### 🛠️ [ TECH STACK & ACCESSORIES ]

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="My Skills" />
  </a>
</p>

---

### 📊 [ DATACENTER STATS ]

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=nord&count_private=true&border_radius=20" alt="Gandi's Stats" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=nord&border_radius=20" alt="Gandi's Languages" />
</p>

---

### 📬 [ ESTABLISH CONNECTION ]

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/ICE_MAIL-00D2FF?style=flat-square&logo=gmail&logoColor=black" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/ICE_IG-00D2FF?style=flat-square&logo=instagram&logoColor=black" alt="Instagram" />
  </a>
</p>

---

<div align="center">
  <code>// End of file. Copyright © 2026 GandiGan</code>
</div>`,

      pixel: `<!-- HEADER RETRO GAME / PIXEL RPG -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=VT323&size=35&duration=2000&pause=500&color=FF5722&center=true&vCenter=true&width=800&lines=PLAYER+1%3A+GANDI+AFRIYADI+READY%3BBOOSTING+STATS...%3BSELECT+YOUR+HERO%3BUNISMUH+CAMPUS+QUEST+ACTIVE" alt="Pixel Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=slice&color=FF5722&height=120&section=header&text=CHOOSE%20YOUR%20CHARACTER&fontSize=35&fontAlignY=40&fontColor=ffffff" alt="Pixel Slice Banner" />
</p>

---

### 👾 [ PLAYER STATUS ]

\`\`\`📋 Root:/GandiGan $ cat hero_profile.txt\`\`\`
> Halo! Saya Gandi, mahasiswa Teknik Informatika Unismuh Makassar. Saya sedang menyelesaikan misi kuliah di dunia pemrograman untuk meningkatkan level skill coding saya.

* 🗡️ **Current Quest:** Membabat habis tugas kuliah & proyek web
* ⚡ **Mana Points:** JavaScript, React, NodeJS & Python
* 🧪 **Potion Power:** Minum Kopi Hitam hangat untuk meregenerasi stamina ngoding

---

### 🛠️ [ SKILL SLOTS / INVENTORY ]

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="Inventory Skills" />
  </a>
</p>

---

### 📊 [ CHARACTER STATS ]

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=blood&count_private=true&border_radius=10" alt="Gandi's Level Stats" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=blood&border_radius=10" alt="Gandi's Weapon Languages" />
</p>

---

### 📬 [ WHISPER / SEND MESSAGE ]

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/GUILD_MAIL-FF5722?style=press-start&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/GUILD_IG-FF5722?style=press-start&logo=instagram&logoColor=white" alt="Instagram" />
  </a>
</p>

---

<div align="center">
  <code>// Game Over. Press [RESET] to run again. GandiGan © 2026</code>
</div>`,

      minimal: `<!-- HEADER PREMIUM MINIMALIST -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=DM+Sans&size=24&duration=3000&pause=1000&color=818CF8&center=true&vCenter=true&width=800&lines=Gandi+Afriyadi+—+Software+Developer;Crafting+digital+products+and+clean+code;Informatics+Engineering+at+Unismuh" alt="Minimal Typing" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/type=soft&color=818cf8&height=100&section=header&text=DESIGN%20AND%20CODE&fontSize=26&fontColor=ffffff" alt="Minimal Soft Banner" />
</p>

---

### 👤 Profile Overview

> Saya adalah mahasiswa Teknik Informatika di Universitas Muhammadiyah Makassar yang menaruh minat tinggi pada pembuatan aplikasi web responsif dan pemrosesan logika backend. Senang memecahkan masalah lewat baris kode yang fungsional dan terstruktur.

* ⚙️ **Focus:** Frontend Web Development & Backend Integration
* 💬 **Tech Ecosystem:** JavaScript, React, Node.js, Python, SQL
* 💡 **Philosophy:** Menulis kode sederhana, bersih, dan mudah dirawat

---

### 🛠️ Core Technologies

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,py,mysql,git,vscode&theme=dark" alt="Core Technologies" />
  </a>
</p>

---

### 📊 Github Metrics

<p align="center">
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api?username=GandiGan&show_icons=true&theme=nord&count_private=true&border_radius=15" alt="Gandi's Metrics" />
  <img height="190" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=GandiGan&layout=compact&theme=nord&border_radius=15" alt="Gandi's Languages" />
</p>

---

### 📬 Direct Contact

<p align="left">
  <a href="mailto:105841106624@student.unismuh.ac.id" target="_blank">
    <img src="https://img.shields.io/badge/E--Mail-818CF8?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://instagram.com/gandiafriy._" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-818CF8?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" />
  </a>
</p>

---

<p align="center">
  <font color="#8b949e">Copyright © 2026 GandiGan • Makassar, Indonesia</font>
</p>`
    };

    // Fungsi Pengubah Tema Dinamis
    function changeTheme(themeName) {
      const body = document.body;
      body.className = 'min-h-screen text-gray-300 pb-16 theme-transition';
      body.classList.add('theme-' + themeName);
      
      // Update Markdown display code box
      const codeBox = document.getElementById('markdown-code-box');
      codeBox.textContent = markdownTemplates[themeName].trim();
      
      // Mengubah Styling Pratinjau sesuai Karakter Tema
      applySimulatorTheming(themeName);
      
      // Restart Typing Animation with specific theme text
      restartTyping(themeName);
    }

    // Mengubah Elemen Simulator agar Terasa Sesuai Karakteristik Tema
    function applySimulatorTheming(theme) {
      const avatarBox = document.getElementById('avatar-icon-box');
      const bgGrid = document.getElementById('bg-grid-overlay');
      const roleTag = document.getElementById('role-tag');
      
      const capContainer = document.getElementById('capsule-container');
      const waveVector = document.getElementById('wave-vector-container');
      const capSubBadge = document.getElementById('capsule-sub-badge');
      const capTitle = document.getElementById('capsule-title');
      const capIcon = document.getElementById('capsule-icon');
      const capStatusText = document.getElementById('capsule-status-text');

      const overviewText = document.getElementById('overview-text');
      const terminalPath = document.getElementById('terminal-path');
      const terminalPrompt = document.getElementById('terminal-prompt');
      const terminalBar = document.getElementById('terminal-bar');
      const terminalGrid = document.getElementById('terminal-grid');

      const techPrefix = document.getElementById('tech-prefix');
      const techTitle = document.getElementById('tech-title');
      const statsPrefix = document.getElementById('stats-prefix');
      const statsTitle = document.getElementById('stats-title');
      const connectPrefix = document.getElementById('connect-prefix');
      const connectTitle = document.getElementById('connect-title');

      const statCardTitle = document.getElementById('stat-card-title');
      const langCardTitle = document.getElementById('lang-card-title');
      const statLabel1 = document.getElementById('stat-label-1');
      const statLabel2 = document.getElementById('stat-label-2');
      const statLabel3 = document.getElementById('stat-label-3');
      const statLabel4 = document.getElementById('stat-label-4');

      const mailBtn = document.getElementById('mail-btn-text');
      const igBtn = document.getElementById('ig-btn-text');
      const footerElement = document.getElementById('footer-text-element');

      // RESET FONTS
      const textElements = [roleTag, capSubBadge, capTitle, capStatusText, overviewText, techTitle, statsTitle, connectTitle, statCardTitle, langCardTitle, mailBtn, igBtn, footerElement];
      textElements.forEach(el => {
        el.className = el.className.replace(/font-orbitron|font-pixel|font-minimal|font-mono-cyber/g, '').trim();
      });

      // DEFAULT TERMINAL VIEWS
      terminalBar.style.display = 'flex';
      terminalPrompt.style.display = 'inline';
      bgGrid.style.display = 'block';
      waveVector.style.display = 'block';
      capContainer.style.borderRadius = '0.75rem';

      if (theme === 'pixel') {
        // TEMA 8-BIT RETRO GAME
        avatarBox.className = "w-24 h-24 bg-gradient-to-tr from-amber-600 to-red-700 rounded-none flex items-center justify-center text-4xl text-white font-bold mb-4 font-pixel shadow-lg border-4 border-amber-400";
        avatarBox.innerHTML = "🎮";
        roleTag.classList.add('font-pixel');
        roleTag.textContent = "LVL_99: INFORMATICS";
        
        capContainer.style.borderRadius = '0';
        capContainer.style.borderWidth = '4px';
        waveVector.style.display = 'none';
        capSubBadge.className = "text-black text-[10px] font-pixel font-bold px-3 py-0.5 rounded-none";
        capSubBadge.textContent = "SELECT CHARACTER";
        capSubBadge.style.backgroundColor = "var(--primary)";
        
        capTitle.className = "text-xl sm:text-2xl font-pixel font-bold tracking-widest mt-1.5";
        capTitle.textContent = "CHOOSE YOUR CHARACTER";
        capStatusText.className = "text-[11px] font-pixel flex items-center space-x-2";
        capStatusText.textContent = "QUEST IN PROGRESS // UNISMUH AREA";
        capIcon.className = "fa-solid fa-gamepad text-3xl animate-bounce hidden sm:block";

        overviewText.classList.add('font-pixel');
        overviewText.textContent = "Halo! Saya Gandi, mahasiswa Teknik Informatika Unismuh Makassar. Saya sedang menyelesaikan misi kuliah di dunia pemrograman untuk meningkatkan level skill coding saya.";
        
        terminalPath.textContent = "GandiGan@rpg_server:~";
        terminalPrompt.innerHTML = "GandiGan@rpg_server:~$ <span class='text-white'>cat hero_profile.txt</span>";
        terminalGrid.innerHTML = `
          <div>
            <span class="block text-gray-500">// Weapon Active</span>
            <span class="text-white font-pixel text-sm">Web / App Code</span>
          </div>
          <div>
            <span class="block text-gray-500">// Magic Skills</span>
            <span class="text-white font-pixel text-sm">React & NodeJS</span>
          </div>
          <div>
            <span class="block text-gray-500">// HP / Stamina</span>
            <span class="text-white font-pixel text-sm">Coffee Powered</span>
          </div>
        `;

        techPrefix.textContent = ">>> ";
        techPrefix.classList.add('font-pixel');
        techTitle.textContent = "SKILL SLOTS / INVENTORY";
        techTitle.classList.add('font-pixel');

        statsPrefix.textContent = ">>> ";
        statsPrefix.classList.add('font-pixel');
        statsTitle.textContent = "CHARACTER METRICS";
        statsTitle.classList.add('font-pixel');

        connectPrefix.textContent = ">>> ";
        connectPrefix.classList.add('font-pixel');
        connectTitle.textContent = "WHISPER TO GANDI";
        connectTitle.classList.add('font-pixel');

        statCardTitle.textContent = "HERO STATS MATRIX";
        statCardTitle.classList.add('font-pixel');
        langCardTitle.textContent = "SPELL MASTERIES";
        langCardTitle.classList.add('font-pixel');

        statLabel1.textContent = "Experience Stars";
        statLabel2.textContent = "Dungeon Commits";
        statLabel3.textContent = "PR Quests";
        statLabel4.textContent = "Bugs Slayed";

        mailBtn.textContent = "GUILD MAIL";
        mailBtn.classList.add('font-pixel');
        igBtn.textContent = "GUILD INSTAGRAM";
        igBtn.classList.add('font-pixel');

        footerElement.innerHTML = "<code>// Game Over. Press [RESET] to run again. GandiGan © 2026</code>";
        footerElement.classList.add('font-pixel');

      } else if (theme === 'minimal') {
        // TEMA MINIMALIST MODERN PREMIUM
        avatarBox.className = "w-24 h-24 bg-gradient-to-tr from-slate-800 to-indigo-950 rounded-2xl flex items-center justify-center text-4xl text-white font-bold mb-4 font-minimal shadow-md border border-indigo-500/30";
        avatarBox.innerHTML = "GA";
        roleTag.classList.add('font-minimal');
        roleTag.textContent = "Software Developer";
        
        capContainer.style.borderRadius = '1rem';
        capContainer.style.borderWidth = '1px';
        waveVector.style.display = 'none';
        capSubBadge.className = "text-white text-[10px] font-minimal font-bold px-3 py-1 rounded-full bg-indigo-600";
        capSubBadge.textContent = "CRAFTING DIGITAL SOLUTIONS";
        
        capTitle.className = "text-lg sm:text-xl font-minimal font-bold tracking-normal mt-1.5";
        capTitle.textContent = "DESIGN AND CODE";
        capStatusText.className = "text-xs font-minimal text-gray-400";
        capStatusText.textContent = "Makassar, South Sulawesi • Active Coding Session";
        capIcon.className = "fa-solid fa-feather text-2xl hidden sm:block";

        overviewText.classList.add('font-minimal');
        overviewText.textContent = "Saya adalah mahasiswa Teknik Informatika di Universitas Muhammadiyah Makassar yang menaruh minat tinggi pada pembuatan aplikasi web responsif dan pemrosesan logika backend. Senang memecahkan masalah lewat baris kode yang fungsional.";

        terminalBar.style.display = 'none';
        terminalPrompt.style.display = 'none';
        terminalGrid.innerHTML = `
          <div>
            <span class="block text-gray-500 font-minimal text-[10px] uppercase tracking-wider">FOCUS ON</span>
            <span class="text-white font-minimal font-bold text-sm">Fullstack Ecosystem</span>
          </div>
          <div>
            <span class="block text-gray-500 font-minimal text-[10px] uppercase tracking-wider">PREFER STACK</span>
            <span class="text-white font-minimal font-bold text-sm">React & Node.js</span>
          </div>
          <div>
            <span class="block text-gray-500 font-minimal text-[10px] uppercase tracking-wider">LOCATION</span>
            <span class="text-white font-minimal font-bold text-sm">Makassar, ID</span>
          </div>
        `;

        techPrefix.textContent = ":: ";
        techPrefix.classList.add('font-minimal');
        techTitle.textContent = "Core Technologies";
        techTitle.classList.add('font-minimal');

        statsPrefix.textContent = ":: ";
        statsPrefix.classList.add('font-minimal');
        statsTitle.textContent = "Github Performance";
        statsTitle.classList.add('font-minimal');

        connectPrefix.textContent = ":: ";
        connectPrefix.classList.add('font-minimal');
        connectTitle.textContent = "Direct Channels";
        connectTitle.classList.add('font-minimal');

        statCardTitle.textContent = "MEMBER METRICS";
        statCardTitle.classList.add('font-minimal');
        langCardTitle.textContent = "STACK RATIO";
        langCardTitle.classList.add('font-minimal');

        statLabel1.textContent = "Stars Achieved";
        statLabel2.textContent = "Total Git Commits";
        statLabel3.textContent = "Pull Requests";
        statLabel4.textContent = "Resolved Issues";

        mailBtn.textContent = "DIRECT EMAIL";
        mailBtn.classList.add('font-minimal');
        igBtn.textContent = "INSTAGRAM HANDLE";
        igBtn.classList.add('font-minimal');

        footerElement.innerHTML = "<font color='#8b949e' class='font-minimal'>Copyright © 2026 GandiGan • Makassar, Indonesia</font>";

      } else {
        // TEMA CYBERPUNK STANDAR (GREEN, PURPLE, AMBER, ICE)
        avatarBox.className = "w-24 h-24 bg-gradient-to-tr from-[#00FF66] to-cyan-500 rounded-full flex items-center justify-center text-4xl text-black font-bold mb-4 font-orbitron shadow-lg";
        avatarBox.innerHTML = "GA";
        roleTag.classList.add('font-orbitron');
        roleTag.textContent = "SECURE_ID: 105841";
        
        capSubBadge.className = "text-black text-[9px] font-orbitron font-bold px-2 py-0.5 rounded-full";
        capSubBadge.textContent = "TERMINAL SECURE";
        capSubBadge.style.backgroundColor = "var(--primary)";
        
        capTitle.className = "font-orbitron text-xl sm:text-2xl font-black tracking-widest mt-1.5";
        capTitle.textContent = "WELCOME TO MY SPACE";
        capStatusText.className = "text-[9px] font-mono-cyber flex items-center space-x-2";
        capStatusText.textContent = "STABLE CONNECTION RECOGNIZED";
        capIcon.className = "fa-solid fa-microchip text-3xl animate-pulse hidden sm:block";

        overviewText.classList.add('font-mono-cyber');
        overviewText.textContent = "Saya adalah mahasiswa Teknik Informatika di Unismuh yang fokus mendalami dunia programming dan eksplorasi teknologi baru. Senang memecahkan masalah lewat baris kode dan membangun proyek digital yang fungsional.";

        terminalPath.textContent = "GandiGan@root:~";
        terminalPrompt.innerHTML = "GandiGan@root:~$ <span class='text-white'>cat about_me.md</span>";
        terminalGrid.innerHTML = `
          <div>
            <span class="block text-gray-500">// Misi Aktif</span>
            <span class="text-white font-bold">Proyek Kuliah</span>
          </div>
          <div>
            <span class="block text-gray-500">// Eksplorasi</span>
            <span class="text-white font-bold">JS & Python Advanced</span>
          </div>
          <div>
            <span class="block text-gray-500">// Keunikan</span>
            <span class="text-white font-bold">Coffee to Code</span>
          </div>
        `;

        techPrefix.textContent = "01 //";
        techPrefix.classList.add('font-orbitron');
        techTitle.textContent = "[ TECH STACK & ACCESSORIES ]";
        techTitle.classList.add('font-orbitron');

        statsPrefix.textContent = "02 //";
        statsPrefix.classList.add('font-orbitron');
        statsTitle.textContent = "[ DATACENTER STATS ]";
        statsTitle.classList.add('font-orbitron');

        connectPrefix.textContent = "03 //";
        connectPrefix.classList.add('font-orbitron');
        connectTitle.textContent = "[ ESTABLISH CONNECTION ]";
        connectTitle.classList.add('font-orbitron');

        statCardTitle.textContent = "GANDI'S STATUS ENGINE";
        statCardTitle.classList.add('font-orbitron');
        langCardTitle.textContent = "LANGUAGE DISTRIBUTION";
        langCardTitle.classList.add('font-orbitron');

        statLabel1.textContent = "Stars Earned";
        statLabel2.textContent = "Total Commits";
        statLabel3.textContent = "PRs Merged";
        statLabel4.textContent = "Issues Solved";

        mailBtn.textContent = "TERMINAL MAIL";
        mailBtn.classList.add('font-orbitron');
        igBtn.textContent = "CYBER INSTAGRAM";
        igBtn.classList.add('font-orbitron');

        footerElement.innerHTML = "<code>// End of file. Copyright © 2026 GandiGan</code>";
        footerElement.classList.add('font-mono-cyber');
      }
    }

    // Sistem Animasi Typing Dinamis
    let typingTimer;
    function restartTyping(theme) {
      clearTimeout(typingTimer);
      
      let phrases = [];
      if (theme === 'green') {
        phrases = [
          "[>] GANDI AFRIYADI :: DEVELOPER",
          "[>] INITIALIZING PROFILE...",
          "[>] STATUS: STUDENT @UNISMUH"
        ];
      } else if (theme === 'purple') {
        phrases = [
          "[>] GANDI AFRIYADI :: SYNTH_DEV",
          "[>] BOOTING SYSTEM...",
          "[>] RETRO_WAVE_ONLINE"
        ];
      } else if (theme === 'amber') {
        phrases = [
          "[>] GANDI AFRIYADI :: AMBER_NET",
          "[>] DECRYPTING DATABASE...",
          "[>] ACCESS GRANTED"
        ];
      } else if (theme === 'ice') {
        phrases = [
          "[>] GANDI AFRIYADI :: ARCTIC_NODE",
          "[>] COOLING CPU...",
          "[>] TEMPERATURE OPTIMIZED"
        ];
      } else if (theme === 'pixel') {
        phrases = [
          "PLAYER 1: GANDI READY",
          "LEVEL 99 TECH INFORMATICS",
          "PRESS START TO PLAY!",
          "COLLECTING COFFEE POTIONS..."
        ];
      } else if (theme === 'minimal') {
        phrases = [
          "Gandi Afriyadi — Software Developer",
          "Crafting digital products with clean code",
          "Makassar, Indonesia"
        ];
      }

      let phraseIndex = 0;
      let characterIndex = 0;
      let currentText = "";
      let isDeleting = false;
      const textElement = document.getElementById("live-typing");

      function type() {
        const currentPhrase = phrases[phraseIndex];
        
        if (isDeleting) {
          currentText = currentPhrase.substring(0, characterIndex - 1);
          characterIndex--;
        } else {
          currentText = currentPhrase.substring(0, characterIndex + 1);
          characterIndex++;
        }

        textElement.textContent = currentText;

        let typeSpeed = 100;
        if (isDeleting) typeSpeed /= 2;

        if (!isDeleting && characterIndex === currentPhrase.length) {
          typeSpeed = 2000;
          isDeleting = true;
        } else if (isDeleting && characterIndex === 0) {
          isDeleting = false;
          phraseIndex = (phraseIndex + 1) % phrases.length;
          typeSpeed = 500;
        }

        typingTimer = setTimeout(type, typeSpeed);
      }

      type();
    }

    // Fungsi Clipboard Tradisional yang Aman untuk iFrame
    function copyToClipboard() {
      const codeText = document.getElementById('markdown-code-box').textContent;
      
      const tempTextArea = document.createElement('textarea');
      tempTextArea.value = codeText;
      document.body.appendChild(tempTextArea);
      tempTextArea.select();
      
      try {
        const successful = document.execCommand('copy');
        const btnText = document.getElementById('copy-btn-text');
        
        if (successful) {
          btnText.textContent = "BERHASIL DISALIN! ✓";
          setTimeout(() => {
            btnText.textContent = "SALIN KODE MARKDOWN";
          }, 3000);
        } else {
          alert('Gagal menyalin. Silakan seleksi kode manual.');
        }
      } catch (err) {
        console.error('Error copying text: ', err);
      }
      
      document.body.removeChild(tempTextArea);
    }

    // Inisialisasi awal saat halaman terbuka
    window.onload = function() {
      changeTheme('green');
    };
  </script>
</body>
</html>
