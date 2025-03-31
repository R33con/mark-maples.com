<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mark Maples - Product Leader Portfolio</title>
    <meta property="og:title" content="Mark Maples - Product Leader Portfolio">
    <meta property="og:description" content="Product Leader with Strategic Programs & Operations Experience">
    <meta property="og:image" content="https://cdn.simulationtheory.ai/gasset/?asset=img&prompt=modern minimalist product manager logo&w=200&h=200&style=professional">
    <meta property="og:type" content="website">
    <link rel="icon" href="https://cdn.simulationtheory.ai/gasset/?asset=img&prompt=minimalist product manager icon&w=32&h=32&style=professional">
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="/chat/cdn/animate.min.css" rel="stylesheet">
    <script src="/chat/cdn/papaparse.min.js"></script>
    <link href="/chat/cdn/all.min.css" rel="stylesheet">
    <script src="/chat/cdn/all.min.js" crossorigin></script>
    <style>
        @font-face {
            font-family: 'Font Awesome 6 Free';
            font-path: '/chat/webfonts/fa-regular-400';
            src: url('/chat/webfonts/fa-regular-400.woff2') format('woff2'),
                url('/chat/webfonts/fa-regular-400.ttf') format('truetype');
        }

        @font-face {
            font-family: 'Font Awesome 6 Free';
            font-path: '/chat/webfonts/fa-solid-900';
            src: url('/chat/webfonts/fa-solid-900.woff2') format('woff2'),
                url('/chat/webfonts/fa-solid-900.ttf') format('truetype');
        }

        @font-face {
            font-family: 'Font Awesome 6 Brands';
            font-path: '/chat/webfonts/fa-brands-400';
            src: url('/chat/webfonts/fa-brands-400.woff2') format('woff2'),
                url('/chat/webfonts/fa-brands-400.ttf') format('truetype');
        }

        html {
            scroll-behavior: smooth;
        }

        /* Updated Color Scheme */
        :root {
            --primary-color: #00022b; /* Deep Navy Blue */
            --primary-dark: #010e54;
            --primary-light: #4fa5d8;
            --accent-color: #0855b1; /* Medium Blue */
            --bg-light: #daeaf7; /* Light Blue Background */
            --text-light: #ffffff;
            --text-dark: #212529;
        }

        .bg-primary {
            background-color: var(--primary-color);
        }

        .bg-primary-dark {
            background-color: var(--primary-dark);
        }

        .bg-primary-light {
            background-color: var(--primary-light);
        }
        
        .bg-accent {
            background-color: var(--accent-color);
        }
        
        .bg-light-blue {
            background-color: var(--bg-light);
        }

        .text-primary {
            color: var(--primary-color);
        }

        .text-accent {
            color: var(--accent-color);
        }

        .border-primary {
            border-color: var(--primary-color);
        }

        .hover-bg-primary-dark:hover {
            background-color: var(--primary-dark);
        }

        .profile-header {
            text-align: left;
        }

        .name {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .tagline {
            font-size: 1.75rem;
            font-weight: 500;
            margin-bottom: 1rem;
        }

        .current-role {
            font-size: 1.25rem;
        }
        
        /* Animation classes */
        .hidden-element {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        
        .visible {
            opacity: 1;
            transform: translateY(0);
        }

        .company-logo {
            width: 120px;
            height: 120px;
            object-fit: contain;
            border-radius: 50%;
            box-shadow: 0 10px 25px rgba(0, 2, 43, 0.2);
            padding: 10px;
            transition: all 0.3s ease;
            margin: 0 auto;
        }
        
        .logo-container {
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .logo-container:hover .company-logo {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 2, 43, 0.3);
        }

        /* Amazon logo - dark blue background */
        .amazon-logo {
            background-color: #00022b;
        }
        
        /* Uber and Deloitte logos - black background */
        .uber-logo, .deloitte-logo {
            background-color: #000000;
        }

        .work-item {
            transition: all 0.3s ease;
            opacity: 0;
            transform: translateY(30px);
        }

        .work-item.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .work-item:hover {
            transform: translateY(-5px);
        }
        
        /* Text animation */
        .text-reveal {
            overflow: hidden;
            position: relative;
        }
        
        .text-reveal-content {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 1s ease, transform 1s ease;
        }
        
        .text-reveal.visible .text-reveal-content {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Image fade in */
        .image-fade {
            opacity: 0;
            transition: opacity 1.2s ease-in-out;
        }
        
        .image-fade.visible {
            opacity: 1;
        }
        
        /* Staggered animation for work items */
        .work-item:nth-child(1) {
            transition-delay: 0.1s;
        }
        
        .work-item:nth-child(2) {
            transition-delay: 0.3s;
        }
        
        .work-item:nth-child(3) {
            transition-delay: 0.5s;
        }
        
        /* Common styles for all logo circles */
        .logo-circle {
            width: 120px;
            height: 120px;
            border-radius: 70%;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0, 2, 43, 0.2);
            transition: all 0.3s ease;
            margin: 0 auto;
        }
        
        .logo-circle:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 2, 43, 0.3);
        }
        




        /* Amazon Logo */
        .amazon-logo-circle {
            background-color: #00022b;
        }





        .amazon-logo-circle img {
            width: 196%;
            height: auto;
            object-fit: contain;
            transform: scale(1.485) translateX(-2%);
        }
        
        
        
        
        
        
        
        
        
        /* Deloitte Logo */
        .deloitte-logo-circle {
            background-color: #000000;
        }
        .deloitte-logo-circle img {
            width: 85%;
            height: auto;
        }
        
        /* Uber Logo */
        .uber-logo-circle {
            background-color: #000000;
        }
        .uber-logo-circle img {
            width: 85%;
            height: auto;
        }
        
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#00022b',
                        'primary-dark': '#010e54',
                        'primary-light': '#4fa5d8',
                        accent: '#0855b1',
                        'bg-light': '#daeaf7',
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-white text-gray-800">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white shadow-md z-50">
        <div class="container mx-auto px-6 py-3 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-gray-800">
                <span class="flex items-center">
                    <img id="logo" src="https://cdn.simulationtheory.ai/gasset/?asset=img&prompt=modern minimalist product manager logo&w=40&h=40&style=professional" alt="Logo" class="mr-2 rounded-full">
                    <span>Mark Maples</span>
                </span>
            </a>
            <div class="hidden md:flex space-x-8">
                <a href="#about" class="hover:text-primary transition-colors">About</a>
                <a href="#work-history" class="hover:text-primary transition-colors">Work History</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden focus:outline-none">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white w-full">
            <div class="container mx-auto px-6 py-3 flex flex-col space-y-4">
                <a href="#about" class="hover:text-primary transition-colors">About</a>
                <a href="#work-history" class="hover:text-primary transition-colors">Work History</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header style="background-color: #00022b;" class="min-h-screen flex items-center">
        <div class="container mx-auto px-6 py-24 md:py-32">
            <div class="profile-header text-left">
                <h1 class="name text-white">Mark Maples</h1>
                <h2 class="tagline text-white">Product leader with strategic programs and operations experience</h2>
                <p class="current-role text-white">Currently helping customers navigate their purchase history and order details at amazon</p>
            </div>
        </div>
    </header>
    
    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/3 mb-12 md:mb-0 image-fade">
                    <img id="profile-image" src="https://res.cloudinary.com/dimqqmfx6/image/upload/v1741670272/u0311051748_profile2_uwysoa.png" alt="Mark Maples" class="rounded-full shadow-xl mx-auto" style="max-width: 300px;">
                </div>
                <div class="md:w-2/3 md:pl-12 text-reveal">
                    <div class="text-reveal-content">

                        <p class="text-lg mb-8">
                            Hi, I'm Mark. I'm a Product Manager based in San Francisco. 

                            I turn customer problems into simple product solutions that work. I pull from my management consulting and strategic ops experiences to move quickly and deliver value.
                        </p>
        
                                            <div class="flex flex-wrap gap-4">
                                                <!-- LinkedIn link removed from here -->
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </section>

                        <!-- Work History Section -->
                        <section id="work-history" class="py-20" style="background-color: #daeaf7;">
                            <div class="container mx-auto px-6">
                                <h2 class="text-3xl font-bold mb-12 text-center" style="color: #00022b;">Select Work History</h2>
                                <div class="space-y-16" id="work-history-container">
                                    <!-- Amazon -->
                                    <div class="work-item">
                                        <div class="flex flex-col md:flex-row items-center">
                                            <div class="md:w-1/4 mb-6 md:mb-0">
                                                <div class="logo-container">
                                                     <div class="logo-circle amazon-logo-circle">
                                                        <img src="https://res.cloudinary.com/dimqqmfx6/image/upload/v1741666625/u0311041703_amazon5_wpzp44.png" alt="Amazon Logo">
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="md:w-3/4">
                                                <h3 class="text-xl font-bold mb-2" style="color: #00022b;">Amazon</h3>
                                                <p class="text-gray-600 mb-4">
                                                    I own the Your Orders and Order Details post-purchase pages at Amazon. I help reimagine how millions of people stay informed, take action, and feel confident when receiving and managing their orders. I simplify complexity at scale, and turn everyday interactions into moments of clarity, trust, and delight.
                                                </p>
                                            </div>
                                        </div>
                                    </div>
        
                                    <!-- Uber -->
                                    <div class="work-item">
                                        <div class="flex flex-col md:flex-row items-center">
                                            <div class="md:w-1/4 mb-6 md:mb-0">
                                                <div class="logo-container">
                                                    <div class="logo-circle uber-logo-circle">
                                                        <img src="https://res.cloudinary.com/dimqqmfx6/image/upload/v1741398623/u0308014708_uberlogo_v5gocx.png" alt="Uber Logo">
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="md:w-3/4">
                                                <h3 class="text-xl font-bold mb-2" style="color: #00022b;">Uber</h3>
                                                <p class="text-gray-600 mb-4">
                                                    Led customer insights and support strategy for Uber’s innovation businesses (U4B, Freight, JUMP); influenced product roadmaps with data-driven CX insights and launched global support programs for Uber’s largest enterprise clients.
                                                </p>
                                            </div>
                                        </div>
                                    </div>
        
                                    <!-- Deloitte -->
                                    <div class="work-item">
                                        <div class="flex flex-col md:flex-row items-center">
                                            <div class="md:w-1/4 mb-6 md:mb-0">
                                                <div class="logo-container">
                                                    <div class="logo-circle deloitte-logo-circle">
                                                        <img src="https://res.cloudinary.com/dimqqmfx6/image/upload/v1741398623/u0308014630_deloitte2_lhje0s.png" alt="Deloitte Logo">
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="md:w-3/4">
                                                <h3 class="text-xl font-bold mb-2" style="color: #00022b;">Deloitte</h3>
                                                <p class="text-gray-600 mb-4">
                                                   Drove strategy and process transformation for large health insurers and public programs; launched agile frameworks, streamlined compliance, and enabled tech investments impacting 750K+ members.
                                                </p>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </section>

                        <!-- Footer -->
                        <footer style="background-color: #00022b;" class="text-white py-8">
                            <div class="container mx-auto px-6">
                                <div class="flex flex-col md:flex-row justify-between items-center">
                                    <div class="mb-6 md:mb-0">
                                        <a href="#" class="text-xl font-bold">Mark Maples</a>
                                        <div class="mt-2 text-gray-300">
                                            <a href="https://www.linkedin.com/in/mark-maples-5b9bb813/" target="_blank" class="flex items-center hover:text-primary-light">
                                                <i class="fab fa-linkedin mr-2"></i> LinkedIn
                                            </a>
                                        </div>
                                    </div>
                                    <div class="flex flex-col md:flex-row md:space-x-8">
                                        <a href="#about" class="hover:text-primary-light mb-2 md:mb-0">About</a>
                                        <a href="#work-history" class="hover:text-primary-light mb-2 md:mb-0">Work History</a>
                                    </div>
                                </div>
                                <hr class="border-gray-700 my-4">
                                <div class="text-center">
                                    <p>© <span id="current-year"></span> Mark Maples. All rights reserved.</p>
                                </div>
                            </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('current-year').textContent = new Date().getFullYear();
            
            // Mobile menu toggle
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            
            mobileMenuButton.addEventListener('click', function() {
                mobileMenu.classList.toggle('hidden');
            });
            
            // Close mobile menu when clicking a link
            const mobileLinks = mobileMenu.querySelectorAll('a');
            mobileLinks.forEach(link => {
                link.addEventListener('click', function() {
                    mobileMenu.classList.add('hidden');
                });
            });
            
            // Handle image loading errors
            const images = document.querySelectorAll('img');
            images.forEach(img => {
                img.onerror = function() {
                    this.src = 'https://cdn.simulationtheory.ai/gasset/?asset=img&prompt=abstract placeholder&w=300&h=300&style=professional';
                };
            });
            
            // Scroll animation for about section
            const profileImage = document.querySelector('.image-fade');
            const textReveal = document.querySelector('.text-reveal');
            
            const aboutObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, {
                threshold: 0.2,
                rootMargin: "0px 0px -50px 0px"
            });
            
            aboutObserver.observe(profileImage);
            aboutObserver.observe(textReveal);
            
            // Scroll animation for work history items
            const workItems = document.querySelectorAll('.work-item');
            
            const workObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, {
                threshold: 0.1,
                rootMargin: "0px 0px -50px 0px"
            });
            
            workItems.forEach(item => workObserver.observe(item));
        });
    </script>
</body>
</html>