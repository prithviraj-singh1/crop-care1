<!DOCTYPE html>
<html lang="en" class="light">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CropCare - Digital Agricultural Intelligence Platform</title>

  <!-- Google Fonts: Inter & Outfit for modern typography -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Outfit:wght@500;600;700;800&display=swap" rel="stylesheet">

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            brand: {
              50: '#f0fdf4',
              100: '#dcfce7',
              200: '#bbf7d0',
              500: '#22c55e',
              600: '#16a34a',
              700: '#15803d',
              800: '#166534',
              900: '#064e3b',
              950: '#022c22',
            },
            amber: {
              500: '#f59e0b',
              600: '#d97706',
              700: '#b45309',
            },
            earth: {
              500: '#f97316',
              600: '#ea580c',
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            display: ['Outfit', 'sans-serif']
          }
        }
      }
    }
  </script>

  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />

  <style>
    /* Custom Scrollbars & Theme Polish */
    ::-webkit-scrollbar {
      width: 8px;
      height: 8px;
    }
    ::-webkit-scrollbar-track {
      background: rgba(0, 0, 0, 0.05);
    }
    ::-webkit-scrollbar-thumb {
      background: rgba(22, 163, 74, 0.3);
      border-radius: 9999px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: rgba(22, 163, 74, 0.6);
    }

    /* Vibrant Gradients & Glassmorphism */
    .bg-gradient-agri {
      background: linear-gradient(135deg, #064e3b 0%, #16a34a 50%, #84cc16 100%);
    }
    .bg-gradient-amber {
      background: linear-gradient(135deg, #b45309 0%, #d97706 50%, #f59e0b 100%);
    }
    .bg-gradient-card {
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.95) 0%, rgba(240, 253, 244, 0.6) 100%);
    }
    .dark .bg-gradient-card {
      background: linear-gradient(180deg, rgba(15, 23, 42, 0.95) 0%, rgba(6, 78, 59, 0.3) 100%);
    }

    /* High-contrast Farmer Mode */
    .farmer-mode {
      font-size: 1.1rem !important;
    }
    .farmer-mode button, .farmer-mode input, .farmer-mode select {
      min-height: 48px !important;
    }

    /* Audio wave animation */
    @keyframes wave {
      0%, 100% { height: 8px; }
      50% { height: 28px; }
    }
    .animate-wave-1 { animation: wave 1s infinite ease-in-out; }
    .animate-wave-2 { animation: wave 1s infinite ease-in-out 0.2s; }
    .animate-wave-3 { animation: wave 1s infinite ease-in-out 0.4s; }
    .animate-wave-4 { animation: wave 1s infinite ease-in-out 0.6s; }
  </style>
</head>

