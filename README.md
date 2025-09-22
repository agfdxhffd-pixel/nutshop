<!DOCTYPE html>

<html lang="th">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Nut Shop - Pro Settings & 3D Art</title>

    <script src="https://cdn.tailwindcss.com"></script>

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Kanit:wght@300;400;600&display=swap" rel="stylesheet">

    <style>

        body {

            font-family: 'Kanit', sans-serif;

            position: relative;

            background-color: #1a1a1a;

        }

        /* Background Image with Blur Effect */

        body::before {

            content: '';

            position: fixed;

            top: 0;

            left: 0;

            width: 100%;

            height: 100%;

            background-image: url('https://i.imgur.com/example.jpg'); /* <-- !!! ใส่ URL รูป 3D ของคุณที่นี่ !!! */

            background-size: cover;

            background-position: center;

            filter: blur(4px) brightness(0.4);

            z-index: -1;

        }

        .font-orbitron {

            font-family: 'Orbitron', sans-serif;

        }

        .card {

            background-color: rgba(26, 26, 26, 0.8);

            backdrop-filter: blur(10px);

            border: 1px solid rgba(255, 255, 255, 0.1);

            transition: all 0.3s ease;

        }

        .card:hover {

            transform: translateY(-5px);

            box-shadow: 0 0 20px rgba(255, 193, 7, 0.5);

            border-color: rgba(255, 193, 7, 0.7);

        }

        .btn-primary {

            background: linear-gradient(90deg, #f59e0b, #ef4444);

            transition: all 0.3s ease;

            box-shadow: 0 0 15px rgba(245, 158, 11, 0.5);

        }

        .btn-primary:hover {

            transform: scale(1.05);

            box-shadow: 0 0 25px rgba(245, 158, 11, 0.8);

        }

        .section-title {

            text-shadow: 0 0 10px rgba(255, 255, 255, 0.7);

        }

    </style>

</head>

<body class="text-white">



    <!-- Header -->

    <header class="sticky top-0 z-50 bg-black bg-opacity-50 backdrop-blur-lg">

        <div class="container mx-auto px-6 py-4 flex justify-between items-center">

            <div class="font-orbitron text-2xl font-bold tracking-widest">

                <a href="#">NUT<span class="text-amber-400">SHOP</span></a>

                <p class="text-xs font-kanit tracking-normal text-gray-300">Nuts setting shop</p>

            </div>

            <nav class="hidden md:flex space-x-6 items-center">

                <a href="#settings" class="hover:text-amber-400 transition-colors">ตั้งค่าเกม</a>

                <a href="#3d-art" class="hover:text-amber-400 transition-colors">งาน 3D</a>

                <a href="#topup" class="hover:text-amber-400 transition-colors">เติมเงิน</a>

                <a href="#contact" class="bg-amber-500 hover:bg-amber-600 px-4 py-2 rounded-md font-bold transition-colors">ติดต่อ</a>

            </nav>

            <button id="mobile-menu-button" class="md:hidden text-2xl">☰</button>

        </div>

        <!-- Mobile Menu -->

        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4">

            <a href="#settings" class="block py-2 hover:text-amber-400">ตั้งค่าเกม</a>

            <a href="#3d-art" class="block py-2 hover:text-amber-400">งาน 3D</a>

            <a href="#topup" class="block py-2 hover:text-amber-400">เติมเงิน</a>

            <a href="#contact" class="block py-2 mt-2 bg-amber-500 text-center rounded-md font-bold">ติดต่อ</a>

        </div>

    </header>



    <!-- Main Content -->

    <main class="container mx-auto px-6 py-12">



        <!-- Hero Section -->

        <section class="text-center py-20">

            <h1 class="font-orbitron text-5xl md:text-7xl font-bold mb-4 section-title">

                ปลดล็อก<span class="text-amber-400">ศักยภาพ</span>การเล่น

            </h1>

            <p class="text-lg text-gray-300 max-w-2xl mx-auto mb-8">

                ยกระดับประสบการณ์ Free Fire ของคุณด้วยการตั้งค่าระดับโปรและงาน 3D สุดเท่ที่ไม่เหมือนใคร

            </p>

            <div class="space-x-4">

                <a href="#settings" class="btn-primary text-white font-bold py-3 px-8 rounded-full text-lg">ดูการตั้งค่า</a>

            </div>

        </section>



        <!-- Game Settings Section -->

        <section id="settings" class="py-16">

            <h2 class="font-orbitron text-4xl font-bold text-center mb-10 section-title">ขายการตั้งค่าเกม</h2>

            <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">

                <!-- iOS Settings Card -->

                <div class="card rounded-lg p-8 text-center">

                    <h3 class="text-2xl font-bold mb-2">ตั้งค่าสำหรับ iOS</h3>

                    <p class="text-amber-400 font-semibold mb-4">เฉพาะสำหรับยิงหัว</p>

                    <div class="my-6">

                        <span class="text-5xl font-bold">100</span>

                        <span class="text-gray-400">บาท</span>

                    </div>

                    <p class="text-gray-300 mb-6">ปรับแต่งมาอย่างดีสำหรับผู้ใช้ iPhone และ iPad เพื่อความแม่นยำสูงสุด</p>

                    <button onclick="showOrderModal()" class="w-full btn-primary text-white font-bold py-3 px-6 rounded-lg">สั่งซื้อ</button>

                </div>

                <!-- PC Settings Card -->

                <div class="card rounded-lg p-8 text-center">

                    <h3 class="text-2xl font-bold mb-2">ตั้งค่าสำหรับ PC</h3>

                    <p class="text-amber-400 font-semibold mb-4">เฉพาะสำหรับยิงหัว</p>

                    <div class="my-6">

                        <span class="text-5xl font-bold">200</span>

                        <span class="text-gray-400">บาท</span>

                    </div>

                    <p class="text-gray-300 mb-6">การตั้งค่าสำหรับ Emulator บน PC ตอบสนองไว ลากหัวคมๆ ไม่มีพลาด</p>

                    <button onclick="showOrderModal()" class="w-full btn-primary text-white font-bold py-3 px-6 rounded-lg">สั่งซื้อ</button>

                </div>

            </div>

        </section>



        <!-- 3D Art Section -->

        <section id="3d-art" class="py-16">

            <h2 class="font-orbitron text-4xl font-bold text-center mb-10 section-title">รับทำ 3D Free Fire</h2>

            <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">

                <!-- 3D Image Card -->

                <div class="card rounded-lg overflow-hidden">

                    <img src="https://i.imgur.com/example.jpg" alt="3D Art Example" class="w-full h-64 object-cover"> <!-- <-- !!! ใส่ URL รูป 3D ของคุณที่นี่ !!! -->

                    <div class="p-6">

                        <h3 class="text-2xl font-bold mb-2">ภาพ 3D</h3>

                        <p class="text-gray-300 mb-4">รับทำรูปโปรไฟล์, Banner, โลโก้ และอื่นๆ ตามสไตล์ที่คุณต้องการ</p>

                        <div class="flex justify-between items-center">

                            <p class="text-xl font-bold text-amber-400">เริ่มต้น 100 บาท</p>

                            <button onclick="showOrderModal()" class="btn-primary text-white font-bold py-2 px-5 rounded-lg">สอบถาม</button>

                        </div>

                    </div>

                </div>

                <!-- 3D Video Card -->

                <div class="card rounded-lg overflow-hidden">

                     <div class="w-full h-64 bg-black">

                        <video class="w-full h-full object-cover" autoplay loop muted playsinline>

                            <!-- 

                                สำคัญมาก! 

                                1. อัปโหลดไฟล์วิดีโอของคุณ (0001-0750.mp4) ไปยังเว็บฝากไฟล์ เช่น Imgur, Streamable

                                2. คัดลอก "ลิงก์ตรง" ที่ลงท้ายด้วย .mp4

                                3. นำลิงก์มาวางแทนที่ "https://i.imgur.com/example.mp4" ด้านล่างนี้

                            -->

                            <source src="https://i.imgur.com/example.mp4" type="video/mp4">

                            เบราว์เซอร์ของคุณไม่รองรับวิดีโอ

                        </video>

                    </div>

                    <div class="p-6">

                        <h3 class="text-2xl font-bold mb-2">วิดีโอคลิป 3D</h3>

                        <p class="text-gray-300 mb-4">Intro, Outro หรือคลิปเท่ๆ สำหรับช่อง YouTube และโซเชียลมีเดีย</p>

                        <div class="flex justify-between items-center">

                            <p class="text-xl font-bold text-amber-400">เริ่มต้น 230 บาท</p>

                            <button onclick="showOrderModal()" class="btn-primary text-white font-bold py-2 px-5 rounded-lg">สอบถาม</button>

                        </div>

                    </div>

                </div>

            </div>

        </section>



        <!-- Top-Up Section -->

        <section id="topup" class="py-16">

            <div class="card max-w-2xl mx-auto p-8">

                <h2 class="font-orbitron text-3xl font-bold text-center mb-2 section-title">เติมเงิน / เครดิต</h2>

                <p class="text-center text-gray-400 mb-6">ระบบนี้เป็นเพียงตัวอย่าง UI สำหรับการพัฒนาต่อในอนาคต</p>

                <div class="mb-4">

                    <label for="amount" class="block mb-2 font-semibold">จำนวนเงิน</label>

                    <input type="number" id="amount" class="w-full bg-gray-900 border border-gray-700 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-amber-500" placeholder="ระบุจำนวนเงิน">

                </div>

                <button class="w-full btn-primary font-bold py-3 rounded-lg">ดำเนินการต่อ</button>

            </div>

        </section>



        <!-- Contact Section -->

        <section id="contact" class="text-center py-16">

             <h2 class="font-orbitron text-4xl font-bold text-center mb-4 section-title">สนใจสั่งซื้อหรือสอบถาม?</h2>

             <p class="text-lg text-gray-300 max-w-2xl mx-auto mb-8">

                ติดต่อมาได้เลยที่ Facebook ส่วนตัว ตอบไว เป็นกันเอง

            </p>

            <a href="https://www.facebook.com/search/top?q=Kraiwitch%20Pacharasuriya" target="_blank" class="btn-primary text-white font-bold py-3 px-8 rounded-full text-lg inline-block">

                ติดต่อผ่าน Facebook

            </a>

        </section>

    </main>



    <!-- Footer -->

    <footer class="bg-black bg-opacity-70 mt-16 py-6">

        <div class="container mx-auto text-center text-gray-400">

            <p>&copy; 2024 Nut Shop. All Rights Reserved.</p>

        </div>

    </footer>



    <!-- Order Modal -->

    <div id="orderModal" class="fixed inset-0 bg-black bg-opacity-70 flex items-center justify-center z-50 hidden">

        <div class="bg-gray-800 rounded-lg p-8 max-w-sm mx-4 text-center border border-amber-500">

            <h3 class="text-2xl font-bold mb-4">ขั้นตอนการสั่งซื้อ</h3>

            <p class="text-gray-300 mb-6">สำหรับการสั่งซื้อสินค้าหรือสอบถามรายละเอียดเพิ่มเติม กรุณาติดต่อเราโดยตรงผ่านทาง Facebook</p>

            <a href="https://www.facebook.com/search/top?q=Kraiwitch%20Pacharasuriya" target="_blank" class="btn-primary text-white font-bold py-2 px-6 rounded-lg inline-block mb-2">ไปที่ Facebook</a>

            <button onclick="closeModal()" class="w-full bg-gray-600 hover:bg-gray-700 text-white font-bold py-2 px-6 rounded-lg">ปิด</button>

        </div>

    </div>

    

    <script>

        // Mobile Menu Toggle

        const mobileMenuButton = document.getElementById('mobile-menu-button');

        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {

            mobileMenu.classList.toggle('hidden');

        });



        // Modal Logic

        const orderModal = document.getElementById('orderModal');

        function showOrderModal() {

            orderModal.classList.remove('hidden');

        }

        function closeModal() {

            orderModal.classList.add('hidden');

        }

    </script>



</body>

</html># nutshop
