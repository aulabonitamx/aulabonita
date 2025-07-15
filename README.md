# aulabonita
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aula Bonita - Aprende IA con Estilo</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'rosa-pastel': '#FBD6D2',
                        'naranja-coral': '#FFD6A5',
                        'celeste-suave': '#D6EFFF',
                    },
                    fontFamily: {
                        'caveat': ['Caveat', 'cursive'],
                        'inter': ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #FBD6D2 0%, #FFD6A5 50%, #D6EFFF 100%);
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .floating {
            animation: float 3s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
    </style>
</head>
<body class="font-inter bg-gray-50">
    <!-- Header -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <h1 class="font-inter text-3xl font-bold text-gray-800 tracking-wide">Aula Bonita</h1>
                    <span class="ml-2 text-2xl">✨</span>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#inicio" class="text-gray-700 hover:text-pink-400 px-3 py-2 rounded-full text-sm font-medium transition-colors">Inicio</a>
                        <a href="#tienda" class="text-gray-700 hover:text-pink-400 px-3 py-2 rounded-full text-sm font-medium transition-colors">Tienda</a>
                        <a href="#tips" class="text-gray-700 hover:text-pink-400 px-3 py-2 rounded-full text-sm font-medium transition-colors">Tips con IA</a>
                        <a href="#nosotras" class="text-gray-700 hover:text-pink-400 px-3 py-2 rounded-full text-sm font-medium transition-colors">Sobre Nosotras</a>
                        <a href="#comunidad" class="bg-rosa-pastel text-gray-800 px-4 py-2 rounded-full text-sm font-medium hover:bg-pink-300 transition-colors">Únete a la comunidad</a>
                    </div>
                </div>
                <div class="md:hidden">
                    <button onclick="toggleMenu()" class="text-gray-700 hover:text-pink-400">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                    </button>
                </div>
            </div>
        </nav>
        <div id="mobile-menu" class="md:hidden hidden bg-white border-t">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#inicio" class="block px-3 py-2 text-gray-700 hover:text-pink-400">Inicio</a>
                <a href="#tienda" class="block px-3 py-2 text-gray-700 hover:text-pink-400">Tienda</a>
                <a href="#tips" class="block px-3 py-2 text-gray-700 hover:text-pink-400">Tips con IA</a>
                <a href="#nosotras" class="block px-3 py-2 text-gray-700 hover:text-pink-400">Sobre Nosotras</a>
                <a href="#comunidad" class="block px-3 py-2 text-gray-700 hover:text-pink-400">Únete a la comunidad</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="gradient-bg py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div class="text-center lg:text-left">
                    <h2 class="font-inter text-4xl lg:text-5xl font-bold text-gray-800 mb-6 leading-tight">
                        ✨ Bienvenida a Aula Bonita
                    </h2>
                    <p class="text-lg text-gray-700 mb-8 leading-relaxed">
                        Aquí vas a encontrar plantillas hermosas y herramientas digitales para organizar tu mente, tus días y tu vida. Todo con ayuda de la tecnología, pero explicado con amor, paciencia y estilo.
                    </p>
                    <button onclick="downloadTemplate()" class="bg-white text-gray-800 px-8 py-4 rounded-full font-semibold text-lg shadow-lg hover:shadow-xl transition-all duration-300 hover:scale-105">
                        🎁 Descarga tu plantilla gratis
                    </button>
                </div>
                <div class="flex justify-center">
                    <div class="floating bg-white p-8 rounded-3xl shadow-xl">
                        <svg class="w-64 h-64" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Notebook -->
                            <rect x="40" y="30" width="120" height="140" rx="8" fill="#FBD6D2" stroke="#FFD6A5" stroke-width="2"/>
                            <rect x="50" y="40" width="100" height="120" rx="4" fill="white"/>
                            <!-- Lines -->
                            <line x1="60" y1="60" x2="140" y2="60" stroke="#D6EFFF" stroke-width="2"/>
                            <line x1="60" y1="80" x2="140" y2="80" stroke="#D6EFFF" stroke-width="2"/>
                            <line x1="60" y1="100" x2="140" y2="100" stroke="#D6EFFF" stroke-width="2"/>
                            <line x1="60" y1="120" x2="140" y2="120" stroke="#D6EFFF" stroke-width="2"/>
                            <!-- Pen -->
                            <circle cx="160" cy="50" r="3" fill="#FFD6A5"/>
                            <rect x="158" y="53" width="4" height="20" rx="2" fill="#FBD6D2"/>
                            <!-- Hearts -->
                            <circle cx="30" cy="60" r="4" fill="#FFD6A5"/>
                            <circle cx="170" cy="120" r="4" fill="#D6EFFF"/>
                            <circle cx="25" cy="140" r="3" fill="#FBD6D2"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="tienda" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-caveat text-4xl font-bold text-gray-800 mb-4">Nuestros Productos Digitales</h3>
                <p class="text-gray-600 text-lg">Plantillas hermosas y funcionales para organizar tu vida</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="card-hover bg-rosa-pastel rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">💰</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Plantillas de Finanzas</h4>
                    <p class="text-gray-700 mb-4">Organiza tu dinero de forma bonita y práctica</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
                <div class="card-hover bg-naranja-coral rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">📅</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Calendarios Imprimibles</h4>
                    <p class="text-gray-700 mb-4">Planifica tus meses con estilo y color</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
                <div class="card-hover bg-celeste-suave rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">📝</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Planificadores Semanales</h4>
                    <p class="text-gray-700 mb-4">Organiza tu semana paso a paso</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
                <div class="card-hover bg-rosa-pastel rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">✅</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Listas de Pendientes</h4>
                    <p class="text-gray-700 mb-4">To-do lists que realmente usarás</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
                <div class="card-hover bg-naranja-coral rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">👩‍🏫</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Para Profes</h4>
                    <p class="text-gray-700 mb-4">Recursos educativos hermosos y funcionales</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
                <div class="card-hover bg-celeste-suave rounded-3xl p-6 text-center">
                    <div class="text-6xl mb-4">💼</div>
                    <h4 class="font-semibold text-xl mb-2 text-gray-800">Para Emprendedoras</h4>
                    <p class="text-gray-700 mb-4">Plantillas para hacer crecer tu negocio</p>
                    <button class="bg-white text-gray-800 px-6 py-2 rounded-full font-medium hover:shadow-lg transition-all">Ver más</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-caveat text-4xl font-bold text-gray-800 mb-4">Lo que dicen nuestras alumnas</h3>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-6 rounded-3xl shadow-lg">
                    <div class="text-center">
                        <div class="text-4xl mb-4">💕</div>
                        <p class="text-gray-700 italic mb-4">"Gracias a Aula Bonita aprendí a organizarme sin estrés y con estilo"</p>
                        <p class="font-semibold text-gray-800">- María Elena</p>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-3xl shadow-lg">
                    <div class="text-center">
                        <div class="text-4xl mb-4">✨</div>
                        <p class="text-gray-700 italic mb-4">"Sus recursos son accesibles, prácticos y hermosos. ¡Los amo!"</p>
                        <p class="font-semibold text-gray-800">- Carmen López</p>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-3xl shadow-lg">
                    <div class="text-center">
                        <div class="text-4xl mb-4">🌟</div>
                        <p class="text-gray-700 italic mb-4">"Finalmente encontré plantillas que combinan funcionalidad con belleza"</p>
                        <p class="font-semibold text-gray-800">- Ana Sofía</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Us -->
    <section id="nosotras" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="font-caveat text-4xl font-bold text-gray-800 mb-6">Quiénes Somos 💛</h3>
                    <p class="text-gray-700 text-lg mb-6 leading-relaxed">
                        Aula Bonita es un sueño compartido entre dos profes mexicanas que creemos que aprender puede ser bello, práctico y humano.
                    </p>
                    <p class="text-gray-700 text-lg mb-6 leading-relaxed">
                        Somos Gabi y Lety, expertas en educación e inteligencia artificial aplicada. Creamos recursos para ayudarte a organizar tu vida, ser más productiva y disfrutar el proceso.
                    </p>
                    <p class="text-gray-700 text-lg leading-relaxed">
                        En cada plantilla, cada curso, cada post, hay un poquito de nosotras 💛
                    </p>
                </div>
                <div class="flex justify-center">
                    <div class="bg-gradient-to-br from-rosa-pastel to-naranja-coral p-8 rounded-3xl">
                        <svg class="w-64 h-64" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <!-- Two figures representing Gabi and Lety -->
                            <circle cx="70" cy="60" r="25" fill="white"/>
                            <circle cx="130" cy="60" r="25" fill="white"/>
                            <rect x="50" y="85" width="40" height="60" rx="20" fill="#D6EFFF"/>
                            <rect x="110" y="85" width="40" height="60" rx="20" fill="#FFD6A5"/>
                            <!-- Hearts and stars -->
                            <circle cx="100" cy="30" r="3" fill="white"/>
                            <circle cx="40" cy="100" r="2" fill="white"/>
                            <circle cx="160" cy="120" r="2" fill="white"/>
                            <!-- Laptop -->
                            <rect x="80" y="160" width="40" height="25" rx="3" fill="white"/>
                            <rect x="85" y="165" width="30" height="15" rx="2" fill="#D6EFFF"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Tips Section -->
    <section id="tips" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h3 class="font-caveat text-4xl font-bold text-gray-800 mb-4">Tips Bonitos con IA</h3>
                <p class="text-gray-600 text-lg">Consejos prácticos para usar la tecnología con estilo</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="card-hover bg-white rounded-3xl p-6 shadow-lg">
                    <div class="text-4xl mb-4">👩‍👧‍👦</div>
                    <h4 class="font-semibold text-lg mb-2 text-gray-800">IA para Mamás</h4>
                    <p class="text-gray-600 text-sm">Cómo usar inteligencia artificial para organizar la vida familiar</p>
                </div>
                <div class="card-hover bg-white rounded-3xl p-6 shadow-lg">
                    <div class="text-4xl mb-4">⚡</div>
                    <h4 class="font-semibold text-lg mb-2 text-gray-800">Automatización Simple</h4>
                    <p class="text-gray-600 text-sm">Tareas que puedes automatizar sin complicarte la vida</p>
                </div>
                <div class="card-hover bg-white rounded-3xl p-6 shadow-lg">
                    <div class="text-4xl mb-4">🎨</div>
                    <h4 class="font-semibold text-lg mb-2 text-gray-800">Prompts para Canva</h4>
                    <p class="text-gray-600 text-sm">Crea diseños hermosos con ayuda de la IA</p>
                </div>
                <div class="card-hover bg-white rounded-3xl p-6 shadow-lg">
                    <div class="text-4xl mb-4">🧘‍♀️</div>
                    <h4 class="font-semibold text-lg mb-2 text-gray-800">Productividad Zen</h4>
                    <p class="text-gray-600 text-sm">Ser productiva sin estrés ni agobio</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Community Form -->
    <section id="comunidad" class="py-20 gradient-bg">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-white rounded-3xl p-8 shadow-xl">
                <div class="text-center mb-8">
                    <h3 class="font-caveat text-4xl font-bold text-gray-800 mb-4">🎁 ¿Quieres probar algo gratis?</h3>
                    <p class="text-gray-700 text-lg">Descarga nuestro mini pack de plantillas y únete a la comunidad más bonita del internet.</p>
                </div>
                <form onsubmit="joinCommunity(event)" class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Nombre</label>
                            <input type="text" required class="w-full px-4 py-3 rounded-2xl border border-gray-200 focus:border-pink-300 focus:outline-none focus:ring-2 focus:ring-pink-100 transition-all">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Correo</label>
                            <input type="email" required class="w-full px-4 py-3 rounded-2xl border border-gray-200 focus:border-pink-300 focus:outline-none focus:ring-2 focus:ring-pink-100 transition-all">
                        </div>
                    </div>
                    <div>
                        <label class="block text-gray-700 font-medium mb-4">¿Cuál es tu interés principal?</label>
                        <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                            <label class="flex items-center space-x-2 cursor-pointer">
                                <input type="checkbox" class="rounded text-pink-400 focus:ring-pink-300">
                                <span class="text-gray-700">Organización</span>
                            </label>
                            <label class="flex items-center space-x-2 cursor-pointer">
                                <input type="checkbox" class="rounded text-pink-400 focus:ring-pink-300">
                                <span class="text-gray-700">Finanzas</span>
                            </label>
                            <label class="flex items-center space-x-2 cursor-pointer">
                                <input type="checkbox" class="rounded text-pink-400 focus:ring-pink-300">
                                <span class="text-gray-700">Docencia</span>
                            </label>
                            <label class="flex items-center space-x-2 cursor-pointer">
                                <input type="checkbox" class="rounded text-pink-400 focus:ring-pink-300">
                                <span class="text-gray-700">Emprender</span>
                            </label>
                        </div>
                    </div>
                    <div class="text-center">
                        <button type="submit" class="bg-rosa-pastel text-gray-800 px-8 py-4 rounded-full font-semibold text-lg hover:bg-pink-300 transition-all duration-300 hover:scale-105 shadow-lg">
                            Únete a la comunidad ✨
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center">
                <h4 class="font-caveat text-3xl font-bold mb-6">Aula Bonita ✨</h4>
                <div class="flex justify-center space-x-6 mb-8">
                    <a href="#" class="text-2xl hover:text-pink-400 transition-colors">📱</a>
                    <a href="#" class="text-2xl hover:text-pink-400 transition-colors">💬</a>
                    <a href="#" class="text-2xl hover:text-pink-400 transition-colors">📧</a>
                </div>
                <p class="text-gray-400 mb-4">Aviso de Privacidad | Términos y Condiciones</p>
                <p class="font-caveat text-xl text-pink-300">Gracias por crear con nosotras 💖</p>
            </div>
        </div>
    </footer>

    <script>
        function toggleMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        function downloadTemplate() {
            alert('¡Gracias por tu interés! 🎁\n\nTu plantilla gratuita se descargará pronto. Te enviaremos un email con el enlace de descarga.');
        }

        function joinCommunity(event) {
            event.preventDefault();
            const formData = new FormData(event.target);
            alert('¡Bienvenida a la comunidad de Aula Bonita! ✨\n\nRecibirás un email de confirmación con tu mini pack de plantillas gratuitas.');
            event.target.reset();
        }

        // Smooth scrolling for navigation links
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

        // Close mobile menu when clicking on a link
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                document.getElementById('mobile-menu').classList.add('hidden');
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'95fb11a0e12ec2fe',t:'MTc1MjYwMTQ3Ny4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
