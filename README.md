<!DOCTYPE html>
<html lang="ru" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CORSO MOTORS — Аренда автомобилей в Астане</title>
    <meta name="description" content="Аренда автомобилей в Астане от CORSO MOTORS. Toyota, Lexus, Hyundai, Kia, BYD, Lixiang и другие автомобили. Посуточная и длительная аренда. Онлайн-бронирование.">
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        darkBg: '#0a0a0a',
                        cardBg: '#121212',
                        cardHover: '#1a1a1a',
                        emeraldAccent: '#0F8F6B',
                        emeraldHover: '#0d7a5c',
                        borderDark: '#262626',
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            background-color: #0a0a0a;
            color: #f5f5f5;
            font-family: 'Inter', sans-serif;
        }
        .glass-card {
            background: rgba(18, 18, 18, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glass-card:hover {
            border-color: rgba(15, 143, 107, 0.4);
        }
    </style>
</head>
<body class="bg-darkBg text-white antialiased selection:bg-emeraldAccent selection:text-white">

    <!-- Header / Navbar -->
    <header class="fixed top-0 left-0 right-0 z-50 glass-card border-b border-borderDark transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <a href="#" class="flex flex-col">
                <span class="text-xl sm:text-2xl font-bold tracking-wider text-white">CORSO <span class="text-emeraldAccent">MOTORS</span></span>
                <span class="text-[9px] text-gray-400 tracking-widest uppercase">Автомобили премиум-класса в аренду</span>
            </a>
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-gray-300">
                <a href="#fleet" class="hover:text-emeraldAccent transition-colors">Автопарк</a>
                <a href="#advantages" class="hover:text-emeraldAccent transition-colors">Преимущества</a>
                <a href="#longterm" class="hover:text-emeraldAccent transition-colors">Долгосрочная аренда</a>
                <a href="#howitworks" class="hover:text-emeraldAccent transition-colors">Как это работает</a>
                <a href="#contacts" class="hover:text-emeraldAccent transition-colors">Контакты</a>
            </nav>
            <div class="hidden lg:flex items-center space-x-4">
                <a href="tel:+77752326443" class="text-sm font-semibold text-gray-200 hover:text-emeraldAccent transition-colors">+7 775 232 64 43</a>
                <button onclick="openBookingModal('Общая заявка')" class="bg-emeraldAccent hover:bg-emeraldHover text-white px-5 py-2.5 rounded-none text-sm font-medium transition-all shadow-lg shadow-emeraldAccent/20">
                    Забронировать
                </button>
            </div>
            <!-- Mobile Menu Button -->
            <button id="menu-btn" class="md:hidden text-gray-300 hover:text-white focus:outline-none">
                <i class="fa-solid fa-bars text-2xl"></i>
            </button>
        </div>
        <!-- Mobile Dropdown -->
        <div id="mobile-menu" class="hidden md:hidden glass-card border-t border-borderDark px-4 pt-4 pb-6 space-y-3">
            <a href="#fleet" class="block text-gray-300 hover:text-emeraldAccent py-1">Автопарк</a>
            <a href="#advantages" class="block text-gray-300 hover:text-emeraldAccent py-1">Преимущества</a>
            <a href="#longterm" class="block text-gray-300 hover:text-emeraldAccent py-1">Долгосрочная аренда</a>
            <a href="#howitworks" class="block text-gray-300 hover:text-emeraldAccent py-1">Как это работает</a>
            <a href="#contacts" class="block text-gray-300 hover:text-emeraldAccent py-1">Контакты</a>
            <div class="pt-2 flex flex-col space-y-2">
                <a href="tel:+77752326443" class="text-sm text-emeraldAccent font-semibold">+7 775 232 64 43</a>
                <button onclick="openBookingModal('Общая заявка')" class="w-full bg-emeraldAccent text-white py-2.5 text-sm font-medium">Забронировать</button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center pt-20 pb-16 overflow-hidden">
        <!-- Background Image with Overlay -->
        <div class="absolute inset-0 z-0">
            <img src="image_ba8a37.jpg" alt="Astana Night" class="w-full h-full object-cover object-center filter brightness-[0.35]">
            <div class="absolute inset-0 bg-gradient-to-t from-darkBg via-darkBg/60 to-transparent"></div>
        </div>
        <div class="relative z-10 max-w-5xl mx-auto px-4 text-center mt-10">
            <div class="inline-block mb-4 px-3 py-1 border border-emeraldAccent/40 bg-emeraldAccent/10 text-emeraldAccent text-xs uppercase tracking-widest font-semibold">
                Luxury Car Rental Astana
            </div>
            <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight text-white uppercase mb-6 leading-tight">
                CORSO MOTORS <br>
                <span class="text-transparent bg-clip-text bg-gradient-to-r from-gray-100 to-gray-400 text-3xl sm:text-5xl font-bold">Прокат автомобилей в Астане</span>
            </h1>
            <p class="text-lg sm:text-xl text-gray-300 max-w-2xl mx-auto font-light mb-10">
                Выберите автомобиль под любую задачу — от комфортной поездки по городу до автомобиля премиум-класса.
            </p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <button onclick="openBookingModal('Быстрый выбор')" class="w-full sm:w-auto bg-emeraldAccent hover:bg-emeraldHover text-white px-8 py-4 font-semibold text-sm tracking-wider uppercase transition-all shadow-xl shadow-emeraldAccent/25">
                    Забронировать авто
                </button>
                <a href="#fleet" class="w-full sm:w-auto glass-card hover:bg-white/10 text-white px-8 py-4 font-semibold text-sm tracking-wider uppercase transition-all border border-white/20">
                    Посмотреть автомобили
                </a>
            </div>
        </div>
    </section>

    <!-- Fleet Section -->
    <section id="fleet" class="py-24 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12">
            <h2 class="text-3xl sm:text-4xl font-bold tracking-tight uppercase mb-4">Наш автопарк</h2>
            <p class="text-gray-400 max-w-xl mx-auto text-sm">Премиальные, чистые и полностью подготовленные автомобили для вашего комфорта в Астане.</p>
        </div>

        <!-- Filters & Sorting Bar -->
        <div class="flex flex-col lg:flex-row items-center justify-between gap-4 mb-12 border-b border-borderDark pb-6">
            <!-- Filters -->
            <div id="filter-buttons" class="flex flex-wrap items-center justify-center lg:justify-start gap-2">
                <button onclick="filterCars('all')" data-filter="all" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-emeraldAccent text-white transition-all">Все автомобили</button>
                <button onclick="filterCars('economy')" data-filter="economy" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all">Эконом</button>
                <button onclick="filterCars('comfort')" data-filter="comfort" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all">Комфорт</button>
                <button onclick="filterCars('business')" data-filter="business" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all">Бизнес</button>
                <button onclick="filterCars('premium')" data-filter="premium" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all">Премиум</button>
                <button onclick="filterCars('suv')" data-filter="suv" class="filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all">SUV</button>
            </div>
            <!-- Sorting -->
            <div class="flex items-center space-x-2 w-full lg:w-auto justify-end">
                <span class="text-xs text-gray-400 uppercase tracking-wider">Сортировка:</span>
                <select id="sort-select" onchange="sortCars()" class="bg-cardBg border border-borderDark text-xs text-gray-300 px-3 py-2 focus:outline-none focus:border-emeraldAccent">
                    <option value="default">Популярные</option>
                    <option value="price-asc">По возрастанию цены</option>
                    <option value="price-desc">По убыванию цены</option>
                </select>
            </div>
        </div>

        <!-- Car Grid -->
        <div id="car-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Car cards will be dynamically inserted via JS to maintain exact ordering and pricing -->
        </div>
    </section>

    <!-- Why Choose Us -->
    <section id="advantages" class="py-24 bg-[#0d0d0d] border-y border-borderDark">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold tracking-tight uppercase mb-4">Почему CORSO MOTORS</h2>
                <p class="text-gray-400 text-sm">Высокие стандарты обслуживания для каждого клиента</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Advantage 1 -->
                <div class="glass-card p-8 relative group">
                    <div class="text-4xl font-extrabold text-emeraldAccent mb-4 opacity-80">01</div>
                    <h3 class="text-lg font-bold uppercase mb-2">Широкий выбор автомобилей</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Автомобили разных классов — от городских моделей до премиальных SUV.</p>
                </div>
                <!-- Advantage 2 -->
                <div class="glass-card p-8 relative group">
                    <div class="text-4xl font-extrabold text-emeraldAccent mb-4 opacity-80">02</div>
                    <h3 class="text-lg font-bold uppercase mb-2">Удобное бронирование</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Забронируйте автомобиль онлайн за несколько минут.</p>
                </div>
                <!-- Advantage 3 -->
                <div class="glass-card p-8 relative group">
                    <div class="text-4xl font-extrabold text-emeraldAccent mb-4 opacity-80">03</div>
                    <h3 class="text-lg font-bold uppercase mb-2">Чистые и подготовленные авто</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Перед каждой арендой автомобиль проходит проверку и подготовку.</p>
                </div>
                <!-- Advantage 4 -->
                <div class="glass-card p-8 relative group">
                    <div class="text-4xl font-extrabold text-emeraldAccent mb-4 opacity-80">04</div>
                    <h3 class="text-lg font-bold uppercase mb-2">Индивидуальный подход</h3>
                    <p class="text-gray-400 text-sm leading-relaxed">Подберём автомобиль под ваши задачи и сроки аренды.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Long-term Rental Section -->
    <section id="longterm" class="py-24 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="glass-card p-8 sm:p-14 relative overflow-hidden border border-emeraldAccent/30">
            <div class="absolute -right-10 -bottom-10 w-64 h-64 bg-emeraldAccent/10 rounded-full blur-3xl pointer-events-none"></div>
            <div class="max-w-2xl relative z-10">
                <span class="text-emeraldAccent text-xs uppercase font-semibold tracking-widest block mb-3">Специальные условия</span>
                <h2 class="text-3xl sm:text-4xl font-extrabold uppercase mb-4 leading-tight">Нужен автомобиль на неделю или месяц?</h2>
                <p class="text-gray-300 text-sm sm:text-base leading-relaxed mb-8">
                    Для длительной аренды действуют индивидуальные условия. Свяжитесь с нами — рассчитаем стоимость под ваш срок.
                </p>
                <button onclick="openBookingModal('Долгосрочная аренда')" class="bg-emeraldAccent hover:bg-emeraldHover text-white px-8 py-4 font-semibold text-sm uppercase tracking-wider transition-all shadow-lg shadow-emeraldAccent/20">
                    Получить расчёт
                </button>
            </div>
        </div>
    </section>

    <!-- How It Works -->
    <section id="howitworks" class="py-24 bg-[#0d0d0d] border-t border-borderDark">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl sm:text-4xl font-bold tracking-tight uppercase mb-4">Как это работает</h2>
                <p class="text-gray-400 text-sm">Простой путь к вашей поездке за 4 шага</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="glass-card p-8 text-center">
                    <span class="text-5xl font-black text-emeraldAccent block mb-4">01</span>
                    <h3 class="text-sm font-bold uppercase tracking-wider mb-2">Выберите автомобиль</h3>
                    <p class="text-gray-400 text-xs">Подберите модель под ваши задачи в нашем каталоге.</p>
                </div>
                <div class="glass-card p-8 text-center">
                    <span class="text-5xl font-black text-emeraldAccent block mb-4">02</span>
                    <h3 class="text-sm font-bold uppercase tracking-wider mb-2">Оставьте заявку</h3>
                    <p class="text-gray-400 text-xs">Заполните простую форму бронирования на сайте.</p>
                </div>
                <div class="glass-card p-8 text-center">
                    <span class="text-5xl font-black text-emeraldAccent block mb-4">03</span>
                    <h3 class="text-sm font-bold uppercase tracking-wider mb-2">Подтверждение</h3>
                    <p class="text-gray-400 text-xs">Менеджер свяжется с вами для подтверждения брони.</p>
                </div>
                <div class="glass-card p-8 text-center">
                    <span class="text-5xl font-black text-emeraldAccent block mb-4">04</span>
                    <h3 class="text-sm font-bold uppercase tracking-wider mb-2">Получите авто</h3>
                    <p class="text-gray-400 text-xs">Заберите чистый и готовый к поездке автомобиль.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Before Footer -->
    <section class="py-20 relative overflow-hidden border-t border-borderDark">
        <div class="max-w-4xl mx-auto px-4 text-center">
            <h2 class="text-3xl sm:text-5xl font-extrabold uppercase mb-6">Ваш идеальный автомобиль уже ждёт.</h2>
            <p class="text-gray-400 text-sm sm:text-base mb-8">Выберите автомобиль и забронируйте его прямо сейчас.</p>
            <a href="#fleet" class="inline-block bg-emeraldAccent hover:bg-emeraldHover text-white px-8 py-4 font-semibold text-sm uppercase tracking-wider transition-all shadow-lg shadow-emeraldAccent/20">
                Посмотреть автопарк
            </a>
        </div>
    </section>

    <!-- Contacts Section -->
    <section id="contacts" class="py-24 bg-[#0d0d0d] border-t border-borderDark">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <div>
                    <h2 class="text-3xl font-bold uppercase mb-4">Контакты</h2>
                    <p class="text-gray-400 text-sm mb-8">Свяжитесь с нами удобным для вас способом. Мы на связи 24/7.</p>
                    
                    <div class="space-y-6 text-sm">
                        <div class="flex items-start space-x-4">
                            <div class="w-10 h-10 glass-card flex items-center justify-center text-emeraldAccent shrink-0">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <span class="text-gray-400 block text-xs uppercase">Адрес</span>
                                <span class="text-white font-medium">Астана, Казахстан</span>
                            </div>
                        </div>
                        <div class="flex items-start space-x-4">
                            <div class="w-10 h-10 glass-card flex items-center justify-center text-emeraldAccent shrink-0">
                                <i class="fa-solid fa-phone"></i>
                            </div>
                            <div>
                                <span class="text-gray-400 block text-xs uppercase">Телефоны</span>
                                <a href="tel:+77752326443" class="text-white font-medium hover:text-emeraldAccent block">+7 775 232 64 43</a>
                                <a href="tel:+77007776626" class="text-white font-medium hover:text-emeraldAccent block">+7 700 777 66 26</a>
                            </div>
                        </div>
                        <div class="flex items-start space-x-4">
                            <div class="w-10 h-10 glass-card flex items-center justify-center text-emeraldAccent shrink-0">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <div>
                                <span class="text-gray-400 block text-xs uppercase">Email</span>
                                <a href="mailto:corsomotors2026@gmail.com" class="text-white font-medium hover:text-emeraldAccent">corsomotors2026@gmail.com</a>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="glass-card p-8 flex flex-col justify-center space-y-4">
                    <h3 class="text-xl font-bold uppercase mb-2">Быстрый контакт</h3>
                    <p class="text-gray-400 text-xs mb-4">Нажмите кнопку ниже, чтобы мгновенно связаться с менеджером в WhatsApp или по телефону.</p>
                    <a href="https://wa.me/77752326443?text=Здравствуйте!%20Хочу%20узнать%20об%20аренде%20автомобилей" target="_blank" class="w-full bg-emeraldAccent hover:bg-emeraldHover text-white py-3.5 font-semibold text-xs uppercase tracking-wider text-center transition-all flex items-center justify-center space-x-2">
                        <i class="fa-brands fa-whatsapp text-lg"></i>
                        <span>Написать в WhatsApp</span>
                    </a>
                    <a href="tel:+77752326443" class="w-full glass-card hover:bg-white/10 text-white py-3.5 font-semibold text-xs uppercase tracking-wider text-center transition-all border border-white/20 flex items-center justify-center space-x-2">
                        <i class="fa-solid fa-phone text-sm"></i>
                        <span>Позвонить</span>
                    </a>
                    <a href="mailto:corsomotors2026@gmail.com" class="w-full glass-card hover:bg-white/10 text-white py-3.5 font-semibold text-xs uppercase tracking-wider text-center transition-all border border-white/20 flex items-center justify-center space-x-2">
                        <i class="fa-solid fa-envelope text-sm"></i>
                        <span>Написать на Email</span>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 border-t border-borderDark text-xs text-gray-400">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between gap-6">
            <div>
                <span class="text-base font-bold text-white tracking-wider block mb-1">CORSO <span class="text-emeraldAccent">MOTORS</span></span>
                <p>Премиальная аренда автомобилей в Астане.</p>
            </div>
            <div class="flex flex-wrap justify-center gap-6 text-gray-300 font-medium">
                <a href="#fleet" class="hover:text-emeraldAccent transition-colors">Автомобили</a>
                <a href="#advantages" class="hover:text-emeraldAccent transition-colors">Условия аренды</a>
                <a href="#howitworks" class="hover:text-emeraldAccent transition-colors">Бронирование</a>
                <a href="#contacts" class="hover:text-emeraldAccent transition-colors">Контакты</a>
            </div>
            <div>
                <p class="text-right md:text-left">© 2026 CORSO MOTORS. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/77752326443?text=Здравствуйте!%20Хочу%20арендовать%20автомобиль" target="_blank" class="fixed bottom-6 right-6 z-40 bg-emeraldAccent hover:bg-emeraldHover text-white w-14 h-14 rounded-full flex items-center justify-center shadow-2xl transition-all transform hover:scale-110">
        <i class="fa-brands fa-whatsapp text-2xl"></i>
    </a>

    <!-- Mobile Fixed Bottom Panel -->
    <div class="fixed bottom-0 left-0 right-0 z-40 md:hidden glass-card border-t border-borderDark p-3 flex gap-3 bg-darkBg/95">
        <a href="https://wa.me/77752326443?text=Здравствуйте!%20Хочу%20арендовать%20автомобиль" target="_blank" class="flex-1 bg-emeraldAccent text-white py-3 font-semibold text-xs uppercase tracking-wider text-center flex items-center justify-center space-x-2">
            <i class="fa-brands fa-whatsapp text-base"></i>
            <span>WhatsApp</span>
        </a>
        <button onclick="openBookingModal('Быстрая заявка с телефона')" class="flex-1 glass-card border border-emeraldAccent text-white py-3 font-semibold text-xs uppercase tracking-wider text-center bg-emeraldAccent/20">
            Забронировать
        </button>
    </div>

    <!-- Booking Modal -->
    <div id="booking-modal" class="fixed inset-0 z-50 hidden items-center justify-center px-4 bg-black/80 backdrop-blur-sm">
        <div class="glass-card max-w-lg w-full p-6 sm:p-8 relative border border-borderDark max-h-[90vh] overflow-y-auto">
            <button onclick="closeBookingModal()" class="absolute top-4 right-4 text-gray-400 hover:text-white text-xl">
                <i class="fa-solid fa-xmark"></i>
            </button>
            <h3 class="text-2xl font-bold uppercase mb-2">Бронирование автомобиля</h3>
            <p id="modal-car-title" class="text-emeraldAccent text-sm font-medium mb-6">Выбранный автомобиль</p>

            <form id="booking-form" onsubmit="submitBooking(event)" class="space-y-4 text-sm">
                <div>
                    <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Выбранный автомобиль</label>
                    <input type="text" id="form-car" readonly class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                </div>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Дата получения</label>
                        <input type="date" id="form-date-from" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                    </div>
                    <div>
                        <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Время получения</label>
                        <input type="time" id="form-time-from" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                    </div>
                </div>
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div>
                        <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Дата возврата</label>
                        <input type="date" id="form-date-to" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                    </div>
                    <div>
                        <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Время возврата</label>
                        <input type="time" id="form-time-to" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                    </div>
                </div>
                <div>
                    <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Имя</label>
                    <input type="text" id="form-name" placeholder="Ваше имя" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                </div>
                <div>
                    <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Номер телефона</label>
                    <input type="tel" id="form-phone" placeholder="+7 (___) ___-__-__" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                </div>
                <div>
                    <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">WhatsApp</label>
                    <input type="text" id="form-whatsapp" placeholder="+7 (___) ___-__-__" required class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent">
                </div>
                <div>
                    <label class="block text-xs uppercase tracking-wider text-gray-400 mb-1">Комментарий</label>
                    <textarea id="form-comment" rows="2" placeholder="Дополнительные пожелания" class="w-full bg-cardBg border border-borderDark px-4 py-3 text-white focus:outline-none focus:border-emeraldAccent"></textarea>
                </div>
                <button type="submit" class="w-full bg-emeraldAccent hover:bg-emeraldHover text-white py-4 font-semibold text-xs uppercase tracking-wider transition-all shadow-lg shadow-emeraldAccent/20">
                    Отправить заявку на бронирование
                </button>
            </form>

            <div id="success-message" class="hidden text-center py-8 space-y-4">
                <div class="w-16 h-16 bg-emeraldAccent/20 text-emeraldAccent rounded-full flex items-center justify-center mx-auto text-3xl">
                    <i class="fa-solid fa-check"></i>
                </div>
                <h4 class="text-xl font-bold uppercase">Заявка принята!</h4>
                <p class="text-gray-300 text-sm leading-relaxed">
                    Спасибо! Ваша заявка принята. Менеджер CORSO MOTORS свяжется с вами для подтверждения бронирования. Сейчас вы будете перенаправлены в WhatsApp.
                </p>
                <button onclick="closeBookingModal()" class="bg-emeraldAccent text-white px-6 py-2.5 text-xs font-semibold uppercase">Закрыть</button>
            </div>
        </div>
    </div>

    <!-- JavaScript Application Logic -->
    <script>
        // Car Data based strictly on user specifications and uploaded photos
        const cars = [
            { id: 1, name: "JAC JS4", category: "suv", price: 25000, image: "image_ba8a37.jpg" },
            { id: 2, name: "Toyota Camry", category: "business", price: 35000, image: "image_ba899e.png" },
            { id: 3, name: "Hyundai Elantra", category: "comfort", price: 25000, image: "image_ba8d25.png" },
            { id: 4, name: "Hyundai Sonata", category: "business", price: 32000, image: "image_ba8da3.jpg" },
            { id: 5, name: "Kia Rio", category: "economy", price: 20000, image: "image_ba90e4.png" },
            { id: 6, name: "BYD Destroyer 05", category: "comfort", price: 20000, image: "image_ba9140.png" },
            { id: 7, name: "Toyota Camry 55", category: "business", price: 25000, image: "image_ba919e.png" },
            { id: 8, name: "Toyota Camry 70 / 80", category: "business", price: 55000, image: "image_ba91dc.png" },
            { id: 9, name: "Lexus ES 250 / GS 350", category: "premium", price: 55000, image: "image_ba9544.png" },
            { id: 10, name: "Hyundai Tucson", category: "suv", price: 42000, image: "image_ba98a6.png" },
            { id: 11, name: "Kia Sportage", category: "suv", price: 42000, image: "image_ba8a37.jpg" },
            { id: 12, name: "Jetour X70", category: "suv", price: 30000, image: "image_ba8d25.png" },
            { id: 13, name: "Chery", category: "suv", price: 30000, image: "image_ba8a37.jpg" },
            { id: 14, name: "Toyota RAV4", category: "suv", price: 30000, image: "image_ba98a6.png" },
            { id: 15, name: "Toyota Highlander", category: "suv", price: 90000, image: "image_ba9544.png" },
            { id: 16, name: "Lixiang L7 / L9", category: "premium", price: 100000, image: "image_ba91dc.png" },
            { id: 17, name: "BYD", category: "economy", price: 24000, image: "image_ba9140.png" }
        ];

        let currentFilter = 'all';

        function renderCars(data) {
            const grid = document.getElementById('car-grid');
            grid.innerHTML = '';
            data.forEach(car => {
                const card = document.createElement('div');
                card.className = 'glass-card overflow-hidden flex flex-col justify-between group transition-all duration-300';
                card.innerHTML = `
                    <div class="relative h-56 overflow-hidden bg-black/40">
                        <img src="${car.image}" alt="${car.name}" class="w-full h-full object-cover object-center group-hover:scale-105 transition-transform duration-500">
                        <div class="absolute top-3 right-3 bg-darkBg/80 backdrop-blur-md px-3 py-1 border border-borderDark text-[10px] uppercase font-semibold text-emeraldAccent">
                            ${car.category.toUpperCase()}
                        </div>
                    </div>
                    <div class="p-6 flex flex-col flex-grow justify-between">
                        <div>
                            <h3 class="text-lg font-bold uppercase mb-2 text-white">${car.name}</h3>
                            <div class="text-xl font-extrabold text-emeraldAccent mb-6">
                                ${car.price.toLocaleString()} ₸ <span class="text-xs font-normal text-gray-400">/ сутки</span>
                            </div>
                        </div>
                        <button onclick="openBookingModal('${car.name}')" class="w-full bg-emeraldAccent/10 hover:bg-emeraldAccent text-emeraldAccent hover:text-white border border-emeraldAccent/40 py-3 font-semibold text-xs uppercase tracking-wider transition-all">
                            Забронировать
                        </button>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        function filterCars(category) {
            currentFilter = category;
            // Update button styles
            document.querySelectorAll('.filter-btn').forEach(btn => {
                if(btn.dataset.filter === category) {
                    btn.className = 'filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-emeraldAccent text-white transition-all';
                } else {
                    btn.className = 'filter-btn px-4 py-2 text-xs font-semibold uppercase tracking-wider bg-cardBg hover:bg-cardHover text-gray-300 border border-borderDark transition-all';
                }
            });

            let filtered = category === 'all' ? cars : cars.filter(c => c.category === category);
            applySorting(filtered);
        }

        function sortCars() {
            let filtered = currentFilter === 'all' ? [...cars] : cars.filter(c => c.category === currentFilter);
            applySorting(filtered);
        }

        function applySorting(data) {
            const sortVal = document.getElementById('sort-select').value;
            if(sortVal === 'price-asc') {
                data.sort((a, b) => a.price - b.price);
            } else if(sortVal === 'price-desc') {
                data.sort((a, b) => b.price - a.price);
            }
            renderCars(data);
        }

        // Mobile Menu Toggle
        document.getElementById('menu-btn').addEventListener('click', () => {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Modal Functions
        function openBookingModal(carName) {
            document.getElementById('form-car').value = carName;
            document.getElementById('modal-car-title').innerText = `Выбранный автомобиль: ${carName}`;
            document.getElementById('booking-form').reset();
            document.getElementById('form-car').value = carName;
            document.getElementById('booking-form').classList.remove('hidden');
            document.getElementById('success-message').classList.add('hidden');
            document.getElementById('booking-modal').classList.remove('hidden');
            document.getElementById('booking-modal').classList.add('flex');
        }

        function closeBookingModal() {
            document.getElementById('booking-modal').classList.remove('flex');
            document.getElementById('booking-modal').classList.add('hidden');
        }

        function submitBooking(e) {
            e.preventDefault();
            const car = document.getElementById('form-car').value;
            const dateFrom = document.getElementById('form-date-from').value;
            const dateTo = document.getElementById('form-date-to').value;
            const name = document.getElementById('form-name').value;
            const phone = document.getElementById('form-phone').value;

            // WhatsApp automatic message generation
            const whatsappMessage = encodeURIComponent(
                `Здравствуйте! Хочу забронировать автомобиль:\n` +
                `🚗 ${car}\n` +
                `📅 Дата получения: ${dateFrom}\n` +
                `📅 Дата возврата: ${dateTo}\n` +
                `👤 Имя: ${name}\n` +
                `📞 Телефон: ${phone}`
            );

            // Hide form and show success message
            document.getElementById('booking-form').classList.add('hidden');
            document.getElementById('success-message').classList.remove('hidden');

            // Redirect to WhatsApp after short delay
            setTimeout(() => {
                window.open(`https://wa.me/77752326443?text=${whatsappMessage}`, '_blank');
            }, 1500);
        }

        // Initial render
        renderCars(cars);
    </script>
</body>
</html><div class="car-catalog">
  <!-- 11. Kia Sportage -->
  <div class="car-item">
    <h3>11. Kia Sportage</h3>
    <img src="image_ba9d39.png" alt="Kia Sportage">
  </div>

  <!-- 12. Jetour X70 -->
  <div class="car-item">
    <h3>12. Jetour X70</h3>
    <img src="image_baa063.png" alt="Jetour X70">
  </div>

  <!-- 13. Chery Tiggo 7 Pro Max 2026 -->
  <div class="car-item">
    <h3>13. Chery Tiggo 7 Pro Max 2026</h3>
    <img src="image_baa3c7.png" alt="Chery Tiggo 7 Pro Max 2026">
  </div>

  <!-- 14. Toyota RAV4 2026 -->
  <div class="car-item">
    <h3>14. Toyota RAV4 2026</h3>
    <img src="image_baa47e.png" alt="Toyota RAV4 2026">
  </div>

  <!-- 15. Toyota Highlander -->
  <div class="car-item">
    <h3>15. Toyota Highlander</h3>
    <img src="image_baa78a.png" alt="Toyota Highlander">
  </div>

  <!-- 16. Lixiang L9 -->
  <div class="car-item">
    <h3>16. Lixiang L9</h3>
    <img src="image_baa81f.png" alt="Lixiang L9">
  </div>

  <!-- 17. BYD Tang L -->
  <div class="car-item">
    <h3>17. BYD Tang L</h3>
    <img src="image_baab4c.png" alt="BYD Tang L">
  </div>
</div>
