<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manish Gupta | Full-Stack Developer Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* Custom styles for smooth scrolling and clean look */
        :root {
            scroll-behavior: smooth;
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: #121212; /* Dark background */
            color: #E0E0E0; /* Light text */
        }
        .section-heading {
            position: relative;
            display: inline-block;
            padding-bottom: 0.25rem;
            margin-bottom: 2rem;
            font-size: 2.25rem; /* text-4xl */
            font-weight: 800; /* font-extrabold */
            color: #61DAFB; /* React blue/cyan for emphasis */
        }
        .section-heading::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50%;
            height: 4px;
            background-color: #2563EB; /* Deep blue underline */
            border-radius: 2px;
        }
        .card {
            background-color: #1E1E1E;
            transition: all 0.3s ease;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.2), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.4), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
            border-color: #61DAFB;
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 shadow-lg backdrop-blur-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center">
                    <a href="#" class="text-2xl font-extrabold text-[#61DAFB] tracking-wider">Manish G.</a>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-4">
                        <a href="#about" class="text-gray-300 hover:bg-gray-700 px-3 py-2 rounded-md text-sm font-medium transition duration-150">About</a>
                        <a href="#skills" class="text-gray-300 hover:bg-gray-700 px-3 py-2 rounded-md text-sm font-medium transition duration-150">Skills</a>
                        <a href="#projects" class="text-gray-300 hover:bg-gray-700 px-3 py-2 rounded-md text-sm font-medium transition duration-150">Projects</a>
                        <a href="#contact" class="text-gray-300 hover:bg-gray-700 px-3 py-2 rounded-md text-sm font-medium transition duration-150">Contact</a>
                    </div>
                </div>
                <div class="-mr-2 flex md:hidden">
                    <button id="mobile-menu-button" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none transition duration-150" aria-controls="mobile-menu" aria-expanded="false">
                        <!-- Menu Icon (lucide-menu) -->
                        <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                        <!-- Close Icon (lucide-x) -->
                        <svg class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile menu, show/hide based on menu state. -->
        <div class="md:hidden hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#about" class="text-gray-300 hover:bg-gray-700 block px-3 py-2 rounded-md text-base font-medium transition duration-150">About</a>
                <a href="#skills" class="text-gray-300 hover:bg-gray-700 block px-3 py-2 rounded-md text-base font-medium transition duration-150">Skills</a>
                <a href="#projects" class="text-gray-300 hover:bg-gray-700 block px-3 py-2 rounded-md text-base font-medium transition duration-150">Projects</a>
                <a href="#contact" class="text-gray-300 hover:bg-gray-700 block px-3 py-2 rounded-md text-base font-medium transition duration-150">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="about" class="bg-gray-900 pt-20 pb-24 sm:py-32">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center">
                <p class="text-xl font-medium text-gray-400 mb-3">Hello, I'm</p>
                <h1 class="text-6xl sm:text-7xl lg:text-8xl font-extrabold text-white mb-6">Manish Gupta</h1>
                <p class="text-2xl sm:text-3xl font-light text-[#61DAFB] mb-10">
                    Full-Stack Developer | Building Robust & Scalable Web Solutions
                </p>
                <div class="space-x-4">
                    <a href="#projects" class="inline-block px-8 py-3 text-lg font-semibold rounded-lg bg-indigo-600 hover:bg-indigo-700 text-white transition duration-200 shadow-md">
                        View Projects
                    </a>
                    <a href="#contact" class="inline-block px-8 py-3 text-lg font-semibold rounded-lg border border-gray-600 hover:border-[#61DAFB] text-gray-300 hover:text-white transition duration-200">
                        Get In Touch
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- Skills Section -->
    <section id="skills" class="py-16 sm:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="section-heading">Tech Stack & Expertise</h2>
            <p class="text-lg text-gray-400 mb-10">I utilize a diverse set of modern tools to deliver high-performance applications.</p>

            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
                <!-- Skill Card: Front-End -->
                <div class="card p-6 rounded-xl border border-transparent">
                    <h3 class="text-xl font-bold text-[#61DAFB] mb-3">Front-End</h3>
                    <ul class="space-y-2 text-gray-300">
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> React & Next.js</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> HTML5 & CSS3</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Tailwind CSS & Responsive Design</li>
                    </ul>
                </div>

                <!-- Skill Card: Back-End -->
                <div class="card p-6 rounded-xl border border-transparent">
                    <h3 class="text-xl font-bold text-green-500 mb-3">Back-End</h3>
                    <ul class="space-y-2 text-gray-300">
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Python (Django/Flask)</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Node.js & Express</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> RESTful API Development</li>
                    </ul>
                </div>

                <!-- Skill Card: Databases -->
                <div class="card p-6 rounded-xl border border-transparent">
                    <h3 class="text-xl font-bold text-indigo-500 mb-3">Databases</h3>
                    <ul class="space-y-2 text-gray-300">
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> PostgreSQL (SQL)</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> MongoDB (NoSQL)</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Database Design & Optimization</li>
                    </ul>
                </div>

                <!-- Skill Card: Tools & DevOps -->
                <div class="card p-6 rounded-xl border border-transparent">
                    <h3 class="text-xl font-bold text-orange-500 mb-3">Tools & DevOps</h3>
                    <ul class="space-y-2 text-gray-300">
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Git & GitHub</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Docker & Containerization</li>
                        <li class="flex items-center"><span class="text-yellow-500 mr-2">•</span> Cloud (AWS/GCP Basics)</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-16 sm:py-24 bg-gray-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="section-heading">My Work</h2>
            <p class="text-lg text-gray-400 mb-10">Highlighting a few key projects that demonstrate my full-stack capabilities.</p>

            <div class="space-y-12">
                <!-- Project 1 Placeholder -->
                <div class="card p-8 rounded-xl border border-transparent md:flex md:space-x-8">
                    <div class="md:w-1/3">
                        <h3 class="text-2xl font-bold text-white mb-2">[Project 1 Title]</h3>
                        <p class="text-sm text-gray-400 mb-4">React, Node.js, MongoDB, Express</p>
                        <p class="text-gray-300 mb-6">
                            [A full-stack e-commerce platform featuring real-time inventory tracking and secure payment gateway integration. Focus on user authentication, complex state management, and API design.]
                        </p>
                        <div class="space-x-3">
                            <a href="[GitHub Repo Link 1]" target="_blank" class="text-indigo-400 hover:text-indigo-300 font-medium">Code &rarr;</a>
                            <a href="[Live Demo Link 1]" target="_blank" class="text-green-400 hover:text-green-300 font-medium">Live Site &rarr;</a>
                        </div>
                    </div>
                    <div class="md:w-2/3 mt-6 md:mt-0 bg-gray-800 rounded-lg p-4 flex items-center justify-center h-48">
                        <p class="text-gray-500">Project Screenshot Placeholder (Replace with image later)</p>
                    </div>
                </div>

                <!-- Project 2 Placeholder -->
                <div class="card p-8 rounded-xl border border-transparent md:flex md:space-x-8">
                    <div class="md:w-1/3">
                        <h3 class="text-2xl font-bold text-white mb-2">[Project 2 Title]</h3>
                        <p class="text-sm text-gray-400 mb-4">Python, Django, PostgreSQL, AWS</p>
                        <p class="text-gray-300 mb-6">
                            [A data visualization dashboard for analyzing public health metrics, deployed on AWS EC2. Demonstrates strong back-end logic, database query optimization, and secure user roles/permissions.]
                        </p>
                        <div class="space-x-3">
                            <a href="[GitHub Repo Link 2]" target="_blank" class="text-indigo-400 hover:text-indigo-300 font-medium">Code &rarr;</a>
                            <a href="[Live Demo Link 2]" target="_blank" class="text-green-400 hover:text-green-300 font-medium">Live Site &rarr;</a>
                        </div>
                    </div>
                    <div class="md:w-2/3 mt-6 md:mt-0 bg-gray-800 rounded-lg p-4 flex items-center justify-center h-48">
                        <p class="text-gray-500">Project Screenshot Placeholder (Replace with image later)</p>
                    </div>
                </div>

                <!-- Project 3 Placeholder -->
                <div class="card p-8 rounded-xl border border-transparent md:flex md:space-x-8">
                    <div class="md:w-1/3">
                        <h3 class="text-2xl font-bold text-white mb-2">[Project 3 Title]</h3>
                        <p class="text-sm text-gray-400 mb-4">Next.js, Tailwind CSS</p>
                        <p class="text-gray-300 mb-6">
                            [My personal portfolio website built with modern design principles and optimized for performance. Showcases fluid, responsive design and accessibility standards.]
                        </p>
                        <div class="space-x-3">
                            <a href="[GitHub Repo Link 3]" target="_blank" class="text-indigo-400 hover:text-indigo-300 font-medium">Code &rarr;</a>
                            <a href="[Live Demo Link 3]" target="_blank" class="text-green-400 hover:text-green-300 font-medium">Live Site &rarr;</a>
                        </div>
                    </div>
                    <div class="md:w-2/3 mt-6 md:mt-0 bg-gray-800 rounded-lg p-4 flex items-center justify-center h-48">
                        <p class="text-gray-500">Project Screenshot Placeholder (Replace with image later)</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 sm:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="section-heading mx-auto">Get In Touch</h2>
            <p class="text-xl text-gray-300 mb-10 max-w-2xl mx-auto">
                I am actively seeking new opportunities and open to exciting collaborations. Let's build something great together.
            </p>

            <div class="flex flex-col md:flex-row justify-center items-center space-y-6 md:space-y-0 md:space-x-12">
                <a href="mailto:websitedeveloper0990@gmail.com" class="card p-6 rounded-xl w-full md:w-64 border border-transparent hover:border-indigo-500">
                    <div class="text-2xl font-bold text-indigo-400">Email</div>
                    <p class="text-gray-400 mt-1">[Your Email Address]</p>
                </a>
                <a href="https://www.linkedin.com/in/guptamanish0990" target="_blank" class="card p-6 rounded-xl w-full md:w-64 border border-transparent hover:border-indigo-500">
                    <div class="text-2xl font-bold text-indigo-400">LinkedIn</div>
                    <p class="text-gray-400 mt-1">/in/ManishGupta</p>
                </a>
                <a href="https://github.com/Guptamanish0990" target="_blank" class="card p-6 rounded-xl w-full md:w-64 border border-transparent hover:border-indigo-500">
                    <div class="text-2xl font-bold text-indigo-400">GitHub</div>
                    <p class="text-gray-400 mt-1">Guptamanish0990</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 border-t border-gray-800 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-gray-500 text-sm">
            &copy; <span id="year"></span> Manish Gupta. All Rights Reserved.
        </div>
    </footer>

    <script>
        // Update copyright year
        document.getElementById('year').textContent = new Date().getFullYear();

        // Mobile Menu Toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            const isExpanded = mobileMenuButton.getAttribute('aria-expanded') === 'true' || false;
            mobileMenuButton.setAttribute('aria-expanded', !isExpanded);
            
            // Toggle menu and icon visibility
            mobileMenu.classList.toggle('hidden');
            mobileMenuButton.querySelectorAll('svg').forEach(icon => icon.classList.toggle('hidden'));
        });

        // Close mobile menu on link click
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                // Ensure the menu icon is shown again
                mobileMenuButton.querySelector('.block').classList.remove('hidden');
                mobileMenuButton.querySelector('.hidden').classList.add('hidden');
                mobileMenuButton.setAttribute('aria-expanded', 'false');
            });
        });

    </script>
</body>
</html>
