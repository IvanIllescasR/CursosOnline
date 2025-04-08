<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Academia de Formación Profesional</title>
<script src="https://cdn.tailwindcss.com/3.4.16"></script>
<script>tailwind.config={theme:{extend:{colors:{primary:'#3b82f6',secondary:'#f59e0b'},borderRadius:{'none':'0px','sm':'4px',DEFAULT:'8px','md':'12px','lg':'16px','xl':'20px','2xl':'24px','3xl':'32px','full':'9999px','button':'8px'}}}}</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/remixicon@4.5.0/fonts/remixicon.css" rel="stylesheet">
<style>
:where([class^="ri-"])::before { content: "\f3c2"; }
body {
font-family: 'Montserrat', sans-serif;
}
.hero-section {
background-image: linear-gradient(to right, rgba(255, 255, 255, 1) 40%, rgba(255, 255, 255, 0.8) 60%, rgba(255, 255, 255, 0.4) 80%, rgba(255, 255, 255, 0) 100%), url('https://public.readdy.ai/ai/img_res/0c524c26c1d3ef1a96dcd46a78eedb6e.jpg');
background-size: cover;
background-position: center right;
}
.testimonial-card {
transition: transform 0.3s ease;
}
.testimonial-card:hover {
transform: translateY(-5px);
}
.course-card {
transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.course-card:hover {
transform: translateY(-5px);
box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
}
input:focus, select:focus {
outline: none;
border-color: #3b82f6;
box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.2);
}
.custom-checkbox {
position: relative;
padding-left: 28px;
cursor: pointer;
user-select: none;
}
.custom-checkbox input {
position: absolute;
opacity: 0;
cursor: pointer;
height: 0;
width: 0;
}
.checkmark {
position: absolute;
top: 0;
left: 0;
height: 20px;
width: 20px;
background-color: #fff;
border: 2px solid #d1d5db;
border-radius: 4px;
}
.custom-checkbox:hover input ~ .checkmark {
border-color: #3b82f6;
}
.custom-checkbox input:checked ~ .checkmark {
background-color: #3b82f6;
border-color: #3b82f6;
}
.checkmark:after {
content: "";
position: absolute;
display: none;
}
.custom-checkbox input:checked ~ .checkmark:after {
display: block;
}
.custom-checkbox .checkmark:after {
left: 6px;
top: 2px;
width: 5px;
height: 10px;
border: solid white;
border-width: 0 2px 2px 0;
transform: rotate(45deg);
}
</style>
</head>
<body class="bg-gray-50">
<!-- Navegación -->
<nav class="bg-white shadow-sm sticky top-0 z-50">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="flex justify-between h-16">
<div class="flex items-center">
<a href="#" class="text-2xl font-['Pacifico'] text-primary">logo</a>
</div>
<div class="hidden md:flex items-center space-x-8">
<a href="#cursos-compras" class="text-gray-700 hover:text-primary font-medium">Compras Públicas</a>
<a href="#cursos-impuestos" class="text-gray-700 hover:text-primary font-medium">Impuestos</a>
<a href="#cursos-ia" class="text-gray-700 hover:text-primary font-medium">Inteligencia Artificial</a>
<a href="#precios" class="text-gray-700 hover:text-primary font-medium">Precios</a>
<a href="#testimonios" class="text-gray-700 hover:text-primary font-medium">Testimonios</a>
</div>
<div class="flex items-center">
<a href="#inscripcion" class="bg-primary text-white px-6 py-2 !rounded-button font-medium whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscríbete Ahora</a>
</div>
<div class="md:hidden flex items-center">
<button class="text-gray-700 w-10 h-10 flex items-center justify-center">
<i class="ri-menu-line ri-lg"></i>
</button>
</div>
</div>
</div>
</nav>
<!-- Hero Section -->
<section class="hero-section py-20">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full">
<div class="w-full md:w-1/2">
<h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-6">Formación Profesional de Excelencia</h1>
<p class="text-lg text-gray-700 mb-8">Especialízate en Compras Públicas, Impuestos o Inteligencia Artificial con cursos diseñados por expertos para impulsar tu carrera profesional.</p>
<div class="flex flex-col sm:flex-row gap-4">
<a href="#cursos" class="bg-primary text-white px-8 py-3 !rounded-button font-medium whitespace-nowrap hover:bg-blue-600 transition duration-300 text-center">Ver Cursos</a>
<a href="#contacto" class="bg-white text-primary border border-primary px-8 py-3 !rounded-button font-medium whitespace-nowrap hover:bg-gray-50 transition duration-300 text-center">Contáctanos</a>
</div>
</div>
</div>
</section>
<!-- Beneficios -->
<section class="py-16 bg-white">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-16">
<h2 class="text-3xl font-bold text-gray-900 mb-4">¿Por qué elegirnos?</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Nuestra metodología garantiza una experiencia de aprendizaje efectiva y adaptada a tus necesidades profesionales.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="bg-gray-50 p-8 rounded-lg shadow-sm text-center">
<div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-6">
<i class="ri-award-line ri-xl text-primary"></i>
</div>
<h3 class="text-xl font-semibold text-gray-900 mb-3">Certificados de Asistencia</h3>
<p class="text-gray-600">Obtén certificados de asistencia y cumplimiento que acreditan tu participación y aprovechamiento en nuestros programas formativos.</p>
</div>
<div class="bg-gray-50 p-8 rounded-lg shadow-sm text-center">
<div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-6">
<i class="ri-time-line ri-xl text-primary"></i>
</div>
<h3 class="text-xl font-semibold text-gray-900 mb-3">Flexibilidad Horaria</h3>
<p class="text-gray-600">Estudia a tu ritmo con acceso 24/7 a nuestra plataforma y contenidos actualizados.</p>
</div>
<div class="bg-gray-50 p-8 rounded-lg shadow-sm text-center">
<div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-6">
<i class="ri-user-star-line ri-xl text-primary"></i>
</div>
<h3 class="text-xl font-semibold text-gray-900 mb-3">Profesores Expertos</h3>
<p class="text-gray-600">Aprende de profesionales con amplia experiencia en el sector público y privado.</p>
</div>
</div>
</div>
</section>
<!-- Catálogo de Cursos: Compras Públicas -->
<section id="cursos-compras" class="py-16 bg-gray-50">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-12">
<h2 class="text-3xl font-bold text-gray-900 mb-4">Cursos de Compras Públicas</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Especialízate en contratación estatal y domina los procesos de licitación pública.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/c63d4a8a9e6208d8a8351eef67458161.jpg" alt="Curso de Contratación Pública" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Fundamentos de Contratación Pública</h3>
<span class="bg-blue-100 text-primary text-xs font-medium px-2.5 py-0.5 rounded">Básico</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>40 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Aprende los conceptos básicos de la contratación estatal, normativa vigente y procedimientos administrativos.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$199</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$149</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/1817a8d4081831c191606223840043e4.jpg" alt="Curso de Licitaciones" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Gestión de Licitaciones Públicas</h3>
<span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded">Intermedio</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>60 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Domina el proceso completo de licitación, desde la preparación de ofertas hasta la adjudicación de contratos.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$249</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$199</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/918b799b56959f8a6a607129e00357e9.jpg" alt="Curso Avanzado" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Contratación Pública Avanzada</h3>
<span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded">Avanzado</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>80 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Especialízate en casos complejos, recursos administrativos y estrategias avanzadas de contratación pública.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$299</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$249</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- Catálogo de Cursos: Impuestos -->
<section id="cursos-impuestos" class="py-16 bg-white">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-12">
<h2 class="text-3xl font-bold text-gray-900 mb-4">Cursos de Impuestos y SRI</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Aprende a gestionar declaraciones de IVA y domina los procedimientos del Servicio de Rentas Internas.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="course-card bg-gray-50 rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/125ace48e9c5826ab0d325b71a91e06e.jpg" alt="Curso de IVA" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Declaración de IVA</h3>
<span class="bg-blue-100 text-primary text-xs font-medium px-2.5 py-0.5 rounded">Básico</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>30 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Aprende a realizar correctamente las declaraciones mensuales y semestrales de IVA para personas naturales y jurídicas.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$179</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$129</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-gray-50 rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/4584744e6fb9aff2fffa6d46c328ce7a.jpg" alt="Curso SRI" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Sistema SRI en Línea</h3>
<span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded">Intermedio</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>45 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Domina la plataforma digital del SRI y aprende a realizar todos los trámites tributarios de forma eficiente.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$219</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$169</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-gray-50 rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/142629e1f0a9a76017cff3d8590ba969.jpg" alt="Curso Planificación Tributaria" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Planificación Tributaria</h3>
<span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded">Avanzado</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>70 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Desarrolla estrategias fiscales legales para optimizar la carga tributaria de empresas y profesionales independientes.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$289</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$229</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- Catálogo de Cursos: Inteligencia Artificial -->
<section id="cursos-ia" class="py-16 bg-gray-50">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-12">
<h2 class="text-3xl font-bold text-gray-900 mb-4">Cursos de Inteligencia Artificial</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Adéntrate en el mundo de la IA con cursos diseñados para todos los niveles de experiencia.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/6d0b751c08e44fde8fa704cba2df9147.jpg" alt="Curso IA Básica" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Introducción a la IA</h3>
<span class="bg-blue-100 text-primary text-xs font-medium px-2.5 py-0.5 rounded">Básico</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>35 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Conoce los fundamentos de la inteligencia artificial, machine learning y su aplicación en el mundo actual.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$199</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$149</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/ded13e30fd51acbf09163b2e67cac297.jpg" alt="Curso IA Práctica" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">IA Práctica para Negocios</h3>
<span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded">Intermedio</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>50 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Implementa soluciones de IA en tu empresa: chatbots, análisis predictivo y automatización de procesos.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$249</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$199</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
<div class="course-card bg-white rounded-lg shadow-sm overflow-hidden">
<div class="h-48 overflow-hidden">
<img src="https://public.readdy.ai/ai/img_res/285807c23a347a4b0ccaeb0a7e7a6fc7.jpg" alt="Curso Data Science" class="w-full h-full object-cover object-top">
</div>
<div class="p-6">
<div class="flex justify-between items-start mb-2">
<h3 class="text-xl font-semibold text-gray-900">Data Science y Machine Learning</h3>
<span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded">Avanzado</span>
</div>
<div class="flex items-center mb-4 text-sm text-gray-500">
<div class="flex items-center mr-4">
<i class="ri-time-line mr-1"></i>
<span>80 horas</span>
</div>
<div class="flex items-center">
<i class="ri-computer-line mr-1"></i>
<span>Online</span>
</div>
</div>
<p class="text-gray-600 mb-6">Profundiza en algoritmos de machine learning, procesamiento de datos y desarrollo de modelos predictivos.</p>
<div class="flex justify-between items-center">
<div>
<span class="text-gray-400 line-through">$329</span>
<span class="text-2xl font-bold text-gray-900 ml-2">$279</span>
</div>
<a href="#inscripcion" class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap hover:bg-blue-600 transition duration-300">Inscribirme</a>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- Testimonios -->
<section id="testimonios" class="py-16 bg-white">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-12">
<h2 class="text-3xl font-bold text-gray-900 mb-4">Lo que dicen nuestros alumnos</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Descubre las experiencias de quienes ya han transformado su carrera profesional con nuestros cursos.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="testimonial-card bg-gray-50 p-8 rounded-lg shadow-sm">
<div class="flex items-center mb-6">
<div class="w-12 h-12 rounded-full overflow-hidden mr-4">
<img src="https://public.readdy.ai/ai/img_res/d3d44f01e94bf94a0c0a85be4a6eb871.jpg" alt="Testimonio" class="w-full h-full object-cover">
</div>
<div>
<h4 class="text-lg font-semibold text-gray-900">Gabriela Mendoza</h4>
<p class="text-sm text-gray-500">Especialista en Contratación Pública</p>
</div>
</div>
<div class="flex mb-4">
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
</div>
<p class="text-gray-600">"El curso de Contratación Pública Avanzada superó mis expectativas. Los contenidos están actualizados y los casos prácticos me ayudaron a enfrentar situaciones reales en mi trabajo. Altamente recomendado."</p>
</div>
<div class="testimonial-card bg-gray-50 p-8 rounded-lg shadow-sm">
<div class="flex items-center mb-6">
<div class="w-12 h-12 rounded-full overflow-hidden mr-4">
<img src="https://public.readdy.ai/ai/img_res/b5be58615374b0b496c6603790f5f055.jpg" alt="Testimonio" class="w-full h-full object-cover">
</div>
<div>
<h4 class="text-lg font-semibold text-gray-900">Carlos Jiménez</h4>
<p class="text-sm text-gray-500">Contador Independiente</p>
</div>
</div>
<div class="flex mb-4">
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-half-fill text-yellow-400"></i>
</div>
<p class="text-gray-600">"Gracias al curso de Declaración de IVA, ahora puedo asesorar mejor a mis clientes. La plataforma es intuitiva y el soporte del instructor fue excelente para resolver todas mis dudas."</p>
</div>
<div class="testimonial-card bg-gray-50 p-8 rounded-lg shadow-sm">
<div class="flex items-center mb-6">
<div class="w-12 h-12 rounded-full overflow-hidden mr-4">
<img src="https://public.readdy.ai/ai/img_res/0092eb2e692c2140c699063c197e068c.jpg" alt="Testimonio" class="w-full h-full object-cover">
</div>
<div>
<h4 class="text-lg font-semibold text-gray-900">Daniela Morales</h4>
<p class="text-sm text-gray-500">Emprendedora Digital</p>
</div>
</div>
<div class="flex mb-4">
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
<i class="ri-star-fill text-yellow-400"></i>
</div>
<p class="text-gray-600">"El curso de IA Práctica para Negocios transformó mi emprendimiento. Implementé un chatbot que atiende consultas 24/7 y mejoré mis estrategias de marketing con análisis predictivo. ¡Inversión que valió cada centavo!"</p>
</div>
</div>
</div>
</section>
<!-- Precios -->
<section id="precios" class="py-16 bg-gray-50">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="text-center mb-12">
<h2 class="text-3xl font-bold text-gray-900 mb-4">Planes de Estudio</h2>
<p class="text-lg text-gray-600 max-w-3xl mx-auto">Elige el plan que mejor se adapte a tus necesidades y objetivos profesionales.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="bg-white rounded-lg shadow-sm overflow-hidden">
<div class="p-8">
<h3 class="text-xl font-semibold text-gray-900 mb-4">Plan Básico</h3>
<div class="flex items-baseline mb-6">
<span class="text-4xl font-bold text-gray-900">$149</span>
<span class="text-gray-500 ml-2">/ curso</span>
</div>
<ul class="space-y-3 mb-8">
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso a 1 curso completo</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Certificado digital</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso por 3 meses</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Soporte por email</span>
</li>
<li class="flex items-start opacity-50">
<i class="ri-close-line text-red-500 mt-1 mr-2"></i>
<span class="text-gray-600">Tutorías personalizadas</span>
</li>
<li class="flex items-start opacity-50">
<i class="ri-close-line text-red-500 mt-1 mr-2"></i>
<span class="text-gray-600">Casos prácticos avanzados</span>
</li>
</ul>
<a href="#inscripcion" class="block w-full bg-gray-100 text-gray-800 text-center px-4 py-3 !rounded-button font-medium whitespace-nowrap hover:bg-gray-200 transition duration-300">Seleccionar Plan</a>
</div>
</div>
<div class="bg-white rounded-lg shadow-lg transform scale-105 overflow-hidden border-2 border-primary">
<div class="bg-primary text-white py-2 text-center">
<span class="text-sm font-medium">Más Popular</span>
</div>
<div class="p-8">
<h3 class="text-xl font-semibold text-gray-900 mb-4">Plan Profesional</h3>
<div class="flex items-baseline mb-6">
<span class="text-4xl font-bold text-gray-900">$299</span>
<span class="text-gray-500 ml-2">/ 3 cursos</span>
</div>
<ul class="space-y-3 mb-8">
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso a 3 cursos completos</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Certificados digitales</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso por 6 meses</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Soporte prioritario</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">2 tutorías personalizadas</span>
</li>
<li class="flex items-start opacity-50">
<i class="ri-close-line text-red-500 mt-1 mr-2"></i>
<span class="text-gray-600">Casos prácticos avanzados</span>
</li>
</ul>
<a href="#inscripcion" class="block w-full bg-primary text-white text-center px-4 py-3 !rounded-button font-medium whitespace-nowrap hover:bg-blue-600 transition duration-300">Seleccionar Plan</a>
</div>
</div>
<div class="bg-white rounded-lg shadow-sm overflow-hidden">
<div class="p-8">
<h3 class="text-xl font-semibold text-gray-900 mb-4">Plan Experto</h3>
<div class="flex items-baseline mb-6">
<span class="text-4xl font-bold text-gray-900">$499</span>
<span class="text-gray-500 ml-2">/ acceso completo</span>
</div>
<ul class="space-y-3 mb-8">
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso a todos los cursos</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Certificados digitales</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Acceso por 12 meses</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Soporte VIP 24/7</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">5 tutorías personalizadas</span>
</li>
<li class="flex items-start">
<i class="ri-check-line text-green-500 mt-1 mr-2"></i>
<span class="text-gray-600">Casos prácticos avanzados</span>
</li>
</ul>
<a href="#inscripcion" class="block w-full bg-gray-100 text-gray-800 text-center px-4 py-3 !rounded-button font-medium whitespace-nowrap hover:bg-gray-200 transition duration-300">Seleccionar Plan</a>
</div>
</div>
</div>
</div>
</section>
<!-- Formulario de Inscripción -->
<section id="inscripcion" class="py-16 bg-white">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
<div>
<h2 class="text-3xl font-bold text-gray-900 mb-6">Inscríbete Ahora</h2>
<p class="text-lg text-gray-600 mb-8">Completa el formulario y un asesor académico te contactará en menos de 24 horas para guiarte en el proceso de inscripción.</p>
<div class="bg-blue-50 p-6 rounded-lg mb-8">
<h3 class="text-xl font-semibold text-gray-900 mb-4">¿Por qué elegirnos?</h3>
<ul class="space-y-3">
<li class="flex items-start">
<div class="w-6 h-6 bg-blue-100 rounded-full flex items-center justify-center mr-3 mt-0.5">
<i class="ri-check-line text-primary"></i>
</div>
<span class="text-gray-600">Docentes con más de 10 años de experiencia profesional</span>
</li>
<li class="flex items-start">
<div class="w-6 h-6 bg-blue-100 rounded-full flex items-center justify-center mr-3 mt-0.5">
<i class="ri-check-line text-primary"></i>
</div>
<span class="text-gray-600">Certificaciones reconocidas por entidades gubernamentales</span>
</li>
<li class="flex items-start">
<div class="w-6 h-6 bg-blue-100 rounded-full flex items-center justify-center mr-3 mt-0.5">
<i class="ri-check-line text-primary"></i>
</div>
<span class="text-gray-600">Plataforma disponible 24/7 con materiales actualizados</span>
</li>
<li class="flex items-start">
<div class="w-6 h-6 bg-blue-100 rounded-full flex items-center justify-center mr-3 mt-0.5">
<i class="ri-check-line text-primary"></i>
</div>
<span class="text-gray-600">Garantía de satisfacción o devolución de tu dinero</span>
</li>
</ul>
</div>
<div class="flex items-center space-x-4">
<span class="text-gray-500">Métodos de pago:</span>
<div class="flex space-x-3">
<div class="w-10 h-10 flex items-center justify-center text-gray-600">
<i class="ri-visa-fill ri-xl"></i>
</div>
<div class="w-10 h-10 flex items-center justify-center text-gray-600">
<i class="ri-mastercard-fill ri-xl"></i>
</div>
<div class="w-10 h-10 flex items-center justify-center text-gray-600">
<i class="ri-paypal-fill ri-xl"></i>
</div>
<div class="w-10 h-10 flex items-center justify-center text-gray-600">
<i class="ri-bank-card-fill ri-xl"></i>
</div>
</div>
</div>
</div>
<div>
<div class="bg-gray-50 p-8 rounded-lg shadow-sm">
<form>
<div class="mb-6">
<label for="nombre" class="block text-sm font-medium text-gray-700 mb-2">Nombre completo</label>
<input type="text" id="nombre" class="w-full px-4 py-3 border border-gray-300 rounded focus:ring-primary focus:border-primary text-sm" placeholder="Ingresa tu nombre completo">
</div>
<div class="mb-6">
<label for="email" class="block text-sm font-medium text-gray-700 mb-2">Correo electrónico</label>
<input type="email" id="email" class="w-full px-4 py-3 border border-gray-300 rounded focus:ring-primary focus:border-primary text-sm" placeholder="ejemplo@correo.com">
</div>
<div class="mb-6">
<label for="telefono" class="block text-sm font-medium text-gray-700 mb-2">Teléfono</label>
<input type="tel" id="telefono" class="w-full px-4 py-3 border border-gray-300 rounded focus:ring-primary focus:border-primary text-sm" placeholder="+593 XX XXX XXXX">
</div>
<div class="mb-6">
<label for="curso" class="block text-sm font-medium text-gray-700 mb-2">Curso de interés</label>
<div class="relative">
<select id="curso" class="w-full px-4 py-3 border border-gray-300 rounded focus:ring-primary focus:border-primary appearance-none text-sm pr-8">
<option value="" disabled selected>Selecciona un curso</option>
<option value="cp1">Fundamentos de Contratación Pública</option>
<option value="cp2">Gestión de Licitaciones Públicas</option>
<option value="cp3">Contratación Pública Avanzada</option>
<option value="imp1">Declaración de IVA</option>
<option value="imp2">Sistema SRI en Línea</option>
<option value="imp3">Planificación Tributaria</option>
<option value="ia1">Introducción a la IA</option>
<option value="ia2">IA Práctica para Negocios</option>
<option value="ia3">Data Science y Machine Learning</option>
</select>
<div class="absolute inset-y-0 right-0 flex items-center pr-3 pointer-events-none">
<i class="ri-arrow-down-s-line text-gray-400"></i>
</div>
</div>
</div>
<div class="mb-8">
<label class="custom-checkbox">
<input type="checkbox">
<span class="checkmark"></span>
<span class="text-sm text-gray-600 ml-2">Acepto recibir información sobre cursos y promociones</span>
</label>
</div>
<button type="submit" class="w-full bg-primary text-white py-3 !rounded-button font-medium whitespace-nowrap hover:bg-blue-600 transition duration-300">Solicitar Información</button>
<p class="text-xs text-gray-500 mt-4 text-center">Al enviar este formulario, aceptas nuestra <a href="#" class="text-primary hover:underline">Política de Privacidad</a> y <a href="#" class="text-primary hover:underline">Términos de Servicio</a>.</p>
</form>
</div>
</div>
</div>
</div>
</section>
<!-- Footer -->
<footer class="bg-gray-900 text-white pt-16 pb-8">
<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
<div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
<div>
<a href="#" class="text-2xl font-['Pacifico'] text-white mb-6 block">logo</a>
<p class="text-gray-400 mb-6">Formación profesional de calidad para impulsar tu carrera en áreas estratégicas del mercado laboral actual.</p>
<div class="flex space-x-4">
<a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-primary transition duration-300">
<i class="ri-facebook-fill"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-primary transition duration-300">
<i class="ri-twitter-x-fill"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-primary transition duration-300">
<i class="ri-instagram-fill"></i>
</a>
<a href="#" class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center hover:bg-primary transition duration-300">
<i class="ri-linkedin-fill"></i>
</a>
</div>
</div>
<div>
<h3 class="text-lg font-semibold mb-6">Enlaces Rápidos</h3>
<ul class="space-y-3">
<li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Inicio</a></li>
<li><a href="#cursos-compras" class="text-gray-400 hover:text-white transition duration-300">Compras Públicas</a></li>
<li><a href="#cursos-impuestos" class="text-gray-400 hover:text-white transition duration-300">Impuestos</a></li>
<li><a href="#cursos-ia" class="text-gray-400 hover:text-white transition duration-300">Inteligencia Artificial</a></li>
<li><a href="#precios" class="text-gray-400 hover:text-white transition duration-300">Planes y Precios</a></li>
<li><a href="#testimonios" class="text-gray-400 hover:text-white transition duration-300">Testimonios</a></li>
</ul>
</div>
<div>
<h3 class="text-lg font-semibold mb-6">Contacto</h3>
<ul class="space-y-3">
<li class="flex items-start">
<i class="ri-map-pin-line mt-1 mr-3 text-primary"></i>
<span class="text-gray-400">Av. Amazonas N36-152, Quito, Ecuador</span>
</li>
<li class="flex items-start">
<i class="ri-phone-line mt-1 mr-3 text-primary"></i>
<span class="text-gray-400">+593 2 394 8760</span>
</li>
<li class="flex items-start">
<i class="ri-mail-line mt-1 mr-3 text-primary"></i>
<span class="text-gray-400">info@academiaformacion.ec</span>
</li>
<li class="flex items-start">
<i class="ri-time-line mt-1 mr-3 text-primary"></i>
<span class="text-gray-400">Lun - Vie: 8:30 AM - 6:00 PM</span>
</li>
</ul>
</div>
<div>
<h3 class="text-lg font-semibold mb-6">Boletín Informativo</h3>
<p class="text-gray-400 mb-4">Suscríbete para recibir noticias, actualizaciones y ofertas especiales.</p>
<form class="mb-4">
<div class="flex">
<input type="email" placeholder="Tu correo electrónico" class="w-full px-4 py-2 border-none !rounded-l-button focus:ring-0 text-gray-900 text-sm">
<button type="submit" class="bg-primary text-white px-4 !rounded-r-button !rounded-l-none hover:bg-blue-600 transition duration-300 whitespace-nowrap">Suscribirse</button>
</div>
</form>
<div>
<h4 class="text-sm font-semibold mb-3 text-gray-300">Certificaciones</h4>
<div class="flex space-x-4">
<div class="w-12 h-12 bg-gray-800 rounded flex items-center justify-center">
<i class="ri-government-line ri-lg text-gray-400"></i>
</div>
<div class="w-12 h-12 bg-gray-800 rounded flex items-center justify-center">
<i class="ri-building-4-line ri-lg text-gray-400"></i>
</div>
<div class="w-12 h-12 bg-gray-800 rounded flex items-center justify-center">
<i class="ri-award-line ri-lg text-gray-400"></i>
</div>
</div>
</div>
</div>
</div>
<div class="border-t border-gray-800 pt-8">
<div class="flex flex-col md:flex-row justify-between items-center">
<p class="text-gray-400 text-sm mb-4 md:mb-0">© 2025 Academia de Formación Profesional. Todos los derechos reservados.</p>
<div class="flex space-x-6">
<a href="#" class="text-gray-400 hover:text-white text-sm">Términos y Condiciones</a>
<a href="#" class="text-gray-400 hover:text-white text-sm">Política de Privacidad</a>
<a href="#" class="text-gray-400 hover:text-white text-sm">Política de Cookies</a>
</div>
</div>
</div>
</div>
</footer>
</body>
</html>
