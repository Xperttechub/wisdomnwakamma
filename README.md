<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wisdom Nwakamma | Technologist & Pastor</title>
    <!-- Cloudinary Logo as Favicon -->
    <link rel="icon" type="image/png" href="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png">
    <!-- Open Graph Meta for Social Sharing -->
    <meta property="og:image" content="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png">
    <meta property="og:title" content="Wisdom Nwakamma | Technologist & Pastor">
    <meta property="og:description" content="Software Engineering Student at Southern Delta University | Founder of Xpert Tech Hub & Spirit Revive Community">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    },
                    colors: {
                        primary: '#1e3a8a',
                        secondary: '#dc2626',
                        accent: '#f59e0b',
                        dark: '#0f172a',
                        light: '#f8fafc',
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'pulse-slow': 'pulse 4s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-20px)' },
                        }
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }
        
        .text-gradient {
            background: linear-gradient(135deg, #1e3a8a 0%, #dc2626 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .glass {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .service-card {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(30, 58, 138, 0.2);
        }
        
        .project-card {
            overflow: hidden;
            position: relative;
        }
        
        .project-card img {
            transition: transform 0.6s ease;
        }
        
        .project-card:hover img {
            transform: scale(1.1);
        }
        
        .project-overlay {
            background: linear-gradient(to top, rgba(30, 58, 138, 0.95), transparent);
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        
        .project-card:hover .project-overlay {
            opacity: 1;
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -4px;
            left: 0;
            background: linear-gradient(90deg, #1e3a8a, #dc2626);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #1e3a8a 0%, #1e40af 100%);
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(30, 58, 138, 0.4);
        }
        
        .btn-secondary {
            background: linear-gradient(135deg, #dc2626 0%, #b91c1c 100%);
            transition: all 0.3s ease;
        }
        
        .btn-secondary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(220, 38, 38, 0.4);
        }
        
        .btn-youtube {
            background: linear-gradient(135deg, #FF0000 0%, #CC0000 100%);
            transition: all 0.3s ease;
        }
        
        .btn-youtube:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(255, 0, 0, 0.4);
        }
        
        .skill-bar {
            width: 0;
            transition: width 1.5s ease-out;
        }
        
        .counter {
            font-variant-numeric: tabular-nums;
        }
        
        ::-webkit-scrollbar {
            width: 10px;
        }
        
        ::-webkit-scrollbar-track {
            background: #0f172a;
        }
        
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(180deg, #1e3a8a, #dc2626);
            border-radius: 5px;
        }

        .profile-image {
            object-position: center top;
        }
        
        .logo-img {
            height: 45px;
            width: auto;
            object-fit: contain;
            filter: drop-shadow(0 0 10px rgba(255,255,255,0.1));
            transition: transform 0.3s ease;
        }
        
        .logo-nav {
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }
        
        .logo-nav:hover .logo-img {
            transform: scale(1.05);
        }
        
        .logo-large {
            height: 100px;
            width: auto;
        }
        
        .logo-medium {
            height: 70px;
            width: auto;
        }
        
        .logo-small {
            height: 50px;
            width: auto;
        }
        
        .logo-badge {
            height: 24px;
            width: auto;
        }
        
        /* Fallback text styling */
        .logo-fallback {
            font-size: 1.5rem;
            font-weight: bold;
            background: linear-gradient(135deg, #1e3a8a 0%, #dc2626 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: none;
        }
        
        .glow-effect {
            filter: drop-shadow(0 0 15px rgba(30, 58, 138, 0.3));
        }
    </style>
</head>
<body class="bg-dark text-light antialiased">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 top-0 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="logo-nav group flex items-center gap-3">
                    <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                         alt="Wisdom Nwakamma Logo" 
                         class="logo-img glow-effect"
                         onerror="this.style.display='none'; document.getElementById('navLogoFallback').style.display='block';">
                    <span id="navLogoFallback" class="logo-fallback">Wisdom Nwakamma</span>
                </a>
                
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#about" class="nav-link text-sm font-medium hover:text-accent transition-colors">About</a>
                    <a href="#services" class="nav-link text-sm font-medium hover:text-accent transition-colors">Services</a>
                    <a href="#xpert-tech" class="nav-link text-sm font-medium hover:text-accent transition-colors">Xpert Tech Hub</a>
                    <a href="#ministry" class="nav-link text-sm font-medium hover:text-accent transition-colors">Ministry</a>
                    <a href="#contact" class="btn-primary px-6 py-2 rounded-full text-sm font-semibold">Get in Touch</a>
                </div>

                <button class="md:hidden text-2xl" onclick="toggleMenu()">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobileMenu" class="hidden md:hidden bg-dark/95 backdrop-blur-lg absolute w-full border-t border-white/10">
            <div class="flex flex-col p-6 space-y-4">
                <div class="flex items-center gap-3 mb-4 pb-4 border-b border-white/10">
                    <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                         alt="Logo" 
                         class="h-12 w-auto"
                         onerror="this.style.display='none'">
                    <span class="text-xl font-bold text-gradient">Wisdom Nwakamma</span>
                </div>
                <a href="#about" onclick="toggleMenu()" class="text-lg font-medium hover:text-accent transition-colors">About</a>
                <a href="#services" onclick="toggleMenu()" class="text-lg font-medium hover:text-accent transition-colors">Services</a>
                <a href="#xpert-tech" onclick="toggleMenu()" class="text-lg font-medium hover:text-accent transition-colors">Xpert Tech Hub</a>
                <a href="#ministry" onclick="toggleMenu()" class="text-lg font-medium hover:text-accent transition-colors">Ministry</a>
                <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" onclick="toggleMenu()" class="text-lg font-medium text-red-500 hover:text-red-400"><i class="fab fa-youtube mr-2"></i>YouTube Channel</a>
                <a href="#contact" onclick="toggleMenu()" class="btn-primary px-6 py-3 rounded-full text-center font-semibold mt-4">Contact Me</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-20">
        <div class="absolute inset-0 z-0">
            <div class="absolute top-20 left-10 w-72 h-72 bg-primary/30 rounded-full blur-[100px] animate-float"></div>
            <div class="absolute bottom-20 right-10 w-96 h-96 bg-secondary/20 rounded-full blur-[100px] animate-float" style="animation-delay: 2s;"></div>
            <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full h-full bg-[url('data:image/svg+xml,%3Csvg width=\'60\' height=\'60\' viewBox=\'0 0 60 60\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cg fill=\'none\' fill-rule=\'evenodd\'%3E%3Cg fill=\'%23ffffff\' fill-opacity=\'0.03\'%3E%3Cpath d=\'M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z\'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E')] opacity-20"></div>
        </div>

        <div class="relative z-10 max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-12 items-center">
            <div class="order-2 md:order-1">
                <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full glass mb-6">
                    <span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
                    <span class="text-sm font-medium">Available for Projects</span>
                </div>
                
                <h1 class="hero-title text-5xl md:text-7xl font-serif font-bold leading-tight mb-6">
                    Bridging <span class="text-gradient">Technology</span> & <span class="text-secondary">Faith</span>
                </h1>
                
                <p class="text-lg md:text-xl text-gray-400 mb-8 leading-relaxed max-w-lg">
                    Software Engineering Student at Southern Delta University • Pastor • Youth Life Coach<br>
                    Founder of Xpert Tech Hub & Spirit Revive Community
                </p>
                
                <div class="flex flex-col sm:flex-row gap-4">
                    <a href="#xpert-tech" class="btn-primary px-8 py-4 rounded-full font-semibold text-center flex items-center justify-center gap-2">
                        <i class="fas fa-laptop-code"></i> Tech Services
                    </a>
                    <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" class="btn-youtube px-8 py-4 rounded-full font-semibold text-center flex items-center justify-center gap-2 text-white">
                        <i class="fab fa-youtube"></i> Subscribe on YouTube
                    </a>
                </div>

                <div class="mt-12 flex items-center gap-6 text-gray-400">
                    <a href="mailto:wisdomnwakamma49@gmail.com" class="hover:text-white transition-colors"><i class="fas fa-envelope text-xl"></i></a>
                    <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" class="hover:text-red-500 transition-colors" title="Spirit Revive Community"><i class="fab fa-youtube text-xl"></i></a>
                    <a href="#" class="hover:text-white transition-colors"><i class="fab fa-linkedin text-xl"></i></a>
                    <a href="#" class="hover:text-white transition-colors"><i class="fab fa-github text-xl"></i></a>
                </div>
            </div>

            <div class="order-1 md:order-2 flex justify-center">
                <div class="relative w-80 h-80 md:w-96 md:h-96">
                    <div class="absolute inset-0 bg-gradient-to-br from-primary to-secondary rounded-full opacity-20 blur-2xl animate-pulse-slow"></div>
                    <div class="relative w-full h-full rounded-full overflow-hidden border-4 border-white/10 shadow-2xl">
                        <img src="https://i.imgur.com/des2ZLO.jpg" 
                             alt="Wisdom Nwakamma - Professional Headshot" 
                             class="w-full h-full object-cover profile-image"
                             onerror="this.src='https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=800&h=800&fit=crop'">
                    </div>
                    <div class="absolute -top-4 -right-4 bg-dark glass px-4 py-2 rounded-full shadow-lg animate-float">
                        <i class="fas fa-code text-primary mr-2"></i>
                        <span class="text-sm font-semibold">Software Engineer</span>
                    </div>
                    <div class="absolute -bottom-4 -left-4 bg-dark glass px-4 py-2 rounded-full shadow-lg animate-float" style="animation-delay: 1s;">
                        <i class="fas fa-church text-secondary mr-2"></i>
                        <span class="text-sm font-semibold">Pastor</span>
                    </div>
                </div>
            </div>
        </div>

        <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
            <a href="#about" class="text-gray-400 hover:text-white transition-colors">
                <i class="fas fa-chevron-down text-2xl"></i>
            </a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-32 relative">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="space-y-6">
                    <div class="flex items-center gap-4 mb-6">
                        <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                             alt="Logo" 
                             class="logo-medium glow-effect"
                             onerror="this.style.display='none'">
                        <div class="w-20 h-1 bg-gradient-to-r from-primary to-secondary rounded-full"></div>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-serif font-bold">About Me</h2>
                    
                    <p class="text-gray-400 text-lg leading-relaxed">
                        I am a Software Engineering student at <strong class="text-white">Southern Delta University</strong>, with a deep passion for technology, innovation, and problem-solving.
                    </p>
                    
                    <p class="text-gray-400 text-lg leading-relaxed">
                        Beyond the screen, I am a <strong class="text-secondary">Christian leader, youth life coach, and pastor</strong>, dedicated to impacting lives through faith, leadership, and mentorship. I believe in the power of combining technical excellence with spiritual guidance to create holistic transformation.
                    </p>
                    
                    <p class="text-gray-400 text-lg leading-relaxed">
                        Through my YouTube channel <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" class="text-red-500 hover:text-red-400 underline">Spirit Revive Community</a>, I share messages that inspire spiritual growth and transformation.
                    </p>

                    <div class="grid grid-cols-2 gap-6 pt-6">
                        <div class="glass p-6 rounded-2xl text-center">
                            <div class="text-3xl font-bold text-primary counter" data-target="50">0</div>
                            <div class="text-sm text-gray-400 mt-2">Tech Projects</div>
                        </div>
                        <div class="glass p-6 rounded-2xl text-center">
                            <div class="text-3xl font-bold text-secondary counter" data-target="100">0</div>
                            <div class="text-sm text-gray-400 mt-2">Lives Impacted</div>
                        </div>
                    </div>
                </div>

                <div class="space-y-8">
                    <h3 class="text-2xl font-serif font-semibold mb-6">Technical Skills</h3>
                    
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">Web Development (HTML, CSS, WordPress)</span>
                                <span class="text-primary">90%</span>
                            </div>
                            <div class="h-2 bg-gray-700 rounded-full overflow-hidden">
                                <div class="skill-bar h-full bg-gradient-to-r from-primary to-blue-400 rounded-full" data-width="90%"></div>
                            </div>
                        </div>

                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">Python Programming</span>
                                <span class="text-primary">85%</span>
                            </div>
                            <div class="h-2 bg-gray-700 rounded-full overflow-hidden">
                                <div class="skill-bar h-full bg-gradient-to-r from-primary to-blue-400 rounded-full" data-width="85%"></div>
                            </div>
                        </div>

                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">Computer Hardware Repair</span>
                                <span class="text-secondary">95%</span>
                            </div>
                            <div class="h-2 bg-gray-700 rounded-full overflow-hidden">
                                <div class="skill-bar h-full bg-gradient-to-r from-secondary to-red-400 rounded-full" data-width="95%"></div>
                            </div>
                        </div>

                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">System Troubleshooting</span>
                                <span class="text-secondary">92%</span>
                            </div>
                            <div class="h-2 bg-gray-700 rounded-full overflow-hidden">
                                <div class="skill-bar h-full bg-gradient-to-r from-secondary to-red-400 rounded-full" data-width="92%"></div>
                            </div>
                        </div>

                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">Leadership & Mentorship</span>
                                <span class="text-accent">88%</span>
                            </div>
                            <div class="h-2 bg-gray-700 rounded-full overflow-hidden">
                                <div class="skill-bar h-full bg-gradient-to-r from-amber-500 to-yellow-400 rounded-full" data-width="88%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-32 bg-dark-light relative overflow-hidden">
        <div class="absolute top-0 right-0 w-1/3 h-full bg-gradient-to-l from-primary/5 to-transparent"></div>
        
        <div class="max-w-7xl mx-auto px-6 relative z-10">
            <div class="text-center mb-16">
                <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                     alt="Logo" 
                     class="logo-small mx-auto mb-6 opacity-80 glow-effect"
                     onerror="this.style.display='none'">
                <h2 class="text-4xl md:text-5xl font-serif font-bold mb-4">What I Offer</h2>
                <p class="text-gray-400 max-w-2xl mx-auto">Combining technical expertise with leadership coaching to provide comprehensive solutions</p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <div class="service-card glass p-8 rounded-3xl border border-white/5">
                    <div class="w-14 h-14 bg-primary/20 rounded-2xl flex items-center justify-center mb-6 text-primary text-2xl">
                        <i class="fas fa-laptop"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Web Development</h3>
                    <p class="text-gray-400 mb-4">Custom websites using HTML, CSS, and WordPress. From portfolio sites to business platforms.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li><i class="fas fa-check text-primary mr-2"></i>Responsive Design</li>
                        <li><i class="fas fa-check text-primary mr-2"></i>SEO Optimization</li>
                        <li><i class="fas fa-check text-primary mr-2"></i>Maintenance & Support</li>
                    </ul>
                </div>

                <div class="service-card glass p-8 rounded-3xl border border-white/5">
                    <div class="w-14 h-14 bg-secondary/20 rounded-2xl flex items-center justify-center mb-6 text-secondary text-2xl">
                        <i class="fas fa-tools"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Computer Repair</h3>
                    <p class="text-gray-400 mb-4">Hardware diagnostics, system upgrades, virus removal, and performance optimization.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li><i class="fas fa-check text-secondary mr-2"></i>Hardware Diagnostics</li>
                        <li><i class="fas fa-check text-secondary mr-2"></i>OS Installation</li>
                        <li><i class="fas fa-check text-secondary mr-2"></i>Data Recovery</li>
                    </ul>
                </div>

                <div class="service-card glass p-8 rounded-3xl border border-white/5">
                    <div class="w-14 h-14 bg-accent/20 rounded-2xl flex items-center justify-center mb-6 text-accent text-2xl">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Youth Coaching</h3>
                    <p class="text-gray-400 mb-4">Leadership development, career guidance, and spiritual mentorship for young people.</p>
                    <ul class="text-sm text-gray-500 space-y-2">
                        <li><i class="fas fa-check text-accent mr-2"></i>1-on-1 Mentorship</li>
                        <li><i class="fas fa-check text-accent mr-2"></i>Career Guidance</li>
                        <li><i class="fas fa-check text-accent mr-2"></i>Spiritual Growth</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Xpert Tech Hub Section -->
    <section id="xpert-tech" class="py-32">
        <div class="max-w-7xl mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="order-2 md:order-1">
                    <div class="inline-flex items-center gap-3 px-4 py-2 rounded-full bg-primary/10 text-primary text-sm font-semibold mb-6">
                        <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                             alt="Logo" 
                             class="logo-badge"
                             onerror="this.style.display='none'">
                        <span>Business Venture</span>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-serif font-bold mb-6">Xpert Tech Hub</h2>
                    <p class="text-gray-400 text-lg mb-6 leading-relaxed">
                        Founded with a vision to make technology accessible and affordable, Xpert Tech Hub provides comprehensive digital solutions for individuals and businesses in Nigeria.
                    </p>
                    
                    <div class="space-y-4 mb-8">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-primary/20 flex items-center justify-center flex-shrink-0 text-primary">
                                <i class="fas fa-laptop-medical"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Laptop Sales & Repairs</h4>
                                <p class="text-gray-400 text-sm">Quality laptops at competitive prices with guaranteed repair services</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-primary/20 flex items-center justify-center flex-shrink-0 text-primary">
                                <i class="fas fa-cogs"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">System Maintenance</h4>
                                <p class="text-gray-400 text-sm">Regular maintenance to keep your devices running optimally</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-full bg-primary/20 flex items-center justify-center flex-shrink-0 text-primary">
                                <i class="fas fa-shield-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Digital Security</h4>
                                <p class="text-gray-400 text-sm">Virus removal and security solutions to protect your data</p>
                            </div>
                        </div>
                    </div>

                    <a href="#contact" class="btn-primary px-8 py-4 rounded-full font-semibold inline-flex items-center gap-2">
                        Get a Quote <i class="fas fa-arrow-right"></i>
                    </a>
                </div>

                <div class="order-1 md:order-2 grid grid-cols-2 gap-4">
                    <div class="space-y-4 mt-8">
                        <div class="project-card rounded-2xl aspect-[3/4]">
                            <img src="https://images.unsplash.com/photo-1597872200969-2b65d56bd16b?w=600&h=800&fit=crop" alt="Tech Repair" class="w-full h-full object-cover rounded-2xl">
                            <div class="project-overlay absolute inset-0 rounded-2xl flex items-end p-6">
                                <span class="text-white font-semibold">Hardware Repair</span>
                            </div>
                        </div>
                    </div>
                    <div class="space-y-4">
                        <div class="project-card rounded-2xl aspect-[3/4]">
                            <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=600&h=800&fit=crop" alt="Laptop Sales" class="w-full h-full object-cover rounded-2xl">
                            <div class="project-overlay absolute inset-0 rounded-2xl flex items-end p-6">
                                <span class="text-white font-semibold">Laptop Sales</span>
                            </div>
                        </div>
                        <div class="project-card rounded-2xl aspect-square">
                            <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?w=600&h=600&fit=crop" alt="Consultation" class="w-full h-full object-cover rounded-2xl">
                            <div class="project-overlay absolute inset-0 rounded-2xl flex items-end p-6">
                                <span class="text-white font-semibold">Tech Consultation</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Ministry Section -->
    <section id="ministry" class="py-32 bg-gradient-to-b from-dark-light to-dark relative overflow-hidden">
        <div class="absolute top-0 left-0 w-full h-full bg-[url('data:image/svg+xml,%3Csvg width=\'100\' height=\'100\' viewBox=\'0 0 100 100\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cpath d=\'M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM6 4V0H4v4H0v2h4v4h2V6h4V4H6zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM16 70c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm40-14c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z\' fill=\'%23dc2626\' fill-opacity=\'0.03\' fill-rule=\'evenodd\'/%3E%3C/svg%3E')] opacity-30"></div>

        <div class="max-w-7xl mx-auto px-6 relative z-10">
            <div class="text-center mb-16">
                <div class="inline-block px-4 py-2 rounded-full bg-secondary/10 text-secondary text-sm font-semibold mb-6">
                    <i class="fas fa-cross mr-2"></i>Spiritual Leadership
                </div>
                <h2 class="text-4xl md:text-5xl font-serif font-bold mb-4">Spirit Revive Community</h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">Inspiring spiritual growth and transformation through faith-based content and mentorship</p>
            </div>

            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="relative rounded-3xl overflow-hidden aspect-video group cursor-pointer" onclick="window.open('https://www.youtube.com/@wisdomnwakamma', '_blank')">
                    <img src="https://images.unsplash.com/photo-1507692049790-de58290a4334?w=1200&h=675&fit=crop" alt="YouTube Channel" class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-110">
                    <div class="absolute inset-0 bg-dark/60 flex items-center justify-center group-hover:bg-dark/40 transition-colors">
                        <div class="w-20 h-20 bg-red-600 rounded-full flex items-center justify-center text-white text-3xl shadow-lg transform group-hover:scale-110 transition-transform">
                            <i class="fab fa-youtube"></i>
                        </div>
                    </div>
                    <div class="absolute bottom-0 left-0 right-0 p-6 bg-gradient-to-t from-dark to-transparent">
                        <h3 class="text-2xl font-bold mb-2">Watch on YouTube</h3>
                        <p class="text-gray-300">Subscribe for weekly messages on faith, leadership, and personal growth</p>
                    </div>
                </div>

                <div class="space-y-8">
                    <div class="space-y-6">
                        <div class="flex gap-4 items-start">
                            <div class="w-12 h-12 rounded-full bg-secondary/20 flex items-center justify-center flex-shrink-0 text-secondary">
                                <i class="fas fa-book-open"></i>
                            </div>
                            <div>
                                <h4 class="text-xl font-bold mb-2">Biblical Teaching</h4>
                                <p class="text-gray-400">Deep, practical teachings from Scripture applied to modern life challenges and opportunities.</p>
                            </div>
                        </div>

                        <div class="flex gap-4 items-start">
                            <div class="w-12 h-12 rounded-full bg-secondary/20 flex items-center justify-center flex-shrink-0 text-secondary">
                                <i class="fas fa-user-graduate"></i>
                            </div>
                            <div>
                                <h4 class="text-xl font-bold mb-2">Youth Mentorship</h4>
                                <p class="text-gray-400">Guiding young people to discover their purpose, develop leadership skills, and grow in faith.</p>
                            </div>
                        </div>

                        <div class="flex gap-4 items-start">
                            <div class="w-12 h-12 rounded-full bg-secondary/20 flex items-center justify-center flex-shrink-0 text-secondary">
                                <i class="fas fa-heart"></i>
                            </div>
                            <div>
                                <h4 class="text-xl font-bold mb-2">Life Transformation</h4>
                                <p class="text-gray-400">Creating content that inspires positive change in relationships, career, and spiritual walk.</p>
                            </div>
                        </div>
                    </div>

                    <div class="glass p-6 rounded-2xl border border-secondary/20">
                        <h4 class="font-bold text-lg mb-3 flex items-center gap-2">
                            <i class="fas fa-book text-accent"></i> Upcoming Book Projects
                        </h4>
                        <p class="text-gray-400 text-sm mb-4">Currently writing books on:</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-accent/10 text-accent rounded-full text-sm">Financial Wisdom</span>
                            <span class="px-3 py-1 bg-accent/10 text-accent rounded-full text-sm">Personal Growth</span>
                            <span class="px-3 py-1 bg-accent/10 text-accent rounded-full text-sm">Leadership</span>
                        </div>
                    </div>

                    <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" class="btn-youtube px-8 py-4 rounded-full font-semibold inline-flex items-center gap-2 w-full justify-center text-white">
                        <i class="fab fa-youtube"></i> Visit @wisdomnwakamma
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-32 relative">
        <div class="max-w-4xl mx-auto px-6">
            <div class="text-center mb-16">
                <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                     alt="Logo" 
                     class="logo-large mx-auto mb-6 glow-effect"
                     onerror="this.style.display='none'">
                <h2 class="text-4xl md:text-5xl font-serif font-bold mb-4">Let's Work Together</h2>
                <p class="text-gray-400">Whether you need tech solutions or spiritual guidance, I'm here to help</p>
            </div>

            <div class="glass rounded-3xl p-8 md:p-12 border border-white/10">
                <form class="space-y-6" onsubmit="event.preventDefault(); alert('Thank you for your message! I will get back to you soon.');">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm font-medium mb-2">Name</label>
                            <input type="text" class="w-full px-4 py-3 bg-dark/50 border border-white/10 rounded-xl focus:outline-none focus:border-primary transition-colors" placeholder="Your name" required>
                        </div>
                        <div>
                            <label class="block text-sm font-medium mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-3 bg-dark/50 border border-white/10 rounded-xl focus:outline-none focus:border-primary transition-colors" placeholder="your@email.com" required>
                        </div>
                    </div>

                    <div>
                        <label class="block text-sm font-medium mb-2">Service Type</label>
                        <select class="w-full px-4 py-3 bg-dark/50 border border-white/10 rounded-xl focus:outline-none focus:border-primary transition-colors text-gray-400">
                            <option value="">Select a service...</option>
                            <option value="web">Web Development</option>
                            <option value="repair">Computer Repair</option>
                            <option value="coaching">Youth Coaching</option>
                            <option value="ministry">Ministry/Counseling</option>
                            <option value="other">Other</option>
                        </select>
                    </div>

                    <div>
                        <label class="block text-sm font-medium mb-2">Message</label>
                        <textarea rows="4" class="w-full px-4 py-3 bg-dark/50 border border-white/10 rounded-xl focus:outline-none focus:border-primary transition-colors resize-none" placeholder="Tell me about your project or inquiry..." required></textarea>
                    </div>

                    <button type="submit" class="w-full btn-primary py-4 rounded-xl font-semibold text-lg flex items-center justify-center gap-2">
                        Send Message <i class="fas fa-paper-plane"></i>
                    </button>
                </form>

                <div class="mt-12 pt-8 border-t border-white/10 grid md:grid-cols-3 gap-6 text-center">
                    <div>
                        <i class="fas fa-envelope text-primary text-2xl mb-3"></i>
                        <p class="text-sm text-gray-400">wisdomnwakamma49@gmail.com</p>
                    </div>
                    <div>
                        <i class="fas fa-map-marker-alt text-secondary text-2xl mb-3"></i>
                        <p class="text-sm text-gray-400">Delta State, Nigeria</p>
                    </div>
                    <div>
                        <i class="fas fa-university text-accent text-2xl mb-3"></i>
                        <p class="text-sm text-gray-400">Southern Delta University</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-white/10 py-12 bg-dark-light">
        <div class="max-w-7xl mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6">
                <div class="flex items-center gap-3">
                    <img src="https://res.cloudinary.com/dnb67qpkt/image/upload/v1774461552/Photoroom-20260325_185650102_ntrol9.png" 
                         alt="Logo" 
                         class="h-12 w-auto glow-effect"
                         onerror="this.style.display='none'">
                    <span class="text-2xl font-serif font-bold text-gradient">Wisdom Nwakamma</span>
                </div>
                
                <div class="flex gap-6">
                    <a href="mailto:wisdomnwakamma49@gmail.com" class="w-10 h-10 rounded-full glass flex items-center justify-center hover:bg-primary hover:border-primary transition-all">
                        <i class="fas fa-envelope"></i>
                    </a>
                    <a href="https://www.youtube.com/@wisdomnwakamma" target="_blank" class="w-10 h-10 rounded-full glass flex items-center justify-center hover:bg-red-600 hover:border-red-600 hover:text-white transition-all" title="Spirit Revive Community">
                        <i class="fab fa-youtube"></i>
                    </a>
                    <a href="#" class="w-10 h-10 rounded-full glass flex items-center justify-center hover:bg-primary hover:border-primary transition-all">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="#" class="w-10 h-10 rounded-full glass flex items-center justify-center hover:bg-white hover:text-dark transition-all">
                        <i class="fab fa-github"></i>
                    </a>
                </div>

                <div class="text-gray-500 text-sm text-center md:text-right">
                    <p>&copy; 2024 Wisdom Nwakamma. All rights reserved.</p>
                    <p class="mt-1">Software Engineering Student at Southern Delta University</p>
                    <p class="mt-1 text-red-500"><i class="fab fa-youtube mr-1"></i> @wisdomnwakamma</p>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Register GSAP
        gsap.registerPlugin(ScrollTrigger);

        // Mobile Menu Toggle
        function toggleMenu() {
            const menu = document.getElementById('mobileMenu');
            menu.classList.toggle('hidden');
        }

        // Navbar scroll effect
        window.addEventListener('scroll', () => {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('bg-dark/90', 'backdrop-blur-lg', 'shadow-lg');
            } else {
                navbar.classList.remove('bg-dark/90', 'backdrop-blur-lg', 'shadow-lg');
            }
        });

        // Hero animations
        gsap.from('.hero-title', {
            y: 50,
            opacity: 0,
            duration: 1.2,
            ease: "power4.out"
        });

        // Skill bars animation
        const skillBars = document.querySelectorAll('.skill-bar');
        skillBars.forEach(bar => {
            const width = bar.getAttribute('data-width');
            gsap.to(bar, {
                width: width,
                duration: 1.5,
                ease: "power2.out",
                scrollTrigger: {
                    trigger: bar,
                    start: "top 80%",
                    toggleActions: "play none none reverse"
                }
            });
        });

        // Counter animation
        const counters = document.querySelectorAll('.counter');
        counters.forEach(counter => {
            const target = parseInt(counter.getAttribute('data-target'));
            gsap.to(counter, {
                innerHTML: target,
                duration: 2,
                snap: { innerHTML: 1 },
                ease: "power2.out",
                scrollTrigger: {
                    trigger: counter,
                    start: "top 85%",
                    toggleActions: "play none none reverse"
                }
            });
        });

        // Service cards animation
        gsap.utils.toArray('.service-card').forEach((card, i) => {
            gsap.from(card, {
                y: 50,
                opacity: 0,
                duration: 0.8,
                delay: i * 0.1,
                ease: "power3.out",
                scrollTrigger: {
                    trigger: card,
                    start: "top 85%",
                    toggleActions: "play none none reverse"
                }
            });
        });

        // Smooth scroll for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Parallax effect for hero background
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallax = document.querySelectorAll('.animate-float');
            parallax.forEach((el, index) => {
                const speed = 0.5 + (index * 0.1);
                el.style.transform = `translateY(${scrolled * speed}px)`;
            });
        });
    </script>
</body>
</html>