<body class="bg-slate-50 text-slate-800 dark:bg-slate-900 dark:text-slate-100 transition-colors duration-200 antialiased selection:bg-brand-500 selection:text-white font-sans min-h-screen flex flex-col">

  <!-- Top Navigation Header -->
  <header class="sticky top-0 z-40 bg-white/90 dark:bg-slate-900/90 backdrop-blur-md border-b border-brand-100 dark:border-brand-900 shadow-sm">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        
        <!-- Logo & Branding -->
        <div class="flex items-center space-x-3 cursor-pointer" onclick="scrollToSection('hero')">
          <div class="w-12 h-12 rounded-2xl bg-gradient-agri flex items-center justify-center text-white shadow-lg shadow-brand-500/30 transform hover:scale-105 transition-transform">
            <i class="fa-solid font-bold fa-leaf text-2xl"></i>
          </div>
          <div>
            <span class="font-display font-extrabold text-2xl tracking-tight text-brand-900 dark:text-brand-100 flex items-center gap-1.5">
              CropCare <span class="bg-brand-100 dark:bg-brand-900/60 text-brand-700 dark:text-brand-300 text-xs px-2.5 py-0.5 rounded-full font-sans font-semibold border border-brand-200 dark:border-brand-700">AI PRO</span>
            </span>
            <p class="text-xs font-medium text-slate-500 dark:text-slate-400 hidden sm:block" id="lang-subhead">Digital Agricultural Intelligence Hub</p>
          </div>
        </div>

        <!-- Desktop Navigation Items -->
        <nav class="hidden md:flex items-center space-x-1 lg:space-x-2 font-medium text-sm">
          <button onclick="scrollToSection('vision-studio')" class="px-3 py-2 rounded-xl text-slate-700 dark:text-slate-200 hover:text-brand-600 dark:hover:text-brand-400 hover:bg-brand-50 dark:hover:bg-slate-800 transition">
            <i class="fa-solid fa-microscope text-brand-600 mr-1.5"></i> <span data-i18n="nav_vision">Crop Vision</span>
          </button>
          <button onclick="scrollToSection('schemes-hub')" class="px-3 py-2 rounded-xl text-slate-700 dark:text-slate-200 hover:text-brand-600 dark:hover:text-brand-400 hover:bg-brand-50 dark:hover:bg-slate-800 transition">
            <i class="fa-solid fa-building-columns text-amber-600 mr-1.5"></i> <span data-i18n="nav_schemes">Govt Schemes</span>
          </button>
          <button onclick="scrollToSection('irrigation-tool')" class="px-3 py-2 rounded-xl text-slate-700 dark:text-slate-200 hover:text-brand-600 dark:hover:text-brand-400 hover:bg-brand-50 dark:hover:bg-slate-800 transition">
            <i class="fa-solid fa-droplet text-blue-500 mr-1.5"></i> <span data-i18n="nav_irrigation">Irrigation AI</span>
          </button>
          <button onclick="scrollToSection('mandi-weather')" class="px-3 py-2 rounded-xl text-slate-700 dark:text-slate-200 hover:text-brand-600 dark:hover:text-brand-400 hover:bg-brand-50 dark:hover:bg-slate-800 transition">
            <i class="fa-solid fa-chart-line text-emerald-600 mr-1.5"></i> <span data-i18n="nav_mandi">Mandi & Weather</span>
          </button>
        </nav>

        <!-- Right Tool Controls -->
        <div class="flex items-center space-x-2 sm:space-x-3">
          
          <!-- Farmer Profile Switcher Select -->
          <div class="relative hidden lg:block">
            <select id="farmer-profile-select" onchange="changeFarmerProfile(this.value)" class="bg-brand-50 dark:bg-slate-800 text-brand-900 dark:text-brand-200 font-medium text-xs rounded-xl px-3 py-2 border border-brand-200 dark:border-slate-700 focus:outline-none focus:ring-2 focus:ring-brand-500 cursor-pointer">
              <option value="haryana">🌾 Rajesh Kumar (Haryana - Rice/Wheat)</option>
              <option value="karnataka">🌴 Basavaraj Patil (Karnataka - Sugarcane)</option>
              <option value="maharashtra">🍇 Ramesh Shinde (Maharashtra - Grapes/Onion)</option>
            </select>
          </div>

          <!-- Multilingual Language Selector -->
          <div class="relative">
            <select id="lang-selector" onchange="switchLanguage(this.value)" class="bg-white dark:bg-slate-800 text-slate-700 dark:text-slate-200 font-semibold text-xs rounded-xl px-2.5 py-2 border border-slate-200 dark:border-slate-700 focus:outline-none focus:ring-2 focus:ring-brand-500 cursor-pointer shadow-sm">
              <option value="en">🇬🇧 English</option>
              <option value="hi">🇮🇳 हिन्दी (Hindi)</option>
              <option value="pa">🇮🇳 ਪੰਜਾਬੀ (Punjabi)</option>
              <option value="mr">🇮🇳 मराठी (Marathi)</option>
              <option value="kn">🇮🇳 ಕನ್ನಡ (Kannada)</option>
              <option value="te">🇮🇳 తెలుగు (Telugu)</option>
              <option value="ta">🇮🇳 தமிழ் (Tamil)</option>
              <option value="bn">🇮🇳 বাংলা (Bengali)</option>
            </select>
          </div>

          <!-- Dark / High Contrast Farmer Mode Toggles -->
          <button onclick="toggleDarkMode()" class="p-2 rounded-xl bg-slate-100 dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition" title="Toggle Dark Theme">
            <i class="fa-solid fa-moon dark:hidden"></i>
            <i class="fa-solid fa-sun hidden dark:inline text-amber-400"></i>
          </button>

          <button id="farmer-mode-btn" onclick="toggleFarmerMode()" class="px-3 py-1.5 rounded-xl text-xs font-bold bg-amber-100 dark:bg-amber-900/50 text-amber-800 dark:text-amber-200 border border-amber-300 dark:border-amber-700 hover:bg-amber-200 transition flex items-center gap-1.5" title="High Contrast & Large Font Mode">
            <i class="fa-solid fa-glasses"></i> <span class="hidden sm:inline" data-i18n="farmer_mode">Farmer Mode</span>
          </button>

          <!-- Notification Drawer Trigger -->
          <button onclick="toggleNotificationDrawer()" class="relative p-2 rounded-xl bg-brand-50 dark:bg-slate-800 text-brand-700 dark:text-brand-300 hover:bg-brand-100 dark:hover:bg-slate-700 transition">
            <i class="fa-regular fa-bell text-lg"></i>
            <span class="absolute top-1 right-1 w-2.5 h-2.5 bg-red-500 rounded-full ring-2 ring-white dark:ring-slate-900 animate-pulse"></span>
          </button>

        </div>
      </div>
    </div>
  </header>

  <!-- Hero Section -->
  <section id="hero" class="relative overflow-hidden bg-gradient-agri text-white py-12 lg:py-16">
    <div class="absolute inset-0 bg-[radial-gradient(ellipse_at_top_right,_var(--tw-gradient-stops))] from-white/10 via-transparent to-black/30 pointer-events-none"></div>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      
      <!-- Active Profile Banner -->
      <div class="mb-6 inline-flex items-center gap-2 bg-white/15 backdrop-blur-md px-4 py-2 rounded-full border border-white/20 text-xs sm:text-sm font-medium">
        <span class="w-2.5 h-2.5 rounded-full bg-emerald-300 animate-ping"></span>
        <span id="active-farmer-text">Logged in: <strong>Rajesh Kumar</strong> (Karnal, Haryana • 8.5 Acres • Rice/Wheat)</span>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
        <div class="lg:col-span-7 space-y-4">
          <h1 class="text-3xl sm:text-5xl font-extrabold tracking-tight leading-tight font-display" data-i18n="hero_title">
            Empowering Indian Farmers with Real-Time AI Intelligence & Direct Govt Grants
          </h1>
          <p class="text-emerald-100 text-base sm:text-lg max-w-2xl font-light leading-relaxed" data-i18n="hero_subtitle">
            Diagnose crop diseases in seconds, apply for 100% verified government schemes, calculate precise dynamic irrigation, and get AI-powered Mandi "Sell vs Hold" recommendations.
          </p>

          <div class="pt-2 flex flex-wrap gap-3">
            <button onclick="scrollToSection('vision-studio')" class="px-6 py-3.5 bg-white text-brand-900 font-bold rounded-2xl shadow-xl hover:bg-emerald-50 transition transform hover:-translate-y-0.5 flex items-center gap-2 text-sm sm:text-base">
              <i class="fa-solid fa-camera text-brand-600"></i> <span data-i18n="btn_scan_crop">Scan Crop Health Now</span>
            </button>
            <button onclick="scrollToSection('schemes-hub')" class="px-6 py-3.5 bg-brand-900/40 backdrop-blur-md text-white border border-white/30 font-semibold rounded-2xl hover:bg-brand-900/60 transition text-sm sm:text-base flex items-center gap-2">
              <i class="fa-solid fa-building-columns text-amber-300"></i> <span data-i18n="btn_explore_schemes">Explore 12+ Schemes</span>
            </button>
          </div>
        </div>

        <!-- Quick AI Weather & Soil Widget -->
        <div class="lg:col-span-5">
          <div class="bg-white/10 backdrop-blur-md border border-white/20 rounded-3xl p-6 text-white shadow-2xl">
            <div class="flex items-center justify-between pb-4 border-b border-white/10">
              <div>
                <p class="text-xs text-emerald-200 uppercase tracking-wider font-semibold" data-i18n="lbl_live_weather">Live Agri-Microclimate</p>
                <h3 class="text-xl font-bold font-display" id="hero-location-name">Karnal, Haryana</h3>
              </div>
              <div class="text-right">
                <span class="text-3xl font-extrabold font-display" id="hero-temp">29°C</span>
                <p class="text-xs text-emerald-200" id="hero-condition">Partly Cloudy</p>
              </div>
            </div>

            <div class="grid grid-cols-3 gap-3 my-4 text-center">
              <div class="bg-black/20 rounded-2xl p-2.5">
                <i class="fa-solid fa-droplet text-blue-300 mb-1"></i>
                <p class="text-[10px] text-emerald-200 uppercase">Humidity</p>
                <p class="font-bold text-sm" id="hero-humidity">68%</p>
              </div>
              <div class="bg-black/20 rounded-2xl p-2.5">
                <i class="fa-solid fa-mountain text-amber-300 mb-1"></i>
                <p class="text-[10px] text-emerald-200 uppercase">Soil Moisture</p>
                <p class="font-bold text-sm" id="hero-soil">42% (Optimal)</p>
              </div>
              <div class="bg-black/20 rounded-2xl p-2.5">
                <i class="fa-solid fa-wind text-emerald-300 mb-1"></i>
                <p class="text-[10px] text-emerald-200 uppercase">Wind Speed</p>
                <p class="font-bold text-sm" id="hero-wind">12 km/h</p>
              </div>
            </div>

            <div class="bg-emerald-950/50 rounded-2xl p-3 border border-emerald-400/30 flex items-center justify-between">
              <div class="flex items-center gap-2.5">
                <i class="fa-solid fa-bullhorn text-amber-400 text-lg"></i>
                <p class="text-xs text-emerald-100" id="hero-advisory">Light rain expected in 48 hrs. Pause nitrogen fertilizer application.</p>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- SECTION 1: Crop Vision Studio & Searchable Crop Selector -->
  <section id="vision-studio" class="py-12 lg:py-16 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center max-w-3xl mx-auto mb-10">
      <span class="px-3 py-1 bg-brand-100 dark:bg-brand-900/60 text-brand-700 dark:text-brand-300 rounded-full text-xs font-extrabold uppercase tracking-widest border border-brand-200 dark:border-brand-800" data-i18n="tag_ai_diagnosis">AI Diagnostics</span>
      <h2 class="text-3xl sm:text-4xl font-extrabold font-display text-slate-900 dark:text-white mt-2" data-i18n="title_crop_vision">
        Crop Vision AI Diagnostic Studio
      </h2>
      <p class="text-slate-600 dark:text-slate-400 text-sm sm:text-base mt-2" data-i18n="sub_crop_vision">
        Select from over 40+ Indian crops or upload a crop photo to instantly detect pests, blights, and deficiency diseases with precise bio-remedies.
      </p>
    </div>

    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
      
      <!-- Left Controls Panel -->
      <div class="lg:col-span-5 space-y-6">
        
        <!-- Searchable Crop Selector Box -->
        <div class="bg-white dark:bg-slate-800 rounded-3xl p-6 shadow-xl border border-slate-100 dark:border-slate-700/60">
          <label class="block text-xs font-bold text-slate-500 dark:text-slate-400 uppercase tracking-wider mb-2" data-i18n="lbl_select_crop">
            1. Select Target Crop (40+ Crop Database)
          </label>

          <!-- Search Filter Input -->
          <div class="relative mb-3">
            <i class="fa-solid fa-magnifying-glass absolute left-3.5 top-3 text-slate-400 text-xs"></i>
            <input type="text" id="crop-search-input" onkeyup="filterCropDropdown()" placeholder="Search crop e.g. Sugarcane, Mango, Tomato..." class="w-full pl-9 pr-3 py-2 text-xs sm:text-sm bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl focus:outline-none focus:ring-2 focus:ring-brand-500 dark:text-white">
          </div>

          <!-- Select List -->
          <select id="crop-select-dropdown" size="5" onchange="selectCropFromList(this.value)" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl p-2 text-xs sm:text-sm focus:outline-none focus:ring-2 focus:ring-brand-500 dark:text-white font-medium cursor-pointer max-h-48">
            <option value="Rice" selected>🌾 Rice / Paddy (चावल)</option>
            <option value="Wheat">🌾 Wheat (गेहूं)</option>
            <option value="Sugarcane">🎋 Sugarcane (गन्ना)</option>
            <option value="Cotton">🧵 Cotton (कपास)</option>
            <option value="Potato">🥔 Potato (आलू)</option>
            <option value="Tomato">🍅 Tomato (टमाटर)</option>
            <option value="Onion">🧅 Onion (प्याज)</option>
            <option value="Chili">🌶️ Chili (मिर्च)</option>
            <option value="Maize">🌽 Maize / Corn (मक्का)</option>
            <option value="Mustard">🌼 Mustard (सरसों)</option>
            <option value="Soybean">🫘 Soybean (सोयाबीन)</option>
            <option value="Mango">🥭 Mango (आम)</option>
            <option value="Banana">🍌 Banana (केला)</option>
            <option value="Grapes">🍇 Grapes (अंगूर)</option>
            <option value="Apple">🍎 Apple (सेब)</option>
            <option value="Papaya">🍈 Papaya (पपीता)</option>
            <option value="Groundnut">🥜 Groundnut (मूंगफली)</option>
            <option value="Gram">🫘 Gram / Cicer (चना)</option>
            <option value="Tur">🫘 Tur / Arhar Dal (तूर)</option>
            <option value="Jute">🌿 Jute (जूट)</option>
            <option value="Tea">🍃 Tea (चाय)</option>
            <option value="Coffee">☕ Coffee (कॉफी)</option>
            <option value="Guava">🍐 Guava (अमरूद)</option>
            <option value="Pomegranate">🍎 Pomegranate (अनार)</option>
            <option value="Brinjal">🍆 Brinjal / Eggplant (बैंगन)</option>
            <option value="Okra">🥬 Okra / Bhindi (भिंडी)</option>
            <option value="Garlic">🧄 Garlic (लहसुन)</option>
            <option value="Ginger">🫚 Ginger (अदरक)</option>
            <option value="Turmeric">🟡 Turmeric (हल्दी)</option>
            <option value="Cabbage">🥬 Cabbage (पत्तागोभी)</option>
            <option value="Cauliflower">🥦 Cauliflower (फूलगोभी)</option>
            <option value="Watermelon">🍉 Watermelon (तरबूज)</option>
            <option value="Muskmelon">🍈 Muskmelon (खरबूजा)</option>
            <option value="Black Gram">🫘 Urad / Black Gram (उड़द)</option>
            <option value="Green Gram">🫘 Moong / Green Gram (मूंग)</option>
            <option value="Castor">🌱 Castor (अंडी)</option>
            <option value="Sunflower">🌻 Sunflower (सूरजमुखी)</option>
            <option value="Sesame">⚪ Sesame (तिल)</option>
            <option value="Cardamom">🫛 Cardamom (इलायची)</option>
            <option value="Black Pepper">🖤 Black Pepper (काली मिर्च)</option>
          </select>
        </div>

        <!-- Diagnostic Mode Upload Box -->
        <div class="bg-white dark:bg-slate-800 rounded-3xl p-6 shadow-xl border border-slate-100 dark:border-slate-700/60">
          <label class="block text-xs font-bold text-slate-500 dark:text-slate-400 uppercase tracking-wider mb-3" data-i18n="lbl_upload_photo">
            2. Upload Leaf Photo or Pick Sample Case
          </label>

          <!-- Upload Dropzone Simulator -->
          <div onclick="triggerSimulatedUpload()" class="border-2 border-dashed border-brand-300 dark:border-brand-700 hover:border-brand-500 rounded-2xl p-6 text-center cursor-pointer bg-brand-50/50 dark:bg-slate-900/50 transition group">
            <div class="w-12 h-12 bg-brand-100 dark:bg-brand-900/60 text-brand-600 dark:text-brand-300 rounded-full flex items-center justify-center mx-auto mb-3 group-hover:scale-110 transition">
              <i class="fa-solid fa-cloud-arrow-up text-xl"></i>
            </div>
            <p class="text-xs font-bold text-slate-700 dark:text-slate-200" data-i18n="drop_zone_text">Click to upload crop leaf image</p>
            <p class="text-[11px] text-slate-400 mt-1">Supports JPG, PNG (Simulated Instant Diagnosis)</p>
          </div>

          <!-- Sample Issue Buttons -->
          <p class="text-[11px] font-bold text-slate-400 uppercase mt-4 mb-2">Or test sample issue preset:</p>
          <div class="grid grid-cols-2 gap-2">
            <button onclick="loadSampleDisease('blast')" class="text-left px-3 py-2 rounded-xl bg-slate-100 dark:bg-slate-700/50 hover:bg-brand-50 dark:hover:bg-slate-700 text-xs font-semibold text-slate-700 dark:text-slate-200 border border-slate-200 dark:border-slate-600 transition">
              <i class="fa-solid fa-bug text-amber-500 mr-1"></i> Rice Leaf Blast
            </button>
            <button onclick="loadSampleDisease('rust')" class="text-left px-3 py-2 rounded-xl bg-slate-100 dark:bg-slate-700/50 hover:bg-brand-50 dark:hover:bg-slate-700 text-xs font-semibold text-slate-700 dark:text-slate-200 border border-slate-200 dark:border-slate-600 transition">
              <i class="fa-solid fa-disease text-red-500 mr-1"></i> Wheat Yellow Rust
            </button>
            <button onclick="loadSampleDisease('borer')" class="text-left px-3 py-2 rounded-xl bg-slate-100 dark:bg-slate-700/50 hover:bg-brand-50 dark:hover:bg-slate-700 text-xs font-semibold text-slate-700 dark:text-slate-200 border border-slate-200 dark:border-slate-600 transition">
              <i class="fa-solid fa-locust text-emerald-600 mr-1"></i> Sugarcane Borer
            </button>
            <button onclick="loadSampleDisease('blight')" class="text-left px-3 py-2 rounded-xl bg-slate-100 dark:bg-slate-700/50 hover:bg-brand-50 dark:hover:bg-slate-700 text-xs font-semibold text-slate-700 dark:text-slate-200 border border-slate-200 dark:border-slate-600 transition">
              <i class="fa-solid fa-triangle-exclamation text-orange-500 mr-1"></i> Tomato Early Blight
            </button>
          </div>
        </div>

      </div>

      <!-- Right Diagnostic Output Display Studio -->
      <div class="lg:col-span-7">
        <div class="bg-white dark:bg-slate-800 rounded-3xl p-6 shadow-2xl border border-slate-100 dark:border-slate-700/60 relative overflow-hidden h-full flex flex-col justify-between">
          
          <div>
            <!-- Status Header -->
            <div class="flex items-center justify-between pb-4 border-b border-slate-100 dark:border-slate-700">
              <div class="flex items-center gap-3">
                <span class="px-3 py-1 rounded-full bg-red-100 dark:bg-red-900/40 text-red-700 dark:text-red-300 font-bold text-xs flex items-center gap-1.5" id="diag-severity">
                  <i class="fa-solid fa-circle-exclamation"></i> Moderate Infection (94% Match)
                </span>
                <span class="text-xs text-slate-400" id="diag-crop-tag">Crop: Rice / Paddy</span>
              </div>
              <button onclick="requestKvkConsultation()" class="px-3 py-1.5 rounded-xl bg-brand-600 hover:bg-brand-700 text-white font-bold text-xs transition flex items-center gap-1 shadow-md">
                <i class="fa-solid fa-user-doctor"></i> KVK Scientist Call
              </button>
            </div>

            <!-- Diagnosis Title & Banner -->
            <div class="my-4">
              <h3 class="text-2xl font-extrabold font-display text-slate-900 dark:text-white" id="diag-title">
                Magnaporthe Oryzae (Paddy Leaf Blast Fungus)
              </h3>
              <p class="text-xs text-slate-500 dark:text-slate-400 mt-1" id="diag-desc">
                Spindle-shaped lesions with grey center causing severe photosynthetic loss in rice tillers. High risk due to recent humidity levels (68%).
              </p>
            </div>

            <!-- Remedy Tabs (Chemical vs Organic Bio-Pesticide) -->
            <div class="mt-6">
              <div class="flex space-x-2 border-b border-slate-200 dark:border-slate-700 pb-2">
                <button id="btn-tab-organic" onclick="switchRemedyTab('organic')" class="px-4 py-2 rounded-xl font-bold text-xs bg-brand-600 text-white transition shadow-sm">
                  🌱 Organic Bio-Remedy (Recommended)
                </button>
                <button id="btn-tab-chemical" onclick="switchRemedyTab('chemical')" class="px-4 py-2 rounded-xl font-bold text-xs bg-slate-100 dark:bg-slate-700 text-slate-600 dark:text-slate-300 hover:bg-slate-200 transition">
                  🧪 Chemical Treatment
                </button>
              </div>

              <!-- Organic Content -->
              <div id="tab-organic-content" class="py-4 space-y-3">
                <div class="p-4 bg-brand-50/70 dark:bg-brand-950/40 border border-brand-200 dark:border-brand-800 rounded-2xl">
                  <h4 class="font-bold text-sm text-brand-900 dark:text-brand-200 flex items-center gap-2">
                    <i class="fa-solid fa-seedling text-brand-600"></i> Pseudomonas Fluorescens + Neem Oil Spray
                  </h4>
                  <p class="text-xs text-slate-600 dark:text-slate-300 mt-1">
                    Foliar spray with 10g/L bio-agent along with 5ml/L cold-pressed neem oil (10,000 PPM).
                  </p>
                </div>
              </div>

              <!-- Chemical Content (Hidden by default) -->
              <div id="tab-chemical-content" class="py-4 space-y-3 hidden">
                <div class="p-4 bg-amber-50/70 dark:bg-amber-950/40 border border-amber-200 dark:border-amber-800 rounded-2xl">
                  <h4 class="font-bold text-sm text-amber-900 dark:text-amber-200 flex items-center gap-2">
                    <i class="fa-solid fa-flask text-amber-600"></i> Tricyclazole 75% WP Spray
                  </h4>
                  <p class="text-xs text-slate-600 dark:text-slate-300 mt-1">
                    Apply Tricyclazole 0.6 grams per liter of water at early disease onset. Re-apply after 12 days if required.
                  </p>
                </div>
              </div>
            </div>

            <!-- Precise Dosage Calculator Component -->
            <div class="mt-4 p-4 bg-slate-50 dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-700">
              <div class="flex items-center justify-between mb-2">
                <label class="text-xs font-bold text-slate-700 dark:text-slate-300 uppercase tracking-wide">Dosage Calculator for Field Size</label>
                <span class="text-xs font-extrabold text-brand-600 dark:text-brand-400" id="dosage-calc-display">3.5 Acres</span>
              </div>
              <input type="range" id="dosage-acre-slider" min="0.5" max="25" step="0.5" value="3.5" oninput="calculateDosage(this.value)" class="w-full accent-brand-600 cursor-pointer">
              
              <div class="grid grid-cols-2 sm:grid-cols-3 gap-3 mt-3 text-center">
                <div class="bg-white dark:bg-slate-800 p-2.5 rounded-xl border border-slate-200 dark:border-slate-700">
                  <p class="text-[10px] text-slate-400 uppercase">Water Required</p>
                  <p class="font-extrabold text-sm text-slate-800 dark:text-white" id="dose-water">700 Liters</p>
                </div>
                <div class="bg-white dark:bg-slate-800 p-2.5 rounded-xl border border-slate-200 dark:border-slate-700">
                  <p class="text-[10px] text-slate-400 uppercase">Bio Quantity</p>
                  <p class="font-extrabold text-sm text-brand-600 dark:text-brand-400" id="dose-qty">7.0 Kg</p>
                </div>
                <div class="bg-white dark:bg-slate-800 p-2.5 rounded-xl border border-slate-200 dark:border-slate-700 col-span-2 sm:col-span-1">
                  <p class="text-[10px] text-slate-400 uppercase">Est. Treatment Cost</p>
                  <p class="font-extrabold text-sm text-emerald-600 dark:text-emerald-400" id="dose-cost">₹1,260</p>
                </div>
              </div>
            </div>

          </div>

          <!-- Bottom Action Bar -->
          <div class="pt-4 mt-6 border-t border-slate-100 dark:border-slate-700 flex flex-wrap items-center justify-between gap-3">
            <span class="text-xs text-slate-500 font-medium"><i class="fa-solid fa-shield-halved text-brand-600 mr-1"></i> ICAR & State Agri University Verified</span>
            <button onclick="shareDiagnosisWhatsApp()" class="px-4 py-2 bg-emerald-600 hover:bg-emerald-700 text-white text-xs font-bold rounded-xl transition flex items-center gap-2 shadow-md">
              <i class="fa-brands fa-whatsapp text-sm"></i> Send Advisory to WhatsApp
            </button>
          </div>

        </div>
      </div>

    </div>
  </section>

  <!-- SECTION 2: Comprehensive Government Schemes Hub -->
  <section id="schemes-hub" class="py-12 lg:py-16 bg-slate-100/70 dark:bg-slate-900/50 border-y border-slate-200 dark:border-slate-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <div class="flex flex-col md:flex-row md:items-end justify-between mb-8 gap-4">
        <div>
          <span class="px-3 py-1 bg-amber-100 dark:bg-amber-900/60 text-amber-800 dark:text-amber-200 rounded-full text-xs font-extrabold uppercase tracking-widest border border-amber-300 dark:border-amber-800" data-i18n="tag_schemes">Direct Subsidies</span>
          <h2 class="text-3xl sm:text-4xl font-extrabold font-display text-slate-900 dark:text-white mt-2" data-i18n="title_schemes">
            Government Schemes & Financial Grants
          </h2>
          <p class="text-slate-600 dark:text-slate-400 text-sm sm:text-base mt-1" data-i18n="sub_schemes">
            Filter 12+ Central & State agricultural schemes with eligibility verification & 1-click document checklists.
          </p>
        </div>

        <!-- Scheme Search Bar -->
        <div class="relative w-full md:w-72">
          <i class="fa-solid fa-magnifying-glass absolute left-3.5 top-3.5 text-slate-400 text-xs"></i>
          <input type="text" id="scheme-search-bar" onkeyup="filterSchemes()" placeholder="Search scheme e.g. PM-KISAN, Solar..." class="w-full pl-9 pr-3 py-2.5 text-xs sm:text-sm bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-2xl focus:outline-none focus:ring-2 focus:ring-amber-500 shadow-sm dark:text-white">
        </div>
      </div>

      <!-- Category Filter Tabs -->
      <div class="flex items-center space-x-2 overflow-x-auto pb-4 mb-6 no-scrollbar">
        <button onclick="filterSchemeCategory('all', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-amber-600 text-white shadow-md transition">
          All Schemes (12)
        </button>
        <button onclick="filterSchemeCategory('financial', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
          💰 Financial & Credit
        </button>
        <button onclick="filterSchemeCategory('insurance', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
          🛡️ Insurance & Safety
        </button>
        <button onclick="filterSchemeCategory('irrigation', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
          ☀️ Irrigation & Solar
        </button>
        <button onclick="filterSchemeCategory('machinery', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
          🚜 Tech & Machinery
        </button>
        <button onclick="filterSchemeCategory('organic', this)" class="scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
          🌿 Organic & Soil
        </button>
      </div>

      <!-- Schemes Grid Container -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6" id="schemes-grid">
        <!-- Dynamically Rendered via JS -->
      </div>

    </div>
  </section>

  <!-- SECTION 3 & 4: Smart Precision Irrigation Scheduler & Mandi Price Radar -->
  <section id="irrigation-tool" class="py-12 lg:py-16 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
      
      <!-- Smart Precision Irrigation Scheduler -->
      <div class="lg:col-span-6 bg-white dark:bg-slate-800 rounded-3xl p-6 sm:p-8 shadow-xl border border-slate-100 dark:border-slate-700/60">
        <div class="flex items-center gap-3 mb-6">
          <div class="w-12 h-12 rounded-2xl bg-blue-100 dark:bg-blue-900/50 text-blue-600 dark:text-blue-300 flex items-center justify-center text-xl shadow-md">
            <i class="fa-solid fa-droplet"></i>
          </div>
          <div>
            <h3 class="text-xl font-extrabold font-display text-slate-900 dark:text-white" data-i18n="title_irrigation">
              Smart Precision Irrigation AI
            </h3>
            <p class="text-xs text-slate-500 dark:text-slate-400" data-i18n="sub_irrigation">Dynamic water dosage calculation based on soil evapotranspiration.</p>
          </div>
        </div>

        <div class="space-y-5">
          <!-- Soil Moisture Input Slider -->
          <div>
            <div class="flex justify-between items-center mb-1">
              <label class="text-xs font-bold text-slate-700 dark:text-slate-300">Current Soil Moisture Sensor Reading</label>
              <span class="text-xs font-extrabold text-blue-600 dark:text-blue-400" id="moisture-slider-val">38% (Moderate)</span>
            </div>
            <input type="range" min="10" max="90" value="38" oninput="updateIrrigationCalc(this.value)" class="w-full accent-blue-600 cursor-pointer">
          </div>

          <!-- Weather Adjustment Notice -->
          <div class="p-3 bg-blue-50 dark:bg-blue-950/40 rounded-2xl border border-blue-200 dark:border-blue-900/50 text-xs flex items-center justify-between">
            <span class="text-slate-700 dark:text-slate-300"><i class="fa-solid fa-cloud-sun-rain text-blue-500 mr-1.5"></i> Weather Offset: 25% Rain Chance Tomorrow</span>
            <span class="font-bold text-blue-700 dark:text-blue-300">-15% Water Adjusted</span>
          </div>

          <!-- Calculated Output Card -->
          <div class="p-5 rounded-2xl bg-gradient-to-br from-blue-900 to-slate-900 text-white space-y-3 shadow-inner">
            <div class="flex justify-between items-center">
              <span class="text-xs text-blue-200 uppercase font-semibold">Recommended Water Run</span>
              <span class="px-2.5 py-0.5 rounded-full bg-blue-500/30 text-blue-200 text-xs font-bold border border-blue-400/30">Drip / Sprinkler</span>
            </div>
            <div class="text-3xl font-extrabold font-display text-blue-100" id="irrig-duration-output">
              1 Hour 45 Mins <span class="text-sm font-normal text-blue-300">(~18,500 Liters)</span>
            </div>
            <p class="text-xs text-blue-200/80">Best application window: Today 06:00 PM to minimize evaporation.</p>
          </div>

          <button onclick="triggerPumpTimerModal()" class="w-full py-3 bg-blue-600 hover:bg-blue-700 text-white font-bold text-xs sm:text-sm rounded-2xl transition shadow-lg flex items-center justify-center gap-2">
            <i class="fa-solid fa-power-off"></i> Set Automated Smart Pump Timer
          </button>
        </div>
      </div>

      <!-- Mandi Price Radar & Sell/Hold AI -->
      <div id="mandi-weather" class="lg:col-span-6 bg-white dark:bg-slate-800 rounded-3xl p-6 sm:p-8 shadow-xl border border-slate-100 dark:border-slate-700/60">
        <div class="flex items-center justify-between mb-6">
          <div class="flex items-center gap-3">
            <div class="w-12 h-12 rounded-2xl bg-emerald-100 dark:bg-emerald-900/50 text-emerald-600 dark:text-emerald-300 flex items-center justify-center text-xl shadow-md">
              <i class="fa-solid fa-chart-line"></i>
            </div>
            <div>
              <h3 class="text-xl font-extrabold font-display text-slate-900 dark:text-white" data-i18n="title_mandi">
                Agmarknet Mandi Radar
              </h3>
              <p class="text-xs text-slate-500 dark:text-slate-400" data-i18n="sub_mandi">Real-time market prices with AI Sell/Hold forecast.</p>
            </div>
          </div>
          <span class="px-2.5 py-1 bg-emerald-100 dark:bg-emerald-900/50 text-emerald-700 dark:text-emerald-300 text-[10px] font-extrabold rounded-full uppercase">Live Updates</span>
        </div>

        <!-- Mandi Price Table -->
        <div class="space-y-3">
          
          <div class="p-3 bg-slate-50 dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-700 flex items-center justify-between">
            <div>
              <div class="flex items-center gap-2">
                <span class="font-extrabold text-sm text-slate-800 dark:text-white">Paddy (Basmati 1509)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-100 dark:bg-emerald-900/60 text-emerald-700 dark:text-emerald-300 text-[10px] font-bold">Karnal Mandi</span>
              </div>
              <p class="text-xs text-slate-400 mt-0.5">MSP: ₹2,183/Qtl • Market: ₹3,850/Qtl</p>
            </div>
            <div class="text-right">
              <span class="inline-block px-2.5 py-1 bg-emerald-600 text-white text-xs font-extrabold rounded-xl shadow-sm">
                🟢 HOLD (Trend ↗ +6%)
              </span>
            </div>
          </div>

          <div class="p-3 bg-slate-50 dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-700 flex items-center justify-between">
            <div>
              <div class="flex items-center gap-2">
                <span class="font-extrabold text-sm text-slate-800 dark:text-white">Sugarcane (Co 0238)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-100 dark:bg-emerald-900/60 text-emerald-700 dark:text-emerald-300 text-[10px] font-bold">Mandya Mandi</span>
              </div>
              <p class="text-xs text-slate-400 mt-0.5">FRP: ₹315/Qtl • Factory Rate: ₹350/Qtl</p>
            </div>
            <div class="text-right">
              <span class="inline-block px-2.5 py-1 bg-blue-600 text-white text-xs font-extrabold rounded-xl shadow-sm">
                🔵 SELL TO MILL
              </span>
            </div>
          </div>

          <div class="p-3 bg-slate-50 dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-700 flex items-center justify-between">
            <div>
              <div class="flex items-center gap-2">
                <span class="font-extrabold text-sm text-slate-800 dark:text-white">Red Onion (Nashik)</span>
                <span class="px-2 py-0.5 rounded bg-emerald-100 dark:bg-emerald-900/60 text-emerald-700 dark:text-emerald-300 text-[10px] font-bold">Lasalgaon Mandi</span>
              </div>
              <p class="text-xs text-slate-400 mt-0.5">Market Rate: ₹2,400/Qtl</p>
            </div>
            <div class="text-right">
              <span class="inline-block px-2.5 py-1 bg-amber-600 text-white text-xs font-extrabold rounded-xl shadow-sm">
                🟡 SELL NOW (Peak)
              </span>
            </div>
          </div>

        </div>

        <div class="mt-4 pt-4 border-t border-slate-100 dark:border-slate-700 flex items-center justify-between text-xs text-slate-500">
          <span>Source: Ministry of Agriculture e-NAM API</span>
          <button onclick="showToast('Refreshed latest mandi prices across 12 markets!')" class="text-brand-600 dark:text-brand-400 font-bold hover:underline">
            <i class="fa-solid fa-rotate-right mr-1"></i> Refresh Prices
          </button>
        </div>

      </div>

    </div>
  </section>

  <!-- SECTION 5 & 6: Innovation Feed & Bhashini AI Voice Assistant -->
  <section class="py-12 lg:py-16 bg-slate-100/70 dark:bg-slate-900/50 border-t border-slate-200 dark:border-slate-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
        
        <!-- Agri-Tech Innovation Feed -->
        <div class="lg:col-span-7 space-y-6">
          <div>
            <span class="px-3 py-1 bg-brand-100 dark:bg-brand-900/60 text-brand-700 dark:text-brand-300 rounded-full text-xs font-extrabold uppercase tracking-widest border border-brand-200 dark:border-brand-800">Innovation Feed</span>
            <h2 class="text-2xl sm:text-3xl font-extrabold font-display text-slate-900 dark:text-white mt-2">
              ICAR Research & Drone CHC Rentals
            </h2>
          </div>

          <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
            
            <div class="bg-white dark:bg-slate-800 p-5 rounded-3xl border border-slate-100 dark:border-slate-700 shadow-md">
              <span class="px-2.5 py-0.5 rounded-full bg-emerald-100 dark:bg-emerald-900/60 text-emerald-700 dark:text-emerald-300 text-[10px] font-bold">Climate Resilient Variety</span>
              <h4 class="font-extrabold text-sm text-slate-900 dark:text-white mt-2">Pusa Basmati 1882 Released</h4>
              <p class="text-xs text-slate-500 dark:text-slate-400 mt-1">Bacterial blight resistant rice seed available at district KVK centers with 50% seed subsidy.</p>
            </div>

            <div class="bg-white dark:bg-slate-800 p-5 rounded-3xl border border-slate-100 dark:border-slate-700 shadow-md">
              <span class="px-2.5 py-0.5 rounded-full bg-amber-100 dark:bg-amber-900/60 text-amber-800 dark:text-amber-200 text-[10px] font-bold">Custom Hiring Center</span>
              <h4 class="font-extrabold text-sm text-slate-900 dark:text-white mt-2">Book Agri Drone Spraying</h4>
              <p class="text-xs text-slate-500 dark:text-slate-400 mt-1">Rent drone sprayers at ₹450/Acre via SMAM Scheme CHC centers nearby.</p>
            </div>

          </div>
        </div>

        <!-- Bhashini AI Voice Assistant Widget ("CropCare Mitra") -->
        <div class="lg:col-span-5 bg-gradient-to-br from-brand-900 via-brand-800 to-slate-900 rounded-3xl p-6 sm:p-8 text-white shadow-2xl relative overflow-hidden flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between pb-4 border-b border-white/10">
              <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-xl bg-white/10 flex items-center justify-center text-amber-300">
                  <i class="fa-solid fa-microphone-lines text-lg"></i>
                </div>
                <div>
                  <h3 class="font-extrabold font-display text-lg">CropCare Mitra</h3>
                  <p class="text-[11px] text-emerald-200">Bhashini AI Regional Voice Assistant</p>
                </div>
              </div>
              <span class="px-2 py-0.5 bg-emerald-500/20 text-emerald-300 text-[10px] rounded-full border border-emerald-400/30">Voice Active</span>
            </div>

            <!-- Audio Wave Visualizer Simulation -->
            <div class="my-6 flex items-center justify-center space-x-1.5 h-10 bg-black/20 rounded-2xl p-2" id="audio-wave-box">
              <div class="w-1.5 bg-emerald-400 rounded-full h-2"></div>
              <div class="w-1.5 bg-emerald-400 rounded-full h-2"></div>
              <div class="w-1.5 bg-emerald-400 rounded-full h-2"></div>
              <div class="w-1.5 bg-emerald-400 rounded-full h-2"></div>
              <div class="w-1.5 bg-emerald-400 rounded-full h-2"></div>
            </div>

            <p class="text-xs text-emerald-100 text-center font-medium" id="voice-status-text">
              "Press a button or speak in your native language to ask about crop diseases or subsidies."
            </p>
          </div>

          <!-- Regional Voice Query Buttons -->
          <div class="mt-6 space-y-2">
            <button onclick="simulateVoiceQuery('hi')" class="w-full py-2.5 px-3 bg-white/10 hover:bg-white/20 border border-white/20 rounded-xl text-xs font-semibold flex items-center justify-between transition">
              <span>🎤 "मेरी गेहूं की फसल में पीला रतुआ है, क्या करूं?"</span>
              <span class="text-[10px] text-emerald-300 font-bold">Hindi</span>
            </button>
            <button onclick="simulateVoiceQuery('kn')" class="w-full py-2.5 px-3 bg-white/10 hover:bg-white/20 border border-white/20 rounded-xl text-xs font-semibold flex items-center justify-between transition">
              <span>🎤 "ಕಬ್ಬಿನ ಸುಳಿ ಕೊರಕ ರೋಗಕ್ಕೆ ಔಷಧ ಯಾವುದು?"</span>
              <span class="text-[10px] text-emerald-300 font-bold">Kannada</span>
            </button>
          </div>

        </div>

      </div>

    </div>
  </section>

  <!-- Scheme Detail Modal -->
  <div id="scheme-modal" class="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm hidden flex items-center justify-center p-4">
    <div class="bg-white dark:bg-slate-800 rounded-3xl max-w-xl w-full p-6 sm:p-8 shadow-2xl border border-slate-100 dark:border-slate-700 relative max-h-[90vh] overflow-y-auto">
      <button onclick="closeSchemeModal()" class="absolute top-5 right-5 text-slate-400 hover:text-slate-600 dark:hover:text-slate-200">
        <i class="fa-solid fa-xmark text-xl"></i>
      </button>

      <div id="modal-scheme-body">
        <!-- Injected via JavaScript -->
      </div>
    </div>
  </div>

  <!-- Automated Pump Timer Modal -->
  <div id="pump-modal" class="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm hidden flex items-center justify-center p-4">
    <div class="bg-white dark:bg-slate-800 rounded-3xl max-w-md w-full p-6 shadow-2xl border border-slate-100 dark:border-slate-700 text-center">
      <div class="w-16 h-16 rounded-full bg-blue-100 dark:bg-blue-900/50 text-blue-600 dark:text-blue-300 flex items-center justify-center text-2xl mx-auto mb-4">
        <i class="fa-solid fa-plug"></i>
      </div>
      <h3 class="text-xl font-extrabold font-display text-slate-900 dark:text-white">Smart Pump Timer Set</h3>
      <p class="text-xs text-slate-500 dark:text-slate-400 mt-2">
        Scheduled 3 HP Tube Well Pump timer for <strong class="text-blue-600 dark:text-blue-400" id="pump-modal-time">1 Hour 45 Minutes</strong> via IoT Smart Relay.
      </p>
      
      <div class="my-6 p-4 bg-slate-50 dark:bg-slate-900 rounded-2xl border border-slate-200 dark:border-slate-700 text-left text-xs space-y-2">
        <div class="flex justify-between"><span class="text-slate-400">Target Field:</span> <span class="font-bold text-slate-700 dark:text-slate-200">Plot B (3.5 Acres)</span></div>
        <div class="flex justify-between"><span class="text-slate-400">Power Source:</span> <span class="font-bold text-slate-700 dark:text-slate-200">PM-KUSUM Solar Pump Grid</span></div>
        <div class="flex justify-between"><span class="text-slate-400">SMS Alert Trigger:</span> <span class="font-bold text-emerald-600">+91 98*** ***12</span></div>
      </div>

      <button onclick="closePumpModal()" class="w-full py-3 bg-brand-600 text-white font-bold text-xs rounded-xl shadow-md hover:bg-brand-700 transition">
        Confirm & Start Automated Cycle
      </button>
    </div>
  </div>

  <!-- Low Bandwidth SMS & WhatsApp Notification Drawer -->
  <div id="notification-drawer" class="fixed inset-y-0 right-0 z-50 w-full sm:w-96 bg-white dark:bg-slate-800 shadow-2xl border-l border-slate-200 dark:border-slate-700 transform translate-x-full transition-transform duration-300 ease-in-out p-6 flex flex-col justify-between">
    <div>
      <div class="flex items-center justify-between pb-4 border-b border-slate-100 dark:border-slate-700">
        <div class="flex items-center gap-2">
          <i class="fa-regular fa-bell text-brand-600 text-lg"></i>
          <h3 class="font-extrabold font-display text-slate-900 dark:text-white text-base">CropCare Push Center</h3>
        </div>
        <button onclick="toggleNotificationDrawer()" class="text-slate-400 hover:text-slate-600 dark:hover:text-slate-200">
          <i class="fa-solid fa-xmark text-lg"></i>
        </button>
      </div>

      <div class="mt-4 space-y-3">
        <div class="p-3 bg-brand-50 dark:bg-brand-950/40 rounded-2xl border border-brand-200 dark:border-brand-800 text-xs">
          <span class="font-bold text-brand-900 dark:text-brand-200 block">PM-KISAN 17th Installment Sent</span>
          <p class="text-slate-600 dark:text-slate-400 text-[11px] mt-0.5">₹2,000 credited to Aadhaar linked bank account xx4012.</p>
        </div>

        <div class="p-3 bg-amber-50 dark:bg-amber-950/40 rounded-2xl border border-amber-200 dark:border-amber-800 text-xs">
          <span class="font-bold text-amber-900 dark:text-amber-200 block">Rainfall Advisory Alert</span>
          <p class="text-slate-600 dark:text-slate-400 text-[11px] mt-0.5">Moderate rainfall expected in Karnal region over next 48 hours.</p>
        </div>
      </div>
    </div>

    <div class="pt-4 border-t border-slate-100 dark:border-slate-700">
      <button onclick="triggerLowBandwidthSms()" class="w-full py-2.5 bg-slate-100 dark:bg-slate-700 hover:bg-slate-200 text-slate-800 dark:text-slate-200 text-xs font-bold rounded-xl transition flex items-center justify-center gap-2">
        <i class="fa-solid fa-comment-sms text-brand-600"></i> Send Low-Bandwidth Offline SMS
      </button>
    </div>
  </div>

  <!-- Toast Notification Bar -->
  <div id="toast" class="fixed bottom-6 right-6 z-50 bg-slate-900 text-white px-5 py-3 rounded-2xl shadow-2xl border border-slate-700 text-xs font-semibold hidden flex items-center gap-2">
    <i class="fa-solid fa-circle-check text-emerald-400"></i> <span id="toast-message">Notification</span>
  </div>

  <!-- Footer -->
  <footer class="mt-auto bg-slate-900 text-slate-400 py-8 border-t border-slate-800 text-xs">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center space-y-2">
      <p class="font-medium text-slate-300">CropCare - Digital Agricultural Intelligence Platform © 2026</p>
      <p class="text-slate-500">Integrating Ministry of Agriculture & Farmers Welfare APIs • ICAR Approved AI Engine</p>
    </div>
  </footer>

  <!-- JavaScript Application Logic -->
  <script>
    /* ==========================================================================
       DATA STORES & SCHEMES DATABASE
       ========================================================================== */
    const farmerProfiles = {
      haryana: {
        name: "Rajesh Kumar",
        state: "Karnal, Haryana",
        acreage: "8.5 Acres",
        crops: "Rice / Wheat",
        temp: "29°C",
        condition: "Partly Cloudy",
        humidity: "68%",
        soil: "42% (Optimal)",
        wind: "12 km/h",
        advisory: "Light rain expected in 48 hrs. Pause nitrogen fertilizer application."
      },
      karnataka: {
        name: "Basavaraj Patil",
        state: "Mandya, Karnataka",
        acreage: "12.0 Acres",
        crops: "Sugarcane / Paddy",
        temp: "31°C",
        condition: "Sunny",
        humidity: "55%",
        soil: "31% (Dry)",
        wind: "18 km/h",
        advisory: "High evapotranspiration detected. Schedule drip irrigation for Sugarcane Plot 2."
      },
      maharashtra: {
        name: "Ramesh Shinde",
        state: "Nashik, Maharashtra",
        acreage: "6.0 Acres",
        crops: "Grapes / Onion",
        temp: "27°C",
        condition: "Overcast",
        humidity: "74%",
        soil: "48% (High)",
        wind: "9 km/h",
        advisory: "High humidity risk for Downy Mildew in Grapes. Consider preventive organic neem spray."
      }
    };

    const schemesDatabase = [
      {
        id: "pm-kisan",
        title: "PM-KISAN Samman Nidhi",
        category: "financial",
        benefit: "₹6,000 / Year Direct Transfer",
        desc: "Direct income support of ₹6,000 per year in three equal installments to all landholding farmer families across India.",
        docs: ["Aadhaar Card", "Land Ownership Registry (Khatoni)", "Active Bank Account"],
        portal: "https://pmkisan.gov.in",
        score: "100% Eligible"
      },
      {
        id: "pmfby",
        title: "PM Fasal Bima Yojana (PMFBY)",
        category: "insurance",
        benefit: "Comprehensive Crop Risk Coverage",
        desc: "Financial support to farmers suffering crop loss/damage arising out of non-preventable natural calamities at lowest premium rates (1.5% - 2%).",
        docs: ["Sowing Certificate", "Land Bank Passbook", "Aadhaar Card"],
        portal: "https://pmfby.gov.in",
        score: "100% Eligible"
      },
      {
        id: "kcc",
        title: "Kisan Credit Card (KCC)",
        category: "financial",
        benefit: "Low Interest Agri Credit (4% Effective)",
        desc: "Access to timely credit for agricultural and allied requirements at highly subsidized interest rates with interest subvention.",
        docs: ["Land Documents", "Passport Photo", "Identity Proof"],
        portal: "https://sansad.in",
        score: "95% Eligible"
      },
      {
        id: "pmksy",
        title: "PMKSY - Per Drop More Crop",
        category: "irrigation",
        benefit: "55% - 80% Subsidy on Drip Irrigation",
        desc: "Financial assistance for installing micro-irrigation systems (drip and sprinkler) to maximize water use efficiency.",
        docs: ["Water Source Proof", "Land Registry", "Aadhaar Card"],
        portal: "https://pmksy.gov.in",
        score: "90% Eligible"
      },
      {
        id: "kusum",
        title: "PM-KUSUM Solar Pump Scheme",
        category: "irrigation",
        benefit: "up to 90% Solar Pump Subsidy",
        desc: "Installation of standalone solar agriculture pumps to replace diesel pumps and solarization of grid-connected agricultural pumps.",
        docs: ["Land Records", "Electricity Connection Copy", "Bank Passbook"],
        portal: "https://pmkusum.mnre.gov.in",
        score: "85% Eligible"
      },
      {
        id: "pkvy",
        title: "Paramparagat Krishi Vikas Yojana (PKVY)",
        category: "organic",
        benefit: "₹50,000 / Hectare Organic Support",
        desc: "Promotes organic farming through cluster approach with financial assistance for bio-inputs, certification, and packaging.",
        docs: ["Farmer Group Registry", "Aadhaar Card", "Soil Test Report"],
        portal: "https://pgsindia-ncof.gov.in",
        score: "90% Eligible"
      },
      {
        id: "smam",
        title: "Sub-Mission on Agricultural Mechanization",
        category: "machinery",
        benefit: "40% - 80% Machinery & Drone Subsidy",
        desc: "Financial assistance for purchasing tractors, harvesters, agricultural drones, and setting up Custom Hiring Centers (CHCs).",
        docs: ["Aadhaar", "Caste Certificate (if applicable)", "Bank Details"],
        portal: "https://agrimachinery.nic.in",
        score: "88% Eligible"
      },
      {
        id: "aif",
        title: "Agriculture Infrastructure Fund (AIF)",
        category: "financial",
        benefit: "3% Interest Subvention on Loans",
        desc: "Medium-long term debt financing facility for investment in viable projects for post-harvest management infrastructure & cold storage.",
        docs: ["DPR Project Report", "Land Lease/Ownership", "KYC Docs"],
        portal: "https://agriinfra.dac.gov.in",
        score: "80% Eligible"
      },
      {
        id: "shc",
        title: "Soil Health Card Scheme",
        category: "organic",
        benefit: "Free Soil Testing & Nutrient Cards",
        desc: "Provides customized soil health status cards advising macro & micro-nutrient dosage to lower fertilizer costs.",
        docs: ["Soil Sample ID", "Aadhaar Card"],
        portal: "https://soilhealth.dac.gov.in",
        score: "100% Eligible"
      },
      {
        id: "enam",
        title: "e-NAM National Agriculture Market",
        category: "financial",
        benefit: "Direct Online Bidding Pan-India",
        desc: "Pan-India electronic trading portal networking existing APMC mandis to create a unified national market for commodities.",
        docs: ["Mandi Gate Pass", "Bank Account Details", "Aadhaar Card"],
        portal: "https://enam.gov.in",
        score: "100% Eligible"
      },
      {
        id: "midh",
        title: "Mission for Integrated Dev of Horticulture",
        category: "organic",
        benefit: "Subsidy for Orchards & Polyhouses",
        desc: "Holistic growth of the horticulture sector covering fruits, vegetables, root & tuber crops, mushroom, and spices.",
        docs: ["Land Title", "Horticulture Proposal", "Aadhaar"],
        portal: "https://midh.gov.in",
        score: "85% Eligible"
      },
      {
        id: "rkvy",
        title: "Rashtriya Krishi Vikas Yojana (RKVY)",
        category: "machinery",
        benefit: "Flexible State Level Agri Grants",
        desc: "Incentivizes states to increase public investment in agriculture and allied sectors tailored to local crop priorities.",
        docs: ["State Registration", "Aadhaar", "Land Record"],
        portal: "https://rkvy.nic.in",
        score: "90% Eligible"
      }
    ];

    const translations = {
      en: {
        nav_vision: "Crop Vision",
        nav_schemes: "Govt Schemes",
        nav_irrigation: "Irrigation AI",
        nav_mandi: "Mandi & Weather",
        farmer_mode: "Farmer Mode",
        hero_title: "Empowering Indian Farmers with Real-Time AI Intelligence & Direct Govt Grants",
        hero_subtitle: "Diagnose crop diseases in seconds, apply for 100% verified government schemes, calculate precise dynamic irrigation, and get AI-powered Mandi 'Sell vs Hold' recommendations.",
        btn_scan_crop: "Scan Crop Health Now",
        btn_explore_schemes: "Explore 12+ Schemes",
        lbl_live_weather: "Live Agri-Microclimate",
        tag_ai_diagnosis: "AI Diagnostics",
        title_crop_vision: "Crop Vision AI Diagnostic Studio",
        sub_crop_vision: "Select from over 40+ Indian crops or upload a crop photo to instantly detect pests, blights, and deficiency diseases with precise bio-remedies.",
        lbl_select_crop: "1. Select Target Crop (40+ Crop Database)",
        lbl_upload_photo: "2. Upload Leaf Photo or Pick Sample Case",
        drop_zone_text: "Click to upload crop leaf image",
        tag_schemes: "Direct Subsidies",
        title_schemes: "Government Schemes & Financial Grants",
        sub_schemes: "Filter 12+ Central & State agricultural schemes with eligibility verification & 1-click document checklists.",
        title_irrigation: "Smart Precision Irrigation AI",
        sub_irrigation: "Dynamic water dosage calculation based on soil evapotranspiration.",
        title_mandi: "Agmarknet Mandi Radar",
        sub_mandi: "Real-time market prices with AI Sell/Hold forecast."
      },
      hi: {
        nav_vision: "फसल दृष्टि",
        nav_schemes: "सरकारी योजनाएं",
        nav_irrigation: "सिंचाई एआई",
        nav_mandi: "मंडी और मौसम",
        farmer_mode: "किसान मोड",
        hero_title: "रियल-टाइम एआई इंटेलिजेंस और सीधी सरकारी सब्सिडी के साथ भारतीय किसानों का सशक्तिकरण",
        hero_subtitle: "सेकंडों में फसल रोगों का निदान करें, सत्यापित सरकारी योजनाओं के लिए आवेदन करें, और मंडी में 'बेचें या रोकें' सिफारिशें प्राप्त करें।",
        btn_scan_crop: "फसल स्वास्थ्य स्कैन करें",
        btn_explore_schemes: "12+ योजनाएं देखें",
        lbl_live_weather: "लाइव कृषि-मौसम",
        tag_ai_diagnosis: "एआई रोग निदान",
        title_crop_vision: "क्रॉप विजन एआई डायग्नोस्टिक स्टूडियो",
        sub_crop_vision: "40+ भारतीय फसलों में से चुनें या कीड़ों और रोगों का तुरंत पता लगाने के लिए फोटो अपलोड करें।",
        lbl_select_crop: "1. फसल का चयन करें (40+ फसल डेटाबेस)",
        lbl_upload_photo: "2. पत्ती की फोटो अपलोड करें या नमूना चुनें",
        drop_zone_text: "फसल की फोटो अपलोड करने के लिए क्लिक करें",
        tag_schemes: "सीधी सब्सिडी",
        title_schemes: "सरकारी योजनाएं और वित्तीय सहायता",
        sub_schemes: "पात्रता जांच और दस्तावेज़ चेकलिस्ट के साथ 12+ केंद्रीय और राज्य योजनाओं को फ़िल्टर करें।",
        title_irrigation: "स्मार्ट सटीक सिंचाई एआई",
        sub_irrigation: "मिट्टी की नमी के आधार पर पानी की खुराक की गणना।",
        title_mandi: "एगमार्कनेट मंडी भाव",
        sub_mandi: "एआई बेचें/रोकें पूर्वानुमान के साथ वास्तविक समय के मंडी भाव।"
      }
    };

    /* ==========================================================================
       INITIALIZATION & INTERACTION LOGIC
       ========================================================================== */
    window.onload = function() {
      renderSchemes(schemesDatabase);
    };

    // Smooth Scroll Helper
    function scrollToSection(id) {
      const element = document.getElementById(id);
      if (element) {
        element.scrollIntoView({ behavior: 'smooth' });
      }
    }

    // Farmer Profile Switcher
    function changeFarmerProfile(profileKey) {
      const p = farmerProfiles[profileKey];
      if (!p) return;

      document.getElementById('active-farmer-text').innerHTML = 
        `Logged in: <strong>${p.name}</strong> (${p.state} • ${p.acreage} • ${p.crops})`;

      document.getElementById('hero-location-name').innerText = p.state;
      document.getElementById('hero-temp').innerText = p.temp;
      document.getElementById('hero-condition').innerText = p.condition;
      document.getElementById('hero-humidity').innerText = p.humidity;
      document.getElementById('hero-soil').innerText = p.soil;
      document.getElementById('hero-wind').innerText = p.wind;
      document.getElementById('hero-advisory').innerText = p.advisory;

      showToast(`Switched to Farmer Profile: ${p.name} (${p.state})`);
    }

    // Multilingual Translation Switcher
    function switchLanguage(langCode) {
      const dict = translations[langCode] || translations['en'];
      document.querySelectorAll('[data-i18n]').forEach(el => {
        const key = el.getAttribute('data-i18n');
        if (dict[key]) {
          el.innerText = dict[key];
        }
      });
      showToast(`Language changed to ${langCode.toUpperCase()}`);
    }

    // Dark Mode Toggle
    function toggleDarkMode() {
      const htmlClass = document.documentElement.classList;
      if (htmlClass.contains('dark')) {
        htmlClass.remove('dark');
        showToast("Light mode enabled");
      } else {
        htmlClass.add('dark');
        showToast("Dark mode enabled");
      }
    }

    // High Contrast Farmer Mode Toggle
    function toggleFarmerMode() {
      const body = document.body;
      const btn = document.getElementById('farmer-mode-btn');
      if (body.classList.contains('farmer-mode')) {
        body.classList.remove('farmer-mode');
        btn.classList.remove('ring-4', 'ring-amber-500');
        showToast("Farmer Mode Disabled");
      } else {
        body.classList.add('farmer-mode');
        btn.classList.add('ring-4', 'ring-amber-500');
        showToast("Farmer Mode Enabled (Large Fonts & Spacing)");
      }
    }

    /* ==========================================================================
       CROP VISION AI STUDIO & SEARCHABLE DROPDOWN
       ========================================================================== */
    function filterCropDropdown() {
      const input = document.getElementById('crop-search-input').value.toLowerCase();
      const select = document.getElementById('crop-select-dropdown');
      const options = select.getElementsByTagName('option');

      for (let i = 0; i < options.length; i++) {
        const txt = options[i].text.toLowerCase();
        if (txt.includes(input)) {
          options[i].style.display = "";
        } else {
          options[i].style.display = "none";
        }
      }
    }

    function selectCropFromList(cropName) {
      document.getElementById('diag-crop-tag').innerText = `Crop: ${cropName}`;
      showToast(`Target Crop updated to: ${cropName}`);
    }

    function triggerSimulatedUpload() {
      showToast("Scanning leaf tissue with AI vision model...");
      setTimeout(() => {
        loadSampleDisease('blast');
      }, 800);
    }

    function loadSampleDisease(type) {
      const titleEl = document.getElementById('diag-title');
      const descEl = document.getElementById('diag-desc');
      const severityEl = document.getElementById('diag-severity');
      const cropTag = document.getElementById('diag-crop-tag');

      if (type === 'blast') {
        titleEl.innerText = "Magnaporthe Oryzae (Paddy Leaf Blast)";
        descEl.innerText = "Spindle-shaped lesions with grey center causing severe photosynthetic loss in rice tillers.";
        severityEl.className = "px-3 py-1 rounded-full bg-red-100 dark:bg-red-900/40 text-red-700 dark:text-red-300 font-bold text-xs flex items-center gap-1.5";
        severityEl.innerHTML = '<i class="fa-solid fa-circle-exclamation"></i> Moderate Infection (94% Match)';
        cropTag.innerText = "Crop: Rice / Paddy";
      } else if (type === 'rust') {
        titleEl.innerText = "Puccinia Striiformis (Wheat Yellow Rust)";
        descEl.innerText = "Linear yellow pustules along leaf veins causing rapid leaf chlorosis and grain yield drop.";
        severityEl.className = "px-3 py-1 rounded-full bg-amber-100 dark:bg-amber-900/40 text-amber-700 dark:text-amber-300 font-bold text-xs flex items-center gap-1.5";
        severityEl.innerHTML = '<i class="fa-solid fa-triangle-exclamation"></i> High Infection Risk (97% Match)';
        cropTag.innerText = "Crop: Wheat";
      } else if (type === 'borer') {
        titleEl.innerText = "Chilo Sacchariphagus (Sugarcane Top Borer)";
        descEl.innerText = "Dead hearts formed in young crop shoot caused by larval tunneling inside central shoot.";
        severityEl.className = "px-3 py-1 rounded-full bg-red-100 dark:bg-red-900/40 text-red-700 dark:text-red-300 font-bold text-xs flex items-center gap-1.5";
        severityEl.innerHTML = '<i class="fa-solid fa-bug"></i> Active Pest Attack (91% Match)';
        cropTag.innerText = "Crop: Sugarcane";
      } else if (type === 'blight') {
        titleEl.innerText = "Alternaria Solani (Tomato Early Blight)";
        descEl.innerText = "Concentric bullseye dark spots on lower leaves leading to premature leaf drop.";
        severityEl.className = "px-3 py-1 rounded-full bg-amber-100 dark:bg-amber-900/40 text-amber-700 dark:text-amber-300 font-bold text-xs flex items-center gap-1.5";
        severityEl.innerHTML = '<i class="fa-solid fa-disease"></i> Early Stage Infection (89% Match)';
        cropTag.innerText = "Crop: Tomato";
      }

      showToast(`Loaded sample diagnostic for ${type.toUpperCase()}`);
    }

    function switchRemedyTab(tabType) {
      const orgBtn = document.getElementById('btn-tab-organic');
      const chemBtn = document.getElementById('btn-tab-chemical');
      const orgContent = document.getElementById('tab-organic-content');
      const chemContent = document.getElementById('tab-chemical-content');

      if (tabType === 'organic') {
        orgBtn.className = "px-4 py-2 rounded-xl font-bold text-xs bg-brand-600 text-white transition shadow-sm";
        chemBtn.className = "px-4 py-2 rounded-xl font-bold text-xs bg-slate-100 dark:bg-slate-700 text-slate-600 dark:text-slate-300 hover:bg-slate-200 transition";
        orgContent.classList.remove('hidden');
        chemContent.classList.add('hidden');
      } else {
        chemBtn.className = "px-4 py-2 rounded-xl font-bold text-xs bg-amber-600 text-white transition shadow-sm";
        orgBtn.className = "px-4 py-2 rounded-xl font-bold text-xs bg-slate-100 dark:bg-slate-700 text-slate-600 dark:text-slate-300 hover:bg-slate-200 transition";
        chemContent.classList.remove('hidden');
        orgContent.classList.add('hidden');
      }
    }

    function calculateDosage(acres) {
      document.getElementById('dosage-calc-display').innerText = `${acres} Acres`;
      const water = Math.round(acres * 200);
      const bioQty = (acres * 2.0).toFixed(1);
      const cost = Math.round(acres * 360);

      document.getElementById('dose-water').innerText = `${water} Liters`;
      document.getElementById('dose-qty').innerText = `${bioQty} Kg`;
      document.getElementById('dose-cost').innerText = `₹${cost.toLocaleString('en-IN')}`;
    }

    function requestKvkConsultation() {
      showToast("Connecting with Karnal Krishi Vigyan Kendra (KVK) Agri Scientist...");
    }

    function shareDiagnosisWhatsApp() {
      const text = encodeURIComponent("CropCare AI Diagnosis: Paddy Leaf Blast detected. Bio-remedy: Pseudomonas Fluorescens (2kg/acre).");
      window.open(`https://api.whatsapp.com/send?text=${text}`, '_blank');
    }

    /* ==========================================================================
       GOVERNMENT SCHEMES HUB RENDER & FILTER LOGIC
       ========================================================================== */
    function renderSchemes(schemes) {
      const grid = document.getElementById('schemes-grid');
      grid.innerHTML = "";

      if (schemes.length === 0) {
        grid.innerHTML = `<div class="col-span-full text-center py-12 text-slate-400 font-medium">No matching government schemes found.</div>`;
        return;
      }

      schemes.forEach(s => {
        const card = document.createElement('div');
        card.className = "bg-white dark:bg-slate-800 rounded-3xl p-6 shadow-xl border border-slate-100 dark:border-slate-700/60 hover:shadow-2xl hover:border-amber-400/50 transition flex flex-col justify-between group";
        
        card.innerHTML = `
          <div>
            <div class="flex items-center justify-between gap-2 mb-3">
              <span class="px-2.5 py-0.5 rounded-full bg-amber-100 dark:bg-amber-900/60 text-amber-800 dark:text-amber-200 font-extrabold text-[10px] uppercase">${s.benefit}</span>
              <span class="text-[10px] font-bold text-emerald-600 dark:text-emerald-400 bg-emerald-50 dark:bg-emerald-950/60 px-2 py-0.5 rounded-full">${s.score}</span>
            </div>
            <h3 class="text-lg font-extrabold font-display text-slate-900 dark:text-white group-hover:text-amber-600 dark:group-hover:text-amber-400 transition">${s.title}</h3>
            <p class="text-xs text-slate-500 dark:text-slate-400 mt-2 line-clamp-3">${s.desc}</p>
          </div>

          <div class="mt-6 pt-4 border-t border-slate-100 dark:border-slate-700/80 flex items-center justify-between">
            <span class="text-[11px] font-semibold text-slate-400"><i class="fa-solid fa-file-check text-brand-600 mr-1"></i> 3 Docs Required</span>
            <button onclick="openSchemeModal('${s.id}')" class="px-3 py-1.5 bg-amber-500 hover:bg-amber-600 text-white font-bold text-xs rounded-xl shadow-md transition flex items-center gap-1">
              Apply & Checklist <i class="fa-solid fa-arrow-right text-[10px]"></i>
            </button>
          </div>
        `;
        grid.appendChild(card);
      });
    }

    function filterSchemeCategory(cat, btn) {
      document.querySelectorAll('.scheme-tab-btn').forEach(b => {
        b.className = "scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-white dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition";
      });
      btn.className = "scheme-tab-btn px-4 py-2 rounded-2xl text-xs font-bold whitespace-nowrap bg-amber-600 text-white shadow-md transition";

      if (cat === 'all') {
        renderSchemes(schemesDatabase);
      } else {
        const filtered = schemesDatabase.filter(s => s.category === cat);
        renderSchemes(filtered);
      }
    }

    function filterSchemes() {
      const query = document.getElementById('scheme-search-bar').value.toLowerCase();
      const filtered = schemesDatabase.filter(s => 
        s.title.toLowerCase().includes(query) || s.desc.toLowerCase().includes(query)
      );
      renderSchemes(filtered);
    }

    function openSchemeModal(id) {
      const s = schemesDatabase.find(item => item.id === id);
      if (!s) return;

      const body = document.getElementById('modal-scheme-body');
      body.innerHTML = `
        <div class="flex items-center gap-2 mb-2">
          <span class="px-2.5 py-0.5 bg-amber-100 dark:bg-amber-900/60 text-amber-800 dark:text-amber-200 text-xs font-bold rounded-full uppercase">${s.benefit}</span>
          <span class="px-2 py-0.5 bg-emerald-100 text-emerald-800 text-xs font-bold rounded-full">${s.score}</span>
        </div>
        <h2 class="text-2xl font-extrabold font-display text-slate-900 dark:text-white">${s.title}</h2>
        <p class="text-xs text-slate-500 dark:text-slate-400 mt-2">${s.desc}</p>

        <div class="my-6">
          <h4 class="text-xs font-bold text-slate-700 dark:text-slate-300 uppercase tracking-wider mb-3">Required Document Checklist:</h4>
          <div class="space-y-2">
            ${s.docs.map(doc => `
              <div class="flex items-center gap-2 text-xs font-medium text-slate-800 dark:text-slate-200 bg-slate-50 dark:bg-slate-900 p-2.5 rounded-xl border border-slate-200 dark:border-slate-700">
                <i class="fa-solid fa-square-check text-emerald-500 text-sm"></i> ${doc}
              </div>
            `).join('')}
          </div>
        </div>

        <div class="flex items-center gap-3">
          <a href="${s.portal}" target="_blank" class="flex-1 py-3 bg-amber-600 hover:bg-amber-700 text-white font-bold text-xs text-center rounded-xl transition shadow-lg">
            Direct Official Portal Link <i class="fa-solid fa-arrow-up-right-from-square ml-1 text-[10px]"></i>
          </a>
          <button onclick="closeSchemeModal()" class="py-3 px-4 bg-slate-100 dark:bg-slate-700 text-slate-700 dark:text-slate-200 font-bold text-xs rounded-xl hover:bg-slate-200 transition">
            Close
          </button>
        </div>
      `;

      document.getElementById('scheme-modal').classList.remove('hidden');
    }

    function closeSchemeModal() {
      document.getElementById('scheme-modal').classList.add('hidden');
    }

    /* ==========================================================================
       IRRIGATION & MODAL TOOL HANDLERS
       ========================================================================== */
    function updateIrrigationCalc(val) {
      const display = document.getElementById('moisture-slider-val');
      const output = document.getElementById('irrig-duration-output');
      
      let status = "Optimal";
      let timeStr = "1 Hour 15 Mins (~14,000 Liters)";

      if (val < 25) {
        status = "Critically Dry";
        timeStr = "2 Hours 30 Mins (~26,000 Liters)";
      } else if (val < 45) {
        status = "Moderate";
        timeStr = "1 Hour 45 Mins (~18,500 Liters)";
      } else if (val < 70) {
        status = "Adequate";
        timeStr = "45 Mins (~8,000 Liters)";
      } else {
        status = "Saturated (Pause Water)";
        timeStr = "0 Mins (No Irrigation Required)";
      }

      display.innerText = `${val}% (${status})`;
      output.innerText = timeStr;
    }

    function triggerPumpTimerModal() {
      const timeText = document.getElementById('irrig-duration-output').innerText.split('(')[0];
      document.getElementById('pump-modal-time').innerText = timeText;
      document.getElementById('pump-modal').classList.remove('hidden');
    }

    function closePumpModal() {
      document.getElementById('pump-modal').classList.add('hidden');
      showToast("Smart IoT Pump Timer successfully synchronized!");
    }

    /* ==========================================================================
       BHASHINI AI VOICE & NOTIFICATION DRAWER
       ========================================================================== */
    function simulateVoiceQuery(lang) {
      const waveBox = document.getElementById('audio-wave-box');
      const statusText = document.getElementById('voice-status-text');

      waveBox.children[0].className = "w-1.5 bg-emerald-400 rounded-full animate-wave-1";
      waveBox.children[1].className = "w-1.5 bg-emerald-400 rounded-full animate-wave-2";
      waveBox.children[2].className = "w-1.5 bg-emerald-400 rounded-full animate-wave-3";
      waveBox.children[3].className = "w-1.5 bg-emerald-400 rounded-full animate-wave-4";

      statusText.innerText = "Listening and processing query with Bhashini Neural Model...";

      setTimeout(() => {
        for (let child of waveBox.children) {
          child.className = "w-1.5 bg-emerald-400 rounded-full h-2";
        }
        if (lang === 'hi') {
          statusText.innerText = 'AI Advisory: "गेहूं के पीले रतुआ के लिए प्रोपिकोनाज़ोल 25% EC (1 मिली/लीटर) छिड़कें।"';
        } else {
          statusText.innerText = 'AI Advisory: "ಕಬ್ಬಿನ ಸುಳಿ ಕೊರಕಕ್ಕೆ ಕ್ಲೋರಾಂಟ್ರಾನಿಲಿಪ್ರೋಲ್ ತಕ್ಷಣ ಸಿಂಪಡಿಸಿ."';
        }
        showToast("Voice query processed successfully!");
      }, 1500);
    }

    function toggleNotificationDrawer() {
      const drawer = document.getElementById('notification-drawer');
      if (drawer.classList.contains('translate-x-full')) {
        drawer.classList.remove('translate-x-full');
      } else {
        drawer.classList.add('translate-x-full');
      }
    }

    function triggerLowBandwidthSms() {
      showToast("Offline SMS Advisory dispatched to farmer phone!");
      toggleNotificationDrawer();
    }

    // Generic Toast Notification
    function showToast(message) {
      const toast = document.getElementById('toast');
      const toastMsg = document.getElementById('toast-message');
      toastMsg.innerText = message;
      toast.classList.remove('hidden');

      setTimeout(() => {
        toast.classList.add('hidden');
      }, 3000);
    }
  </script>
</body>
</html>
