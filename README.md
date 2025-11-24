<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sitios Web Personalizados | Diseño Moderno y Plantillas Únicas</title>
    <!-- Carga de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Configuración de color para un azul moderno -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary-blue': '#3B82F6', // Un azul vibrante
                        'secondary-gray': '#F9FAFB',
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        /* Estilos personalizados para la fuente Inter (si no está disponible por defecto) */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
    </style>
</head>
<body class="bg-white font-sans text-gray-800">

    <!-- Navegación Fija -->
    <nav class="sticky top-0 z-50 bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Logo -->
                <a href="#" class="flex items-center space-x-2">
                    <svg class="h-8 w-8 text-primary-blue" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path></svg>
                    <span class="text-xl font-bold text-gray-900">WebSolutions</span>
                </a>
                <!-- Menú Desktop -->
                <div class="hidden sm:ml-6 sm:flex sm:space-x-8">
                    <a href="#servicios" class="text-gray-900 hover:text-primary-blue px-3 py-2 rounded-md text-sm font-medium transition duration-150">Servicios</a>
                    <a href="#caracteristicas" class="text-gray-900 hover:text-primary-blue px-3 py-2 rounded-md text-sm font-medium transition duration-150">Características</a>
                    <a href="#precios" class="text-gray-900 hover:text-primary-blue px-3 py-2 rounded-md text-sm font-medium transition duration-150">Planes</a>
                    <a href="#pagos" class="text-gray-900 hover:text-primary-blue px-3 py-2 rounded-md text-sm font-medium transition duration-150">Pagos</a>
                    <a href="#contacto" class="text-white bg-primary-blue hover:bg-indigo-700 px-3 py-2 rounded-lg text-sm font-medium transition duration-150 shadow-md">Contacto</a>
                </div>
                <!-- Menú Móvil (Simple, ya que es una página de un archivo) -->
                <div class="sm:hidden">
                    <button id="mobile-menu-button" class="text-gray-500 hover:text-primary-blue focus:outline-none focus:text-primary-blue">
                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Contenedor del menú móvil (oculto) -->
        <div id="mobile-menu" class="hidden sm:hidden px-2 pt-2 pb-3 space-y-1">
             <a href="#servicios" class="block text-gray-900 hover:bg-gray-100 px-3 py-2 rounded-md text-base font-medium">Servicios</a>
             <a href="#caracteristicas" class="block text-gray-900 hover:bg-gray-100 px-3 py-2 rounded-md text-base font-medium">Características</a>
             <a href="#precios" class="block text-gray-900 hover:bg-gray-100 px-3 py-2 rounded-md text-base font-medium">Planes</a>
             <a href="#pagos" class="block text-gray-900 hover:bg-gray-100 px-3 py-2 rounded-md text-base font-medium">Pagos</a>
             <a href="#contacto" class="block text-white bg-primary-blue px-3 py-2 rounded-md text-base font-medium">Contacto</a>
        </div>
    </nav>

    <!-- Sección 1: Hero / Impacto -->
    <header class="bg-white py-16 md:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-gray-900 leading-tight mb-4">
                El Sitio Web que Siempre <span class="text-primary-blue">Imaginaste</span>
            </h1>
            <p class="text-xl text-gray-600 mb-8 max-w-3xl mx-auto">
                Diseño profesional, totalmente personalizado y con 20 plantillas de nicho para empezar a dominar tu mercado.
            </p>
            <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-4">
                <a href="#precios" class="bg-primary-blue text-white font-bold py-3 px-8 rounded-xl shadow-lg hover:bg-indigo-700 transition duration-300 transform hover:scale-105">
                    Ver Nuestros Planes
                </a>
                <a href="#contacto" class="bg-gray-100 text-gray-800 font-bold py-3 px-8 rounded-xl border border-gray-300 hover:bg-gray-200 transition duration-300 transform hover:scale-105">
                    Solicitar Demo
                </a>
            </div>
        </div>
    </header>

    <!-- Sección 2: Servicios (El valor de las 20 plantillas) -->
    <section id="servicios" class="py-16 bg-secondary-gray">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl font-bold text-gray-900 mb-4">Sitios Web a tu Medida</h2>
            <p class="text-lg text-gray-600 mb-12 max-w-4xl mx-auto">
                Creamos experiencias digitales únicas. Nuestro valor diferencial: en cada plan, obtienes 20 plantillas de nicho para que la personalización sea más rápida y precisa que nunca.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Tarjeta 1 -->
                <div class="bg-white p-6 rounded-xl shadow-xl transition duration-300 hover:shadow-2xl border-t-4 border-primary-blue">
                    <div class="text-primary-blue mb-4 flex justify-center">
                         <!-- Icono de Diseño Web -->
                        <svg class="h-10 w-10" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-1-3m-6 0h6m-5-5a1 1 0 110-2 1 1 0 010 2zm1-5a1 1 0 110-2 1 1 0 010 2zm4 4a1 1 0 110-2 1 1 0 010 2zm1-5a1 1 0 110-2 1 1 0 010 2zm-4 4a1 1 0 110-2 1 1 0 010 2zM12 11h.01M17 11h.01M12 16h.01M17 16h.01"></path></svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Diseño 100% Personalizado</h3>
                    <p class="text-gray-500">Cada proyecto comienza desde cero, centrado en tus objetivos y la identidad de tu marca. No usamos temas genéricos.</p>
                </div>
                <!-- Tarjeta 2 -->
                <div class="bg-white p-6 rounded-xl shadow-xl transition duration-300 hover:shadow-2xl border-t-4 border-primary-blue">
                    <div class="text-primary-blue mb-4 flex justify-center">
                         <!-- Icono de Plantillas -->
                        <svg class="h-10 w-10" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m0 0V8a2 2 0 012-2h4l2-2h2m0 0V6m0 6V8"></path></svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">20 Plantillas de Nicho Únicas</h3>
                    <p class="text-gray-500">Un impulso de diseño. Elige entre 20 diseños pre-construidos específicos para tu industria (Restaurantes, Agencias, Blogs, etc.).</p>
                </div>
                <!-- Tarjeta 3 -->
                <div class="bg-white p-6 rounded-xl shadow-xl transition duration-300 hover:shadow-2xl border-t-4 border-primary-blue">
                    <div class="text-primary-blue mb-4 flex justify-center">
                        <!-- Icono de Responsivo -->
                        <svg class="h-10 w-10" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M7 21h10a2 2 0 002-2V5a2 2 0 00-2-2H7a2 2 0 00-2 2v14a2 2 0 002 2z"></path></svg>
                    </div>
                    <h3 class="text-xl font-semibold mb-3">Totalmente Responsivo</h3>
                    <p class="text-gray-500">Tu web se verá increíble en cualquier dispositivo: móvil, tablet y escritorio. Garantizamos la mejor experiencia de usuario.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección 3: Precios / Planes (El foco del requisito) -->
    <section id="precios" class="py-16 md:py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <span class="text-primary-blue text-sm font-semibold uppercase tracking-wider mb-2 block">Inversión Inteligente</span>
            <h2 class="text-4xl font-extrabold text-gray-900 mb-12">Escoge tu Plan de Éxito</h2>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Plan 1: Plan Inicio -->
                <div class="bg-secondary-gray p-8 rounded-xl shadow-2xl flex flex-col transform hover:scale-[1.02] transition duration-300">
                    <h3 class="text-2xl font-bold mb-3 text-primary-blue">Plan Inicio</h3>
                    <p class="text-gray-600 mb-6">Ideal para profesionales y pequeños negocios que necesitan presencia online.</p>
                    <div class="flex items-baseline justify-center mb-6">
                        <span class="text-4xl font-extrabold text-gray-900">$20</span>
                        <span class="text-xl font-medium text-gray-500">/pago único</span>
                    </div>

                    <!-- Característica Clave -->
                    <div class="mb-6 bg-primary-blue/10 text-primary-blue p-3 rounded-lg font-semibold text-center">
                        <span class="block text-xl">20 Plantillas Personalizables</span>
                        <span class="text-sm">Incluidas en este plan.</span>
                    </div>

                    <ul class="text-left space-y-3 mb-8 flex-grow">
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Web de 5 Secciones (Landing)
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Diseño Responsivo Básico
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Formulario de Contacto
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Integración con Redes Sociales
                        </li>
                    </ul>
                    <a href="#pagos" class="mt-auto bg-primary-blue text-white font-bold py-3 rounded-xl hover:bg-indigo-700 transition duration-300 shadow-md">
                        Seleccionar Plan
                    </a>
                </div>

                <!-- Plan 2: Tienda Online (Destacado) -->
                <div class="bg-white p-8 rounded-xl shadow-2xl ring-4 ring-primary-blue flex flex-col transform scale-[1.05] hover:scale-[1.08] transition duration-300">
                    <p class="text-sm font-bold text-white bg-primary-blue py-1 px-4 rounded-full self-center mb-3 -mt-12 shadow-lg">Más Popular</p>
                    <h3 class="text-3xl font-bold mb-3 text-gray-900">Tienda Online</h3>
                    <p class="text-gray-600 mb-6">Perfecto para negocios que buscan vender productos en línea de inmediato.</p>
                    <div class="flex items-baseline justify-center mb-6">
                        <span class="text-5xl font-extrabold text-primary-blue">$30</span>
                        <span class="text-xl font-medium text-gray-500">/pago único</span>
                    </div>
                    
                    <!-- Característica Clave -->
                    <div class="mb-6 bg-primary-blue text-white p-3 rounded-lg font-semibold text-center shadow-lg">
                        <span class="block text-xl">20 Plantillas Personalizables</span>
                        <span class="text-sm">¡Plantillas de E-commerce incluidas!</span>
                    </div>

                    <ul class="text-left space-y-3 mb-8 flex-grow">
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            <strong class="font-semibold">Plataforma E-commerce Completa</strong>
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Pasarelas de Pago Integradas (3)
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Gestión de Inventario y Pedidos
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Certificado SSL y Seguridad Avanzada
                        </li>
                    </ul>
                    <a href="#pagos" class="mt-auto bg-primary-blue text-white font-bold py-3 rounded-xl hover:bg-indigo-700 transition duration-300 shadow-xl">
                        Comenzar con Tienda
                    </a>
                </div>

                <!-- Plan 3: Plan Empresarial -->
                <div class="bg-secondary-gray p-8 rounded-xl shadow-2xl flex flex-col transform hover:scale-[1.02] transition duration-300">
                    <h3 class="text-2xl font-bold mb-3 text-primary-blue">Plan Empresarial</h3>
                    <p class="text-gray-600 mb-6">Para empresas grandes o proyectos con alta complejidad y tráfico.</p>
                    <div class="flex items-baseline justify-center mb-6">
                        <span class="text-4xl font-extrabold text-gray-900">$55</span>
                        <span class="text-xl font-medium text-gray-500">/pago único</span>
                    </div>

                    <!-- Característica Clave -->
                    <div class="mb-6 bg-primary-blue/10 text-primary-blue p-3 rounded-lg font-semibold text-center">
                        <span class="block text-xl">20 Plantillas Personalizables</span>
                        <span class="text-sm">Adaptadas a entornos corporativos.</span>
                    </div>
                    
                    <ul class="text-left space-y-3 mb-8 flex-grow">
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Todo lo del Plan Tienda Online
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Soporte 24/7 Dedicado
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Integración con CRM/ERP
                        </li>
                        <li class="flex items-center text-gray-700">
                            <svg class="h-5 w-5 text-green-500 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                            Optimización SEO Avanzada
                        </li>
                    </ul>
                    <a href="#pagos" class="mt-auto bg-primary-blue text-white font-bold py-3 rounded-xl hover:bg-indigo-700 transition duration-300 shadow-md">
                        Seleccionar Plan
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección 4: Características Adicionales -->
    <section id="caracteristicas" class="py-16 bg-secondary-gray">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-3xl font-bold text-center text-gray-900 mb-12">Nuestras Ventajas</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                
                <!-- Ventaja 1 -->
                <div class="flex flex-col items-center text-center bg-white p-6 rounded-xl shadow-lg border-b-4 border-primary-blue">
                    <div class="p-3 mb-4 rounded-full bg-primary-blue/20 text-primary-blue">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                    </div>
                    <h3 class="font
