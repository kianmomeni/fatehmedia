<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رسانه هنری فاتح | Fateh Art Media</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Almarai:wght@300;400;700;800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Almarai', sans-serif;
            background-color: #000;
            color: #fff;
        }
        
        .blood-red {
            color: #8b0000;
        }
        
        .bg-blood-red {
            background-color: #8b0000;
        }
        
        .border-blood-red {
            border-color: #8b0000;
        }
        
        .hover\:bg-blood-red:hover {
            background-color: #8b0000;
        }
        
        .hero-section {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1490730141103-6cac27aaab94?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
        }
        
        .portfolio-item {
            transition: all 0.3s ease;
        }
        
        .portfolio-item:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(139, 0, 0, 0.5);
        }
        
        .form-input {
            background-color: #111;
            border: 1px solid #333;
            color: white;
        }
        
        .form-input:focus {
            outline: none;
            border-color: #8b0000;
            box-shadow: 0 0 0 2px rgba(139, 0, 0, 0.3);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -2px;
            right: 0;
            background-color: #8b0000;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .mobile-menu {
            transition: all 0.3s ease;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="bg-black border-b border-gray-800 fixed w-full z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center">
                        <span class="text-white text-2xl font-bold blood-red">فاتح</span>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-8 space-x-reverse">
                    <a href="#home" class="nav-link text-white hover:text-red-700 px-3 py-2 text-sm font-medium">صفحه اصلی</a>
                    <a href="#services" class="nav-link text-white hover:text-red-700 px-3 py-2 text-sm font-medium">خدمات</a>
                    <a href="#portfolio" class="nav-link text-white hover:text-red-700 px-3 py-2 text-sm font-medium">نمونه کارها</a>
                    <a href="#about" class="nav-link text-white hover:text-red-700 px-3 py-2 text-sm font-medium">درباره ما</a>
                    <a href="#contact" class="nav-link text-white hover:text-red-700 px-3 py-2 text-sm font-medium">تماس با ما</a>
                    <a href="#login" class="bg-blood-red text-white px-4 py-2 rounded-md text-sm font-medium hover:bg-red-900 transition duration-300">ورود / ثبت نام</a>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-button" class="text-white hover:text-red-700 focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="mobile-menu hidden md:hidden bg-black border-t border-gray-800">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="block px-3 py-2 text-base font-medium text-white hover:text-red-700">صفحه اصلی</a>
                <a href="#services" class="block px-3 py-2 text-base font-medium text-white hover:text-red-700">خدمات</a>
                <a href="#portfolio" class="block px-3 py-2 text-base font-medium text-white hover:text-red-700">نمونه کارها</a>
                <a href="#about" class="block px-3 py-2 text-base font-medium text-white hover:text-red-700">درباره ما</a>
                <a href="#contact" class="block px-3 py-2 text-base font-medium text-white hover:text-red-700">تماس با ما</a>
                <a href="#login" class="block bg-blood-red text-white px-4 py-2 rounded-md text-sm font-medium hover:bg-red-900 transition duration-300 text-center mx-4">ورود / ثبت نام</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section flex items-center justify-center text-center pt-16">
        <div class="max-w-4xl px-4">
            <h1 class="text-4xl md:text-6xl font-bold mb-6">رسانه هنری <span class="blood-red">فاتح</span></h1>
            <p class="text-lg md:text-xl mb-8">تخصص ما در خلق آثار هنری منحصر به فرد و تدوین حرفه‌ای است. هر پروژه داستان منحصر به فرد خود را دارد و ما اینجا هستیم تا آن را به زیباترین شکل روایت کنیم.</p>
            <div class="flex justify-center space-x-4 space-x-reverse">
                <a href="#portfolio" class="bg-blood-red text-white px-6 py-3 rounded-md text-lg font-medium hover:bg-red-900 transition duration-300">نمونه کارها</a>
                <a href="#contact" class="border border-blood-red text-white px-6 py-3 rounded-md text-lg font-medium hover:bg-red-900 hover:bg-opacity-10 transition duration-300">تماس با ما</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 px-4">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">خدمات <span class="blood-red">ما</span></h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="bg-gray-900 p-8 rounded-lg border border-gray-800 hover:border-blood-red transition duration-300">
                    <div class="text-blood-red text-4xl mb-4">
                        <i class="fas fa-film"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">تدوین حرفه‌ای</h3>
                    <p class="text-gray-300">تدوین ویدیو با کیفیت بالا، ویرایش حرفه‌ای، اضافه کردن افکت‌های ویژه و صداگذاری با بهترین کیفیت ممکن.</p>
                </div>
                
                <!-- Service 2 -->
                <div class="bg-gray-900 p-8 rounded-lg border border-gray-800 hover:border-blood-red transition duration-300">
                    <div class="text-blood-red text-4xl mb-4">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">فتح گراف</h3>
                    <p class="text-gray-300">طراحی پوستر، تراکت، بنر و سایر آثار گرافیکی با ایده‌های نو و خلاقانه برای رویدادهای مختلف.</p>
                </div>
                
                <!-- Service 3 -->
                <div class="bg-gray-900 p-8 rounded-lg border border-gray-800 hover:border-blood-red transition duration-300">
                    <div class="text-blood-red text-4xl mb-4">
                        <i class="fas fa-camera"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">عکاسی هنری</h3>
                    <p class="text-gray-300">عکاسی حرفه‌ای با دید هنری، ترکیب‌بندی خلاقانه و پردازش تصاویر با کیفیت بالا.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 px-4 bg-gray-900">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">نمونه <span class="blood-red">کارها</span></h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Portfolio Item 1 -->
                <div class="portfolio-item bg-black rounded-lg overflow-hidden border border-gray-800">
                    <img src="https://images.unsplash.com/photo-1485846234645-a62644f84728?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1459&q=80" alt="Video Editing" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">تدوین فیلم کوتاه</h3>
                        <p class="text-gray-400 mb-4">تدوین و ویرایش حرفه‌ای فیلم کوتاه با افکت‌های ویژه</p>
                        <a href="#" class="text-blood-red font-medium hover:underline">مشاهده پروژه</a>
                    </div>
                </div>
                
                <!-- Portfolio Item 2 -->
                <div class="portfolio-item bg-black rounded-lg overflow-hidden border border-gray-800">
                    <img src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Graphic Design" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">طراحی پوستر کنسرت</h3>
                        <p class="text-gray-400 mb-4">طراحی خلاقانه پوستر برای رویداد موسیقی</p>
                        <a href="#" class="text-blood-red font-medium hover:underline">مشاهده پروژه</a>
                    </div>
                </div>
                
                <!-- Portfolio Item 3 -->
                <div class="portfolio-item bg-black rounded-lg overflow-hidden border border-gray-800">
                    <img src="https://images.unsplash.com/photo-1516035069371-29a1b244cc32?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1528&q=80" alt="Photography" class="w-full h-64 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-2">عکاسی پرتره هنری</h3>
                        <p class="text-gray-400 mb-4">عکاسی پرتره با نورپردازی خلاقانه</p>
                        <a href="#" class="text-blood-red font-medium hover:underline">مشاهده پروژه</a>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-block bg-blood-red text-white px-6 py-3 rounded-md text-lg font-medium hover:bg-red-900 transition duration-300">مشاهده همه نمونه کارها</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-4">
        <div class="max-w-6xl mx-auto">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pl-12">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">درباره <span class="blood-red">رسانه هنری فاتح</span></h2>
                    <p class="text-gray-300 mb-4">رسانه هنری فاتح با سال‌ها تجربه در زمینه تولید محتوای هنری و رسانه‌ای، همواره در تلاش بوده تا با ارائه خدمات با کیفیت و خلاقانه، رضایت کامل مشتریان خود را جلب نماید.</p>
                    <p class="text-gray-300 mb-6">تیم ما متشکل از هنرمندان و متخصصان خلاق است که هر پروژه را با دقت و حساسیت خاصی انجام می‌دهند تا نتیجه نهایی کاملاً مطابق با انتظارات شما باشد.</p>
                    <div class="flex space-x-4 space-x-reverse">
                        <div class="text-center">
                            <div class="text-blood-red text-3xl font-bold mb-1">+500</div>
                            <div class="text-gray-400">پروژه انجام شده</div>
                        </div>
                        <div class="text-center">
                            <div class="text-blood-red text-3xl font-bold mb-1">+100</div>
                            <div class="text-gray-400">مشتری راضی</div>
                        </div>
                        <div class="text-center">
                            <div class="text-blood-red text-3xl font-bold mb-1">10+</div>
                            <div class="text-gray-400">سال تجربه</div>
                        </div>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="About Us" class="rounded-lg shadow-xl w-full">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-4 bg-gray-900">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">تماس <span class="blood-red">با ما</span></h2>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <h3 class="text-xl font-bold mb-4">اطلاعات تماس</h3>
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="text-blood-red text-xl mr-3 mt-1">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">آدرس</h4>
                                <p class="text-gray-400">تهران، خیابان آزادی، پلاک 123</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-blood-red text-xl mr-3 mt-1">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">تلفن</h4>
                                <p class="text-gray-400">021-12345678</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-blood-red text-xl mr-3 mt-1">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">ایمیل</h4>
                                <p class="text-gray-400">info@fatehartmedia.com</p>
                            </div>
                        </div>
                    </div>
                    
                    <h3 class="text-xl font-bold mt-8 mb-4">ما را دنبال کنید</h3>
                    <div class="flex space-x-4 space-x-reverse">
                        <a href="#" class="text-white hover:text-blood-red text-2xl">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-white hover:text-blood-red text-2xl">
                            <i class="fab fa-telegram"></i>
                        </a>
                        <a href="#" class="text-white hover:text-blood-red text-2xl">
                            <i class="fab fa-youtube"></i>
                        </a>
                        <a href="#" class="text-white hover:text-blood-red text-2xl">
                            <i class="fab fa-aparat"></i>
                        </a>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <form class="space-y-4">
                        <div>
                            <label for="name" class="block mb-1">نام و نام خانوادگی</label>
                            <input type="text" id="name" class="form-input w-full px-4 py-2 rounded-md">
                        </div>
                        <div>
                            <label for="email" class="block mb-1">ایمیل</label>
                            <input type="email" id="email" class="form-input w-full px-4 py-2 rounded-md">
                        </div>
                        <div>
                            <label for="phone" class="block mb-1">شماره تماس</label>
                            <input type="tel" id="phone" class="form-input w-full px-4 py-2 rounded-md">
                        </div>
                        <div>
                            <label for="message" class="block mb-1">پیام شما</label>
                            <textarea id="message" rows="4" class="form-input w-full px-4 py-2 rounded-md"></textarea>
                        </div>
                        <button type="submit" class="bg-blood-red text-white px-6 py-3 rounded-md w-full font-medium hover:bg-red-900 transition duration-300">ارسال پیام</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Login Modal -->
    <div id="login-modal" class="fixed inset-0 bg-black bg-opacity-75 flex items-center justify-center z-50 hidden">
        <div class="bg-gray-900 rounded-lg max-w-md w-full p-8 relative">
            <button id="close-login-modal" class="absolute left-4 top-4 text-gray-400 hover:text-white">
                <i class="fas fa-times text-2xl"></i>
            </button>
            
            <div class="text-center mb-8">
                <h3 class="text-2xl font-bold">ورود به حساب کاربری</h3>
            </div>
            
            <form class="space-y-4">
                <div>
                    <label for="login-username" class="block mb-1">نام کاربری</label>
                    <input type="text" id="login-username" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div>
                    <label for="login-password" class="block mb-1">رمز عبور</label>
                    <input type="password" id="login-password" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div class="flex justify-between items-center">
                    <div class="flex items-center">
                        <input type="checkbox" id="remember-me" class="form-checkbox h-4 w-4 text-blood-red">
                        <label for="remember-me" class="mr-2">مرا به خاطر بسپار</label>
                    </div>
                    <a href="#" class="text-blood-red hover:underline">فراموشی رمز عبور</a>
                </div>
                <button type="submit" class="bg-blood-red text-white px-6 py-3 rounded-md w-full font-medium hover:bg-red-900 transition duration-300">ورود</button>
            </form>
            
            <div class="text-center mt-6">
                <p class="text-gray-400">حساب کاربری ندارید؟ <a href="#register" class="text-blood-red hover:underline font-medium">ثبت نام کنید</a></p>
            </div>
        </div>
    </div>

    <!-- Register Modal -->
    <div id="register-modal" class="fixed inset-0 bg-black bg-opacity-75 flex items-center justify-center z-50 hidden">
        <div class="bg-gray-900 rounded-lg max-w-md w-full p-8 relative">
            <button id="close-register-modal" class="absolute left-4 top-4 text-gray-400 hover:text-white">
                <i class="fas fa-times text-2xl"></i>
            </button>
            
            <div class="text-center mb-8">
                <h3 class="text-2xl font-bold">ثبت نام کاربر جدید</h3>
            </div>
            
            <form class="space-y-4">
                <div>
                    <label for="register-name" class="block mb-1">نام و نام خانوادگی</label>
                    <input type="text" id="register-name" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div>
                    <label for="register-email" class="block mb-1">ایمیل</label>
                    <input type="email" id="register-email" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div>
                    <label for="register-phone" class="block mb-1">شماره تماس</label>
                    <input type="tel" id="register-phone" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div>
                    <label for="register-password" class="block mb-1">رمز عبور</label>
                    <input type="password" id="register-password" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div>
                    <label for="register-confirm-password" class="block mb-1">تکرار رمز عبور</label>
                    <input type="password" id="register-confirm-password" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                <div class="flex items-center">
                    <input type="checkbox" id="terms" class="form-checkbox h-4 w-4 text-blood-red">
                    <label for="terms" class="mr-2">با <a href="#" class="text-blood-red hover:underline">قوانین و شرایط</a> موافقم</label>
                </div>
                <button type="submit" class="bg-blood-red text-white px-6 py-3 rounded-md w-full font-medium hover:bg-red-900 transition duration-300">ثبت نام</button>
            </form>
            
            <div class="text-center mt-6">
                <p class="text-gray-400">حساب کاربری دارید؟ <a href="#login" class="text-blood-red hover:underline font-medium">وارد شوید</a></p>
            </div>
        </div>
    </div>

    <!-- Order Modal -->
    <div id="order-modal" class="fixed inset-0 bg-black bg-opacity-75 flex items-center justify-center z-50 hidden">
        <div class="bg-gray-900 rounded-lg max-w-2xl w-full p-8 relative">
            <button id="close-order-modal" class="absolute left-4 top-4 text-gray-400 hover:text-white">
                <i class="fas fa-times text-2xl"></i>
            </button>
            
            <div class="text-center mb-8">
                <h3 class="text-2xl font-bold">ثبت سفارش جدید</h3>
            </div>
            
            <form class="space-y-4">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <div>
                        <label for="order-name" class="block mb-1">نام و نام خانوادگی</label>
                        <input type="text" id="order-name" class="form-input w-full px-4 py-2 rounded-md">
                    </div>
                    <div>
                        <label for="order-phone" class="block mb-1">شماره تماس</label>
                        <input type="tel" id="order-phone" class="form-input w-full px-4 py-2 rounded-md">
                    </div>
                </div>
                
                <div>
                    <label for="order-service" class="block mb-1">نوع خدمت</label>
                    <select id="order-service" class="form-input w-full px-4 py-2 rounded-md">
                        <option value="">انتخاب کنید</option>
                        <option value="video-editing">تدوین ویدیو</option>
                        <option value="graphic-design">طراحی گرافیک</option>
                        <option value="photography">عکاسی</option>
                        <option value="other">سایر</option>
                    </select>
                </div>
                
                <div>
                    <label for="order-description" class="block mb-1">توضیحات پروژه</label>
                    <textarea id="order-description" rows="4" class="form-input w-full px-4 py-2 rounded-md"></textarea>
                </div>
                
                <div>
                    <label for="order-deadline" class="block mb-1">مهلت تحویل</label>
                    <input type="date" id="order-deadline" class="form-input w-full px-4 py-2 rounded-md">
                </div>
                
                <div>
                    <label for="order-files" class="block mb-1">فایل‌های مورد نیاز (اختیاری)</label>
                    <div class="border-2 border-dashed border-gray-700 rounded-md p-4 text-center">
                        <input type="file" id="order-files" class="hidden" multiple>
                        <label for="order-files" class="cursor-pointer">
                            <div class="text-blood-red text-3xl mb-2">
                                <i class="fas fa-cloud-upload-alt"></i>
                            </div>
                            <p class="text-gray-400">فایل‌های خود را اینجا رها کنید یا برای انتخاب کلیک کنید</p>
                            <p class="text-sm text-gray-500 mt-1">حداکثر حجم فایل: 50MB</p>
                        </label>
                    </div>
                </div>
                
                <button type="submit" class="bg-blood-red text-white px-6 py-3 rounded-md w-full font-medium hover:bg-red-900 transition duration-300">ثبت سفارش</button>
            </form>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-black py-12 px-4 border-t border-gray-800">
        <div class="max-w-6xl mx-auto">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4">رسانه هنری فاتح</h3>
                    <p class="text-gray-400">تخصص ما در خلق آثار هنری منحصر به فرد و تدوین حرفه‌ای است. هر پروژه داستان منحصر به فرد خود را دارد.</p>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold mb-4">لینک‌های سریع</h3>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-blood-red transition duration-300">صفحه اصلی</a></li>
                        <li><a href="#services" class="text-gray-400 hover:text-blood-red transition duration-300">خدمات</a></li>
                        <li><a href="#portfolio" class="text-gray-400 hover:text-blood-red transition duration-300">نمونه کارها</a></li>
                        <li><a href="#about" class="text-gray-400 hover:text-blood-red transition duration-300">درباره ما</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-blood-red transition duration-300">تماس با ما</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold mb-4">خدمات</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-blood-red transition duration-300">تدوین ویدیو</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-blood-red transition duration-300">طراحی گرافیک</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-blood-red transition duration-300">عکاسی</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-blood-red transition duration-300">موسیقی</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-blood-red transition duration-300">پست‌پردازش</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold mb-4">خبرنامه</h3>
                    <p class="text-gray-400 mb-4">برای دریافت آخرین اخبار و نمونه کارهای جدید در خبرنامه ما عضو شوید.</p>
                    <form class="flex">
                        <input type="email" placeholder="ایمیل شما" class="form-input px-4 py-2 rounded-r-none rounded-l-md w-full">
                        <button type="submit" class="bg-blood-red text-white px-4 py-2 rounded-l-none rounded-r-md hover:bg-red-900 transition duration-300">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 text-sm">© 2023 رسانه هنری فاتح. تمامی حقوق محفوظ است.</p>
                <div class="flex space-x-4 space-x-reverse mt-4 md:mt-0">
                    <a href="#" class="text-gray-500 hover:text-blood-red transition duration-300">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="#" class="text-gray-500 hover:text-blood-red transition duration-300">
                        <i class="fab fa-telegram"></i>
                    </a>
                    <a href="#" class="text-gray-500 hover:text-blood-red transition duration-300">
                        <i class="fab fa-youtube"></i>
                    </a>
                    <a href="#" class="text-gray-500 hover:text-blood-red transition duration-300">
                        <i class="fab fa-aparat"></i>
                    </a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Floating Order Button -->
    <div class="fixed bottom-8 left-8 z-40">
        <button id="order-button" class="bg-blood-red text-white p-4 rounded-full shadow-lg hover:bg-red-900 transition duration-300">
            <i class="fas fa-plus text-xl"></i>
        </button>
    </div>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Login modal
        const loginLinks = document.querySelectorAll('a[href="#login"]');
        const loginModal = document.getElementById('login-modal');
        const closeLoginModal = document.getElementById('close-login-modal');
        
        loginLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                loginModal.classList.remove('hidden');
            });
        });
        
        closeLoginModal.addEventListener('click', () => {
            loginModal.classList.add('hidden');
        });
        
        // Register modal
        const registerLinks = document.querySelectorAll('a[href="#register"]');
        const registerModal = document.getElementById('register-modal');
        const closeRegisterModal = document.getElementById('close-register-modal');
        
        registerLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                registerModal.classList.remove('hidden');
                loginModal.classList.add('hidden');
            });
        });
        
        closeRegisterModal.addEventListener('click', () => {
            registerModal.classList.add('hidden');
        });
        
        // Order modal
        const orderButton = document.getElementById('order-button');
        const orderModal = document.getElementById('order-modal');
        const closeOrderModal = document.getElementById('close-order-modal');
        
        orderButton.addEventListener('click', () => {
            orderModal.classList.remove('hidden');
        });
        
        closeOrderModal.addEventListener('click', () => {
            orderModal.classList.add('hidden');
        });
        
        // Close modals when clicking outside
        [loginModal, registerModal, orderModal].forEach(modal => {
            modal.addEventListener('click', (e) => {
                if (e.target === modal) {
                    modal.classList.add('hidden');
                }
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                if (this.getAttribute('href') === '#login' || 
                    this.getAttribute('href') === '#register' || 
                    this.getAttribute('href') === '#order') {
                    return;
                }
                
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    mobileMenu.classList.add('hidden');
                }
            });
        });
    </script>
</body>
</html>
