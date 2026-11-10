<!DOCTYPE html>
<html lang="ru" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Котегова Анна — Графический и веб-дизайнер</title>

  <!-- Шрифты Manrope и Inter -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Manrope:wght@600;700;800&display=swap" rel="stylesheet">

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: '#cde648',
            'brand-hover': '#bada32',
            darkBg: '#121212',
            darkCard: '#1a1a1a',
          },
          fontFamily: {
            heading: ['Manrope', 'sans-serif'],
            sans: ['Inter', 'sans-serif'],
          }
        }
      }
    }
  </script>

  <style>
    body {
      font-family: 'Inter', sans-serif;
      background-color: #121212;
      color: #ffffff;
      overflow-x: hidden;
    }
    h1, h2, h3, h4, .font-heading {
      font-family: 'Manrope', sans-serif;
    }
    .ticker-wrap {
      display: flex;
      overflow: hidden;
      white-space: nowrap;
    }
    .ticker-move {
      display: flex;
      animation: ticker 25s linear infinite;
    }
    @keyframes ticker {
      0% { transform: translateX(0); }
      100% { transform: translateX(-50%); }
    }
  </style>
</head>
<body class="bg-darkBg text-white antialiased selection:bg-brand selection:text-black">

  <!-- ==================== HEADER ==================== -->
  <header class="sticky top-0 z-50 bg-brand text-black py-4 px-6 md:px-12 transition-all shadow-md">
    <div class="max-w-7xl mx-auto flex items-center justify-between">
      
      <!-- Переключатель языка -->
      <div class="flex items-center space-x-2 text-sm font-semibold">
        <button id="lang-ru" onclick="setLanguage('ru')" class="px-2.5 py-1 rounded bg-black text-white transition">RU</button>
        <span class="opacity-40">|</span>
        <button id="lang-en" onclick="setLanguage('en')" class="px-2.5 py-1 rounded text-black hover:opacity-70 transition">EN</button>
      </div>

      <!-- Логотип / Имя -->
      <a href="#" class="text-xl md:text-2xl font-extrabold tracking-wider font-heading">
        KOTEGOVA
      </a>

      <!-- Навигация и кнопка -->
      <div class="flex items-center space-x-6 md:space-x-8">
        <nav class="hidden md:flex space-x-6 font-medium text-sm">
          <a href="#services" class="hover:underline transition" data-i18n="nav-services">УСЛУГИ</a>
          <a href="#about" class="hover:underline transition" data-i18n="nav-about">ОБО МНЕ</a>
          <a href="#footer" class="hover:underline transition" data-i18n="nav-contacts">КОНТАКТЫ</a>
        </nav>
        <a href="https://t.me/KOTEGOVAAA" target="_blank" class="bg-white text-black font-semibold px-4 py-2 md:px-5 md:py-2.5 rounded-full text-xs md:text-sm hover:bg-black hover:text-white transition flex items-center gap-1 shadow-sm" data-i18n="btn-discuss">
          ОБСУДИТЬ ПРОЕКТ &rarr;
        </a>
      </div>
    </div>
  </header>


  <!-- ==================== HERO SECTION (ТЁМНЫЙ ФОН БЕЗ КАРТИНКИ) ==================== -->
  <section class="relative min-h-[85vh] bg-darkBg text-white flex flex-col justify-between py-16 px-6 md:px-12 border-b border-white/10">
    <div class="max-w-4xl mx-auto text-center my-auto pt-10">
      <p class="text-xs md:text-sm uppercase tracking-widest text-gray-400 font-semibold mb-6" data-i18n="hero-tag">
        НЕЗАВИСИМЫЙ ДИЗАЙНЕР — 6 ЛЕТ ОПЫТА
      </p>
      <h1 class="text-3xl sm:text-5xl md:text-6xl lg:text-7xl font-extrabold uppercase leading-tight tracking-tight mb-8 font-heading" data-i18n="hero-title">
        ВАШЕЙ КОМАНДЕ НУЖЕН ДИЗАЙНЕР<br><span class="text-brand">Я МОГУ ПОМОЧЬ</span>
      </h1>
      <p class="text-sm md:text-base lg:text-lg text-gray-300 max-w-2xl mx-auto mb-10 font-normal leading-relaxed" data-i18n="hero-sub">
        Графический и веб-дизайн для бизнеса и творческих команд. От повседневных дизайн-задач до крупных проектов — когда вашей команде нужна дополнительная помощь.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <a href="https://t.me/KOTEGOVAAA" target="_blank" class="w-full sm:w-auto bg-brand text-black font-bold px-8 py-4 rounded-full hover:bg-brand-hover transition text-sm flex items-center justify-center gap-2 shadow-lg" data-i18n="hero-btn-cta">
          ОБСУДИТЬ ПРОЕКТ &rarr;
        </a>
        <a href="https://www.behance.net/749cae0e" target="_blank" class="w-full sm:w-auto border border-white/40 hover:border-white text-white font-medium px-8 py-4 rounded-full transition text-sm flex items-center justify-center" data-i18n="hero-btn-portfolio">
          ПОСМОТРЕТЬ РАБОТЫ
        </a>
      </div>
    </div>

    <!-- Бегущая строка -->
    <div class="w-full overflow-hidden border-t border-b border-white/10 py-3 mt-12 bg-black/40">
      <div class="ticker-wrap">
        <div class="ticker-move text-xs md:text-sm font-semibold uppercase tracking-widest text-gray-400 gap-8">
          <span data-i18n="ticker">6 ЛЕТ В ДИЗАЙНЕ &bull; ГРАФИЧЕСКИЙ ДИЗАЙН &bull; ГИБКОЕ СОТРУДНИЧЕСТВО &bull; ВЕБ-ДИЗАЙН &bull; 6 ЛЕТ В ДИЗАЙНЕ &bull; ГРАФИЧЕСКИЙ ДИЗАЙН &bull; ГИБКОЕ СОТРУДНИЧЕСТВО &bull; ВЕБ-ДИЗАЙН &bull;</span>
          <span data-i18n="ticker">6 ЛЕТ В ДИЗАЙНЕ &bull; ГРАФИЧЕСКИЙ ДИЗАЙН &bull; ГИБКОЕ СОТРУДНИЧЕСТВО &bull; ВЕБ-ДИЗАЙН &bull; 6 ЛЕТ В ДИЗАЙНЕ &bull; ГРАФИЧЕСКИЙ ДИЗАЙН &bull; ГИБКОЕ СОТРУДНИЧЕСТВО &bull; ВЕБ-ДИЗАЙН &bull;</span>
        </div>
      </div>
    </div>
  </section>


  <!-- ==================== SERVICES SECTION ==================== -->
  <section id="services" class="py-20 px-6 md:px-12 bg-white text-black">
    <div class="max-w-7xl mx-auto">
      <div class="mb-14">
        <h2 class="text-3xl md:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading mb-6" data-i18n="services-title">
          ЧЕМ Я МОГУ ПОМОЧЬ<br>ВАШЕЙ КОМАНДЕ?
        </h2>
        <p class="text-gray-600 max-w-xl text-base md:text-lg leading-relaxed" data-i18n="services-desc">
          Один дизайнер — несколько направлений работы. Помогаю бизнесу поддерживать единый визуальный стиль и двигать проекты вперёд.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
        <!-- Блок 1 -->
        <div class="space-y-4">
          <h3 class="text-xl font-bold uppercase tracking-wide font-heading border-b-2 border-black pb-2" data-i18n="s1-title">ГРАФИЧЕСКИЙ ДИЗАЙН</h3>
          <p class="text-sm text-gray-500" data-i18n="s1-desc">Визуальная коммуникация вашего бренда.</p>
          <div class="flex flex-wrap gap-2 pt-2">
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s1-t1">Рекламные материалы</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s1-t2">Афиши и баннеры</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s1-t3">Презентации</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s1-t4">Графика для соцсетей</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s1-t5">Полиграфия и вёрстка</span>
          </div>
        </div>

        <!-- Блок 2 -->
        <div class="space-y-4">
          <h3 class="text-xl font-bold uppercase tracking-wide font-heading border-b-2 border-black pb-2" data-i18n="s2-title">ВЕБ-ДИЗАЙН</h3>
          <p class="text-sm text-gray-500" data-i18n="s2-desc">Цифровые решения для вашего бизнеса.</p>
          <div class="flex flex-wrap gap-2 pt-2">
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s2-t1">Лендинги</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s2-t2">Дизайн сайтов</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s2-t3">UI-дизайн</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s2-t4">Редизайн сайтов</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s2-t5">Цифровые макеты</span>
          </div>
        </div>

        <!-- Блок 3 -->
        <div class="space-y-4">
          <h3 class="text-xl font-bold uppercase tracking-wide font-heading border-b-2 border-black pb-2" data-i18n="s3-title">ПОСТОЯННАЯ ПОДДЕРЖКА</h3>
          <p class="text-sm text-gray-500" data-i18n="s3-desc">Дополнительные творческие ресурсы, когда они нужны.</p>
          <div class="flex flex-wrap gap-2 pt-2">
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s3-t1">Регулярные задачи</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s3-t2">Материалы для спецпроектов</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s3-t3">Помощь при высокой загрузке</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s3-t4">Работа с командами</span>
            <span class="bg-brand text-black font-medium text-xs md:text-sm px-4 py-2 rounded-full" data-i18n="s3-t5">Долгосрочное партнерство</span>
          </div>
        </div>
      </div>
    </div>
  </section>


  <!-- ==================== HOW I WORK SECTION ==================== -->
  <section class="py-20 px-6 md:px-12 bg-brand text-black">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-3xl md:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading mb-14" data-i18n="how-title">
        ДОПОЛНИТЕЛЬНЫЙ ДИЗАЙНЕР<br>БЕЗ НЕОБХОДИМОСТИ НАНИМАТЬ СОТРУДНИКА
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Step 1 -->
        <div class="bg-darkBg text-white p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="h1-step">Шаг 01</span>
            <h3 class="text-xl md:text-2xl font-bold uppercase font-heading mt-2 mb-4" data-i18n="h1-title">РАССКАЖИТЕ О ЗАДАЧАХ</h3>
            <p class="text-gray-300 text-sm leading-relaxed" data-i18n="h1-desc">
              Познакомимся с вашим бизнесом, текущими проектами и потребностями в дизайне.
            </p>
          </div>
        </div>

        <!-- Step 2 -->
        <div class="bg-darkBg text-white p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="h2-step">Шаг 02</span>
            <h3 class="text-xl md:text-2xl font-bold uppercase font-heading mt-2 mb-4" data-i18n="h2-title">ПОДБЕРЁМ ФОРМАТ РАБОТЫ</h3>
            <p class="text-gray-300 text-sm leading-relaxed" data-i18n="h2-desc">
              Определим объём задач, приоритеты, сроки и удобный способ коммуникации.
            </p>
          </div>
        </div>

        <!-- Step 3 -->
        <div class="bg-darkBg text-white p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="h3-step">Шаг 03</span>
            <h3 class="text-xl md:text-2xl font-bold uppercase font-heading mt-2 mb-4" data-i18n="h3-title">Я ПОДКЛЮЧАЮСЬ К ПРОЦЕССУ</h3>
            <p class="text-gray-300 text-sm leading-relaxed" data-i18n="h3-desc">
              Беру на себя дизайн-задачи, взаимодействую с вашей командой и передаю готовые материалы.
            </p>
          </div>
        </div>

        <!-- Step 4 -->
        <div class="bg-darkBg text-white p-8 rounded-2xl flex flex-col justify-between">
          <div>
            <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="h4-step">Шаг 04</span>
            <h3 class="text-xl md:text-2xl font-bold uppercase font-heading mt-2 mb-4" data-i18n="h4-title">ПРОДОЛЖАЕМ СОТРУДНИЧЕСТВО</h3>
            <p class="text-gray-300 text-sm leading-relaxed" data-i18n="h4-desc">
              Работаем на постоянной основе или подключаемся друг к другу по мере необходимости.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>


  <!-- ==================== ABOUT ME SECTION ==================== -->
  <section id="about" class="py-20 px-6 md:px-12 bg-darkBg text-white">
    <div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
      
      <!-- Текстовая колонка -->
      <div class="lg:col-span-7 space-y-6">
        <p class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="about-subtitle">
          Немного о человеке за всеми этими пикселями
        </p>
        <h2 class="text-3xl sm:text-5xl font-extrabold uppercase leading-tight font-heading" data-i18n="about-title">
          МЕНЯ ЗОВУТ<br><span class="text-brand">КОТЕГОВА АННА</span>
        </h2>
        <p class="text-gray-300 text-sm sm:text-base leading-relaxed max-w-2xl" data-i18n="about-desc">
          Работаю с визуальной идентичностью, цифровым дизайном и коммуникационными материалами, помогая бизнесу превращать идеи в понятные и продуманные визуальные решения.
        </p>

        <!-- Статистические плашки -->
        <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 py-4">
          <div class="bg-brand text-black p-4 md:p-6 rounded-2xl text-center">
            <div class="text-2xl sm:text-4xl font-extrabold font-heading">6 лет</div>
            <div class="text-xs sm:text-sm font-medium mt-1" data-i18n="about-s1">В дизайне</div>
          </div>
          <div class="bg-brand text-black p-4 md:p-6 rounded-2xl text-center">
            <div class="text-2xl sm:text-4xl font-extrabold font-heading">15+</div>
            <div class="text-xs sm:text-sm font-medium mt-1" data-i18n="about-s2">Оформленных мероприятий</div>
          </div>
          <div class="bg-brand text-black p-4 md:p-6 rounded-2xl text-center">
            <div class="text-2xl sm:text-4xl font-extrabold font-heading">30+</div>
            <div class="text-xs sm:text-sm font-medium mt-1" data-i18n="about-s3">Личных проектов</div>
          </div>
        </div>

        <div class="pt-2">
          <p class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="about-goal-label">МОЯ ЦЕЛЬ ПРОСТА:</p>
          <p class="text-base sm:text-lg font-medium text-white" data-i18n="about-goal-text">
            Стать надёжным дизайн-партнёром, на которого можно рассчитывать.
          </p>
        </div>
      </div>

      <!-- Ваше фото -->
      <div class="lg:col-span-5 flex justify-center">
        <div class="relative w-full max-w-md rounded-3xl overflow-hidden shadow-2xl border border-white/10">
          <img src="https://i.ibb.co/9HHnZYpp/image.png" alt="Анна Котегова" class="w-full h-auto object-cover transform hover:scale-105 transition duration-500">
        </div>
      </div>

    </div>
  </section>


  <!-- ==================== PORTFOLIO SECTION ==================== -->
  <section id="portfolio" class="py-20 px-6 md:px-12 bg-white text-black">
    <div class="max-w-7xl mx-auto">
      <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-6">
        <div>
          <h2 class="text-3xl md:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading" data-i18n="portfolio-title">
            ИЗБРАННЫЕ ПРОЕКТЫ
          </h2>
          <p class="text-gray-600 max-w-xl text-sm md:text-base mt-4" data-i18n="portfolio-desc">
            Подборка проектов в области визуальной идентичности, цифрового и графического дизайна.
          </p>
        </div>
        <a href="https://www.behance.net/749cae0e" target="_blank" class="border-2 border-black text-black px-6 py-3 rounded-full text-xs font-bold uppercase hover:bg-black hover:text-white transition self-start md:self-auto" data-i18n="portfolio-btn">
          ПОСМОТРЕТЬ РАБОТЫ
        </a>
      </div>

      <!-- Карточки порфолио -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        
        <!-- Карточка 1: Брендинг и айдентика -->
        <a href="https://www.behance.net/749cae0e" target="_blank" class="group block">
          <div class="rounded-2xl overflow-hidden bg-gray-100 mb-4 border border-gray-200 aspect-[4/5] flex items-center justify-center">
            <img src="https://i.ibb.co/pjGw6c8c/Frame-2085661117.png" alt="Брендинг и айдентика" class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
          </div>
          <h3 class="text-lg font-bold uppercase font-heading group-hover:text-brand-hover transition" data-i18n="p1-title">
            БРЕНДИНГ И АЙДЕНТИКА
          </h3>
        </a>

        <!-- Карточка 2: Графический дизайн и полиграфия -->
        <a href="https://www.behance.net/749cae0e" target="_blank" class="group block">
          <div class="rounded-2xl overflow-hidden bg-gray-100 mb-4 border border-gray-200 aspect-[4/5] flex items-center justify-center">
            <img src="https://i.ibb.co/JFHzXtk9/Frame-2085661119.png" alt="Графический дизайн и полиграфия" class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
          </div>
          <h3 class="text-lg font-bold uppercase font-heading group-hover:text-brand-hover transition" data-i18n="p2-title">
            ГРАФИЧЕСКИЙ ДИЗАЙН И ПОЛИГРАФИЯ
          </h3>
        </a>

        <!-- Карточка 3: Цифровой дизайн и веб-дизайн -->
        <a href="https://www.behance.net/749cae0e" target="_blank" class="group block">
          <div class="rounded-2xl overflow-hidden bg-gray-100 mb-4 border border-gray-200 aspect-[4/5] flex items-center justify-center">
            <img src="https://i.ibb.co/s98bfDH6/Frame-2085661118.png" alt="Цифровой дизайн и веб-дизайн" class="w-full h-full object-cover group-hover:scale-105 transition duration-500">
          </div>
          <h3 class="text-lg font-bold uppercase font-heading group-hover:text-brand-hover transition" data-i18n="p3-title">
            ЦИФРОВОЙ ДИЗАЙН И ВЕБ-ДИЗАЙН
          </h3>
        </a>

      </div>
    </div>
  </section>


  <!-- ==================== COOPERATION SECTION (ИСПРАВЛЕНА АДАПТИВНОСТЬ) ==================== -->
  <section class="py-20 px-6 md:px-12 bg-brand text-black">
    <div class="max-w-7xl mx-auto flex flex-col lg:flex-row gap-12 items-start justify-between">
      
      <!-- Заголовок и левый текст (разделены сеткой, не накладываются на плашки) -->
      <div class="w-full lg:w-1/2 space-y-6 lg:sticky lg:top-28">
        <h2 class="text-3xl sm:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading" data-i18n="coop-title">
          ФОРМАТЫ<br>СОТРУДНИЧЕСТВА
        </h2>
        <div class="space-y-4 text-sm sm:text-base leading-relaxed text-black/90 max-w-lg">
          <p class="font-semibold text-lg" data-i18n="coop-sub">Давайте найдём подходящий формат сотрудничества.</p>
          <p data-i18n="coop-desc">
            Любое сотрудничество начинается с разговора. Помогу подобрать формат, который подойдёт вашей команде и бюджету.
          </p>
        </div>
      </div>

      <!-- Варианты плашек -->
      <div class="w-full lg:w-1/2 space-y-6">
        
        <!-- Вариант 01 -->
        <div class="bg-darkBg text-white p-6 sm:p-8 rounded-2xl space-y-3 shadow-lg">
          <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="v1-opt">Вариант 01</span>
          <h3 class="text-xl md:text-2xl font-bold uppercase font-heading text-white" data-i18n="v1-title">
            ПОСТОЯННОЕ СОТРУДНИЧЕСТВО
          </h3>
          <p class="text-gray-300 text-sm leading-relaxed" data-i18n="v1-desc">
            Регулярная дизайн-поддержка для бизнеса, которому нужен надёжный творческий партнёр.
          </p>
        </div>

        <!-- Вариант 02 -->
        <div class="bg-darkBg text-white p-6 sm:p-8 rounded-2xl space-y-3 shadow-lg">
          <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="v2-opt">Вариант 02</span>
          <h3 class="text-xl md:text-2xl font-bold uppercase font-heading text-white" data-i18n="v2-title">
            ПРОЕКТНАЯ РАБОТА
          </h3>
          <p class="text-gray-300 text-sm leading-relaxed" data-i18n="v2-desc">
            Определённый объём задач с согласованными сроками и результатами.
          </p>
        </div>

        <!-- Вариант 03 -->
        <div class="bg-darkBg text-white p-6 sm:p-8 rounded-2xl space-y-3 shadow-lg">
          <span class="text-xs uppercase tracking-widest text-gray-400 font-medium" data-i18n="v3-opt">Вариант 03</span>
          <h3 class="text-xl md:text-2xl font-bold uppercase font-heading text-white" data-i18n="v3-title">
            ПОДКЛЮЧЕНИЕ ПО ЗАПРОСУ
          </h3>
          <p class="text-gray-300 text-sm leading-relaxed" data-i18n="v3-desc">
            Дополнительные ресурсы для дизайна, когда команда перегружена или сроки поджимают.
          </p>
        </div>

      </div>

    </div>
  </section>


  <!-- ==================== FAQ SECTION ==================== -->
  <section class="py-20 px-6 md:px-12 bg-darkBg text-white">
    <div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
      
      <div class="lg:col-span-5">
        <h2 class="text-3xl sm:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading sticky top-28" data-i18n="faq-title">
          ЧАСТЫЕ<br>ВОПРОСЫ
        </h2>
      </div>

      <!-- Диалоговые бабблы -->
      <div class="lg:col-span-7 space-y-8">
        
        <!-- Q1 -->
        <div class="space-y-2">
          <span class="text-xs uppercase tracking-wider text-gray-400 block" data-i18n="faq-client">Клиент</span>
          <div class="bg-brand text-black p-5 rounded-2xl rounded-tl-none font-medium text-sm md:text-base max-w-xl" data-i18n="q1">
            Вы работаете с компаниями на постоянной основе?
          </div>
          <span class="text-xs uppercase tracking-wider text-gray-400 block text-right" data-i18n="faq-designer">Дизайнер</span>
          <div class="bg-white text-black p-5 rounded-2xl rounded-tr-none text-sm md:text-base max-w-xl ml-auto" data-i18n="a1">
            Да! Мне особенно интересен формат долгосрочного сотрудничества и роль внешнего дизайн-специалиста для бизнеса и творческих команд.
          </div>
        </div>

        <!-- Q2 -->
        <div class="space-y-2">
          <span class="text-xs uppercase tracking-wider text-gray-400 block" data-i18n="faq-client">Клиент</span>
          <div class="bg-brand text-black p-5 rounded-2xl rounded-tl-none font-medium text-sm md:text-base max-w-xl" data-i18n="q2">
            Можете ли вы работать с нашей внутренней командой?
          </div>
          <span class="text-xs uppercase tracking-wider text-gray-400 block text-right" data-i18n="faq-designer">Дизайнер</span>
          <div class="bg-white text-black p-5 rounded-2xl rounded-tr-none text-sm md:text-base max-w-xl ml-auto" data-i18n="a2">
            Конечно. Могу взаимодействовать с маркетологами, арт-директорами, разработчиками и другими дизайнерами.
          </div>
        </div>

        <!-- Q3 -->
        <div class="space-y-2">
          <span class="text-xs uppercase tracking-wider text-gray-400 block" data-i18n="faq-client">Клиент</span>
          <div class="bg-brand text-black p-5 rounded-2xl rounded-tl-none font-medium text-sm md:text-base max-w-xl" data-i18n="q3">
            Вы берёте только большие проекты?
          </div>
          <span class="text-xs uppercase tracking-wider text-gray-400 block text-right" data-i18n="faq-designer">Дизайнер</span>
          <div class="bg-white text-black p-5 rounded-2xl rounded-tr-none text-sm md:text-base max-w-xl ml-auto" data-i18n="a3">
            Нет. Я могу выполнять как отдельные задачи, так и работать над крупными проектами.
          </div>
        </div>

        <!-- Q4 -->
        <div class="space-y-2">
          <span class="text-xs uppercase tracking-wider text-gray-400 block" data-i18n="faq-client">Клиент</span>
          <div class="bg-brand text-black p-5 rounded-2xl rounded-tl-none font-medium text-sm md:text-base max-w-xl" data-i18n="q4">
            Как начать сотрудничество?
          </div>
          <span class="text-xs uppercase tracking-wider text-gray-400 block text-right" data-i18n="faq-designer">Дизайнер</span>
          <div class="bg-white text-black p-5 rounded-2xl rounded-tr-none text-sm md:text-base max-w-xl ml-auto" data-i18n="a4">
            Просто свяжитесь со мной, расскажите о компании и о том, какая помощь с дизайном вам нужна. Обсудим детали и дальнейшие шаги.
          </div>
        </div>

        <!-- Q5 -->
        <div class="space-y-2">
          <span class="text-xs uppercase tracking-wider text-gray-400 block" data-i18n="faq-client">Клиент</span>
          <div class="bg-brand text-black p-5 rounded-2xl rounded-tl-none font-medium text-sm md:text-base max-w-xl" data-i18n="q5">
            Сколько стоят ваши услуги?
          </div>
          <span class="text-xs uppercase tracking-wider text-gray-400 block text-right" data-i18n="faq-designer">Дизайнер</span>
          <div class="bg-white text-black p-5 rounded-2xl rounded-tr-none text-sm md:text-base max-w-xl ml-auto" data-i18n="a5">
            Стоимость зависит от объёма, сложности задач и формата сотрудничества. Напишите мне, чтобы получить индивидуальный расчёт.
          </div>
        </div>

      </div>

    </div>
  </section>


  <!-- ==================== FINAL CTA SECTION ==================== -->
  <section class="py-24 px-6 md:px-12 bg-white text-black text-center">
    <div class="max-w-4xl mx-auto space-y-8">
      <h2 class="text-3xl sm:text-5xl lg:text-6xl font-extrabold uppercase leading-tight font-heading" data-i18n="cta-title">
        НУЖЕН ДОПОЛНИТЕЛЬНЫЙ<br>ДИЗАЙНЕР В КОМАНДУ?
      </h2>
      <p class="text-gray-600 max-w-xl mx-auto text-base sm:text-lg" data-i18n="cta-desc">
        Давайте обсудим ваши проекты, цели и то, как я могу облегчить работу вашей команды.
      </p>
      <div>
        <a href="https://t.me/KOTEGOVAAA" target="_blank" class="inline-flex items-center gap-2 bg-brand text-black font-extrabold px-8 py-4 rounded-full hover:bg-brand-hover transition text-sm shadow-md" data-i18n="cta-btn">
          ОБСУДИТЬ ПРОЕКТ &rarr;
        </a>
      </div>
      <p class="text-gray-500 text-xs sm:text-sm pt-4" data-i18n="cta-note">
        Никаких обязательств.<br>Просто разговор о возможном сотрудничестве.
      </p>
    </div>
  </section>


  <!-- ==================== FOOTER ==================== -->
  <footer id="footer" class="bg-white text-black border-t border-gray-200 pt-16 pb-12 px-6 md:px-12">
    <div class="max-w-7xl mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-12 gap-12 pb-16 border-b border-gray-200">
        
        <!-- Левая колонка -->
        <div class="md:col-span-5 space-y-6">
          <h3 class="text-2xl font-extrabold uppercase font-heading">KOTEGOVA</h3>
          <p class="text-gray-600 text-sm max-w-sm leading-relaxed" data-i18n="footer-desc">
            Независимый графический и веб-дизайнер.<br>Открыта к новым проектам и долгосрочному сотрудничеству.
          </p>
          <a href="https://t.me/KOTEGOVAAA" target="_blank" class="inline-flex items-center gap-2 bg-brand text-black font-extrabold px-6 py-3 rounded-full text-xs hover:bg-brand-hover transition" data-i18n="footer-btn">
            ОБСУДИТЬ ПРОЕКТ &rarr;
          </a>
        </div>

        <!-- Средняя колонка -->
        <div class="md:col-span-3 space-y-3 font-heading font-bold text-sm tracking-wide">
          <div><a href="#services" class="hover:text-brand-hover transition" data-i18n="nav-services">УСЛУГИ</a></div>
          <div><a href="#portfolio" class="hover:text-brand-hover transition" data-i18n="nav-portfolio">ПОРТФОЛИО</a></div>
          <div><a href="#about" class="hover:text-brand-hover transition" data-i18n="nav-about">ОБО МНЕ</a></div>
          <div><a href="#footer" class="hover:text-brand-hover transition" data-i18n="nav-contacts">КОНТАКТЫ</a></div>
        </div>

        <!-- Правая колонка контактов -->
        <div class="md:col-span-4 space-y-4 text-xs sm:text-sm">
          <div>
            <span class="text-gray-400 uppercase tracking-wider block text-[10px] mb-1">EMAIL:</span>
            <a href="mailto:KOTEGOVA2005@MAIL.RU" class="font-bold font-heading hover:underline">KOTEGOVA2005@MAIL.RU</a>
          </div>
          <div>
            <span class="text-gray-400 uppercase tracking-wider block text-[10px] mb-1">TELEGRAM:</span>
            <a href="https://t.me/KOTEGOVAAA" target="_blank" class="font-bold font-heading hover:underline">@KOTEGOVAAA</a>
          </div>
          <div>
            <span class="text-gray-400 uppercase tracking-wider block text-[10px] mb-1">BEHANCE:</span>
            <a href="https://www.behance.net/749cae0e" target="_blank" class="font-bold font-heading hover:underline">ANNA KOTEGOVA</a>
          </div>
          <div>
            <span class="text-gray-400 uppercase tracking-wider block text-[10px] mb-1">INSTAGRAM:</span>
            <a href="#" class="font-bold font-heading hover:underline">ANNA KOTEGOVA | DESIGNER</a>
          </div>
        </div>

      </div>

      <!-- Нижняя плашка -->
      <div class="flex flex-col sm:flex-row justify-between items-center pt-8 text-xs text-gray-500 gap-4">
        <div>© 2026 Анна Котегова.</div>
        <div data-i18n="footer-rights">Все права защищены</div>
      </div>
    </div>
  </footer>


  <!-- ==================== DUAL LANGUAGE SCRIPT ==================== -->
  <script>
    const dictionary = {
      ru: {
        "nav-services": "УСЛУГИ",
        "nav-about": "ОБО МНЕ",
        "nav-portfolio": "ПОРТФОЛИО",
        "nav-contacts": "КОНТАКТЫ",
        "btn-discuss": "ОБСУДИТЬ ПРОЕКТ →",

        "hero-tag": "НЕЗАВИСИМЫЙ ДИЗАЙНЕР — 6 ЛЕТ ОПЫТА",
        "hero-title": "ВАШЕЙ КОМАНДЕ НУЖЕН ДИЗАЙНЕР<br><span class=\"text-brand\">Я МОГУ ПОМОЧЬ</span>",
        "hero-sub": "Графический и веб-дизайн для бизнеса и творческих команд. От повседневных дизайн-задач до крупных проектов — когда вашей команде нужна дополнительная помощь.",
        "hero-btn-cta": "ОБСУДИТЬ ПРОЕКТ →",
        "hero-btn-portfolio": "ПОСМОТРЕТЬ РАБОТЫ",
        "ticker": "6 ЛЕТ В ДИЗАЙНЕ • ГРАФИЧЕСКИЙ ДИЗАЙН • ГИБКОЕ СОТРУДНИЧЕСТВО • ВЕБ-ДИЗАЙН • 6 ЛЕТ В ДИЗАЙНЕ • ГРАФИЧЕСКИЙ ДИЗАЙН • ГИБКОЕ СОТРУДНИЧЕСТВО • ВЕБ-ДИЗАЙН •",

        "services-title": "ЧЕМ Я МОГУ ПОМОЧЬ<br>ВАШЕЙ КОМАНДЕ?",
        "services-desc": "Один дизайнер — несколько направлений работы. Помогаю бизнесу поддерживать единый визуальный стиль и двигать проекты вперёд.",
        "s1-title": "ГРАФИЧЕСКИЙ ДИЗАЙН",
        "s1-desc": "Визуальная коммуникация вашего бренда.",
        "s1-t1": "Рекламные материалы",
        "s1-t2": "Афиши и баннеры",
        "s1-t3": "Презентации",
        "s1-t4": "Графика для соцсетей",
        "s1-t5": "Полиграфия и вёрстка",
        "s2-title": "ВЕБ-ДИЗАЙН",
        "s2-desc": "Цифровые решения для вашего бизнеса.",
        "s2-t1": "Лендинги",
        "s2-t2": "Дизайн сайтов",
        "s2-t3": "UI-дизайн",
        "s2-t4": "Редизайн сайтов",
        "s2-t5": "Цифровые макеты",
        "s3-title": "ПОСТОЯННАЯ ПОДДЕРЖКА",
        "s3-desc": "Дополнительные творческие ресурсы, когда они нужны.",
        "s3-t1": "Регулярные задачи",
        "s3-t2": "Материалы для спецпроектов",
        "s3-t3": "Помощь при высокой загрузке",
        "s3-t4": "Работа с командами",
        "s3-t5": "Долгосрочное партнерство",

        "how-title": "ДОПОЛНИТЕЛЬНЫЙ ДИЗАЙНЕР<br>БЕЗ НЕОБХОДИМОСТИ НАНИМАТЬ СОТРУДНИКА",
        "h1-step": "Шаг 01",
        "h1-title": "РАССКАЖИТЕ О ЗАДАЧАХ",
        "h1-desc": "Познакомимся с вашим бизнесом, текущими проектами и потребностями в дизайне.",
        "h2-step": "Шаг 02",
        "h2-title": "ПОДБЕРЁМ ФОРМАТ РАБОТЫ",
        "h2-desc": "Определим объём задач, приоритеты, сроки и удобный способ коммуникации.",
        "h3-step": "Шаг 03",
        "h3-title": "Я ПОДКЛЮЧАЮСЬ К ПРОЦЕССУ",
        "h3-desc": "Беру на себя дизайн-задачи, взаимодействую с вашей командой и передаю готовые материалы.",
        "h4-step": "Шаг 04",
        "h4-title": "ПРОДОЛЖАЕМ СОТРУДНИЧЕСТВО",
        "h4-desc": "Работаем на постоянной основе или подключаемся друг к другу по мере необходимости.",

        "about-subtitle": "Немного о человеке за всеми этими пикселями",
        "about-title": "МЕНЯ ЗОВУТ<br><span class=\"text-brand\">КОТЕГОВА АННА</span>",
        "about-desc": "Работаю с визуальной идентичностью, цифровым дизайном и коммуникационными материалами, помогая бизнесу превращать идеи в понятные и продуманные визуальные решения.",
        "about-s1": "В дизайне",
        "about-s2": "Оформленных мероприятий",
        "about-s3": "Личных проектов",
        "about-goal-label": "МОЯ ЦЕЛЬ ПРОСТА:",
        "about-goal-text": "Стать надёжным дизайн-партнёром, на которого можно рассчитывать.",

        "portfolio-title": "ИЗБРАННЫЕ ПРОЕКТЫ",
        "portfolio-desc": "Подборка проектов в области визуальной идентичности, цифрового и графического дизайна.",
        "portfolio-btn": "ПОСМОТРЕТЬ РАБОТЫ",
        "p1-title": "БРЕНДИНГ И АЙДЕНТИКА",
        "p2-title": "ГРАФИЧЕСКИЙ ДИЗАЙН И ПОЛИГРАФИЯ",
        "p3-title": "ЦИФРОВОЙ ДИЗАЙН И ВЕБ-ДИЗАЙН",

        "coop-title": "ФОРМАТЫ<br>СОТРУДНИЧЕСТВА",
        "coop-sub": "Давайте найдём подходящий формат сотрудничества.",
        "coop-desc": "Любое сотрудничество начинается с разговора. Помогу подобрать формат, который подойдёт вашей команде и бюджету.",
        "v1-opt": "Вариант 01",
        "v1-title": "ПОСТОЯННОЕ СОТРУДНИЧЕСТВО",
        "v1-desc": "Регулярная дизайн-поддержка для бизнеса, которому нужен надёжный творческий партнёр.",
        "v2-opt": "Вариант 02",
        "v2-title": "ПРОЕКТНАЯ РАБОТА",
        "v2-desc": "Определённый объём задач с согласованными сроками и результатами.",
        "v3-opt": "Вариант 03",
        "v3-title": "ПОДКЛЮЧЕНИЕ ПО ЗАПРОСУ",
        "v3-desc": "Дополнительные ресурсы для дизайна, когда команда перегружена или сроки поджимают.",

        "faq-title": "ЧАСТЫЕ<br>ВОПРОСЫ",
        "faq-client": "Клиент",
        "faq-designer": "Дизайнер",
        "q1": "Вы работаете с компаниями на постоянной основе?",
        "a1": "Да! Мне особенно интересен формат долгосрочного сотрудничества и роль внешнего дизайн-специалиста для бизнеса и творческих команд.",
        "q2": "Можете ли вы работать с нашей внутренней командой?",
        "a2": "Конечно. Могу взаимодействовать с маркетологами, арт-директорами, разработчиками и другими дизайнерами.",
        "q3": "Вы берёте только большие проекты?",
        "a3": "Нет. Я могу выполнять как отдельные задачи, так и работать над крупными проектами.",
        "q4": "Как начать сотрудничество?",
        "a4": "Просто свяжитесь со мной, расскажите о компании и о том, какая помощь с дизайном вам нужна. Обсудим детали и дальнейшие шаги.",
        "q5": "Сколько стоят ваши услуги?",
        "a5": "Стоимость зависит от объёма, сложности задач и формата сотрудничества. Напишите мне, чтобы получить индивидуальный расчёт.",

        "cta-title": "НУЖЕН ДОПОЛНИТЕЛЬНЫЙ<br>ДИЗАЙНЕР В КОМАНДУ?",
        "cta-desc": "Давайте обсудим ваши проекты, цели и то, как я могу облегчить работу вашей команды.",
        "cta-btn": "ОБСУДИТЬ ПРОЕКТ →",
        "cta-note": "Никаких обязательств.<br>Просто разговор о возможном сотрудничестве.",

        "footer-desc": "Независимый графический и веб-дизайнер.<br>Открыта к новым проектам и долгосрочному сотрудничеству.",
        "footer-btn": "ОБСУДИТЬ ПРОЕКТ →",
        "footer-rights": "Все права защищены"
      },
      en: {
        "nav-services": "SERVICES",
        "nav-about": "ABOUT ME",
        "nav-portfolio": "PORTFOLIO",
        "nav-contacts": "CONTACTS",
        "btn-discuss": "DISCUSS PROJECT →",

        "hero-tag": "INDEPENDENT DESIGNER — 6 YEARS OF EXPERIENCE",
        "hero-title": "YOUR TEAM NEEDS A DESIGNER<br><span class=\"text-brand\">I CAN HELP</span>",
        "hero-sub": "Graphic and web design for business and creative teams. From daily tasks to large-scale projects — when your team needs extra support.",
        "hero-btn-cta": "DISCUSS PROJECT →",
        "hero-btn-portfolio": "VIEW WORKS",
        "ticker": "6 YEARS IN DESIGN • GRAPHIC DESIGN • FLEXIBLE COOPERATION • WEB DESIGN • 6 YEARS IN DESIGN • GRAPHIC DESIGN • FLEXIBLE COOPERATION • WEB DESIGN •",

        "services-title": "HOW I CAN HELP<br>YOUR TEAM?",
        "services-desc": "One designer — multiple directions. Helping businesses maintain a consistent visual identity and drive projects forward.",
        "s1-title": "GRAPHIC DESIGN",
        "s1-desc": "Visual communication for your brand.",
        "s1-t1": "Marketing materials",
        "s1-t2": "Posters & banners",
        "s1-t3": "Presentations",
        "s1-t4": "Social media graphics",
        "s1-t5": "Print & prepress",
        "s2-title": "WEB DESIGN",
        "s2-desc": "Digital solutions for your business.",
        "s2-t1": "Landing pages",
        "s2-t2": "Website design",
        "s2-t3": "UI Design",
        "s2-t4": "Website redesign",
        "s2-t5": "Digital mockups",
        "s3-title": "ONGOING SUPPORT",
        "s3-desc": "Additional creative power whenever required.",
        "s3-t1": "Regular design tasks",
        "s3-t2": "Special campaign assets",
        "s3-t3": "High-workload support",
        "s3-t4": "Team collaboration",
        "s3-t5": "Long-term partnership",

        "how-title": "AN EXTRA DESIGNER<br>WITHOUT HIRING A FULL-TIME EMPLOYEE",
        "h1-step": "Step 01",
        "h1-title": "TELL ME ABOUT YOUR TASKS",
        "h1-desc": "Let's get acquainted with your business, ongoing projects, and design requirements.",
        "h2-step": "Step 02",
        "h2-title": "CHOOSE WORK FORMAT",
        "h2-desc": "We will define the scope, priorities, deadlines, and preferred communication channels.",
        "h3-step": "Step 03",
        "h3-title": "I JOIN YOUR WORKFLOW",
        "h3-desc": "I handle the design tasks, collaborate smoothly with your team, and deliver final assets.",
        "h4-step": "Step 04",
        "h4-title": "CONTINUOUS COLLABORATION",
        "h4-desc": "We work on an ongoing retainer or step in on-demand as needed.",

        "about-subtitle": "A little about the person behind all these pixels",
        "about-title": "MY NAME IS<br><span class=\"text-brand\">ANNA KOTEGOVA</span>",
        "about-desc": "I focus on visual identity, digital design, and promotional media, helping businesses transform ideas into clean, thoughtful visual solutions.",
        "about-s1": "Years in Design",
        "about-s2": "Events Designed",
        "about-s3": "Personal Projects",
        "about-goal-label": "MY GOAL IS SIMPLE:",
        "about-goal-text": "To become a reliable design partner you can fully count on.",

        "portfolio-title": "SELECTED WORKS",
        "portfolio-desc": "A curated collection of projects in visual identity, digital design, and branding.",
        "portfolio-btn": "VIEW WORKS",
        "p1-title": "BRANDING & IDENTITY",
        "p2-title": "GRAPHIC DESIGN & PRINT",
        "p3-title": "DIGITAL & WEB DESIGN",

        "coop-title": "COOPERATION<br>FORMATS",
        "coop-sub": "Let's find the best format for your needs.",
        "coop-desc": "Every collaboration starts with a conversation. I'll help select a setup tailored to your budget and team.",
        "v1-opt": "Option 01",
        "v1-title": "ONGOING PARTNERSHIP",
        "v1-desc": "Regular design support for businesses seeking a dependable creative partner.",
        "v2-opt": "Option 02",
        "v2-title": "PROJECT-BASED WORK",
        "v2-desc": "A defined scope of deliverables with agreed deadlines and targets.",
        "v3-opt": "Option 03",
        "v3-title": "ON-DEMAND SUPPORT",
        "v3-desc": "Extra creative support when your in-house team is overloaded or under tight deadlines.",

        "faq-title": "FREQUENTLY ASKED<br>QUESTIONS",
        "faq-client": "Client",
        "faq-designer": "Designer",
        "q1": "Do you work with companies on an ongoing retainer?",
        "a1": "Yes! I particularly focus on long-term partnerships as an external design specialist for businesses and creative teams.",
        "q2": "Can you collaborate with our in-house team?",
        "a2": "Absolutely. I regularly collaborate with marketers, art directors, developers, and other designers.",
        "q3": "Do you only accept large projects?",
        "a3": "No. I take on both individual single-task requests and complex, end-to-end projects.",
        "q4": "How do we start working together?",
        "a4": "Simply reach out, share a brief about your company and design needs. We'll discuss details and next steps.",
        "q5": "How much do your services cost?",
        "a5": "Pricing depends on project scope, complexity, and cooperation model. Message me for a custom quote.",

        "cta-title": "NEED AN ADDITIONAL<br>DESIGNER ON YOUR TEAM?",
        "cta-desc": "Let's discuss your projects, goals, and how I can help streamline your team's workload.",
        "cta-btn": "DISCUSS PROJECT →",
        "cta-note": "No obligations.<br>Just a conversation about potential collaboration.",

        "footer-desc": "Independent graphic and web designer.<br>Open for new projects and long-term partnerships.",
        "footer-btn": "DISCUSS PROJECT →",
        "footer-rights": "All rights reserved"
      }
    };

    function setLanguage(lang) {
      const ruBtn = document.getElementById('lang-ru');
      const enBtn = document.getElementById('lang-en');

      if (lang === 'ru') {
        ruBtn.className = "px-2.5 py-1 rounded bg-black text-white transition";
        enBtn.className = "px-2.5 py-1 rounded text-black hover:opacity-70 transition";
      } else {
        enBtn.className = "px-2.5 py-1 rounded bg-black text-white transition";
        ruBtn.className = "px-2.5 py-1 rounded text-black hover:opacity-70 transition";
      }

      document.querySelectorAll('[data-i18n]').forEach(element => {
        const key = element.getAttribute('data-i18n');
        if (dictionary[lang][key]) {
          element.innerHTML = dictionary[lang][key];
        }
      });
    }
  </script>
</body>
</html>
