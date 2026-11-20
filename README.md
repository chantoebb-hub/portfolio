<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Si Thu Min Htet | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Plus+Jakarta+Sans:wght@400;500;600;700&family=Noto+Sans+Myanmar:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'Noto Sans Myanmar', 'sans-serif'],
                        display: ['Space Grotesk', 'Noto Sans Myanmar', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #060913;
            color: #e2e8f0;
            background-image:
                radial-gradient(at 0% 0%, rgba(14, 165, 233, 0.14) 0px, transparent 50%),
                radial-gradient(at 100% 10%, rgba(16, 185, 129, 0.12) 0px, transparent 50%),
                radial-gradient(at 50% 100%, rgba(99, 102, 241, 0.12) 0px, transparent 50%);
            background-attachment: fixed;
        }
        .grid-bg {
            background-size: 40px 40px;
            background-image: linear-gradient(to right, rgba(255, 255, 255, 0.03) 1px, transparent 1px),
                              linear-gradient(to bottom, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
        }
        .bento-card {
            background: rgba(15, 23, 42, 0.65);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            transition: all 0.35s cubic-bezier(0.22, 1, 0.36, 1);
        }
        .bento-card:hover {
            border-color: rgba(56, 189, 248, 0.45);
            transform: translateY(-4px);
            box-shadow: 0 20px 40px -15px rgba(2, 132, 199, 0.2);
        }
        .gradient-text {
            background: linear-gradient(135deg, #38bdf8 0%, #34d399 50%, #818cf8 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .filter-pill.active {
            background: linear-gradient(135deg, #0284c7, #10b981);
            color: #ffffff;
            border-color: transparent;
        }
        .edu-tab.active {
            background: rgba(56, 189, 248, 0.18);
            color: #7dd3fc;
            border-color: rgba(56, 189, 248, 0.5);
        }
    </style>
</head>
<body class="grid-bg antialiased selection:bg-sky-500/30 selection:text-sky-200">

    <!-- Floating Glass Navigation -->
    <header class="fixed top-4 inset-x-0 z-50 px-4">
        <nav class="max-w-6xl mx-auto rounded-2xl bg-slate-900/80 backdrop-blur-xl border border-white/10 px-5 py-3 flex items-center justify-between shadow-2xl">
            <a href="#" class="font-display font-bold text-lg tracking-tight text-white flex items-center gap-2">
                <span class="w-2.5 h-2.5 rounded-full bg-gradient-to-tr from-sky-400 to-emerald-400"></span>
                <span>Si Thu<span class="text-sky-400">.</span></span>
            </a>

            <div class="hidden md:flex items-center gap-6 text-sm text-slate-300">
                <a href="#bento-about" class="hover:text-sky-400 transition" data-i18n="nav_about">Overview</a>
                <a href="#skills" class="hover:text-sky-400 transition" data-i18n="nav_skills">Capabilities</a>
                <a href="#experience" class="hover:text-sky-400 transition" data-i18n="nav_experience">Experience &amp; Outcomes</a>
                <a href="#education" class="hover:text-sky-400 transition" data-i18n="nav_education">Education &amp; Courses</a>
            </div>

            <div class="flex items-center gap-2.5">
                <button id="lang-btn" class="px-3 py-1.5 rounded-xl bg-white/5 hover:bg-white/10 border border-white/10 text-xs font-semibold text-sky-300 transition">
                    မြန်မာ / EN
                </button>
                <a href="#contact" class="px-4 py-1.5 rounded-xl bg-gradient-to-r from-sky-500 to-emerald-500 text-slate-950 font-bold text-xs sm:text-sm hover:opacity-90 transition" data-i18n="nav_contact">
                    Connect
                </a>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="pt-36 pb-14 px-4">
        <div class="max-w-6xl mx-auto">
            <div class="bento-card rounded-3xl p-8 sm:p-12 md:p-14 relative overflow-hidden">
                <div class="absolute -top-24 -right-24 w-72 h-72 bg-sky-500/20 rounded-full blur-3xl pointer-events-none"></div>
                <div class="absolute -bottom-24 -left-24 w-72 h-72 bg-emerald-500/15 rounded-full blur-3xl pointer-events-none"></div>

                <div class="relative z-10 max-w-3xl">
                    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-white/5 border border-white/10 text-xs font-medium text-emerald-300 mb-6">
                        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
                        <span data-i18n="hero_badge">Taunggyi, Myanmar • Youth &amp; Civic Leadership</span>
                    </div>

                    <h1 class="font-display text-4xl sm:text-6xl font-bold text-white tracking-tight leading-tight mb-4">
                        <span data-i18n="hero_name">Si Thu Min Htet</span>
                    </h1>

                    <p class="font-display text-xl sm:text-2xl font-semibold gradient-text mb-6" data-i18n="hero_role">
                        Community Educator &amp; Public Administration Enthusiast
                    </p>

                    <p class="text-slate-300 text-base sm:text-lg leading-relaxed mb-8" data-i18n="hero_summary">
                        Dedicated community educator, youth leader, and founder with hands-on experience in grassroots development, civic education, and teaching public administration concepts. Passionate about empowering local youth and communities through capacity-building, transparent governance awareness, and effective community management.
                    </p>

                    <div class="flex flex-wrap gap-3">
                        <a href="#experience" class="px-6 py-3 rounded-xl bg-white text-slate-950 font-semibold text-sm hover:bg-sky-100 transition inline-flex items-center gap-2">
                            <span data-i18n="hero_btn1">Outcomes &amp; Experience</span>
                            <i class="fas fa-chart-line text-xs"></i>
                        </a>
                        <a href="#contact" class="px-6 py-3 rounded-xl bg-white/5 hover:bg-white/10 border border-white/15 text-white font-semibold text-sm transition inline-flex items-center gap-2">
                            <i class="far fa-paper-plane text-sky-400"></i>
                            <span data-i18n="hero_btn2">Start a Conversation</span>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Bento Grid: Personal Details, Languages, Interests & Highlight -->
    <section id="bento-about" class="py-8 px-4">
        <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-12 gap-5">

            <!-- Highlight Spotlight Card -->
            <div class="md:col-span-7 bento-card rounded-3xl p-7 flex flex-col justify-between bg-gradient-to-br from-sky-950/60 via-slate-900/70 to-emerald-950/40">
                <div>
                    <span class="text-xs font-bold uppercase tracking-widest text-sky-400" data-i18n="spot_tag">Flagship Initiative</span>
                    <h2 class="font-display text-2xl sm:text-3xl font-bold text-white mt-2 mb-3" data-i18n="spot_title">Founder &amp; Volunteer Trainer at Future Youth Centre</h2>
                    <p class="text-slate-300 text-sm sm:text-base leading-relaxed" data-i18n="spot_desc">
                        Managing community educational initiatives and facilitating modules on basic public administration, governance concepts, and leadership to inspire active youth civic participation.
                    </p>
                </div>
                <div class="mt-6 pt-5 border-t border-white/10 flex flex-wrap gap-2">
                    <span class="px-3 py-1 rounded-lg bg-sky-500/15 text-sky-300 text-xs font-medium" data-i18n="tag_1">Civic Education</span>
                    <span class="px-3 py-1 rounded-lg bg-emerald-500/15 text-emerald-300 text-xs font-medium" data-i18n="tag_2">Grassroots Development</span>
                    <span class="px-3 py-1 rounded-lg bg-indigo-500/15 text-indigo-300 text-xs font-medium" data-i18n="tag_3">Youth Capacity Building</span>
                </div>
            </div>

            <!-- Personal Details Card -->
            <div class="md:col-span-5 bento-card rounded-3xl p-7">
                <h3 class="font-display text-lg font-bold text-white mb-5 flex items-center gap-2">
                    <i class="fas fa-id-badge text-sky-400"></i>
                    <span data-i18n="pd_title">Personal Details</span>
                </h3>
                <div class="space-y-3.5 text-sm">
                    <div class="flex justify-between border-b border-white/5 pb-2.5">
                        <span class="text-slate-400" data-i18n="pd_dob_lbl">Date of Birth</span>
                        <span class="text-white font-medium" data-i18n="pd_dob_val">October 30, 2004</span>
                    </div>
                    <div class="flex justify-between border-b border-white/5 pb-2.5">
                        <span class="text-slate-400" data-i18n="pd_gen_lbl">Gender</span>
                        <span class="text-white font-medium" data-i18n="pd_gen_val">Male</span>
                    </div>
                    <div class="flex justify-between border-b border-white/5 pb-2.5">
                        <span class="text-slate-400" data-i18n="pd_addr_lbl">Address</span>
                        <span class="text-white font-medium text-right">Pan Tin Road, Taunggyi</span>
                    </div>
                    <div class="flex justify-between border-b border-white/5 pb-2.5">
                        <span class="text-slate-400" data-i18n="pd_phone_lbl">Phone</span>
                        <a href="tel:09986713234" class="text-sky-400 hover:underline font-medium">09986713234</a>
                    </div>
                    <div class="flex justify-between">
                        <span class="text-slate-400" data-i18n="pd_email_lbl">Email</span>
                        <a href="mailto:sithu30102004@gmail.com" class="text-emerald-400 hover:underline font-medium truncate max-w-[190px]">sithu30102004@gmail.com</a>
                    </div>
                </div>
            </div>

            <!-- Languages Card -->
            <div class="md:col-span-5 bento-card rounded-3xl p-7">
                <h3 class="font-display text-lg font-bold text-white mb-5 flex items-center gap-2">
                    <i class="fas fa-language text-emerald-400"></i>
                    <span data-i18n="lang_heading">Languages</span>
                </h3>
                <div class="space-y-4">
                    <div>
                        <div class="flex justify-between text-sm mb-1.5">
                            <span class="text-white font-medium" data-i18n="lang_my">Burmese</span>
                            <span class="text-emerald-400 text-xs font-semibold" data-i18n="lang_my_lvl">Native</span>
                        </div>
                        <div class="w-full h-2 rounded-full bg-white/10 overflow-hidden">
                            <div class="h-full rounded-full bg-gradient-to-r from-sky-400 to-emerald-400 w-full"></div>
                        </div>
                    </div>
                    <div>
                        <div class="flex justify-between text-sm mb-1.5">
                            <span class="text-white font-medium" data-i18n="lang_en">English</span>
                            <span class="text-sky-400 text-xs font-semibold" data-i18n="lang_en_lvl">Pre-Intermediate (A2) / Working</span>
                        </div>
                        <div class="w-full h-2 rounded-full bg-white/10 overflow-hidden">
                            <div class="h-full rounded-full bg-gradient-to-r from-sky-400 to-indigo-400 w-[55%]"></div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Interests Card -->
            <div class="md:col-span-7 bento-card rounded-3xl p-7 flex flex-col justify-between">
                <h3 class="font-display text-lg font-bold text-white mb-4 flex items-center gap-2">
                    <i class="fas fa-sparkles text-indigo-400"></i>
                    <span data-i18n="int_heading">Interests &amp; Creative Focus</span>
                </h3>
                <div class="grid grid-cols-2 gap-3">
                    <div class="p-3.5 rounded-2xl bg-white/5 border border-white/5 flex items-center gap-3">
                        <div class="w-9 h-9 rounded-xl bg-sky-500/20 text-sky-300 flex items-center justify-center"><i class="fas fa-microphone-lines"></i></div>
                        <span class="text-sm font-medium text-slate-200" data-i18n="int_1">Public Speaking</span>
                    </div>
                    <div class="p-3.5 rounded-2xl bg-white/5 border border-white/5 flex items-center gap-3">
                        <div class="w-9 h-9 rounded-xl bg-emerald-500/20 text-emerald-300 flex items-center justify-center"><i class="fas fa-chalkboard-user"></i></div>
                        <span class="text-sm font-medium text-slate-200" data-i18n="int_2">Teaching</span>
                    </div>
                    <div class="p-3.5 rounded-2xl bg-white/5 border border-white/5 flex items-center gap-3">
                        <div class="w-9 h-9 rounded-xl bg-indigo-500/20 text-indigo-300 flex items-center justify-center"><i class="fas fa-magnifying-glass-chart"></i></div>
                        <span class="text-sm font-medium text-slate-200" data-i18n="int_3">Social Sciences Research</span>
                    </div>
                    <div class="p-3.5 rounded-2xl bg-white/5 border border-white/5 flex items-center gap-3">
                        <div class="w-9 h-9 rounded-xl bg-amber-500/20 text-amber-300 flex items-center justify-center"><i class="fas fa-feather-pointed"></i></div>
                        <span class="text-sm font-medium text-slate-200" data-i18n="int_4">Creative Prose Writing</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Core Skills Section -->
    <section id="skills" class="py-14 px-4">
        <div class="max-w-6xl mx-auto">
            <div class="mb-8">
                <span class="text-xs font-bold uppercase tracking-widest text-sky-400" data-i18n="sk_tag">Core Competencies</span>
                <h2 class="font-display text-3xl font-bold text-white mt-1" data-i18n="sk_heading">Skills &amp; Domain Strengths</h2>
            </div>

            <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-5">
                <div class="bento-card rounded-3xl p-6">
                    <div class="w-11 h-11 rounded-2xl bg-sky-500/15 text-sky-400 flex items-center justify-center text-lg mb-4">
                        <i class="fas fa-landmark"></i>
                    </div>
                    <h3 class="font-display font-bold text-white text-base mb-3" data-i18n="sk1_t">Public Administration &amp; Governance</h3>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-sky-400"></span><span data-i18n="sk1_1">Civic Education</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-sky-400"></span><span data-i18n="sk1_2">Community Management</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-sky-400"></span><span data-i18n="sk1_3">Policy Basics</span></li>
                    </ul>
                </div>

                <div class="bento-card rounded-3xl p-6">
                    <div class="w-11 h-11 rounded-2xl bg-emerald-500/15 text-emerald-400 flex items-center justify-center text-lg mb-4">
                        <i class="fas fa-users-gear"></i>
                    </div>
                    <h3 class="font-display font-bold text-white text-base mb-3" data-i18n="sk2_t">Training &amp; Facilitation</h3>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-emerald-400"></span><span data-i18n="sk2_1">Public Speaking</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-emerald-400"></span><span data-i18n="sk2_2">Youth Capacity Building</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-emerald-400"></span><span data-i18n="sk2_3">Curriculum Support</span></li>
                    </ul>
                </div>

                <div class="bento-card rounded-3xl p-6">
                    <div class="w-11 h-11 rounded-2xl bg-indigo-500/15 text-indigo-400 flex items-center justify-center text-lg mb-4">
                        <i class="fas fa-diagram-project"></i>
                    </div>
                    <h3 class="font-display font-bold text-white text-base mb-3" data-i18n="sk3_t">Project &amp; Leadership</h3>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-indigo-400"></span><span data-i18n="sk3_1">Founder &amp; Director</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-indigo-400"></span><span data-i18n="sk3_2">Community Engagement</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-indigo-400"></span><span data-i18n="sk3_3">Grassroots Development</span></li>
                    </ul>
                </div>

                <div class="bento-card rounded-3xl p-6">
                    <div class="w-11 h-11 rounded-2xl bg-amber-500/15 text-amber-400 flex items-center justify-center text-lg mb-4">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3 class="font-display font-bold text-white text-base mb-3" data-i18n="sk4_t">Digital Tools</h3>
                    <ul class="space-y-2 text-xs sm:text-sm text-slate-300">
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-amber-400"></span><span>Zoom &amp; Google Workspace</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-amber-400"></span><span>Google Sheets</span></li>
                        <li class="flex items-center gap-2"><span class="w-1.5 h-1.5 rounded-full bg-amber-400"></span><span>Canva</span></li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience & Outcomes Section -->
    <section id="experience" class="py-14 px-4">
        <div class="max-w-6xl mx-auto">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-4 mb-8">
                <div>
            
