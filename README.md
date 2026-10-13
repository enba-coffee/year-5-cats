[index.html.html](https://github.com/user-attachments/files/33363642/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YEAR 5 ENGLISH: CATS POETRY ADVENTURE</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Fredoka & Quicksand for playful primary school aesthetics -->
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        catAmber: '#F59E0B',
                        catOrange: '#F97316',
                        catTeal: '#0D9488',
                        catBlue: '#0284C7',
                        catPurple: '#8B5CF6',
                        catSoftBg: '#FFFBEB',
                        catCard: '#FFFFFF',
                    },
                    fontFamily: {
                        heading: ['Fredoka', 'sans-serif'],
                        body: ['Quicksand', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #FEF3C7;
            background-image: radial-gradient(#FDE68A 1.5px, transparent 1.5px);
            background-size: 24px 24px;
        }
        .font-heading {
            font-family: 'Fredoka', sans-serif;
        }
        .bounce-gentle {
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }
        .highlight-number {
            background-color: #FEF08A;
            border-bottom: 2px solid #EAB308;
            padding: 0 4px;
            border-radius: 4px;
            font-weight: bold;
            color: #854D0E;
        }
        .highlight-action {
            background-color: #BFDBFE;
            border-bottom: 2px solid #3B82F6;
            padding: 0 4px;
            border-radius: 4px;
            font-weight: bold;
            color: #1E40AF;
        }
        /* Custom scrollbars */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #FEF3C7;
        }
        ::-webkit-scrollbar-thumb {
            background: #F59E0B;
            border-radius: 10px;
        }
    </style>
</head>
<body class="text-slate-800 min-h-screen flex flex-col justify-between pb-12">

    <!-- Top Sticky Progress Bar & Help Banner -->
    <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md shadow-md border-b-4 border-amber-400">
        <div class="max-w-4xl mx-auto px-4 py-3 flex items-center justify-between gap-2">
            <div class="flex items-center gap-2">
                <span class="text-2xl">🐱</span>
                <div>
                    <h1 class="text-sm md:text-base font-bold font-heading text-amber-700 leading-tight">PdPR English Year 5</h1>
                    <p class="text-xs text-slate-500 font-semibold">Cats Poetry Adventure</p>
                </div>
            </div>

            <!-- Progress Indicator -->
            <div class="flex-1 max-w-xs mx-2">
                <div class="flex justify-between text-xs font-bold text-amber-800 mb-1">
                    <span>Worksheet Progress</span>
                    <span id="progress-percent">0%</span>
                </div>
                <div class="w-full bg-slate-200 rounded-full h-3 overflow-hidden border border-amber-300">
                    <div id="progress-bar" class="bg-gradient-to-r from-amber-400 to-orange-500 h-full w-0 transition-all duration-500"></div>
                </div>
            </div>

            <!-- Help Button -->
            <button onclick="toggleHelpModal()" class="bg-amber-500 hover:bg-amber-600 text-white font-bold py-1.5 px-3 rounded-xl shadow transition flex items-center gap-1 text-sm transform hover:scale-105 active:scale-95">
                <i class="fa-solid fa-circle-question"></i>
                <span class="hidden sm:inline">NEED HELP?</span>
            </button>
        </div>
    </header>

    <!-- Main Container -->
    <main class="max-w-4xl mx-auto px-4 py-6 w-full space-y-8">

        <!-- Banner & Welcome Section -->
        <section class="bg-gradient-to-br from-amber-400 via-orange-400 to-amber-500 rounded-3xl p-6 md:p-8 shadow-xl text-white relative overflow-hidden border-4 border-white">
            <div class="absolute -right-6 -bottom-6 text-9xl opacity-20 pointer-events-none select-none">🐾</div>
            <div class="relative z-10 flex flex-col md:flex-row items-center justify-between gap-6">
                <div class="text-center md:text-left space-y-3">
                    <span class="inline-block bg-amber-900/30 text-amber-100 font-bold text-xs uppercase px-3 py-1 rounded-full tracking-wider border border-amber-200/30">
                        Language Arts & Writing
                    </span>
                    <h1 class="text-3xl md:text-4xl font-extrabold font-heading tracking-wide drop-shadow">
                        YEAR 5 ENGLISH: CATS POETRY ADVENTURE
                    </h1>
                    <p class="text-lg md:text-xl font-medium text-amber-100 italic">
                        Read, Explore, Play and Create!
                    </p>
                </div>
                <!-- Cute SVG Cat Mascot -->
                <div class="flex-shrink-0 bg-white/20 p-4 rounded-2xl backdrop-blur-sm border border-white/30 bounce-gentle text-center">
                    <svg class="w-24 h-24 mx-auto text-amber-900 drop-shadow-md" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12 2C6.48 2 2 6.48 2 12c0 3.69 2.47 6.86 6 8.25V22l3-2 3 2v-1.75c3.53-1.39 6-4.56 6-8.25 0-5.52-4.48-10-10-10zm-3 8c.83 0 1.5.67 1.5 1.5S9.83 13 9 13s-1.5-.67-1.5-1.5S8.17 10 9 10zm6 0c.83 0 1.5.67 1.5 1.5s-.67 1.5-1.5 1.5-1.5-.67-1.5-1.5.67-1.5 1.5-1.5zm-3 7c-2 0-3.3-1-3.3-1h6.6s-1.3 1-3.3 1z"/>
                    </svg>
                    <span class="text-xs font-bold text-white uppercase tracking-wider block mt-1">Whisker the Guide</span>
                </div>
            </div>

            <!-- Welcome Message Box -->
            <div class="mt-6 bg-white/95 rounded-2xl p-5 text-slate-800 shadow-inner border-2 border-amber-200">
                <div class="flex items-start gap-3">
                    <span class="text-3xl">🐱</span>
                    <div>
                        <h2 class="font-bold text-amber-800 text-lg mb-1 font-heading">Welcome, Year 5 Explorer!</h2>
                        <p class="text-sm md:text-base leading-relaxed text-slate-700">
                            Hello, Year 5 pupils! Welcome to our <strong>Cats Poetry Adventure</strong>. Today, you will read a fun poem about cats, answer questions, practise spelling, and create your own imaginative response. Read each instruction carefully and complete all the activities. Have fun learning at home!
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Learning Objectives Card -->
        <section class="bg-white rounded-2xl p-6 shadow-md border-2 border-amber-200">
            <h2 class="text-xl font-bold font-heading text-amber-800 mb-3 flex items-center gap-2">
                <i class="fa-solid fa-bullseye text-orange-500"></i> Learning Objectives
            </h2>
            <p class="text-sm text-slate-600 mb-3">By the end of this lesson, you will be able to:</p>
            <ul class="grid grid-cols-1 md:grid-cols-2 gap-3 text-sm font-semibold text-slate-700">
                <li class="flex items-center gap-2 bg-amber-50 p-3 rounded-xl border border-amber-100">
                    <i class="fa-solid fa-check-circle text-amber-600 text-base"></i>
                    <span>Understand the main ideas in the poem "Cats".</span>
                </li>
                <li class="flex items-center gap-2 bg-amber-50 p-3 rounded-xl border border-amber-100">
                    <i class="fa-solid fa-check-circle text-amber-600 text-base"></i>
                    <span>Identify number words and action words.</span>
                </li>
                <li class="flex items-center gap-2 bg-amber-50 p-3 rounded-xl border border-amber-100">
                    <i class="fa-solid fa-check-circle text-amber-600 text-base"></i>
                    <span>Spell selected words from the poem accurately.</span>
                </li>
                <li class="flex items-center gap-2 bg-amber-50 p-3 rounded-xl border border-amber-100">
                    <i class="fa-solid fa-check-circle text-amber-600 text-base"></i>
                    <span>Create a simple poem, story, or role-play response.</span>
                </li>
            </ul>
        </section>

        <!-- Poem Section -->
        <section class="bg-gradient-to-b from-orange-50 to-amber-50 rounded-3xl p-6 md:p-8 shadow-md border-2 border-orange-300 relative">
            <div class="flex flex-col md:flex-row justify-between items-start md:items-center gap-4 border-b border-orange-200 pb-4 mb-4">
                <div>
                    <span class="text-xs font-bold text-orange-600 uppercase tracking-widest">Main Reading Text</span>
                    <h2 class="text-2xl font-extrabold font-heading text-slate-800">POEM: CATS</h2>
                </div>
                <!-- Read Aloud Speech Synthesis Button -->
                <button onclick="readPoemAloud()" id="audio-btn" class="bg-orange-500 hover:bg-orange-600 text-white font-bold py-2 px-4 rounded-xl shadow transition flex items-center gap-2 text-sm">
                    <i class="fa-solid fa-volume-high"></i>
                    <span id="audio-btn-text">Listen to Poem</span>
                </button>
            </div>

            <!-- Reading Instructions -->
            <div class="bg-amber-100/70 border-l-4 border-amber-500 p-3 rounded-r-xl mb-6 text-xs md:text-sm text-amber-900 font-medium">
                <p class="font-bold mb-1"><i class="fa-solid fa-list-check"></i> Reading Instructions:</p>
                <ol class="list-decimal list-inside space-y-1">
                    <li>Read the poem silently to yourself.</li>
                    <li>Read it aloud if possible for practice.</li>
                    <li>Read it again carefully before answering the questions.</li>
                    <li>You may scroll back to reread this poem anytime!</li>
                </ol>
            </div>

            <!-- Legend Toggle for Highlights -->
            <div class="flex flex-wrap items-center justify-between gap-2 mb-4 text-xs font-bold bg-white p-3 rounded-xl border border-orange-200">
                <span class="text-slate-600">Word Legend:</span>
                <div class="flex items-center gap-3">
                    <span class="highlight-number">Number Words (One, Two...)</span>
                    <span class="highlight-action">Action Words (scratching...)</span>
                </div>
            </div>

            <!-- Poem Content Box -->
            <div class="bg-white rounded-2xl p-6 md:p-8 shadow-inner border border-amber-200 font-body text-base md:text-xl text-slate-800 leading-relaxed text-center space-y-6">
                <!-- Verse 1 -->
                <div class="p-3 rounded-xl hover:bg-amber-50 transition border border-transparent hover:border-amber-200">
                    <p><span class="highlight-number">One</span> cat, <span class="highlight-number">two</span> cats, <span class="highlight-number">three</span> cats, <span class="highlight-number">four</span>,</p>
                    <p><span class="highlight-number">Four</span> cats <span class="highlight-action">scratching</span></p>
                    <p>At my gran's back door.</p>
                </div>
                
                <!-- Verse 2 -->
                <div class="p-3 rounded-xl hover:bg-amber-50 transition border border-transparent hover:border-amber-200">
                    <p><span class="highlight-number">Five</span> cats, <span class="highlight-number">six</span> cats, <span class="highlight-number">seven</span> cats, <span class="highlight-number">eight</span>,</p>
                    <p><span class="highlight-number">Eight</span> cats <span class="highlight-action">scratching</span></p>
                    <p>At my grandma's gate.</p>
                </div>

                <!-- Verse 3 -->
                <div class="p-3 rounded-xl hover:bg-amber-50 transition border border-transparent hover:border-amber-200">
                    <p><span class="highlight-number">Eight</span> cats, <span class="highlight-number">seven</span> cats, <span class="highlight-number">six</span> cats, <span class="highlight-number">five</span>,</p>
                    <p><span class="highlight-number">Five</span> cats <span class="highlight-action">scratching</span></p>
                    <p>At the old bee-hive.</p>
                </div>

                <!-- Verse 4 -->
                <div class="p-3 rounded-xl hover:bg-amber-50 transition border border-transparent hover:border-amber-200">
                    <p><span class="highlight-number">Four</span> cats, <span class="highlight-number">three</span> cats, <span class="highlight-number">two</span> cats, <span class="highlight-number">one</span>,</p>
                    <p><span class="highlight-number">One</span> cat <span class="highlight-action">napping</span></p>
                    <p>In the noon-day sun.</p>
                </div>
            </div>
        </section>

        <!-- ACTIVITY 1: LET'S UNDERSTAND THE POEM -->
        <section id="act1" class="bg-white rounded-3xl p-6 md:p-8 shadow-md border-2 border-slate-200">
            <div class="flex items-center justify-between mb-4 border-b pb-3">
                <div class="flex items-center gap-3">
                    <span class="bg-amber-500 text-white font-heading font-bold px-3 py-1 rounded-xl text-lg">1</span>
                    <h3 class="text-xl font-bold font-heading text-slate-800">Activity 1: Let's Understand the Poem</h3>
                </div>
                <span id="act1-badge" class="text-xs font-bold px-3 py-1 rounded-full bg-slate-100 text-slate-500">5 Questions</span>
            </div>
            <p class="text-sm text-slate-600 mb-6">Read the questions carefully and choose the correct answer for each.</p>

            <div class="space-y-6" id="act1-container">
                <!-- MCQ Q1 -->
                <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="act1-q1">
                    <p class="font-bold text-slate-800 mb-3 text-sm md:text-base">1. How many cats are scratching at the back door?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <button onclick="checkMCQ(1, 'Four', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Four</button>
                        <button onclick="checkMCQ(1, 'Five', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Five</button>
                        <button onclick="checkMCQ(1, 'Eight', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Eight</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- MCQ Q2 -->
                <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="act1-q2">
                    <p class="font-bold text-slate-800 mb-3 text-sm md:text-base">2. Where are the cats scratching in the second verse?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <button onclick="checkMCQ(2, 'At the gate', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">At the gate</button>
                        <button onclick="checkMCQ(2, 'In the garden', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">In the garden</button>
                        <button onclick="checkMCQ(2, 'Under the tree', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Under the tree</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- MCQ Q3 -->
                <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="act1-q3">
                    <p class="font-bold text-slate-800 mb-3 text-sm md:text-base">3. How many cats are scratching at the old bee-hive?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <button onclick="checkMCQ(3, 'One', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">One</button>
                        <button onclick="checkMCQ(3, 'Four', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Four</button>
                        <button onclick="checkMCQ(3, 'Five', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Five</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- MCQ Q4 -->
                <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="act1-q4">
                    <p class="font-bold text-slate-800 mb-3 text-sm md:text-base">4. What is the last cat doing?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <button onclick="checkMCQ(4, 'Running', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Running</button>
                        <button onclick="checkMCQ(4, 'Napping', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Napping</button>
                        <button onclick="checkMCQ(4, 'Climbing', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">Climbing</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- MCQ Q5 -->
                <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="act1-q5">
                    <p class="font-bold text-slate-800 mb-3 text-sm md:text-base">5. What is the weather or setting suggested by "in the noon-day sun"?</p>
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-2">
                        <button onclick="checkMCQ(5, 'A sunny daytime setting', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">A sunny daytime setting</button>
                        <button onclick="checkMCQ(5, 'A snowy night', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">A snowy night</button>
                        <button onclick="checkMCQ(5, 'A rainy evening', this)" class="act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 hover:border-amber-400 hover:bg-amber-50 transition">A rainy evening</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>
            </div>
        </section>

        <!-- ACTIVITY 2: COUNT THE CATS -->
        <section id="act2" class="bg-white rounded-3xl p-6 md:p-8 shadow-md border-2 border-slate-200">
            <div class="flex items-center justify-between mb-4 border-b pb-3">
                <div class="flex items-center gap-3">
                    <span class="bg-amber-500 text-white font-heading font-bold px-3 py-1 rounded-xl text-lg">2</span>
                    <h3 class="text-xl font-bold font-heading text-slate-800">Activity 2: Count the Cats</h3>
                </div>
                <span id="act2-badge" class="text-xs font-bold px-3 py-1 rounded-full bg-slate-100 text-slate-500">5 Questions</span>
            </div>
            <p class="text-sm text-slate-600 mb-6">Count the cartoon cats in each picture carefully, then select the matching number word.</p>

            <div class="space-y-6" id="act2-container">
                <!-- Q1: 3 Cats -->
                <div class="bg-amber-50/50 p-4 rounded-2xl border border-amber-200" id="act2-q1">
                    <div class="flex flex-col sm:flex-row items-center gap-4 mb-3">
                        <div class="bg-white p-3 rounded-2xl border border-amber-300 flex flex-wrap justify-center gap-2 max-w-xs w-full shadow-inner">
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                        </div>
                        <p class="font-bold text-slate-800 text-sm md:text-base">Question 1: How many cats are here?</p>
                    </div>
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="checkCount(1, 'three', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">two</button>
                        <button onclick="checkCount(1, 'three', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">three</button>
                        <button onclick="checkCount(1, 'three', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">five</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- Q2: 6 Cats -->
                <div class="bg-amber-50/50 p-4 rounded-2xl border border-amber-200" id="act2-q2">
                    <div class="flex flex-col sm:flex-row items-center gap-4 mb-3">
                        <div class="bg-white p-3 rounded-2xl border border-amber-300 flex flex-wrap justify-center gap-2 max-w-xs w-full shadow-inner">
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                        </div>
                        <p class="font-bold text-slate-800 text-sm md:text-base">Question 2: How many cats are here?</p>
                    </div>
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="checkCount(2, 'six', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">four</button>
                        <button onclick="checkCount(2, 'six', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">six</button>
                        <button onclick="checkCount(2, 'six', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">seven</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- Q3: 8 Cats -->
                <div class="bg-amber-50/50 p-4 rounded-2xl border border-amber-200" id="act2-q3">
                    <div class="flex flex-col sm:flex-row items-center gap-4 mb-3">
                        <div class="bg-white p-3 rounded-2xl border border-amber-300 flex flex-wrap justify-center gap-2 max-w-xs w-full shadow-inner">
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                        </div>
                        <p class="font-bold text-slate-800 text-sm md:text-base">Question 3: How many cats are here?</p>
                    </div>
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="checkCount(3, 'eight', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">six</button>
                        <button onclick="checkCount(3, 'eight', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">seven</button>
                        <button onclick="checkCount(3, 'eight', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">eight</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- Q4: 2 Cats -->
                <div class="bg-amber-50/50 p-4 rounded-2xl border border-amber-200" id="act2-q4">
                    <div class="flex flex-col sm:flex-row items-center gap-4 mb-3">
                        <div class="bg-white p-3 rounded-2xl border border-amber-300 flex flex-wrap justify-center gap-2 max-w-xs w-full shadow-inner">
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                        </div>
                        <p class="font-bold text-slate-800 text-sm md:text-base">Question 4: How many cats are here?</p>
                    </div>
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="checkCount(4, 'two', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">one</button>
                        <button onclick="checkCount(4, 'two', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">two</button>
                        <button onclick="checkCount(4, 'two', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">four</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>

                <!-- Q5: 5 Cats -->
                <div class="bg-amber-50/50 p-4 rounded-2xl border border-amber-200" id="act2-q5">
                    <div class="flex flex-col sm:flex-row items-center gap-4 mb-3">
                        <div class="bg-white p-3 rounded-2xl border border-amber-300 flex flex-wrap justify-center gap-2 max-w-xs w-full shadow-inner">
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                            <span class="text-3xl">🐱</span><span class="text-3xl">🐱</span>
                        </div>
                        <p class="font-bold text-slate-800 text-sm md:text-base">Question 5: How many cats are here?</p>
                    </div>
                    <div class="grid grid-cols-3 gap-2">
                        <button onclick="checkCount(5, 'five', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">three</button>
                        <button onclick="checkCount(5, 'five', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">five</button>
                        <button onclick="checkCount(5, 'five', this)" class="p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 hover:border-amber-400 transition text-center">eight</button>
                    </div>
                    <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                </div>
            </div>
        </section>

        <!-- ACTIVITY 3: SPELLING CHALLENGE -->
        <section id="act3" class="bg-white rounded-3xl p-6 md:p-8 shadow-md border-2 border-slate-200">
            <div class="flex items-center justify-between mb-4 border-b pb-3">
                <div class="flex items-center gap-3">
                    <span class="bg-amber-500 text-white font-heading font-bold px-3 py-1 rounded-xl text-lg">3</span>
                    <h3 class="text-xl font-bold font-heading text-slate-800">Activity 3: Spelling Challenge</h3>
                </div>
                <span id="act3-badge" class="text-xs font-bold px-3 py-1 rounded-full bg-slate-100 text-slate-500">7 Words</span>
            </div>
            <p class="text-sm text-slate-600 mb-6">Complete the missing letters, unscramble words, and choose correct spellings!</p>

            <div class="space-y-6">
                <!-- Part A: Missing Letters -->
                <div>
                    <h4 class="font-bold text-amber-800 text-sm uppercase tracking-wide mb-3 flex items-center gap-2">
                        <i class="fa-solid fa-pen-to-square"></i> Part A: Fill in the missing letters
                    </h4>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <!-- Q1: s_r_t_h_n_ (scratching) -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-1">
                            <label class="block text-xs font-bold text-slate-500 mb-1">Clue: Action of using claws on a door</label>
                            <p class="font-bold text-base mb-2 tracking-widest text-slate-700">s c r <span class="underline text-amber-600">a</span> t c h i <span class="underline text-amber-600">n</span> g</p>
                            <div class="flex gap-2">
                                <input type="text" id="spell-in-1" placeholder="Type full word" class="w-full px-3 py-2 border-2 border-slate-300 rounded-xl font-semibold text-sm focus:border-amber-500 outline-none">
                                <button onclick="checkSpellingInput(1, 'scratching')" class="bg-amber-500 text-white font-bold px-4 py-2 rounded-xl text-sm hover:bg-amber-600 transition">Check</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>

                        <!-- Q2: n_p_i_g (napping) -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-2">
                            <label class="block text-xs font-bold text-slate-500 mb-1">Clue: Sleeping for a short time in the sun</label>
                            <p class="font-bold text-base mb-2 tracking-widest text-slate-700">n <span class="underline text-amber-600">a</span> p p i <span class="underline text-amber-600">n</span> g</p>
                            <div class="flex gap-2">
                                <input type="text" id="spell-in-2" placeholder="Type full word" class="w-full px-3 py-2 border-2 border-slate-300 rounded-xl font-semibold text-sm focus:border-amber-500 outline-none">
                                <button onclick="checkSpellingInput(2, 'napping')" class="bg-amber-500 text-white font-bold px-4 py-2 rounded-xl text-sm hover:bg-amber-600 transition">Check</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>
                    </div>
                </div>

                <!-- Part B: Unscramble -->
                <div>
                    <h4 class="font-bold text-amber-800 text-sm uppercase tracking-wide mb-3 flex items-center gap-2">
                        <i class="fa-solid fa-shuffle"></i> Part B: Unscramble the letters
                    </h4>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <!-- Q3: g r a n d m a -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-3">
                            <p class="text-xs font-bold text-slate-500 mb-1">Unscramble: <span class="text-orange-600 bg-orange-100 px-2 py-0.5 rounded font-mono">m a g r d n a</span></p>
                            <div class="flex gap-2">
                                <input type="text" id="spell-in-3" placeholder="Type correct word" class="w-full px-3 py-2 border-2 border-slate-300 rounded-xl font-semibold text-sm focus:border-amber-500 outline-none">
                                <button onclick="checkSpellingInput(3, 'grandma')" class="bg-amber-500 text-white font-bold px-4 py-2 rounded-xl text-sm hover:bg-amber-600 transition">Check</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>

                        <!-- Q4: h i v e -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-4">
                            <p class="text-xs font-bold text-slate-500 mb-1">Unscramble: <span class="text-orange-600 bg-orange-100 px-2 py-0.5 rounded font-mono">v e h i</span></p>
                            <div class="flex gap-2">
                                <input type="text" id="spell-in-4" placeholder="Type correct word" class="w-full px-3 py-2 border-2 border-slate-300 rounded-xl font-semibold text-sm focus:border-amber-500 outline-none">
                                <button onclick="checkSpellingInput(4, 'hive')" class="bg-amber-500 text-white font-bold px-4 py-2 rounded-xl text-sm hover:bg-amber-600 transition">Check</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>
                    </div>
                </div>

                <!-- Part C: Choose correct spelling -->
                <div>
                    <h4 class="font-bold text-amber-800 text-sm uppercase tracking-wide mb-3 flex items-center gap-2">
                        <i class="fa-solid fa-list-check"></i> Part C: Choose the correct spelling
                    </h4>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <!-- Q5: cats -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-5">
                            <p class="font-bold text-slate-700 text-sm mb-2">Word 5: Plural of cat</p>
                            <div class="space-y-1.5">
                                <button onclick="checkSpellMCQ(5, 'cats', 'cats', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">cats</button>
                                <button onclick="checkSpellMCQ(5, 'katz', 'cats', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">katz</button>
                                <button onclick="checkSpellMCQ(5, 'catse', 'cats', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">catse</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>

                        <!-- Q6: gate -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-6">
                            <p class="font-bold text-slate-700 text-sm mb-2">Word 6: Outdoor door in fence</p>
                            <div class="space-y-1.5">
                                <button onclick="checkSpellMCQ(6, 'gaet', 'gate', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">gaet</button>
                                <button onclick="checkSpellMCQ(6, 'gate', 'gate', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">gate</button>
                                <button onclick="checkSpellMCQ(6, 'gait', 'gate', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">gait</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>

                        <!-- Q7: sun -->
                        <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200" id="spell-7">
                            <p class="font-bold text-slate-700 text-sm mb-2">Word 7: Bright star in day sky</p>
                            <div class="space-y-1.5">
                                <button onclick="checkSpellMCQ(7, 'son', 'sun', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">son</button>
                                <button onclick="checkSpellMCQ(7, 'san', 'sun', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">san</button>
                                <button onclick="checkSpellMCQ(7, 'sun', 'sun', this)" class="w-full text-left p-2 rounded-lg border bg-white hover:bg-amber-50 text-xs font-bold">sun</button>
                            </div>
                            <div class="feedback-box mt-2 text-xs font-bold hidden"></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- ACTIVITY 4: PUT THE VERSES IN ORDER -->
        <section id="act4" class="bg-white rounded-3xl p-6 md:p-8 shadow-md border-2 border-slate-200">
            <div class="flex items-center justify-between mb-4 border-b pb-3">
                <div class="flex items-center gap-3">
                    <span class="bg-amber-500 text-white font-heading font-bold px-3 py-1 rounded-xl text-lg">4</span>
                    <h3 class="text-xl font-bold font-heading text-slate-800">Activity 4: Put the Verses in Order</h3>
                </div>
                <span id="act4-badge" class="text-xs font-bold px-3 py-1 rounded-full bg-slate-100 text-slate-500">Sequencing</span>
            </div>
            <p class="text-sm text-slate-600 mb-6">These verses are mixed up! Assign numbers 1, 2, 3, and 4 to set them in the correct sequence of the poem.</p>

            <!-- Mixed up verses -->
            <div class="space-y-4" id="verse-order-list">
                <!-- Mixed Item A (Verse 3 original) -->
                <div class="bg-amber-50/60 p-4 rounded-2xl border-2 border-amber-200 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-3">
                    <div class="text-sm font-medium text-slate-800 space-y-1">
                        <p class="font-bold text-amber-900">Verse Box A:</p>
                        <p>Eight cats, seven cats, six cats, five,</p>
                        <p>Five cats scratching</p>
                        <p>At the old bee-hive.</p>
                    </div>
                    <div class="flex items-center gap-2 self-end sm:self-center">
                        <label class="text-xs font-bold text-slate-600">Position:</label>
                        <select id="verse-select-A" class="bg-white border-2 border-amber-400 rounded-xl px-3 py-2 font-bold text-amber-900 text-sm outline-none focus:ring-2 focus:ring-amber-500">
                            <option value="">Select #</option>
                            <option value="1">Verse 1</option>
                            <option value="2">Verse 2</option>
                            <option value="3">Verse 3</option>
                            <option value="4">Verse 4</option>
                        </select>
                    </div>
                </div>

                <!-- Mixed Item B (Verse 1 original) -->
                <div class="bg-amber-50/60 p-4 rounded-2xl border-2 border-amber-200 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-3">
                    <div class="text-sm font-medium text-slate-800 space-y-1">
                        <p class="font-bold text-amber-900">Verse Box B:</p>
                        <p>One cat, two cats, three cats, four,</p>
                        <p>Four cats scratching</p>
                        <p>At my gran's back door.</p>
                    </div>
                    <div class="flex items-center gap-2 self-end sm:self-center">
                        <label class="text-xs font-bold text-slate-600">Position:</label>
                        <select id="verse-select-B" class="bg-white border-2 border-amber-400 rounded-xl px-3 py-2 font-bold text-amber-900 text-sm outline-none focus:ring-2 focus:ring-amber-500">
                            <option value="">Select #</option>
                            <option value="1">Verse 1</option>
                            <option value="2">Verse 2</option>
                            <option value="3">Verse 3</option>
                            <option value="4">Verse 4</option>
                        </select>
                    </div>
                </div>

                <!-- Mixed Item C (Verse 4 original) -->
                <div class="bg-amber-50/60 p-4 rounded-2xl border-2 border-amber-200 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-3">
                    <div class="text-sm font-medium text-slate-800 space-y-1">
                        <p class="font-bold text-amber-900">Verse Box C:</p>
                        <p>Four cats, three cats, two cats, one,</p>
                        <p>One cat napping</p>
                        <p>In the noon-day sun.</p>
                    </div>
                    <div class="flex items-center gap-2 self-end sm:self-center">
                        <label class="text-xs font-bold text-slate-600">Position:</label>
                        <select id="verse-select-C" class="bg-white border-2 border-amber-400 rounded-xl px-3 py-2 font-bold text-amber-900 text-sm outline-none focus:ring-2 focus:ring-amber-500">
                            <option value="">Select #</option>
                            <option value="1">Verse 1</option>
                            <option value="2">Verse 2</option>
                            <option value="3">Verse 3</option>
                            <option value="4">Verse 4</option>
                        </select>
                    </div>
                </div>

                <!-- Mixed Item D (Verse 2 original) -->
                <div class="bg-amber-50/60 p-4 rounded-2xl border-2 border-amber-200 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-3">
                    <div class="text-sm font-medium text-slate-800 space-y-1">
                        <p class="font-bold text-amber-900">Verse Box D:</p>
                        <p>Five cats, six cats, seven cats, eight,</p>
                        <p>Eight cats scratching</p>
                        <p>At my grandma's gate.</p>
                    </div>
                    <div class="flex items-center gap-2 self-end sm:self-center">
                        <label class="text-xs font-bold text-slate-600">Position:</label>
                        <select id="verse-select-D" class="bg-white border-2 border-amber-400 rounded-xl px-3 py-2 font-bold text-amber-900 text-sm outline-none focus:ring-2 focus:ring-amber-500">
                            <option value="">Select #</option>
                            <option value="1">Verse 1</option>
                            <option value="2">Verse 2</option>
                            <option value="3">Verse 3</option>
                            <option value="4">Verse 4</option>
                        </select>
                    </div>
                </div>
            </div>

            <div class="mt-6 flex flex-col sm:flex-row items-center gap-4">
                <button onclick="checkVerseOrder()" class="w-full sm:w-auto bg-amber-500 hover:bg-amber-600 text-white font-bold py-3 px-6 rounded-2xl shadow transition flex items-center justify-center gap-2 text-sm">
                    <i class="fa-solid fa-check"></i> Check Verse Sequence
                </button>
                <div id="act4-feedback" class="text-sm font-bold hidden"></div>
            </div>
        </section>

        <!-- ACTIVITY 5: MY IMAGINATIVE RESPONSE -->
        <section id="act5" class="bg-gradient-to-br from-purple-50 to-indigo-50 rounded-3xl p-6 md:p-8 shadow-md border-2 border-purple-200">
            <div class="flex items-center justify-between mb-4 border-b border-purple-200 pb-3">
                <div class="flex items-center gap-3">
                    <span class="bg-purple-600 text-white font-heading font-bold px-3 py-1 rounded-xl text-lg">5</span>
                    <h3 class="text-xl font-bold font-heading text-purple-900">Activity 5: My Imaginative Response</h3>
                </div>
                <span class="text-xs font-bold px-3 py-1 rounded-full bg-purple-100 text-purple-700">Creative Task</span>
            </div>
            <p class="text-sm text-slate-700 mb-6">Choose <strong>ONE</strong> of the three tasks below to complete!</p>

            <!-- Option Tabs -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-3 mb-6">
                <button onclick="selectCreativeOption('A')" id="btn-opt-A" class="p-4 rounded-2xl border-2 border-purple-400 bg-white text-left transition hover:shadow-md">
                    <span class="text-xs font-bold text-purple-600 uppercase block mb-1">Option A</span>
                    <h4 class="font-bold text-slate-800 text-sm">Write Your Own Cat Poem</h4>
                    <p class="text-xs text-slate-500 mt-1">Write 4-6 lines about cats</p>
                </button>

                <button onclick="selectCreativeOption('B')" id="btn-opt-B" class="p-4 rounded-2xl border-2 border-slate-200 bg-white/70 text-left transition hover:shadow-md">
                    <span class="text-xs font-bold text-slate-500 uppercase block mb-1">Option B</span>
                    <h4 class="font-bold text-slate-800 text-sm">Create a Cat Adventure</h4>
                    <p class="text-xs text-slate-500 mt-1">Write 3-5 sentences about what happens next</p>
                </button>

                <button onclick="selectCreativeOption('C')" id="btn-opt-C" class="p-4 rounded-2xl border-2 border-slate-200 bg-white/70 text-left transition hover:shadow-md">
                    <span class="text-xs font-bold text-slate-500 uppercase block mb-1">Option C</span>
                    <h4 class="font-bold text-slate-800 text-sm">A Cat Role-Play Dialogue</h4>
                    <p class="text-xs text-slate-500 mt-1">Write a 4-6 line short dialogue between characters</p>
                </button>
            </div>

            <!-- Prompts & Helpful Word Bank -->
            <div id="creative-prompts-box" class="bg-white rounded-2xl p-4 border border-purple-200 mb-4 text-xs md:text-sm text-slate-700 space-y-2">
                <!-- Content dynamically updated via JS -->
            </div>

            <!-- Text Input Box -->
            <div class="space-y-3">
                <label for="creative-textarea" class="block font-bold text-purple-900 text-sm">
                    Type your work below (or write in your exercise book):
                </label>
                <textarea id="creative-textarea" rows="6" oninput="updateCreativeWordCount()" placeholder="Type your poem, story, or dialogue here..." class="w-full p-4 border-2 border-purple-300 rounded-2xl text-slate-800 font-medium focus:ring-2 focus:ring-purple-400 focus:border-purple-500 outline-none shadow-inner"></textarea>
                <div class="flex justify-between items-center text-xs text-slate-500 font-bold">
                    <span id="creative-word-count">Word count: 0 words</span>
                    <button onclick="copyCreativeText()" class="text-purple-700 hover:text-purple-900 flex items-center gap-1 bg-purple-100 px-3 py-1 rounded-lg">
                        <i class="fa-regular fa-copy"></i> Copy My Work
                    </button>
                </div>
            </div>

            <!-- Self-Check Checklist -->
            <div class="mt-6 bg-purple-100/60 p-4 rounded-2xl border border-purple-200">
                <h4 class="font-bold text-purple-900 text-sm mb-3 flex items-center gap-2">
                    <i class="fa-solid fa-square-check text-purple-600"></i> Self-Check Checklist
                </h4>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-2 text-xs font-bold text-purple-900">
                    <label class="flex items-center gap-2 cursor-pointer bg-white p-2.5 rounded-xl border border-purple-200">
                        <input type="checkbox" onchange="checkCreativeProgress()" class="chk-self rounded text-purple-600 focus:ring-purple-500 w-4 h-4">
                        <span>I completed my chosen task.</span>
                    </label>
                    <label class="flex items-center gap-2 cursor-pointer bg-white p-2.5 rounded-xl border border-purple-200">
                        <input type="checkbox" onchange="checkCreativeProgress()" class="chk-self rounded text-purple-600 focus:ring-purple-500 w-4 h-4">
                        <span>I used my own imaginative ideas.</span>
                    </label>
                    <label class="flex items-center gap-2 cursor-pointer bg-white p-2.5 rounded-xl border border-purple-200">
                        <input type="checkbox" onchange="checkCreativeProgress()" class="chk-self rounded text-purple-600 focus:ring-purple-500 w-4 h-4">
                        <span>I checked my spelling.</span>
                    </label>
                    <label class="flex items-center gap-2 cursor-pointer bg-white p-2.5 rounded-xl border border-purple-200">
                        <input type="checkbox" onchange="checkCreativeProgress()" class="chk-self rounded text-purple-600 focus:ring-purple-500 w-4 h-4">
                        <span>I used capital letters & full stops.</span>
                    </label>
                </div>
            </div>
        </section>

        <!-- Total Score Summary Card -->
        <section class="bg-gradient-to-r from-amber-500 to-orange-500 rounded-3xl p-6 text-white shadow-lg text-center space-y-4">
            <h3 class="text-2xl font-extrabold font-heading">YOUR WORKSHEET SUMMARY</h3>
            <p class="text-sm text-amber-100">Automatically graded objective sections (Activities 1 - 4):</p>
            <div class="inline-block bg-white text-amber-900 font-heading font-extrabold text-3xl md:text-4xl px-8 py-3 rounded-2xl shadow-inner">
                <span id="total-score-num">0</span> / 21 Points
            </div>
            <p class="text-xs text-amber-100 max-w-md mx-auto">
                Note: Your creative response in Activity 5 will be read and checked directly by your English teacher!
            </p>
            <div class="pt-2">
                <button onclick="resetAllActivities()" class="bg-amber-900/40 hover:bg-amber-900/60 text-white font-bold text-xs py-2 px-4 rounded-xl transition border border-white/30">
                    <i class="fa-solid fa-rotate-left"></i> Reset Worksheet & Try Again
                </button>
            </div>
        </section>

        <!-- GOOGLE CLASSROOM SUBMISSION INSTRUCTIONS -->
        <section class="bg-white rounded-3xl p-6 md:p-8 shadow-md border-2 border-teal-200">
            <h3 class="text-xl font-bold font-heading text-teal-800 mb-2 flex items-center gap-2">
                <i class="fa-solid fa-cloud-arrow-up text-teal-600"></i> HOW TO SUBMIT YOUR WORK
            </h3>
            <p class="text-xs text-slate-500 mb-4">Follow these simple steps when you finish your activities at home:</p>

            <ol class="space-y-3 text-sm text-slate-700">
                <li class="flex items-start gap-3 bg-teal-50/60 p-3 rounded-xl border border-teal-100">
                    <span class="bg-teal-600 text-white font-bold w-6 h-6 rounded-full flex items-center justify-center text-xs flex-shrink-0 mt-0.5">1</span>
                    <span>Complete all activities (1 to 5) on this page.</span>
                </li>
                <li class="flex items-start gap-3 bg-teal-50/60 p-3 rounded-xl border border-teal-100">
                    <span class="bg-teal-600 text-white font-bold w-6 h-6 rounded-full flex items-center justify-center text-xs flex-shrink-0 mt-0.5">2</span>
                    <span>If you typed your Activity 5 response here, copy your text or write it down clearly in your English exercise book.</span>
                </li>
                <li class="flex items-start gap-3 bg-teal-50/60 p-3 rounded-xl border border-teal-100">
                    <span class="bg-teal-600 text-white font-bold w-6 h-6 rounded-full flex items-center justify-center text-xs flex-shrink-0 mt-0.5">3</span>
                    <span>If written in your exercise book, take a clear photograph of your work.</span>
                </li>
                <li class="flex items-start gap-3 bg-teal-50/60 p-3 rounded-xl border border-teal-100">
                    <span class="bg-teal-600 text-white font-bold w-6 h-6 rounded-full flex items-center justify-center text-xs flex-shrink-0 mt-0.5">4</span>
                    <span>Open <strong>Google Classroom</strong> and go to the <strong>"Cats Poetry Adventure"</strong> assignment.</span>
                </li>
                <li class="flex items-start gap-3 bg-teal-50/60 p-3 rounded-xl border border-teal-100">
                    <span class="bg-teal-600 text-white font-bold w-6 h-6 rounded-full flex items-center justify-center text-xs flex-shrink-0 mt-0.5">5</span>
                    <span>Attach your photograph or text response, then click <strong>"Turn in"</strong> or <strong>"Hand in"</strong>.</span>
                </li>
            </ol>

            <!-- Technical Note -->
            <div class="mt-4 bg-slate-100 p-3 rounded-xl border border-slate-300 text-xs text-slate-600 italic">
                <i class="fa-solid fa-circle-info text-slate-500 mr-1"></i>
                <strong>Notice for pupils:</strong> This interactive page operates on your phone/computer screen. Answers are checked instantly on this page, but your creative response must be attached in Google Classroom so your teacher can award your final mark.
            </div>
        </section>

        <!-- FINAL COMPLETION CARD -->
        <section id="completion-screen" class="bg-gradient-to-br from-green-500 to-emerald-600 rounded-3xl p-6 md:p-8 text-white shadow-xl text-center space-y-4">
            <div class="text-5xl bounce-gentle">🎉</div>
            <h3 class="text-3xl font-extrabold font-heading">CONGRATULATIONS!</h3>
            <p class="text-base text-green-100 max-w-lg mx-auto">
                You have completed the Cats Poetry Adventure! Well done for reading, learning new words and using your imagination.
            </p>

            <div class="bg-white/10 backdrop-blur-md rounded-2xl p-4 max-w-md mx-auto text-left text-xs md:text-sm space-y-2 border border-white/20">
                <p class="font-bold text-green-200 uppercase tracking-wider mb-2">Completion Checklist:</p>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I read the poem.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I answered the comprehension questions.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I completed the spelling challenge.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I arranged the verses in order.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I created my imaginative response.</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check text-green-300"></i> I am ready to submit on Google Classroom.</div>
            </div>

            <p class="text-sm font-semibold text-green-100 pt-2">
                Keep learning and keep imagining. See you in our next English lesson!
            </p>
        </section>

    </main>

    <!-- Footer -->
    <footer class="text-center text-xs font-bold text-slate-500 py-6 border-t border-amber-200 mt-12">
        <p>Year 5 English Language PdPR • Content Standard 5.3 & 4.3</p>
        <p class="text-slate-400 font-normal mt-1">Made for independent home learning in Google Classroom</p>
    </footer>

    <!-- NEED HELP MODAL -->
    <div id="help-modal" class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm z-50 flex items-center justify-center p-4 hidden">
        <div class="bg-white rounded-3xl max-w-lg w-full max-h-[85vh] overflow-y-auto p-6 shadow-2xl border-4 border-amber-400 space-y-5 relative">
            
            <button onclick="toggleHelpModal()" class="absolute top-4 right-4 bg-slate-100 hover:bg-slate-200 text-slate-600 rounded-full w-8 h-8 flex items-center justify-center font-bold">
                ✕
            </button>

            <div class="flex items-center gap-3 border-b pb-3">
                <span class="text-3xl">🐱💡</span>
                <div>
                    <h3 class="text-xl font-bold font-heading text-amber-800">NEED HELP?</h3>
                    <p class="text-xs text-slate-500">Quick Helper Guide for Pupils</p>
                </div>
            </div>

            <!-- Helpful Definitions -->
            <div class="space-y-3 text-sm">
                <h4 class="font-bold text-amber-900 uppercase text-xs tracking-wider flex items-center gap-1">
                    <i class="fa-solid fa-book-open"></i> Word Definitions
                </h4>
                <div class="grid grid-cols-1 gap-2 text-xs text-slate-700">
                    <div class="bg-amber-50 p-2.5 rounded-xl border border-amber-200">
                        <strong>scratching:</strong> Rubbing claws against something.
                    </div>
                    <div class="bg-amber-50 p-2.5 rounded-xl border border-amber-200">
                        <strong>napping:</strong> Sleeping for a short time during the day.
                    </div>
                    <div class="bg-amber-50 p-2.5 rounded-xl border border-amber-200">
                        <strong>bee-hive:</strong> A home built for bees.
                    </div>
                    <div class="bg-amber-50 p-2.5 rounded-xl border border-amber-200">
                        <strong>noon-day:</strong> The middle of the day (12:00 PM).
                    </div>
                </div>

                <h4 class="font-bold text-amber-900 uppercase text-xs tracking-wider flex items-center gap-1 pt-2">
                    <i class="fa-solid fa-hashtag"></i> Number Words (1 - 8)
                </h4>
                <p class="text-xs font-semibold bg-slate-100 p-2.5 rounded-xl text-slate-800 tracking-wide">
                    one (1), two (2), three (3), four (4), five (5), six (6), seven (7), eight (8)
                </p>

                <h4 class="font-bold text-amber-900 uppercase text-xs tracking-wider flex items-center gap-1 pt-2">
                    <i class="fa-solid fa-running"></i> Action Words (Verbs)
                </h4>
                <p class="text-xs bg-slate-100 p-2.5 rounded-xl text-slate-800">
                    scratching, napping, playing, jumping, running, climbing, sleeping
                </p>

                <h4 class="font-bold text-amber-900 uppercase text-xs tracking-wider flex items-center gap-1 pt-2">
                    <i class="fa-solid fa-lightbulb text-amber-500"></i> Encouraging Message
                </h4>
                <div class="bg-orange-100 p-3 rounded-xl border border-orange-200 text-xs font-bold text-orange-900 text-center">
                    "Take your time! Read the poem as many times as you like. You can do it!"
                </div>
            </div>

            <button onclick="toggleHelpModal()" class="w-full bg-amber-500 hover:bg-amber-600 text-white font-bold py-2.5 rounded-xl transition text-sm">
                Got it! Back to Lesson
            </button>
        </div>
    </div>

    <script>
        // Global State Tally
        const scores = {
            act1: { 1: false, 2: false, 3: false, 4: false, 5: false },
            act2: { 1: false, 2: false, 3: false, 4: false, 5: false },
            act3: { 1: false, 2: false, 3: false, 4: false, 5: false, 6: false, 7: false },
            act4: false, // 4 points
            act5: false  // checklist done
        };

        const totalPossibleObjectivePoints = 21; // 5 + 5 + 7 + 4

        // Toggle Help Modal
        function toggleHelpModal() {
            const modal = document.getElementById('help-modal');
            modal.classList.toggle('hidden');
        }

        // Speech Synthesis for Poem Reading
        function readPoemAloud() {
            const btnText = document.getElementById('audio-btn-text');
            if ('speechSynthesis' in window) {
                if (window.speechSynthesis.speaking) {
                    window.speechSynthesis.cancel();
                    btnText.innerText = "Listen to Poem";
                    return;
                }

                const poemText = `
                    Cats.
                    One cat, two cats, three cats, four,
                    Four cats scratching at my gran's back door.
                    Five cats, six cats, seven cats, eight,
                    Eight cats scratching at my grandma's gate.
                    Eight cats, seven cats, six cats, five,
                    Five cats scratching at the old bee-hive.
                    Four cats, three cats, two cats, one,
                    One cat napping in the noon-day sun.
                `;

                const utterance = new SpeechSynthesisUtterance(poemText);
                utterance.rate = 0.85; // Slightly slower for primary students
                utterance.pitch = 1.1;

                utterance.onstart = () => {
                    btnText.innerText = "Playing... (Click to Stop)";
                };
                utterance.onend = () => {
                    btnText.innerText = "Listen to Poem";
                };

                window.speechSynthesis.speak(utterance);
            } else {
                alert("Speech synthesis is not supported on this device/browser.");
            }
        }

        // Activity 1: MCQ Checking
        const mcqAnswers = {
            1: "Four",
            2: "At the gate",
            3: "Five",
            4: "Napping",
            5: "A sunny daytime setting"
        };

        function checkMCQ(qNum, selectedVal, btnElement) {
            const parent = btnElement.closest('.bg-slate-50');
            const feedback = parent.querySelector('.feedback-box');
            const allBtns = parent.querySelectorAll('.act1-opt');

            // Reset buttons visual
            allBtns.forEach(b => {
                b.className = "act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 transition";
            });

            if (selectedVal === mcqAnswers[qNum]) {
                btnElement.className = "act1-opt text-left p-3 bg-green-100 rounded-xl border-2 border-green-500 font-bold text-green-900 transition";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-green-700 bg-green-50 p-2 rounded-lg border border-green-200 block";
                feedback.innerHTML = '<i class="fa-solid fa-circle-check"></i> Correct! Excellent job.';
                scores.act1[qNum] = true;
            } else {
                btnElement.className = "act1-opt text-left p-3 bg-red-100 rounded-xl border-2 border-red-400 font-bold text-red-900 transition";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-red-600 bg-red-50 p-2 rounded-lg border border-red-200 block";
                feedback.innerHTML = '<i class="fa-solid fa-circle-xmark"></i> Not quite right. Try again!';
                scores.act1[qNum] = false;
            }

            updateProgress();
        }

        // Activity 2: Count checking
        function checkCount(qNum, selectedWord, btnElement) {
            const correctWords = { 1: 'three', 2: 'six', 3: 'eight', 4: 'two', 5: 'five' };
            const parent = document.getElementById(`act2-q${qNum}`);
            const feedback = parent.querySelector('.feedback-box');
            const btns = parent.querySelectorAll('button');

            btns.forEach(b => {
                b.className = "p-2.5 bg-white rounded-xl border-2 border-slate-200 font-bold text-slate-700 transition text-center";
            });

            if (selectedWord === correctWords[qNum]) {
                btnElement.className = "p-2.5 bg-green-100 rounded-xl border-2 border-green-500 font-bold text-green-900 transition text-center";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-green-700 bg-green-50 p-2 rounded-lg block";
                feedback.innerHTML = '✨ Correct count!';
                scores.act2[qNum] = true;
            } else {
                btnElement.className = "p-2.5 bg-red-100 rounded-xl border-2 border-red-400 font-bold text-red-900 transition text-center";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-red-600 bg-red-50 p-2 rounded-lg block";
                feedback.innerHTML = '❌ Oops! Count the cats again.';
                scores.act2[qNum] = false;
            }

            updateProgress();
        }

        // Activity 3: Spelling Input Checking
        function checkSpellingInput(qNum, correctWord) {
            const input = document.getElementById(`spell-in-${qNum}`);
            const val = input.value.trim().toLowerCase();
            const parent = document.getElementById(`spell-${qNum}`);
            const feedback = parent.querySelector('.feedback-box');

            if (val === correctWord) {
                input.className = "w-full px-3 py-2 border-2 border-green-500 bg-green-50 rounded-xl font-bold text-sm text-green-900 outline-none";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-green-700 block";
                feedback.innerHTML = '✔ Correct spelling!';
                scores.act3[qNum] = true;
            } else {
                input.className = "w-full px-3 py-2 border-2 border-red-400 bg-red-50 rounded-xl font-bold text-sm text-red-900 outline-none";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-red-600 block";
                feedback.innerHTML = '✖ Incorrect spelling. Try again!';
                scores.act3[qNum] = false;
            }

            updateProgress();
        }

        function checkSpellMCQ(qNum, chosen, correct, btn) {
            const parent = document.getElementById(`spell-${qNum}`);
            const feedback = parent.querySelector('.feedback-box');
            const btns = parent.querySelectorAll('button');

            btns.forEach(b => b.className = "w-full text-left p-2 rounded-lg border bg-white text-xs font-bold");

            if (chosen === correct) {
                btn.className = "w-full text-left p-2 rounded-lg border-2 border-green-500 bg-green-100 text-green-900 text-xs font-bold";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-green-700 block";
                feedback.innerHTML = '✔ Correct!';
                scores.act3[qNum] = true;
            } else {
                btn.className = "w-full text-left p-2 rounded-lg border-2 border-red-400 bg-red-100 text-red-900 text-xs font-bold";
                feedback.className = "feedback-box mt-2 text-xs font-bold text-red-600 block";
                feedback.innerHTML = '✖ Try again!';
                scores.act3[qNum] = false;
            }

            updateProgress();
        }

        // Activity 4: Verse Sequencing
        function checkVerseOrder() {
            // Original poem order:
            // Verse Box A = original Verse 3 (should be position 3)
            // Verse Box B = original Verse 1 (should be position 1)
            // Verse Box C = original Verse 4 (should be position 4)
            // Verse Box D = original Verse 2 (should be position 2)

            const valA = document.getElementById('verse-select-A').value;
            const valB = document.getElementById('verse-select-B').value;
            const valC = document.getElementById('verse-select-C').value;
            const valD = document.getElementById('verse-select-D').value;

            const feedback = document.getElementById('act4-feedback');

            if (valB === '1' && valD === '2' && valA === '3' && valC === '4') {
                feedback.className = "text-sm font-bold text-green-700 bg-green-100 p-3 rounded-xl border border-green-300 block";
                feedback.innerHTML = '🎉 Perfect! All 4 verses are in the correct order!';
                scores.act4 = true;
            } else {
                feedback.className = "text-sm font-bold text-red-600 bg-red-100 p-3 rounded-xl border border-red-300 block";
                feedback.innerHTML = '❌ Some verses are in the wrong place. Reread the poem and try again!';
                scores.act4 = false;
            }

            updateProgress();
        }

        // Activity 5 Options & Prompt Switcher
        const creativePrompts = {
            A: `
                <p class="font-bold text-purple-900"><i class="fa-solid fa-pen-fancy"></i> Writing Starter (Option A - Poem):</p>
                <p class="italic text-purple-800">"One cat, two cats, playing in the ______."<br>"Three cats, four cats, jumping on the ______."</p>
                <p class="text-xs text-slate-500 pt-1">Useful words: jump, run, sleep, play, garden, tree, house, sun, one, two, three, four</p>
            `,
            B: `
                <p class="font-bold text-purple-900"><i class="fa-solid fa-book-open"></i> Story Starters (Option B - Adventure):</p>
                <p class="italic text-purple-800">• After that, the cats...<br>• Suddenly, the cats...<br>• The cats went to...<br>• At the end, ...</p>
            `,
            C: `
                <p class="font-bold text-purple-900"><i class="fa-solid fa-comments"></i> Role-Play Ideas (Option C - Dialogue):</p>
                <p class="italic text-purple-800">Person: "Hello little cats, why are you scratching?"<br>Cat: "Meow! We are looking for..."</p>
            `
        };

        function selectCreativeOption(option) {
            ['A', 'B', 'C'].forEach(opt => {
                const btn = document.getElementById(`btn-opt-${opt}`);
                if (opt === option) {
                    btn.className = "p-4 rounded-2xl border-2 border-purple-500 bg-purple-50 text-left transition shadow-sm";
                    btn.querySelector('span').className = "text-xs font-bold text-purple-700 uppercase block mb-1";
                } else {
                    btn.className = "p-4 rounded-2xl border-2 border-slate-200 bg-white/70 text-left transition hover:shadow-md";
                    btn.querySelector('span').className = "text-xs font-bold text-slate-400 uppercase block mb-1";
                }
            });

            document.getElementById('creative-prompts-box').innerHTML = creativePrompts[option];
        }

        function updateCreativeWordCount() {
            const text = document.getElementById('creative-textarea').value.trim();
            const words = text ? text.split(/\s+/).length : 0;
            document.getElementById('creative-word-count').innerText = `Word count: ${words} words`;
            checkCreativeProgress();
        }

        function copyCreativeText() {
            const textarea = document.getElementById('creative-textarea');
            if (!textarea.value.trim()) {
                alert("Please write something before copying!");
                return;
            }
            textarea.select();
            document.execCommand('copy');

            // Quick visual confirmation indicator
            const countLabel = document.getElementById('creative-word-count');
            const originalText = countLabel.innerText;
            countLabel.innerText = "✓ Copied to clipboard!";
            countLabel.style.color = "#0D9488";
            setTimeout(() => {
                countLabel.innerText = originalText;
                countLabel.style.color = "";
            }, 2000);
        }

        function checkCreativeProgress() {
            const text = document.getElementById('creative-textarea').value.trim();
            const checkboxes = document.querySelectorAll('.chk-self');
            let allChecked = true;
            checkboxes.forEach(c => { if (!c.checked) allChecked = false; });

            scores.act5 = (text.length > 10 && allChecked);
            updateProgress();
        }

        // Progress Tally Calculator
        function updateProgress() {
            let correctPoints = 0;

            // Act 1
            Object.values(scores.act1).forEach(v => { if (v) correctPoints++; });
            // Act 2
            Object.values(scores.act2).forEach(v => { if (v) correctPoints++; });
            // Act 3
            Object.values(scores.act3).forEach(v => { if (v) correctPoints++; });
            // Act 4 (4 points)
            if (scores.act4) correctPoints += 4;

            // Display Score
            document.getElementById('total-score-num').innerText = correctPoints;

            // Calculate percentage
            let totalItems = totalPossibleObjectivePoints + 1; // +1 for creative
            let currentDone = correctPoints + (scores.act5 ? 1 : 0);
            let percent = Math.min(100, Math.round((currentDone / totalItems) * 100));

            document.getElementById('progress-bar').style.width = percent + '%';
            document.getElementById('progress-percent').innerText = percent + '%';
        }

        // Reset Worksheet Function
        function resetAllActivities() {
            // Reset state
            for (let k in scores.act1) scores.act1[k] = false;
            for (let k in scores.act2) scores.act2[k] = false;
            for (let k in scores.act3) scores.act3[k] = false;
            scores.act4 = false;
            scores.act5 = false;

            // Clear inputs and styling
            document.querySelectorAll('input[type="text"]').forEach(i => {
                i.value = '';
                i.className = "w-full px-3 py-2 border-2 border-slate-300 rounded-xl font-semibold text-sm focus:border-amber-500 outline-none";
            });
            document.querySelectorAll('textarea').forEach(t => t.value = '');
            document.querySelectorAll('select').forEach(s => s.value = '');
            document.querySelectorAll('.chk-self').forEach(c => c.checked = false);
            document.querySelectorAll('.feedback-box').forEach(f => f.classList.add('hidden'));

            // Reset buttons
            document.querySelectorAll('.act1-opt').forEach(b => {
                b.className = "act1-opt text-left p-3 bg-white rounded-xl border-2 border-slate-200 font-semibold text-slate-700 transition";
            });

            updateProgress();
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Initialize defaults on load
        window.onload = function() {
            selectCreativeOption('A');
            updateProgress();
        };
    </script>
</body>
</html>
