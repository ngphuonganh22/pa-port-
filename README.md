# pa-port-
my portfolio 
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nguyễn Phương Anh | Portfolio</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- AOS Animation Library -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        brandDark: '#121212',
                        brandAccent: '#2A2A2A',
                        brandCard: '#1E1E1E',
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #0f0f10;
            color: #e4e4e7;
            overflow-x: hidden;
        }
        .polaroid-frame {
            background: #f4f4f0;
            padding: 12px 12px 40px 12px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5), 0 8px 10px -6px rgba(0, 0, 0, 0.5);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
        }
        .polaroid-frame:hover {
            transform: rotate(-2deg) scale(1.03);
            box-shadow: 0 25px 30px -5px rgba(255, 255, 255, 0.1);
        }
        .glass-card {
            background: rgba(30, 30, 35, 0.6);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glass-card:hover {
            border-color: rgba(255, 255, 255, 0.2);
        }
        .social-btn {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px -5px rgba(255, 255, 255, 0.15);
        }
    </style>
</head>
<body class="font-sans antialiased selection:bg-white selection:text-black">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 w-full z-50 glass-card px-6 py-4 flex justify-between items-center border-b border-white/10">
        <span class="text-xl font-bold tracking-tight text-white">Phuong Anh<span class="text-xs text-gray-400 font-normal">.portfolio</span></span>
        <div class="flex items-center space-x-6">
            <a href="#about" class="text-sm text-gray-400 hover:text-white transition">Giới thiệu</a>
            <a href="#projects" class="text-sm text-gray-400 hover:text-white transition">Dự án</a>
            <a href="#skills" class="text-sm text-gray-400 hover:text-white transition">Kỹ năng</a>
            <a href="#contact" class="px-4 py-2 bg-white text-black text-xs font-semibold rounded-full hover:bg-gray-200 transition">Liên hệ</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="min-h-screen pt-32 pb-20 px-6 max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-between gap-12">
        <div class="md:w-1/2 space-y-6" data-aos="fade-right" data-aos-duration="1000">
            <div class="inline-block px-3 py-1 bg-white/10 rounded-full text-xs tracking-wider uppercase text-gray-300 border border-white/10">
                Founder & Communications Executive
            </div>
            <h1 class="text-5xl md:text-7xl font-extrabold tracking-tight text-white leading-tight">
                Hello, I'm <br/><span class="text-transparent bg-clip-text bg-gradient-to-r from-white via-gray-300 to-gray-500">Phuong Anh.</span>
            </h1>
            <p class="text-lg text-gray-400 leading-relaxed max-w-lg">
                <span class="text-white font-medium">Curious by nature. Structured by mindset.</span><br/>
                Kết hợp tư duy phân tích sắc bén & sáng tạo nghệ thuật để tạo ra những giải pháp truyền thông chỉn chu.
            </p>

            <!-- Social Links Box -->
            <div class="pt-4 flex flex-wrap items-center gap-4">
                <a href="https://linkedin.com/in/www.linkedin.com/in/phuong-anh-nguyen-935198340" target="_blank" rel="noopener noreferrer" 
                   class="social-btn flex items-center space-x-3 px-5 py-3 rounded-2xl bg-white/5 border border-white/10 hover:bg-white hover:text-black group">
                    <i class="fab fa-linkedin-in text-lg group-hover:text-black"></i>
                    <span class="text-sm font-medium">LinkedIn</span>
                    <i class="fas font-thin fa-arrow-up-right-from-square text-xs opacity-50 group-hover:opacity-100"></i>
                </a>

                <a href="https://instagram.com/https://www.instagram.com/nguynpa_/" target="_blank" rel="noopener noreferrer" 
                   class="social-btn flex items-center space-x-3 px-5 py-3 rounded-2xl bg-white/5 border border-white/10 hover:bg-gradient-to-tr hover:from-amber-500 hover:via-rose-500 hover:to-purple-600 hover:border-transparent group">
                    <i class="fab fa-instagram text-lg"></i>
                    <span class="text-sm font-medium">Instagram</span>
                    <i class="fas font-thin fa-arrow-up-right-from-square text-xs opacity-50 group-hover:opacity-100"></i>
                </a>
            </div>
        </div>

        <!-- Polaroid Style Avatar Container -->
        <div class="md:w-1/2 flex justify-center" data-aos="fade-left" data-aos-duration="1000">
            <div class="polaroid-frame relative max-w-xs md:max-w-sm rounded-sm">
                <!-- Chú ý: Bạn có thể thay link ảnh đại diện của bạn vào tag src bên dưới -->
                <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=800&q=80" 
                     alt="Nguyễn Phương Anh" class="w-full h-80 object-cover rounded-sm grayscale contrast-125 hover:grayscale-0 transition duration-500">
                <div class="mt-4 flex justify-between items-center px-1">
                    <span class="font-serif italic text-black font-semibold text-lg">Phuong Anh</span>
                    <i class="fas fa-star text-black text-xs"></i>
                </div>
            </div>
        </div>
    </section>

    <!-- Key Stats / Highlights -->
    <section class="py-12 border-y border-white/10 bg-white/[0.02]">
        <div class="max-w-6xl mx-auto px-6 grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
            <div data-aos="zoom-in" data-aos-delay="100">
                <div class="text-3xl md:text-4xl font-bold text-white">300+</div>
                <div class="text-xs text-gray-400 mt-1 uppercase tracking-wider">Khách hàng / Tương tác</div>
            </div>
            <div data-aos="zoom-in" data-aos-delay="200">
                <div class="text-3xl md:text-4xl font-bold text-white">100+</div>
                <div class="text-xs text-gray-400 mt-1 uppercase tracking-wider">Đơn hàng / Sản phẩm</div>
            </div>
            <div data-aos="zoom-in" data-aos-delay="300">
                <div class="text-3xl md:text-4xl font-bold text-white">VND 40-50M</div>
                <div class="text-xs text-gray-400 mt-1 uppercase tracking-wider">Doanh thu dự án</div>
            </div>
            <div data-aos="zoom-in" data-aos-delay="400">
                <div class="text-3xl md:text-4xl font-bold text-white">2.5+</div>
                <div class="text-xs text-gray-400 mt-1 uppercase tracking-wider">Năm kinh nghiệm</div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-24 px-6 max-w-6xl mx-auto">
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-16" data-aos="fade-up">
            <div>
                <h2 class="text-xs font-semibold tracking-widest text-gray-400 uppercase">Portfolio</h2>
                <p class="text-3xl md:text-4xl font-bold text-white mt-2">Things I've worked on.</p>
            </div>
            <p class="text-gray-400 text-sm mt-4 md:mt-0 max-w-md">A few things I've built, studied, and worked on from personal projects to professional experience.</p>
        </div>

        <div class="grid md:grid-cols-2 gap-8">
            <!-- Project 1: Monochic -->
            <div class="glass-card rounded-3xl p-8 relative overflow-hidden group transition duration-500 hover:-translate-y-2" data-aos="fade-up" data-aos-delay="100">
                <div class="flex justify-between items-start mb-6">
                    <span class="text-xs font-mono px-3 py-1 bg-white/10 rounded-full text-gray-300">Building Monochic</span>
                    <span class="text-xs text-gray-500">Business Project</span>
                </div>
                <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-gray-200">Monochic Ceramic</h3>
                <p class="text-gray-400 text-sm leading-relaxed mb-6">
                    Dự án kinh doanh gốm sứ nghệ thuật kết hợp phân tích Business Model Canvas, tối ưu hoá kênh bán và chiến dịch truyền thông đa nền tảng.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Commercial Analysis</span>
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Product Strategy</span>
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Execution</span>
                </div>
                <div class="pt-4 border-t border-white/5 flex items-center justify-between text-xs text-gray-400">
                    <span>Key Results: High Retention</span>
                    <i class="fas fa-arrow-right group-hover:translate-x-2 transition duration-300"></i>
                </div>
            </div>

            <!-- Project 2: Communications Executive -->
            <div class="glass-card rounded-3xl p-8 relative overflow-hidden group transition duration-500 hover:-translate-y-2" data-aos="fade-up" data-aos-delay="200">
                <div class="flex justify-between items-start mb-6">
                    <span class="text-xs font-mono px-3 py-1 bg-white/10 rounded-full text-gray-300">Startup Venture</span>
                    <span class="text-xs text-gray-500">Corporate Experience</span>
                </div>
                <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-gray-200">Communications & Digital Delivery</h3>
                <p class="text-gray-400 text-sm leading-relaxed mb-6">
                    Thực thi các chiến dịch truyền thông sự kiện, xây dựng quan hệ báo chí (Media Relations) và quản lý dự án số đạt hiệu quả chuyển đổi cao.
                </p>
                <div class="flex flex-wrap gap-2 mb-6">
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Internal Comms</span>
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Event Delivery</span>
                    <span class="text-xs px-2.5 py-1 bg-white/5 rounded-md text-gray-400">Media Relation</span>
                </div>
                <div class="pt-4 border-t border-white/5 flex items-center justify-between text-xs text-gray-400">
                    <span>Strategic Outputs</span>
                    <i class="fas fa-arrow-right group-hover:translate-x-2 transition duration-300"></i>
                </div>
            </div>
        </div>
    </section>

    <!-- Mindset & Skills -->
    <section id="skills" class="py-24 px-6 max-w-6xl mx-auto border-t border-white/10">
        <div class="text-center max-w-2xl mx-auto mb-16" data-aos="fade-up">
            <h2 class="text-xs font-semibold tracking-widest text-gray-400 uppercase mb-2">Capabilities</h2>
            <p class="text-3xl font-bold text-white">A mix of analytical & creative.</p>
        </div>

        <div class="grid md:grid-cols-3 gap-8">
            <div class="glass-card p-6 rounded-2xl" data-aos="fade-up" data-aos-delay="100">
                <div class="w-10 h-10 rounded-xl bg-white/10 flex items-center justify-center mb-4 text-white">
                    <i class="fas fa-wrench"></i>
                </div>
                <h4 class="text-lg font-bold text-white mb-2">Tools & Tech</h4>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Sử dụng thành thạo các công cụ thiết kế, phân tích dữ liệu, hệ thống quản lý công việc và truyền thông số.
                </p>
            </div>

            <div class="glass-card p-6 rounded-2xl" data-aos="fade-up" data-aos-delay="200">
                <div class="w-10 h-10 rounded-xl bg-white/10 flex items-center justify-center mb-4 text-white">
                    <i class="fas fa-language"></i>
                </div>
                <h4 class="text-lg font-bold text-white mb-2">Languages</h4>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Tiếng Việt (Bản ngữ), Tiếng Anh (Giao tiếp công việc & Viết nội dung chuyên nghiệp).
                </p>
            </div>

            <div class="glass-card p-6 rounded-2xl" data-aos="fade-up" data-aos-delay="300">
                <div class="w-10 h-10 rounded-xl bg-white/10 flex items-center justify-center mb-4 text-white">
                    <i class="fas fa-award"></i>
                </div>
                <h4 class="text-lg font-bold text-white mb-2">Awards & Honors</h4>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Ghi nhận qua các dự án thực tế, các giải thưởng truyền thông và khởi nghiệp.
                </p>
            </div>
        </div>
    </section>

    <!-- Footer / Contact Section -->
    <footer id="contact" class="py-20 px-6 border-t border-white/10 text-center">
        <div class="max-w-4xl mx-auto space-y-8" data-aos="zoom-in">
            <h2 class="text-4xl md:text-5xl font-extrabold text-white">
                Let's make <br/><span class="text-gray-500">something meaningful.</span>
            </h2>

            <!-- Social Links Box in Footer -->
            <div class="flex justify-center items-center gap-6 pt-4">
                <a href="https://linkedin.com/in/YOUR_LINKEDIN" target="_blank" class="w-12 h-12 rounded-full bg-white/5 border border-white/10 flex items-center justify-center text-white hover:bg-white hover:text-black transition">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="https://instagram.com/YOUR_INSTAGRAM" target="_blank" class="w-12 h-12 rounded-full bg-white/5 border border-white/10 flex items-center justify-center text-white hover:bg-rose-500 transition">
                    <i class="fab fa-instagram"></i>
                </a>
            </div>

            <p class="text-xs text-gray-600 pt-8">
                &copy; 2026 Nguyễn Phương Anh. Designed with minimal aesthetic.
            </p>
        </div>
    </footer>

    <!-- AOS JS for Scroll Animations -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({
            once: true,
            duration: 800,
            easing: 'ease-out-cubic'
        });
    </script>
</body>
</html>
