<!DOCTYPE html>
<html lang="pl" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SocialBoost AI - Asystent Social Media AI do Tworzenia Treści</title>
    
    <!-- === META TAGI SEO === -->
    <meta name="description" content="SocialBoost AI to asystent social media wykorzystujący AI. Generuj posty, artykuły, grafiki i planuj content 10x szybciej w ponad 10 językach.">
    <meta name="keywords" content="AI social media, asystent social media, generowanie treści AI, generator postów, generator grafik AI, planowanie social media, marketing AI, SocialBoost">
    <meta name="robots" content="index, follow">
    
    <!-- === Open Graph (Facebook, LinkedIn, etc.) === -->
    <meta property="og:title" content="SocialBoost AI - Asystent Social Media AI">
    <meta property="og:description" content="Generuj posty, grafiki i planuj content 10x szybciej dzięki sztucznej inteligencji.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://twoja-domena.pl"> <!-- ZMIEŃ NA SWOJĄ DOMENĘ -->
    <meta property="og:image" content="https://placehold.co/1200x630/4f46e5/ffffff?text=SocialBoost+AI&font=inter"> <!-- ZMIEŃ NA LINK DO OBRAZKA PROMO -->

    <!-- === Twitter Card === -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="SocialBoost AI - Asystent Social Media AI">
    <meta name="twitter:description" content="Generuj posty, grafiki i planuj content 10x szybciej dzięki sztucznej inteligencji.">
    <meta name="twitter:image" content="https://placehold.co/1200x630/4f46e5/ffffff?text=SocialBoost+AI&font=inter"> <!-- ZMIEŃ NA LINK DO OBRAZKA PROMO -->

    <!-- Import Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Import Inter Font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Ikony (Heroicons) -->
    <script type"module" src="https://cdn.jsdelivr.net/npm/heroicons@2.1.3/24/outline/index.js"></script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Style dla aktywnych tabów */
        .tab-active {
            border-bottom-color: #4f46e5; /* indigo-600 */
            color: #eef2ff; /* indigo-100 */
        }
        /* Style dla nieaktywnych tabów */
        .tab-inactive {
            border-bottom-color: transparent;
            color: #9ca3af; /* gray-400 */
        }
        /* Style dla spinnera */
        .spinner {
            border: 4px solid rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            border-top: 4px solid #ffffff;
            width: 40px;
            height: 40px;
            animation: spin 1s linear infinite;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Style dla przycisku Kopiuj */
        .copy-button {
            position: absolute;
            top: 0.75rem; /* 12px */
            right: 0.75rem; /* 12px */
            background-color: #374151; /* gray-700 */
            color: #d1d5db; /* gray-300 */
            padding: 0.25rem 0.75rem; /* py-1 px-3 */
            border-radius: 0.5rem; /* rounded-lg */
            font-size: 0.75rem; /* text-xs */
            display: flex;
            align-items: center;
            opacity: 0; /* Ukryty domyślnie */
            transition: opacity 0.2s, background-color 0.2s;
            cursor: pointer;
        }
        .relative:hover .copy-button {
            opacity: 1; /* Widoczny na hover kontenera */
        }
        .copy-button:hover {
            background-color: #4b5563; /* gray-600 */
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-100 min-h-screen">

    <!-- ==== Nawigacja ==== -->
    <nav class="bg-gray-900/80 backdrop-blur-md shadow-lg sticky top-0 z-50">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-white">
                <span class="text-indigo-400">Social</span>Boost
            </a>
            <div class="flex space-x-6 items-center">
                <a href="#home" class="text-gray-300 hover:text-indigo-400 transition-colors">Start</a>
                <a href="#features" class="text-gray-300 hover:text-indigo-400 transition-colors">Funkcje</a>
                <a href="#apps" class="text-gray-300 hover:text-indigo-400 transition-colors">Aplikacje</a>
                <a href="#pricing" class="text-gray-300 hover:text-indigo-400 transition-colors">Cennik</a>
                <a href="#faq" class="text-gray-300 hover:text-indigo-400 transition-colors">FAQ</a>
                <button id="loginButton" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-4 rounded-lg transition-colors">
                    Zaloguj się
                </button>
            </div>
        </div>
    </nav>

    <!-- ==== Sekcja Hero (Home) ==== -->
    <header id="home" class="container mx-auto px-6 py-24 text-center">
        <h1 class="text-5xl md:text-6xl font-extrabold leading-tight mb-6">
            Twórz <span class="text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 to-purple-500">treści 10x szybciej</span>
            dzięki AI
        </h1>
        <p class="text-lg md:text-xl text-gray-300 max-w-3xl mx-auto mb-10">
            Przestań tracić czas na wymyślanie postów. Nasze narzędzia AI pomogą Ci wygenerować genialny content na social media w kilka sekund, w każdym języku.
        </p>
        <a href="#pricing" class="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-lg text-lg transition-transform hover:scale-105 inline-block">
            Zobacz plany
        </a>
    </header>

    <!-- ==== Sekcja Funkcji (Features) - Widoczna przed zakupem ==== -->
    <section id="features" class="container mx-auto px-6 py-16">
        <h2 class="text-4xl font-bold text-center mb-12">Poznaj Nasze Narzędzia</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Karta: Post Creator -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Post Creator</h3>
                <p class="text-gray-400">Wpisz temat, a my stworzymy gotowy post na media społecznościowe wraz z idealnie dobranymi hashtagami.</p>
            </div>
            <!-- Karta: Idea Generator -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Idea Generator</h3>
                <p class="text-gray-400">Brakuje Ci pomysłów? Wpisz słowo kluczowe, a my wygenerujemy listę 10 wiralowych tematów na posty.</p>
            </div>
            <!-- Karta: Caption Polisher -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Caption Polisher</h3>
                <p class="text-gray-400">Masz już tekst, ale nie brzmi dobrze? Wklej go, aby AI go poprawiło, uatrakcyjniło i dodało CTA.</p>
            </div>
            <!-- Karta: Article Writer -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Article Writer</h3>
                <p class="text-gray-400">Wygeneruj kompletny, zoptymalizowany pod SEO artykuł na bloga, wybierając styl i inspirując się ekspertami.</p>
            </div>
            <!-- Karta: Graphic Creator -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Graphic Creator</h3>
                <p class="text-gray-400">Opisz swój pomysł, a AI wygeneruje unikalną, wysokiej jakości grafikę idealną do Twoich postów na social media.</p>
            </div>
            <!-- Karta: Planner -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Planner</h3>
                <p class="text-gray-400">Stwórz kompletny plan contentowy na cały miesiąc. Otrzymasz tematy, teksty i propozycje grafik.</p>
            </div>
             <!-- Karta: Great Minds -->
            <div class="bg-gray-800 p-6 rounded-xl shadow-lg transform transition-all hover:scale-105 md:col-span-1 lg:col-span-1">
                <h3 class="text-2xl font-semibold mb-3 text-indigo-300">Great Minds</h3>
                <p class="text-gray-400">Zadaj trudne pytanie i uzyskaj odpowiedź w stylu największych myślicieli i wizjonerów, np. co zrobiłby Steve Jobs.</p>
            </div>
        </div>
    </section>

    <!-- ==== Sekcja Aplikacji (Apps) - Zablokowana ==== -->
    <main id="apps" class="container mx-auto px-4 sm:px-6 py-16">
        <h2 class="text-4xl font-bold text-center mb-12">Panel Aplikacji</h2>
        
        <!-- Kontener Aplikacji (z blokadą) -->
        <div class="bg-gray-800 rounded-xl shadow-2xl p-4 sm:p-8 relative min-h-[600px]">
            
            <!-- Blokada subskrypcji (domyślnie widoczna) -->
            <div id="subscriptionOverlay" class="absolute inset-0 bg-gray-900/70 backdrop-blur-md rounded-xl z-20 flex flex-col items-center justify-center text-center p-8">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-20 h-20 text-indigo-400 mb-4">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M16.5 10.5V6.75a4.5 4.5 0 1 0-9 0v3.75m-.75 11.25h10.5a2.25 2.25 0 0 0 2.25-2.25v-6.75a2.25 2.25 0 0 0-2.25-2.25H6.75a2.25 2.25 0 0 0-2.25 2.25v6.75a2.25 2.25 0 0 0 2.25 2.25Z" />
                </svg>
                <h3 class="text-3xl font-bold mb-4">Narzędzia są zablokowane</h3>
                <p class="text-lg text-gray-300 mb-8">Aby uzyskać dostęp do wszystkich aplikacji, wybierz plan subskrypcyjny.</p>
                <a href="#pricing" class="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-lg text-lg transition-transform hover:scale-105 inline-block">
                    Wybierz Plan
                </a>
            </div>

            <!-- Kontener z zakładkami (Tabs) -->
            <div class="mb-6 border-b border-gray-700">
                <nav class="-mb-px flex space-x-4 sm:space-x-8 overflow-x-auto" aria-label="Tabs">
                    <button class="tab-button tab-active whitespace-nowrap" data-tab="postCreator">Post Creator</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="ideaGenerator">Idea Generator</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="captionPolisher">Caption Polisher</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="articleWriter">Article Writer</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="graphicCreator">Graphic Creator</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="planner">Planner</button>
                    <button class="tab-button tab-inactive whitespace-nowrap" data-tab="greatMinds">Great Minds</button>
                </nav>
            </div>

            <!-- Panel Wyboru Języka (wspólny) -->
            <div class="mb-6 max-w-md">
                <label for="languageSelect" class="block text-sm font-medium text-gray-300 mb-2">Wybierz język generowania:</label>
                <select id="languageSelect" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500">
                    <option value="Polski">Polski</option>
                    <option value="English">English</option>
                    <option value="Mandarin Chinese (中文)">Mandarin Chinese (中文)</option>
                    <option value="Hindi (हिन्दी)">Hindi (हिन्दी)</option>
                    <option value="Español">Español</option>
                    <option value="Français">Français</option>
                    <option value="Standard Arabic (العربية)">Standard Arabic (العربية)</option>
                    <option value="Bengali (বাংলা)">Bengali (বাংলা)</option>
                    <option value="Português">Português</option>
                    <option value="Русский">Русский</option>
                    <option value="Urdu (اردو)">Urdu (اردو)</option>
                    <option value="Indonesian (Bahasa Indonesia)">Indonesian (Bahasa Indonesia)</option>
                    <option value="Deutsch">Deutsch</option>
                    <option value="日本語">日本語</option>
                    <option value="Nigerian Pidgin">Nigerian Pidgin</option>
                    <option value="Marathi (मराठी)">Marathi (मराठी)</option>
                    <option value="Telugu (తెలుగు)">Telugu (తెలుగు)</option>
                    <option value="Turkish (Türkçe)">Turkish (Türkçe)</option>
                    <option value="Tamil (தமிழ்)">Tamil (தமிழ்)</option>
                    <option value="Yue Chinese (Cantonese, 粵語)">Yue Chinese (Cantonese, 粵語)</option>
                    <option value="Vietnamese (Tiếng Việt)">Vietnamese (Tiếng Việt)</option>
                    <option value="Korean (한국어)">Korean (한국어)</option>
                    <option value="Javanese (Basa Jawa)">Javanese (Basa Jawa)</option>
                    <option value="Italiano">Italiano</option>
                    <option value="Egyptian Arabic (اللهجة المصرية)">Egyptian Arabic (اللهجة المصرية)</option>
                    <option value="Hausa (Harshen Hausa)">Hausa (Harshen Hausa)</option>
                    <option value="Persian (فارسی)">Persian (فارسی)</option>
                    <option value="Swahili (Kiswahili)">Swahili (Kiswahili)</option>
                    <option value="Gujarati (ગુજરાતી)">Gujarati (ગુજરાતી)</option>
                    <option value="Kannada (ಕನ್ನಡ)">Kannada (ಕನ್ನಡ)</option>
                    <option value="Bhojpuri (भोजपुरी)">Bhojpuri (भोजपुरी)</option>
                    <option value="Southern Pashto (پښتو)">Southern Pashto (پښتو)</option>
                    <option value="Odia (ଓଡ଼ିଆ)">Odia (ଓଡ଼ିଆ)</option>
                    <option value="Maithili (मैथिली)">Maithili (मैथिली)</option>
                    <option value="Ukrainian (Українська)">Ukrainian (Українська)</option>
                    <option value="Igbo (Asụsụ Igbo)">Igbo (Asụsụ Igbo)</option>
                    <option value="Northern Uzbek (Oʻzbekcha)">Northern Uzbek (Oʻzbekcha)</option>
                    <option value="Sindhi (सिन्धी)">Sindhi (सिन्धी)</option>
                    <option value="Malay (Bahasa Melayu)">Malay (Bahasa Melayu)</option>
                    <option value="Amharic (አማርኛ)">Amharic (አማርኛ)</option>
                    <option value="Fula">Fula</option>
                    <option value="Romanian (Română)">Romanian (Română)</option>
                    <option value="Oromo (Afaan Oromoo)">Oromo (Afaan Oromoo)</option>
                    <option value="Dutch (Nederlands)">Dutch (Nederlands)</option>
                    <option value="Yoruba (Èdè Yorùbá)">Yoruba (Èdè Yorùbá)</option>
                    <option value="Sundanese (Basa Sunda)">Sundanese (Basa Sunda)</option>
                    <option value="Thai (ไทย)">Thai (ไทย)</option>
                    <option value="Haitian Creole (Kreyòl ayisyen)">Haitian Creole (Kreyòl ayisyen)</option>
                    <option value="Azerbaijani (Azərbaycan dili)">Azerbaijani (Azərbaycan dili)</option>
                    <option value="Greek (Ελληνικά)">Greek (Ελληνικά)</option>
                </select>
            </div>

            <!-- ==== 1. Aplikacja: Post Creator ==== -->
            <div id="postCreator" class="tab-content">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Post Creator</h3>
                <p class="text-gray-400 mb-6">Wpisz temat, a my stworzymy gotowy post na media społecznościowe wraz z hashtagami.</p>
                <div class="space-y-4">
                    <label for="postPrompt" class="block text-sm font-medium text-gray-300">O czym ma być post?</label>
                    <textarea id="postPrompt" rows="4" class="w-full bg-gray-700 border border-gray-600 rounded-lg p-4 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'premierowy produkt: nowe buty do biegania z recyklingu, podkreśl ekologię i wygodę'"></textarea>
                    
                    <div class="flex items-center my-4">
                        <input id="postEmojiToggle" type="checkbox" class="h-4 w-4 text-indigo-600 border-gray-600 rounded bg-gray-700 focus:ring-indigo-500" checked>
                        <label for="postEmojiToggle" class="ml-2 block text-sm font-medium text-gray-300">Dołącz emoji</label>
                    </div>
                    
                    <button id="generatePostBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="M9.813 15.904 9 18.75l-.813-2.846a4.5 4.5 0 0 0-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 0 0 3.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 0 0 3.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 0 0-3.09 3.09ZM18.25 12l2.846-.813a4.5 4.5 0 0 0 3.09-3.09L24.998 9l-.813-2.846a4.5 4.5 0 0 0-3.09-3.09L18.25 3l-.813 2.846a4.5 4.5 0 0 0-3.09 3.09L11.503 9l2.846.813a4.5 4.5 0 0 0 3.09 3.09L18.25 12Z" /></svg>
                        <span>Generuj Post</span>
                    </button>
                    <div class="relative">
                        <pre id="postOutput" class="w-full bg-gray-900 rounded-lg p-4 min-h-[200px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto"></pre>
                        <button class="copy-button" data-target="postOutput">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                            <span>Kopiuj</span>
                        </button>
                    </div>
                </div>
            </div>

            <!-- ==== 2. Aplikacja: Idea Generator ==== -->
            <div id="ideaGenerator" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Idea Generator</h3>
                <p class="text-gray-400 mb-6">Brakuje Ci pomysłów? Wpisz słowo kluczowe, a my wygenerujemy listę tematów na posty.</p>
                <div class="space-y-4">
                    <label for="ideaPrompt" class="block text-sm font-medium text-gray-300">Główny temat / słowo kluczowe:</label>
                    <input type="text" id="ideaPrompt" class="w-full bg-gray-700 border border-gray-600 rounded-lg p-4 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'marketing', 'zdrowe odżywianie', 'podróże po Azji'">
                    <button id="generateIdeaBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="M12 18v-5.25m0 0a6.01 6.01 0 0 0 1.5-.189m-1.5.189a6.01 6.01 0 0 1-1.5-.189m3.75 7.478a12.06 12.06 0 0 1-3.75 0m3.75 0a12.06 12.06 0 0 0-3.75 0m-3.75 0a12.06 12.06 0 0 1-3.75 0m3.75 0a12.06 12.06 0 0 0-3.75 0m9.75 0a12.06 12.06 0 0 1-3.75 0m3.75 0a12.06 12.06 0 0 0-3.75 0M9.75 6.75a1.5 1.5 0 0 1 1.5-1.5h1.5a1.5 1.5 0 0 1 1.5 1.5v4.5c0 .828-.672 1.5-1.5 1.5h-1.5a1.5 1.5 0 0 1-1.5-1.5v-4.5Z" /></svg>
                        <span>Generuj Pomysły</span>
                    </button>
                    <div class="relative">
                        <pre id="ideaOutput" class="w-full bg-gray-900 rounded-lg p-4 min-h-[200px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto"></pre>
                        <button class="copy-button" data-target="ideaOutput">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                            <span>Kopiuj</span>
                        </button>
                    </div>
                </div>
            </div>

            <!-- ==== 3. Aplikacja: Caption Polisher ==== -->
            <div id="captionPolisher" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Caption Polisher</h3>
                <p class="text-gray-400 mb-6">Masz już tekst, ale nie brzmi dobrze? Wklej go tutaj, aby AI go poprawiło i uatrakcyjniło.</p>
                <div class="space-y-4">
                    <label for="polishPrompt" class="block text-sm font-medium text-gray-300">Tekst do poprawy:</label>
                    <textarea id="polishPrompt" rows="6" class="w-full bg-gray-700 border border-gray-600 rounded-lg p-4 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'Sprzedajemy nowe buty. Są fajne i ekologiczne. Kup teraz.'"></textarea>
                    <button id="generatePolishBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="m16.862 4.487 1.687-1.688a1.875 1.875 0 1 1 2.652 2.652L6.832 19.82a4.5 4.5 0 0 1-1.897 1.13l-2.685.8.8-2.685a4.5 4.5 0 0 1 1.13-1.897L16.863 4.487Zm0 0L19.5 7.125" /></svg>
                        <span>Popraw Tekst</span>
                    </button>
                    <div class="relative">
                        <pre id="polishOutput" class="w-full bg-gray-900 rounded-lg p-4 min-h-[200px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto"></pre>
                        <button class="copy-button" data-target="polishOutput">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                            <span>Kopiuj</span>
                        </button>
                    </div>
                </div>
            </div>

            <!-- ==== 4. Aplikacja: Article Writer ==== -->
            <div id="articleWriter" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Article Writer</h3>
                <p class="text-gray-400 mb-6">Wygeneruj kompletny artykuł na bloga lub stronę. Zawsze zoptymalizowany pod SEO.</p>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <!-- Lewa kolumna: Opcje -->
                    <div class="space-y-4">
                        <div>
                            <label for="articlePrompt" class="block text-sm font-medium text-gray-300">Temat artykułu:</label>
                            <input type="text" id="articlePrompt" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'Przyszłość sztucznej inteligencji w marketingu'">
                        </div>
                        <div>
                            <label for="articleStyle" class="block text-sm font-medium text-gray-300">Styl pisania:</label>
                            <select id="articleStyle" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500">
                                <option value="Profesjonalny">Profesjonalny</option>
                                <option value="Konwersacyjny">Konwersacyjny (na 'Ty')</option>
                                <option value="Techniczny">Techniczny</option>
                                <option value="Przekonujący">Przekonujący (Marketingowy)</option>
                                <option value="Akademicki">Akademicki</option>
                            </select>
                        </div>
                        <div>
                            <label for="articleAuthor" class="block text-sm font-medium text-gray-300">Inspiruj się stylem (opcjonalne):</label>
                            <select id="articleAuthor" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500">
                                <option value="Neutralny Dziennikarz">Neutralny Dziennikarz</option>
                                <option value="Ernest Hemingway">Ernest Hemingway (Zwięzły, mocny)</option>
                                <option value="Malcolm Gladwell">Malcolm Gladwell (Opowiadanie historii, anegdoty)</option>
                                <option value="Steve Jobs">Steve Jobs (Wizjonerski, inspirujący)</option>
                                <option value="Gary Vaynerchuk">Gary Vaynerchuk (Bezpośredni, energiczny)</option>
                                <option value="J.K. Rowling">J.K. Rowling (Opisowy, budujący świat)</option>
                                <option value="Stephen King">Stephen King (Napięcie, potoczny)</option>
                                <option value="Neil Gaiman">Neil Gaiman (Mroczny, fantastyczny, baśniowy)</option>
                                <option value="George Orwell">George Orwell (Krytyczny, klarowny, polityczny)</option>
                                <option value="Hunter S. Thompson">Hunter S. Thompson (Gonzo, subiektywny, przesadzony)</option>
                                <option value="Joan Didion">Joan Didion (Precyzyjny, analityczny, osobisty)</option>
                                <option value="Yuval Noah Harari">Yuval Noah Harari (Wielki obraz, filozoficzny, historyczny)</option>
                                <option value="Tim Ferriss">Tim Ferriss (Optymalizacja, 'hacki', wywiady)</option>
                                <option value="Seth Godin">Seth Godin (Marketingowy, zwięzły, prowokujący)</option>
                                <option value="Anna Wintour">Anna Wintour (Autorytatywny, modowy, elitarny)</option>
                                <option value="Bill Bryson">Bill Bryson (Humorystyczny, podróżniczy, ciekawostki)</option>
                            </select>
                        </div>
                        <button id="generateArticleBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-3 px-6 rounded-lg transition-colors w-full flex items-center justify-center space-x-2 text-lg">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 14.25v-2.625a3.375 3.375 0 0 0-3.375-3.375h-1.5A1.125 1.125 0 0 1 13.5 7.125v-1.5a3.375 3.375 0 0 0-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 0 0-9-9Z" /></svg>
                            <span>Generuj Artykuł</span>
                        </button>
                    </div>
                    <!-- Prawa kolumna: Wynik -->
                    <div>
                        <label class="block text-sm font-medium text-gray-300 mb-2">Wygenerowany Artykuł:</label>
                        <div class="relative">
                            <pre id="articleOutput" class="w-full bg-gray-900 rounded-lg p-4 h-[450px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto border border-gray-700"></pre>
                            <button class="copy-button" data-target="articleOutput">
                                <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                                <span>Kopiuj</span>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ==== 5. Aplikacja: Graphic Creator ==== -->
            <div id="graphicCreator" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Graphic Creator</h3>
                <p class="text-gray-400 mb-6">Wygeneruj unikalną grafikę do swojego postu. Opisz, co chcesz zobaczyć.</p>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <!-- Lewa kolumna: Opcje -->
                    <div class="space-y-4">
                        <label for="graphicPrompt" class="block text-sm font-medium text-gray-300">Opis grafiki (prompt):</label>
                        <textarea id="graphicPrompt" rows="5" class="w-full bg-gray-700 border border-gray-600 rounded-lg p-4 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'minimalistyczna ilustracja wektorowa człowieka pijącego kawę przy biurku', 'hiperrealistyczne zdjęcie kosmonauty na Marsie'"></textarea>
                        <button id="generateGraphicBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-3 px-6 rounded-lg transition-colors w-full flex items-center justify-center space-x-2 text-lg">
                            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" d="m2.25 15.75 5.159-5.159a2.25 2.25 0 0 1 3.182 0l5.159 5.159m-1.5-1.5 1.409-1.409a2.25 2.25 0 0 1 3.182 0l2.909 2.909m-18 3.75h16.5a1.5 1.5 0 0 0 1.5-1.5V6a1.5 1.5 0 0 0-1.5-1.5H3.75A1.5 1.5 0 0 0 2.25 6v12a1.5 1.5 0 0 0 1.5 1.5Zm16.5-1.5H3.75v-1.5m16.5 0v-1.5m0 0H3.75m16.5 0v-1.5m0 0H3.75M10.5 6H13.5v-1.5H10.5V6Z" /></svg>
                            <span>Generuj Grafikę</span>
                        </button>
                    </div>
                    <!-- Prawa kolumna: Wynik -->
                    <div>
                        <label class="block text-sm font-medium text-gray-300 mb-2">Wygenerowana Grafika:</label>
                        <div class="w-full h-[450px] bg-gray-900 rounded-lg border border-gray-700 flex items-center justify-center overflow-hidden">
                            <div id="graphicLoader" class="spinner hidden"></div>
                            <img id="graphicOutput" src="https://placehold.co/512x512/0f172a/312e81?text=Twoja+Grafika+AI&font=inter" alt="Wygenerowana grafika" class="w-full h-full object-contain">
                        </div>
                    </div>
                </div>
            </div>

            <!-- ==== 6. Aplikacja: Planner ==== -->
            <div id="planner" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Planner</h3>
                <p class="text-gray-400 mb-6">Zaplanuj swój content na cały miesiąc. Podaj główny temat, a my zajmiemy się resztą.</p>
                <div class="space-y-4">
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <div>
                            <label for="planTheme" class="block text-sm font-medium text-gray-300">Główny temat / Nisza:</label>
                            <input type="text" id="planTheme" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white" placeholder="np. 'Marketing B2B', 'Fitness', 'Gotowanie'">
                        </div>
                        <div>
                            <label for="planMonth" class="block text-sm font-medium text-gray-300">Wybierz miesiąc:</label>
                            <select id="planMonth" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white">
                                <option value="Styczeń">Styczeń</option>
                                <option value="Luty">Luty</option>
                                <option value="Marzec">Marzec</option>
                                <option value="Kwiecień">Kwiecień</option>
                                <option value="Maj">Maj</option>
                                <option value="Czerwiec">Czerwiec</option>
                                <option value="Lipiec">Lipiec</option>
                                <option value="Sierpień">Sierpień</option>
                                <option value="Wrzesień">Wrzesień</option>
                                <option value="Październik">Październik</option>
                                <option value="Listopad">Listopad</option>
                                <option value="Grudzień">Grudzień</option>
                            </select>
                        </div>
                        <div>
                            <label for="planPostsPerWeek" class="block text-sm font-medium text-gray-300">Ilość postów / tydzień:</label>
                            <input type="number" id="planPostsPerWeek" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white" value="3" min="1" max="7">
                        </div>
                    </div>
                    <button id="generatePlanBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 0 1 2.25-2.25h13.5A2.25 2.25 0 0 1 21 7.5v11.25m-18 0A2.25 2.25 0 0 0 5.25 21h13.5A2.25 2.25 0 0 0 21 18.75m-18 0v-7.5A2.25 2.25 0 0 1 5.25 9h13.5A2.25 2.25 0 0 1 21 11.25v7.5" /></svg>
                        <span>Generuj Plan</span>
                    </button>
                    <div class="relative">
                        <pre id="planOutput" class="w-full bg-gray-900 rounded-lg p-4 min-h-[400px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto border border-gray-700"></pre>
                        <button class="copy-button" data-target="planOutput">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                            <span>Kopiuj</span>
                        </button>
                    </div>
                </div>
            </div>

            <!-- ==== 7. Aplikacja: Great Minds ==== -->
            <div id="greatMinds" class="tab-content hidden">
                <h3 class="text-2xl font-semibold mb-4 text-indigo-300">Great Minds</h3>
                <p class="text-gray-400 mb-6">Zmagasz się z problemem? Zapytaj o radę największych wizjonerów w historii.</p>
                <div class="space-y-4">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label for="mindSelect" class="block text-sm font-medium text-gray-300">Wybierz umysł:</label>
                            <select id="mindSelect" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white">
                                <option value="Steve Jobs">Steve Jobs</option>
                                <option value="Elon Musk">Elon Musk</option>
                                <option value="Albert Einstein">Albert Einstein</option>
                                <option value="Marie Skłodowska-Curie">Marie Skłodowska-Curie</option>
                                <option value="Isaac Newton">Isaac Newton</option>
                                <option value="Jeff Bezos">Jeff Bezos</option>
                                <option value="Nikola Tesla">Nikola Tesla</option>
                                <option value="Leonardo da Vinci">Leonardo da Vinci</option>
                                <option value="Marcus Aurelius">Marcus Aurelius (Marek Aureliusz)</option>
                                <option value="Sun Tzu">Sun Tzu</option>
                            </select>
                        </div>
                    </div>
                    <div>
                        <label for="mindPrompt" class="block text-sm font-medium text-gray-300">Twoje pytanie lub problem:</label>
                        <textarea id="mindPrompt" rows="4" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-4 text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="np. 'Mam świetny pomysł na aplikację, ale boję się porażki.' lub 'Jak zmotywować mój zespół do większej kreatywności?'"></textarea>
                    </div>
                    <button id="generateMindBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors flex items-center space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5"><path stroke-linecap="round" stroke-linejoin="round" d="M8.25 15 12 18.75 15.75 15m-7.5-6L12 5.25 15.75 9" /></svg>
                        <span>Zapytaj o Radę</span>
                    </button>
                    <div class="relative">
                        <pre id="mindOutput" class="w-full bg-gray-900 rounded-lg p-4 min-h-[200px] text-gray-200 whitespace-pre-wrap font-sans overflow-auto"></pre>
                        <button class="copy-button" data-target="mindOutput">
                            <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" /></svg>
                            <span>Kopiuj</span>
                        </button>
                    </div>
                </div>
            </div>

        </div>
    </main>

    <!-- ==== Sekcja Cennika (Pricing) ==== -->
    <section id="pricing" class="bg-gray-800 py-24 px-6">
        <div class="container mx-auto max-w-7xl text-center">
            <h2 class="text-4xl font-bold mb-4">Wybierz plan dla siebie</h2>
            <p class="text-lg text-gray-300 mb-12">Uzyskaj dostęp do narzędzi, których potrzebujesz, bez limitów.</p>
            
            <div class="flex flex-col lg:flex-row justify-center gap-8">
                
                <!-- Plan Basic -->
                <div class="bg-gray-900 p-8 rounded-xl shadow-lg border-2 border-transparent hover:border-indigo-500 transition-all transform hover:scale-105 w-full lg:w-1/3">
                    <h3 class="text-2xl font-semibold mb-4">Basic</h3>
                    <p class="text-5xl font-extrabold mb-4">49<span class="text-xl text-gray-400"> zł/mc</span></p>
                    <p class="text-gray-400 mb-4 h-6">Idealny na start.</p>
                    <ul class="space-y-3 text-gray-300 mb-8 text-left min-h-[160px]">
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Dostęp do <strong>1 wybranego</strong> narzędzia</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Nielimitowane generowanie</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Wszystkie 10 języków</li>
                    </ul>
                    <button class="buy-button bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-lg text-lg w-full transition-colors">
                        Kup Teraz
                    </button>
                </div>

                <!-- Plan Pro (Wyróżniony) -->
                <div class="bg-gray-900 p-8 rounded-xl shadow-lg border-2 border-indigo-500 relative w-full lg:w-1/3">
                    <span class="absolute top-0 right-8 -mt-4 bg-indigo-500 text-white text-xs font-bold px-3 py-1 rounded-full">NAJLEPSZA OFERTA</span>
                    <h3 class="text-2xl font-semibold mb-4">Pro</h3>
                    <p class="text-5xl font-extrabold mb-4">249<span class="text-xl text-gray-400"> zł/mc</span></p>
                    <p class="text-gray-400 mb-4 h-6">Pełna moc dla profesjonalistów.</p>
                    <ul class="space-y-3 text-gray-300 mb-8 text-left min-h-[160px]">
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Dostęp do <strong>wszystkich 7</strong> narzędzi</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Nielimitowane generowanie</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Wszystkie 10 języków</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Generator grafik AI</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Priorytetowe wsparcie 24/7</li>
                    </ul>
                    <button class="buy-button bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-lg text-lg w-full transition-colors">
                        Kup Teraz
                    </button>
                </div>
                
                <!-- Plan Roczny -->
                <div class="bg-gray-900 p-8 rounded-xl shadow-lg border-2 border-transparent hover:border-indigo-500 transition-all transform hover:scale-105 w-full lg:w-1/3">
                    <h3 class="text-2xl font-semibold mb-4">Pro Roczny</h3>
                    <p class="text-5xl font-extrabold mb-4">2490<span class="text-xl text-gray-400"> zł/rok</span></p>
                    <p class="text-green-400 mb-4 h-6">2 miesiące gratis!</p>
                    <ul class="space-y-3 text-gray-300 mb-8 text-left min-h-[160px]">
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Wszystko z planu Pro</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Dostęp na 12 miesięcy</li>
                        <li class="flex items-center"><svg class="w-5 h-5 text-green-400 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>Największa oszczędność</li>
                    </ul>
                    <button class="buy-button bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-lg text-lg w-full transition-colors">
                        Kup Teraz
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- ==== Sekcja FAQ (NOWA) ==== -->
    <section id="faq" class="bg-gray-900 py-24 px-6">
        <div class="container mx-auto max-w-4xl">
            <h2 class="text-4xl font-bold text-center mb-12">Najczęściej Zadawane Pytania (FAQ)</h2>
            <div class="space-y-6">
                <!-- Pytanie 1 -->
                <details class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <summary class="text-xl font-semibold text-indigo-300 cursor-pointer list-none flex justify-between items-center">
                        Jak działają płatności i czy moje dane są bezpieczne?
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 transform transition-transform" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" /></svg>
                    </summary>
                    <p class="text-gray-300 mt-4">Korzystamy ze Stripe, światowego lidera płatności online. Wszystkie Twoje dane karty są przetwarzane bezpośrednio przez bezpieczne serwery Stripe i nigdy nie są przechowywane na naszych serwerach. Gwarantuje to najwyższy poziom bezpieczeństwa (certyfikat PCI DSS Level 1) i pełną poufność Twoich danych finansowych.</p>
                </details>
                <!-- Pytanie 2 -->
                <details class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <summary class="text-xl font-semibold text-indigo-300 cursor-pointer list-none flex justify-between items-center">
                        Czy mogę anulować subskrypcję w dowolnym momencie?
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 transform transition-transform" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" /></svg>
                    </summary>
                    <p class="text-gray-300 mt-4">Tak. Po wdrożeniu pełnego systemu płatności, będziesz mógł/mogła anulować swoją subskrypcję w dowolnym momencie z poziomu panelu użytkownika. W przypadku planu miesięcznego, dostęp zostanie zakończony z końcem bieżącego okresu rozliczeniowego. W przypadku planu rocznego, dostęp będzie aktywny do końca opłaconego roku.</p>
                </details>
                <!-- Pytanie 3 -->
                <details class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <summary class="text-xl font-semibold text-indigo-300 cursor-pointer list-none flex justify-between items-center">
                        Czy generowanie treści jest naprawdę "nielimitowane"?
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 transform transition-transform" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" /></svg>
                    </summary>
                    <p class="text-gray-300 mt-4">Tak. Nasze plany "Pro" oraz "Basic" (dla wybranego narzędzia) oferują nielimitowane generowanie treści. Chcemy, abyś mógł/mogła tworzyć bez obaw o limity. Monitorujemy jedynie obciążenie systemu, aby zapobiegać nadużyciom (np. automatycznym botom), co jest standardową praktyką "Fair Use Policy".</p>
                </details>
                <!-- Pytanie 4 -->
                <details class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <summary class="text-xl font-semibold text-indigo-300 cursor-pointer list-none flex justify-between items-center">
                        Jaki model AI jest używany do generowania grafik?
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 transform transition-transform" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" /></svg>
                    </summary>
                    <p class="text-gray-300 mt-4">Nasz "Graphic Creator" korzysta z jednego z najnowszych modeli generowania obrazów - Google Imagen 4. Pozwala to na tworzenie wysokiej jakości, fotorealistycznych lub stylizowanych obrazów na podstawie Twoich opisów tekstowych.</p>
                </details>
                 <!-- Pytanie 5 -->
                <details class="bg-gray-800 p-6 rounded-lg shadow-lg">
                    <summary class="text-xl font-semibold text-indigo-300 cursor-pointer list-none flex justify-between items-center">
                        Czym różni się plan Basic od Pro?
                        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 transform transition-transform" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" /></svg>
                    </summary>
                    <p class="text-gray-300 mt-4">Plan Basic (49 zł/mc) daje Ci nielimitowany dostęp do JEDNEGO, wybranego przez Ciebie narzędzia (np. tylko Post Creator). Plan Pro (249 zł/mc) odblokowuje WSZYSTKIE 7 narzędzi, w tym Graphic Creator i Planner, oraz oferuje priorytetowe wsparcie.</p>
                </details>
            </div>
        </div>
    </section>


    <!-- ==== Stopka (ZAKTUALIZOWANA) ==== -->
    <footer class="bg-gray-900 border-t border-gray-800 pt-16 pb-8">
        <div class="container mx-auto px-6 text-center text-gray-500">
            <div class="flex justify-center space-x-6 mb-8">
                <a href="#privacy-policy" class="hover:text-indigo-400 transition-colors">Polityka Prywatności</a>
                <a href="#cookie-policy" class="hover:text-indigo-400 transition-colors">Polityka Cookies</a>
                <a href="mailto:kontakt@socialboost.ai" class="hover:text-indigo-400 transition-colors">Kontakt</a>
            </div>
            <p>&copy; 2025 SocialBoost AI. Wszelkie prawa zastrzeżone.</p>
        </div>
    </footer>


    <!-- ==== BANER COOKIES (NOWY) ==== -->
    <div id="cookieBanner" class="fixed bottom-0 left-0 right-0 bg-gray-800 border-t border-gray-700 p-4 z-50 hidden">
        <div class="container mx-auto flex flex-col md:flex-row justify-between items-center text-center md:text-left">
            <p class="text-gray-300 text-sm mb-4 md:mb-0">
                Używamy plików cookie i przetwarzamy dane osobowe, aby zapewnić najlepsze działanie strony. 
                Klikając "Akceptuj", zgadzasz się na naszą 
                <a href="#privacy-policy" class="text-indigo-400 underline">Politykę Prywatności</a>.
            </p>
            <button id="acceptCookieBtn" class="bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors whitespace-nowrap">
                Akceptuj
            </button>
        </div>
    </div>


    <!-- ==== MODALE ==== -->

    <!-- Modal Płatności (Symulacja) -->
    <div id="paymentModal" class="fixed inset-0 bg-gray-900/80 backdrop-blur-sm z-50 hidden items-center justify-center">
        <div class="bg-gray-800 rounded-lg shadow-2xl p-8 max-w-md w-full relative">
            <button id="closePaymentModal" aria-label="Zamknij modal" class="absolute top-4 right-4 text-gray-400 hover:text-white">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12" /></svg>
            </button>
            <h3 class="text-2xl font-bold mb-6 text-white text-center">Symulacja Płatności</h3>
            <p class="text-gray-300 text-center mb-6">To jest tylko demonstracja. Kliknij 'Zapłać', aby symulować udaną transakcję i odblokować aplikacje.</p>
            <div class="space-y-4">
                <div>
                    <label for="card" class="block text-sm font-medium text-gray-300">Numer karty (demo)</label>
                    <input type="text" id="card" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white" value="**** **** **** 1234" disabled>
                </div>
                <div class="flex space-x-4">
                    <div class="w-1/2">
                        <label for="expiry" class="block text-sm font-medium text-gray-300">Data ważności (demo)</label>
                        <input type="text" id="expiry" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white" value="12/28" disabled>
                    </div>
                    <div class="w-1/2">
                        <label for="cvc" class="block text-sm font-medium text-gray-300">CVC (demo)</label>
                        <input type="text" id="cvc" class="mt-1 w-full bg-gray-700 border border-gray-600 rounded-lg p-3 text-white" value="***" disabled>
                    </div>
                </div>
                <button id="confirmPaymentBtn" class="w-full bg-green-600 hover:bg-green-700 text-white font-bold py-3 px-6 rounded-lg transition-colors text-lg">
                    Zapłać (Symulacja)
                </button>
            </div>
        </div>
    </div>

    <!-- Modal Ładowania -->
    <div id="loadingModal" class="fixed inset-0 bg-gray-900/80 backdrop-blur-sm z-50 hidden items-center justify-center">
        <div class="flex flex-col items-center">
            <div class="spinner"></div>
            <p class="text-white text-lg mt-4">AI myśli...</p>
        </div>
    </div>

    <!-- Modal Błędu -->
    <div id="errorModal" class="fixed inset-0 bg-gray-900/80 backdrop-blur-sm z-50 hidden items-center justify-center">
        <div class="bg-gray-800 rounded-lg shadow-2xl p-8 max-w-md w-full">
            <h3 class="text-2xl font-bold mb-4 text-red-400 text-center">Wystąpił Błąd</h3>
            <p id="errorMessage" class="text-gray-300 text-center mb-6"></p>
            <button id="closeErrorModal" class="w-full bg-indigo-600 hover:bg-indigo-700 text-white font-medium py-2 px-6 rounded-lg transition-colors">
                OK
            </button>
        </div>
    </div>


    <!-- ==== Logika JavaScript ==== -->
    <script type="module">
        // ==== ZMIENNE STANU ====
        let currentTab = 'postCreator'; // Domyślna zakładka
        let isSubscribed = false; // Status subskrypcji
        let isLoading = false;
        
        // Zostaw pusty, klucz API zostanie automatycznie dodany przez środowisko Canvas
        const GEMINI_API_KEY = "";
        const GEMINI_API_URL = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${GEMINI_API_KEY}`;
        const IMAGEN_API_URL = `https://generativelanguage.googleapis.com/v1beta/models/imagen-4.0-generate-001:predict?key=${GEMINI_API_KEY}`;

        // ==== SELEKTORY DOM ====
        const tabButtons = document.querySelectorAll('.tab-button');
        const tabContents = document.querySelectorAll('.tab-content');
        const languageSelect = document.getElementById('languageSelect');
        const subscriptionOverlay = document.getElementById('subscriptionOverlay');
        
        // Modale
        const loadingModal = document.getElementById('loadingModal');
        const errorModal = document.getElementById('errorModal');
        const errorMessage = document.getElementById('errorMessage');
        const closeErrorModal = document.getElementById('closeErrorModal');
        const paymentModal = document.getElementById('paymentModal');
        const buyButtons = document.querySelectorAll('.buy-button');
        const closePaymentModal = document.getElementById('closePaymentModal');
        const confirmPaymentBtn = document.getElementById('confirmPaymentBtn');

        // Baner Cookies
        const cookieBanner = document.getElementById('cookieBanner');
        const acceptCookieBtn = document.getElementById('acceptCookieBtn');

        // App 1: Post Creator
        const generatePostBtn = document.getElementById('generatePostBtn');
        const postPrompt = document.getElementById('postPrompt');
        const postOutput = document.getElementById('postOutput');
        
        // App 2: Idea Generator
        const generateIdeaBtn = document.getElementById('generateIdeaBtn');
        const ideaPrompt = document.getElementById('ideaPrompt');
        const ideaOutput = document.getElementById('ideaOutput');

        // App 3: Caption Polisher
        const generatePolishBtn = document.getElementById('generatePolishBtn');
        const polishPrompt = document.getElementById('polishPrompt');
        const polishOutput = document.getElementById('polishOutput');

        // App 4: Article Writer
        const generateArticleBtn = document.getElementById('generateArticleBtn');
        const articlePrompt = document.getElementById('articlePrompt');
        const articleStyle = document.getElementById('articleStyle');
        const articleAuthor = document.getElementById('articleAuthor');
        const articleOutput = document.getElementById('articleOutput');

        // App 5: Graphic Creator
        const generateGraphicBtn = document.getElementById('generateGraphicBtn');
        const graphicPrompt = document.getElementById('graphicPrompt');
        const graphicOutput = document.getElementById('graphicOutput');
        const graphicLoader = document.getElementById('graphicLoader');

        // App 6: Planner
        const generatePlanBtn = document.getElementById('generatePlanBtn');
        const planTheme = document.getElementById('planTheme');
        const planMonth = document.getElementById('planMonth');
        const planPostsPerWeek = document.getElementById('planPostsPerWeek');
        const planOutput = document.getElementById('planOutput');

        // App 7: Great Minds
        const generateMindBtn = document.getElementById('generateMindBtn');
        const mindSelect = document.getElementById('mindSelect');
        const mindPrompt = document.getElementById('mindPrompt');
        const mindOutput = document.getElementById('mindOutput');

        // ==== GŁÓWNA FUNKCJA API (z ponowieniami) ====
        async function callGeminiAPI(prompt, systemInstruction) {
            setLoading(true);
            let retries = 3;
            let delay = 1000;

            const payload = {
                contents: [{ parts: [{ text: prompt }] }],
            };

            if (systemInstruction) {
                payload.systemInstruction = {
                    parts: [{ text: systemInstruction }]
                };
            }

            while (retries > 0) {
                try {
                    const response = await fetch(GEMINI_API_URL, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (!response.ok) {
                        const errorData = await response.json();
                        console.error('API Error Response:', errorData);
                        throw new Error(`Błąd API: ${response.status} ${response.statusText}. ${errorData?.error?.message || ''}`);
                    }

                    const result = await response.json();
                    
                    if (result.candidates && result.candidates[0].content && result.candidates[0].content.parts[0].text) {
                        setLoading(false);
                        return result.candidates[0].content.parts[0].text;
                    } else {
                        // Obsługa błędu 'safety' lub pustej odpowiedzi
                        console.warn('API response missing content:', result);
                        let finishReason = result.candidates?.[0]?.finishReason;
                        let safetyRatings = result.candidates?.[0]?.safetyRatings;
                        if (finishReason === 'SAFETY') {
                            throw new Error(`Odpowiedź zablokowana z powodu bezpieczeństwa. Powód: ${safetyRatings?.map(r => r.category).join(', ')}`);
                        }
                        throw new Error('Otrzymano nieoczekiwaną lub pustą odpowiedź od AI.');
                    }

                } catch (error) {
                    console.error('Błąd podczas wywołania API Gemini:', error);
                    retries--;
                    if (retries === 0) {
                        setLoading(false);
                        showError(`Błąd AI: ${error.message}. Spróbuj ponownie później.`);
                        return null; // Zwraca null w przypadku ostatecznej porażki
                    }
                    console.log(`Ponawianie próby za ${delay / 1000}s...`);
                    await new Promise(res => setTimeout(res, delay));
                    delay *= 2; // Exponential backoff
                }
            }
        }

        // ==== FUNKCJA API IMAGEN (Generowanie Obrazów) ====
        async function callImagenAPI(prompt) {
            setLoading(true);
            graphicLoader.classList.remove('hidden');
            graphicOutput.classList.add('hidden');
            
            let retries = 3;
            let delay = 1000;

            const payload = { 
                instances: [ { prompt: prompt } ], 
                parameters: { "sampleCount": 1 } 
            };

            while (retries > 0) {
                try {
                    const response = await fetch(IMAGEN_API_URL, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (!response.ok) {
                        const errorData = await response.json();
                        console.error('API Error Response:', errorData);
                        throw new Error(`Błąd API Obrazów: ${response.status} ${response.statusText}. ${errorData?.error?.message || ''}`);
                    }

                    const result = await response.json();
                    
                    if (result.predictions && result.predictions.length > 0 && result.predictions[0].bytesBase64Encoded) {
                        setLoading(false);
                        graphicLoader.classList.add('hidden');
                        graphicOutput.classList.remove('hidden');
                        return result.predictions[0].bytesBase64Encoded;
                    } else {
                        console.warn('API response missing image data:', result);
                        throw new Error('Otrzymano nieoczekiwaną lub pustą odpowiedź od API obrazów.');
                    }

                } catch (error) {
                    console.error('Błąd podczas wywołania API Imagen:', error);
                    retries--;
                    if (retries === 0) {
                        setLoading(false);
                        graphicLoader.classList.add('hidden');
                        graphicOutput.classList.remove('hidden'); // Pokaż z powrotem placeholder
                        showError(`Błąd AI Obrazów: ${error.message}. Spróbuj ponownie później.`);
                        return null;
                    }
                    console.log(`Ponawianie próby (Obraz) za ${delay / 1000}s...`);
                    await new Promise(res => setTimeout(res, delay));
                    delay *= 2; // Exponential backoff
                }
            }
        }

        // ==== LOGIKA APLIKACJI ====

        // 1. Post Creator
        generatePostBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const prompt = postPrompt.value;
            const lang = languageSelect.value;
            const includeEmojis = document.getElementById('postEmojiToggle').checked; // Get checkbox value

            if (!prompt) {
                showError("Wpisz temat postu.");
                return;
            }

            const systemPrompt = `Jesteś ekspertem od social media. Twoim zadaniem jest tworzenie angażujących postów. Odpowiedz TYLKO treścią posta.`;
            
            // Add conditional instruction for emojis
            const emojiInstruction = includeEmojis 
                ? "Używaj odpowiednich emoji, aby post był bardziej angażujący." 
                : "WAŻNE: NIE UŻYWAJ absolutnie żadnych emoji w tekście ani w hashtagach. Post ma być czystym tekstem.";

            const userPrompt = `Stwórz krótki (3-5 zdań) post na social media (np. Instagram/Facebook) w języku ${lang} na temat: "${prompt}". 
            Na końcu dodaj sekcję z 5-7 trafnymi, popularnymi hashtagami powiązanymi z tematem.
            ${emojiInstruction}`;
            
            postOutput.textContent = "Generowanie...";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                postOutput.textContent = result;
            } else {
                postOutput.textContent = "";
            }
        });

        // 2. Idea Generator
        generateIdeaBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const prompt = ideaPrompt.value;
            const lang = languageSelect.value;
            if (!prompt) {
                showError("Wpisz temat lub słowo kluczowe.");
                return;
            }

            const systemPrompt = `Jesteś kreatywnym strategiem contentu. Twoim zadaniem jest generowanie wiralowych pomysłów. Odpowiedz TYLKO listą pomysłów.`;
            const userPrompt = `Wygeneruj listę 10 pomysłów na content (np. posty, wideo, artykuły) w języku ${lang} na temat: "${prompt}". 
            Formatuj jako listę punktowaną (np. '- Pomysł 1').`;
            
            ideaOutput.textContent = "Generowanie...";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                ideaOutput.textContent = result;
            } else {
                ideaOutput.textContent = "";
            }
        });

        // 3. Caption Polisher
        generatePolishBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const prompt = polishPrompt.value;
            const lang = languageSelect.value;
            if (!prompt) {
                showError("Wklej tekst do poprawy.");
                return;
            }

            const systemPrompt = `Jesteś światowej klasy copywriterem i edytorem. Twoim zadaniem jest ulepszanie tekstów, aby były bardziej chwytliwe, jasne i angażujące. Zachowaj oryginalny język. Odpowiedz TYLKO poprawionym tekstem.`;
            const userPrompt = `Popraw i 'wypoleruj' ten tekst (w języku ${lang}), aby był idealny na social media. Spraw, by był bardziej dynamiczny i profesjonalny, popraw błędy i dodaj wezwanie do działania (CTA), jeśli pasuje:
            
            "${prompt}"`;
            
            polishOutput.textContent = "Generowanie...";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                polishOutput.textContent = result;
            } else {
                polishOutput.textContent = "";
            }
        });

        // 4. Article Writer
        generateArticleBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const topic = articlePrompt.value;
            const style = articleStyle.value;
            const author = articleAuthor.value;
            const lang = languageSelect.value;
            
            if (!topic) {
                showError("Wpisz temat artykułu.");
                return;
            }

            const systemPrompt = getArticleSystemPrompt(style, author, lang);
            const userPrompt = `Napisz artykuł na temat: "${topic}". Język: ${lang}.`;
            
            articleOutput.textContent = "Generowanie artykułu... To może zająć chwilę.";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                articleOutput.textContent = result;
            } else {
                articleOutput.textContent = "";
            }
        });

        // 5. Graphic Creator
        generateGraphicBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const prompt = graphicPrompt.value;
            if (!prompt) {
                showError("Wpisz opis grafiki, którą chcesz wygenerować.");
                return;
            }

            const base64Data = await callImagenAPI(prompt);
            if (base64Data) {
                graphicOutput.src = `data:image/png;base64,${base64Data}`;
            }
        });

        // 6. Planner
        generatePlanBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const theme = planTheme.value;
            const month = planMonth.value;
            const postsPerWeek = planPostsPerWeek.value;
            const lang = languageSelect.value;

            if (!theme) {
                showError("Wpisz główny temat lub niszę.");
                return;
            }

            const systemPrompt = `Jesteś strategiem content marketingu. Twoim zadaniem jest stworzenie miesięcznego planu postów. Odpowiedz TYLKO planem.`;
            const userPrompt = `Stwórz plan postów na social media dla tematu: "${theme}".
            Miesiąc: ${month}
            Ilość postów: ${postsPerWeek} na tydzień.
            Język: ${lang}.
            
            Dla każdego postu podaj:
            - Dzień (np. Tydzień 1, Dzień 1):
            - Tytuł/Temat: [Chwytliwy tytuł]
            - Krótki Tekst: [2-3 zdania rozwinięcia tematu]
            - Propozycja Grafiki: [Opis grafiki lub wideo, które pasuje do postu]
            
            Formatuj odpowiedź w przejrzysty, czytelny sposób, używając markdown.`;
            
            planOutput.textContent = "Generowanie planu...";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                planOutput.textContent = result;
            } else {
                planOutput.textContent = "";
            }
        });

        // 7. Great Minds
        generateMindBtn.addEventListener('click', async () => {
            if (!checkSubscription()) return;
            const mind = mindSelect.value;
            const prompt = mindPrompt.value;
            const lang = languageSelect.value;

            if (!prompt) {
                showError("Wpisz swoje pytanie lub problem.");
                return;
            }

            const systemPrompt = `Jesteś emulatorem AI. Twoim zadaniem jest odpowiedzieć na pytanie z perspektywy wybranej postaci. Dogłębnie przeanalizuj jej znane cechy, styl myślenia, filozofię i publiczne wypowiedzi, aby sformułować odpowiedź, jakiej ta osoba mogłaby udzielić. Mów w pierwszej osobie (jako 'ja').
            
            Postać: ${mind}.
            Odpowiedz TYLKO jako ta postać. Nie dodawaj żadnych wstępów typu "Jako ${mind}, powiedziałbym...". Po prostu zacznij odpowiedź.`;
            
            const userPrompt = `Jako ${mind}, co byś mi doradził(a) lub co myślisz o tej sytuacji: "${prompt}"? Odpowiedz w języku ${lang}.`;
            
            mindOutput.textContent = "Generowanie porady...";
            const result = await callGeminiAPI(userPrompt, systemPrompt);
            if (result) {
                mindOutput.textContent = `"${result}"\n\n- ${mind}`;
            } else {
                mindOutput.textContent = "";
            }
        });


        // Funkcja pomocnicza do budowania system promptu dla Article Writer
        function getArticleSystemPrompt(style, author, lang) {
            let outline = "Użyj standardowego, logicznego podziału na sekcje (wstęp, rozwinięcie z podtytułami, zakończenie).";
            let technical = "";
            
            // Definiowanie outline na podstawie autora
            switch(author) {
                case "Ernest Hemingway":
                    outline = "Stwórz artykuł używając krótkich, dosadnych zdań. Unikaj zbędnych przymiotników. Skup się na faktach i bezpośrednim przekazie.";
                    break;
                case "Malcolm Gladwell":
                    outline = "Zacznij od intrygującej anegdoty lub historii, która przyciągnie uwagę. Połącz ją z głównym tematem. Użyj analogii i odniesień do badań (nawet jeśli są hipotetyczne).";
                    break;
                case "Steve Jobs":
                    outline = "Napisz w wizjonerskim, inspirującym tonie. Skup się na 'dlaczego' (why) danego tematu. Używaj mocnych, deklaratywnych stwierdzeń. Zakończ inspirującym wezwaniem do myślenia inaczej.";
                    break;
                case "Gary Vaynerchuk":
                    outline = "Pisze bardzo bezpośrednio, energicznie, używając języka potocznego. Skup się na praktycznym działaniu ('hustle') i bezkompromisowej szczerości. Zachęcaj do działania 'tu i teraz'.";
                    break;
                case "J.K. Rowling":
                    outline = "Buduj narrację z bogatymi opisami. Używaj metafor i twórz atmosferę tajemnicy lub odkrycia. Skup się na emocjonalnym połączeniu z czytelnikiem.";
                    break;
                case "Stephen King":
                    outline = "Używaj potocznego języka, jakbyś rozmawiał z przyjacielem. Buduj napięcie i skupiaj się na ludzkich (często mrocznych) aspektach tematu. Używaj wyrazistych obrazów.";
                    break;
                case "Neil Gaiman":
                    outline = "Twój ton jest baśniowy, lekko mroczny i poetycki. Mieszaj rzeczywistość z metaforą. Zadawaj prowokujące do myślenia pytania.";
                    break;
                case "George Orwell":
                    outline = "Pisze z absolutną klarownością. Używaj prostego, bezpośredniego języka. Bądź krytyczny, analityczny i skupiony na prawdzie, nawet jeśli jest niewygodna.";
                    break;
                case "Hunter S. Thompson":
                    outline = "Styl 'Gonzo'. Pisz subiektywnie, przesadnie i z pasją. Bądź w centrum narracji. Używaj hiperboli i mocnego, obrazoburczego języka.";
                    break;
                case "Joan Didion":
                    outline = "Pisz z chłodną precyzją i elegancją. Skup się na szczegółach, które ujawniają większy obraz. Ton jest analityczny, ale głęboko osobisty.";
                    break;
                case "Yuval Noah Harari":
                    outline = "Patrz na temat z perspektywy 'wielkiego obrazu'. Łącz go z historią, filozofią i przyszłością ludzkości. Używaj klarownych, ale głębokich uogólnień.";
                    break;
                case "Tim Ferriss":
                    outline = "Skup się na optymalizacji i 'hackach'. Dziel złożone problemy na proste kroki. Używaj list, punktów i praktycznych porad. Cytuj ekspertów (hipotetycznie).";
                    break;
                case "Seth Godin":
                    outline = "Pisz krótko, zwięzle i prowokująco. Używaj metafor marketingowych. Każde zdanie ma znaczenie. Zakończ mocnym wezwaniem do myślenia lub działania.";
                    break;
                case "Anna Wintour":
                    outline = "Pisz autorytatywnie, z wyczuciem stylu i ekskluzywności. Ton jest zdecydowany, dyktujący trendy. Używaj wyszukanego słownictwa.";
                    break;
                case "Bill Bryson":
                    outline = "Ton jest ciepły, humorystyczny i pełen ciekawostek. Tłumacz złożone tematy w prosty i zabawny sposób. Używaj anegdot i osobistych wtrąceń.";
                    break;
            }

            // Definiowanie dodatków dla stylu technicznego
            if (style === "Techniczny") {
                technical = "Ponieważ styl jest techniczny, jeśli temat na to pozwala (np. porównania, dane, kroki procesu), wpleć w treść artykułu listę punktowaną lub prostą tabelę w formacie markdown, aby ułatwić zrozumienie danych.";
            }

            return `Jesteś ekspertem w pisaniu artykułów. Twój styl to: ${style}. 
            Masz się inspirować stylem pisania ${author}.
            
            ZASADY:
            1.  ZAWSZE na samym początku odpowiedzi wygeneruj meta tagi SEO (title i description) dla tego artykułu, w języku ${lang}. Muszą być w formacie:
                <meta name="title" content="Tytuł SEO artykułu (max 60 znaków)">
                <meta name="description" content="Opis SEO artykułu (max 155 znaków)">
            
            2.  Po meta tagach, dodaj dwie linie przerwy (\\n\\n).
            3.  Następnie napisz pełny, wyczerpujący artykuł (minimum 500 słów) na zadany przez użytkownika temat.
            4.  Struktura: Zastosuj jasną strukturę z tytułem, wstępem, logicznie podzielonymi sekcjami (używaj podtytułów) i podsumowaniem.
            5.  Wskazówki stylu (${author}): ${outline}
            6.  ${technical}
            7.  Odpowiedz TYLKO wygenerowaną treścią (meta tagi + artykuł). Nie dodawaj żadnych wstępnych komentarzy typu "Oto artykuł:".`;
        }


        // ==== LOGIKA UI (TABY, MODALE, SUBSKRYPCJA) ====

        // Przełączanie zakładek
        tabButtons.forEach(button => {
            button.addEventListener('click', () => {
                // Deaktywuj wszystkie
                tabButtons.forEach(btn => {
                    btn.classList.remove('tab-active');
                    btn.classList.add('tab-inactive');
                });
                tabContents.forEach(content => {
                    content.classList.add('hidden');
                });

                // Aktywuj kliknięty
                button.classList.add('tab-active');
                button.classList.remove('tab-inactive');
                currentTab = button.dataset.tab;
                document.getElementById(currentTab).classList.remove('hidden');
            });
        });

        // Ustawianie stanu ładowania
        function setLoading(isLoading) {
            if (isLoading) {
                loadingModal.classList.remove('hidden');
                loadingModal.classList.add('flex');
            } else {
                loadingModal.classList.add('hidden');
                loadingModal.classList.remove('flex');
            }
        }

        // Pokazywanie błędu
        function showError(message) {
            errorMessage.textContent = message;
            errorModal.classList.remove('hidden');
            errorModal.classList.add('flex');
        }

        // Zamykanie modalu błędu
        closeErrorModal.addEventListener('click', () => {
            errorModal.classList.add('hidden');
            errorModal.classList.remove('flex');
        });

        // ==== LOGIKA SUBSKRYPCJI (SYMULACJA) ====

        // Otwieranie modalu płatności
        buyButtons.forEach(button => {
            button.addEventListener('click', () => {
                paymentModal.classList.remove('hidden');
                paymentModal.classList.add('flex');
            });
        });

        // Zamykanie modalu płatności
        closePaymentModal.addEventListener('click', () => {
            paymentModal.classList.add('hidden');
            paymentModal.classList.remove('flex');
        });

        // Potwierdzenie "płatności"
        confirmPaymentBtn.addEventListener('click', () => {
            isSubscribed = true;
            paymentModal.classList.add('hidden');
            paymentModal.classList.remove('flex');
            
            // Odblokuj aplikacje
            subscriptionOverlay.classList.add('hidden');
            
            // Pokaż powiadomienie o sukcesie (proste)
            alert("Płatność zakończona sukcesem! Aplikacje odblokowane.");
        });

        // Sprawdzanie subskrypcji przed akcją
        function checkSubscription() {
            if (!isSubscribed) {
                showError("Ta funkcja wymaga aktywnej subskrypcji. Wybierz plan w sekcji Cennik.");
                // Przewiń do cennika
                document.getElementById('pricing').scrollIntoView({ behavior: 'smooth' });
                return false;
            }
            return true;
        }

        // ==== LOGIKA PRZYCISKU KOPIOWANIA ====

        // Używamy delegacji zdarzeń, aby obsłużyć wszystkie przyciski kopiowania
        document.body.addEventListener('click', (e) => {
            // Szukamy klikniętego przycisku (lub jego rodzica, jeśli kliknięto ikonę/span)
            const copyButton = e.target.closest('.copy-button');
            
            if (copyButton) {
                const targetId = copyButton.dataset.target;
                const outputElement = document.getElementById(targetId);
                
                if (outputElement && outputElement.textContent) {
                    copyToClipboard(outputElement.textContent, copyButton);
                } else {
                    showError("Nie ma nic do skopiowania.");
                }
            }
        });

        function copyToClipboard(text, buttonElement) {
            // Używamy document.execCommand('copy') dla kompatybilności z iFrame
            const textarea = document.createElement('textarea');
            textarea.value = text;
            textarea.style.position = 'absolute';
            textarea.style.left = '-9999px'; // Ukryj element
            document.body.appendChild(textarea);
            textarea.select();
            
            try {
                document.execCommand('copy');
                // Zmień tekst przycisku, aby dać znać użytkownikowi
                const originalText = buttonElement.innerHTML;
                buttonElement.innerHTML = `
                    <svg xmlns="http://www.w3.org/2000/svg" class="w-4 h-4 inline-block mr-1" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7" />
                    </svg>
                    <span>Skopiowano!</span>`;
                
                setTimeout(() => {
                    buttonElement.innerHTML = originalText;
                }, 2000); // Wróć do oryginału po 2 sekundach

            } catch (err) {
                console.error('Błąd kopiowania do schowka:', err);
                showError('Nie udało się skopiować tekstu. Spróbuj ręcznie.');
            } finally {
                document.body.removeChild(textarea);
            }
        }

        // ==== LOGIKA BANERA COOKIES (NOWA) ====
        if (localStorage.getItem('cookiesAccepted') === 'true') {
            cookieBanner.classList.add('hidden');
        } else {
            cookieBanner.classList.remove('hidden');
        }

        acceptCookieBtn.addEventListener('click', () => {
            cookieBanner.classList.add('hidden');
            localStorage.setItem('cookiesAccepted', 'true');
        });

        // Otwieranie/zamykanie <details> w FAQ
        document.querySelectorAll('#faq details').forEach((detail) => {
            detail.addEventListener('toggle', (event) => {
                const summary = event.target.querySelector('summary');
                const icon = summary.querySelector('svg');
                if (event.target.open) {
                    icon.style.transform = 'rotate(180deg)';
                } else {
                    icon.style.transform = 'rotate(0deg)';
                }
            });
        });


    </script>
</body>
</html>
