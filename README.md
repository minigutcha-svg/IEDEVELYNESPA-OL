<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Macro Currículo: Lengua Castellana</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }
        
        /* Estilos para flip cards */
        .flip-card {
            perspective: 1000px;
            height: 180px;
            cursor: pointer;
        }
        .flip-card-inner {
            position: relative;
            width: 100%;
            height: 100%;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        .flip-card:hover .flip-card-inner,
        .flip-card.flipped .flip-card-inner {
            transform: rotateY(180deg);
        }
        .flip-card-front, .flip-card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 1.5rem;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
        }
        .flip-card-back {
            transform: rotateY(180deg);
        }
        
        /* Estilos para tabla de criterios */
        .criteria-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            gap: 10px;
        }
        
        .criteria-item {
            background: white;
            border-radius: 8px;
            padding: 12px 8px;
            text-align: center;
            font-weight: 600;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .criteria-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 4px 8px rgba(0,0,0,0.15);
        }
        
        .criteria-adquisicion {
            background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%);
            color: white;
        }
        
        .criteria-profundizacion {
            background: linear-gradient(135deg, #10b981 0%, #047857 100%);
            color: white;
        }
        
        .criteria-transferencia {
            background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);
            color: white;
        }
        
        /* Estilos para navegación rápida */
        .nav-card {
            transition: all 0.3s ease;
        }
        
        .nav-card:hover {
            transform: translateY(-5px);
        }
        
        /* Badge para Banda */
        .banda-badge {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.7; }
            100% { opacity: 1; }
        }
    </style>
</head>
<body class="gradient-bg min-h-screen p-4 sm:p-6 lg:p-8">
    <div class="w-full max-w-7xl mx-auto bg-white rounded-2xl shadow-2xl p-6 sm:p-8 md:p-12">

        <!-- TÍTULO PRINCIPAL -->
        <header class="text-center mb-10 md:mb-16">
            <h1 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-800 tracking-tight">MACRO CURRÍCULO LENGUA CASTELLANA</h1>
            <p class="mt-2 text-lg sm:text-xl text-gray-600">IED EVELYN ABUCHAIBE DE DAES</p>
        </header>

        <!-- MISIÓN DEL DEPARTAMENTO -->
        <div class="mb-12">
            <h2 class="font-semibold text-teal-800 text-xl mb-3 text-center">Misión del Departamento</h2>
            <div class="bg-teal-50 border-2 border-teal-200 rounded-xl p-6">
                <p class="text-gray-700 text-center italic">
                    "PORQUE la misión institucional nos encarga desarrollar autonomía, pensamiento crítico y la capacidad de crear soluciones sostenibles a retos locales y globales, EL DEPARTAMENTO DE Lengua Castellana desarrolla la competencia comunicativa experta en la lengua materna, PARA que los estudiantes usen el lenguaje como una herramienta de precisión para investigar, construir argumentos, colaborar y liderar proyectos de impacto en su comunidad".
                </p>
            </div>
        </div>

        <!-- NAVEGACIÓN RÁPIDA -->
        <div class="mb-12">
            <h2 class="text-2xl font-bold text-gray-800 mb-6 text-center">Navegación Rápida</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <a href="#vision" class="nav-card bg-yellow-50 hover:bg-yellow-100 p-4 rounded-lg text-center transition-all duration-300 border-2 border-yellow-200">
                    <i class="fas fa-lightbulb text-yellow-500 text-xl mb-2"></i>
                    <p class="font-semibold text-yellow-700">Visión</p>
                </a>
                <a href="#lentes" class="nav-card bg-blue-50 hover:bg-blue-100 p-4 rounded-lg text-center transition-all duration-300 border-2 border-blue-200">
                    <i class="fas fa-search text-blue-500 text-xl mb-2"></i>
                    <p class="font-semibold text-blue-700">Lentes</p>
                </a>
                <a href="#grandes-ideas" class="nav-card bg-teal-50 hover:bg-teal-100 p-4 rounded-lg text-center transition-all duration-300 border-2 border-teal-200">
                    <i class="fas fa-brain text-teal-500 text-xl mb-2"></i>
                    <p class="font-semibold text-teal-700">Grandes Ideas</p>
                </a>
                <a href="#unidades" class="nav-card bg-purple-50 hover:bg-purple-100 p-4 rounded-lg text-center transition-all duration-300 border-2 border-purple-200">
                    <i class="fas fa-book-open text-purple-500 text-xl mb-2"></i>
                    <p class="font-semibold text-purple-700">Unidades</p>
                </a>
            </div>
        </div>

        <!-- VISIÓN DE LA DISCIPLINA -->
        <div id="vision" class="mt-12 mb-20">
            <h2 class="font-semibold text-yellow-800 text-2xl mb-6 text-center">Visión de la Disciplina: ¿Por Qué el Lenguaje? 💡</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 text-center min-h-[250px]">
                
                <!-- Tarjeta 1: Dar Poder -->
                <div class="flip-card col-span-1" onclick="this.classList.toggle('flipped')">
                    <div class="flip-card-inner">
                        <div class="flip-card-front bg-yellow-50 border-2 border-yellow-200">
                            <svg class="h-10 w-10 text-yellow-600 mx-auto mb-3" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0zM10 7v3m0 0v3m0-3h3m-3 0H7"/></svg>
                            <h3 class="font-bold text-yellow-900 text-xl">Dar Poder</h3>
                            <p class="text-xs text-gray-600 mt-2 italic font-medium">Haz clic para descubrir la visión</p>
                        </div>
                        <div class="flip-card-back bg-yellow-100 border-2 border-yellow-300">
                            <p class="text-sm text-gray-700 font-medium mt-1">El lenguaje se convierte en su herramienta para **pensar, cuestionar y construir sentido**, para expresar su voz con claridad, empatía y propósito.</p>
                        </div>
                    </div>
                </div>

                <!-- Tarjeta 2: Inspirar -->
                <div class="flip-card col-span-1" onclick="this.classList.toggle('flipped')">
                    <div class="flip-card-inner">
                        <div class="flip-card-front bg-yellow-50 border-2 border-yellow-200">
                           <svg class="h-10 w-10 text-yellow-600 mx-auto mb-3" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" /></svg>
                           <h3 class="font-bold text-yellow-900 text-xl">Inspirar</h3>
                           <p class="text-xs text-gray-600 mt-2 italic font-medium">Haz clic para descubrir la visión</p>
                        </div>
                        <div class="flip-card-back bg-yellow-100 border-2 border-yellow-300">
                            <p class="text-sm text-gray-700 font-medium mt-1">Les inspira al revelar cómo las **palabras, las historias y los discursos** moldean nuestra comprensión de nosotros mismos, de los demás y de la sociedad.</p>
                        </div>
                    </div>
                </div>

                <!-- Tarjeta 3: Formar a Futuro -->
                <div class="flip-card col-span-1" onclick="this.classList.toggle('flipped')">
                    <div class="flip-card-inner">
                        <div class="flip-card-front bg-yellow-50 border-2 border-yellow-200">
                            <svg class="h-10 w-10 text-yellow-600 mx-auto mb-3" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v.01M12 6v-1m0-1V4m0 2.01V8m0 0h.01M12 5h.01M12 5h-.01M12 8h.01M12 8h-.01M12 5h.01M12 5h-.01" /></svg>
                            <h3 class="font-bold text-yellow-900 text-xl">Formar a Futuro</h3>
                            <p class="text-xs text-gray-600 mt-2 italic font-medium">Haz clic para descubrir la visión</p>
                        </div>
                        <div class="flip-card-back bg-yellow-100 border-2 border-yellow-300">
                            <p class="text-sm text-gray-700 font-medium mt-1">Esperamos que continúen **leyendo el mundo con mirada crítica y sensible**, comunicándose con rigor y respeto, y usando su voz para defender la verdad, la justicia y la dignidad humana.</p>
                        </div>
                    </div>
                </div>

                <!-- Tarjeta 4: Transformar con Ética -->
                <div class="flip-card col-span-1" onclick="this.classList.toggle('flipped')">
                    <div class="flip-card-inner">
                        <div class="flip-card-front bg-yellow-50 border-2 border-yellow-200">
                            <svg class="h-10 w-10 text-yellow-600 mx-auto mb-3" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" > <path stroke-linecap="round" stroke-linejoin="round" d="M13 10V3L4 14h7v7l9-11h-7z" /> </svg>
                            <h3 class="font-bold text-yellow-900 text-xl">Transformar con Ética</h3>
                            <p class="text-xs text-gray-600 mt-2 italic font-medium">Haz clic para descubrir la visión</p>
                        </div>
                        <div class="flip-card-back bg-yellow-100 border-2 border-yellow-300">
                            <p class="text-sm text-gray-700 font-medium mt-1">Les invita a usar el lenguaje como **fuerza creadora y responsable**, consciente de que toda palabra tiene impacto ético y potencial para la transformación.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- LENTES CONCEPTUALES -->
        <div id="lentes" class="mt-20 mb-12 md:mb-20">
            <h2 class="text-3xl sm:text-4xl font-bold text-gray-800 text-center mb-10">Lentes Conceptuales</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Lente 1: La Lupa -->
                <div class="bg-blue-50 border-2 border-blue-200 rounded-xl p-6 text-center transform hover:scale-105 transition-transform duration-300">
                    <div class="flex justify-center mb-4">
                        <svg class="h-16 w-16 text-blue-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
                        </svg>
                    </div>
                    <h2 class="text-2xl font-bold text-blue-800 mb-2">La Lupa 🔎</h2>
                    <h3 class="text-lg font-semibold text-blue-700 mb-4">Construcción de Significado (CS)</h3>
                    <p class="text-gray-700 mb-4">Nos permite mirar **DENTRO** del texto para analizar las elecciones del autor (palabras, estructura, imágenes) y entender **CÓMO** funciona el mensaje.</p>
                    <div class="bg-blue-100 rounded-lg p-3 mt-3">
                        <p class="text-sm text-blue-800 font-medium">Se usa para leer un artículo científico, una infografía, una columna de opinión o un meme.</p>
                    </div>
                </div>
    
                <!-- Lente 2: La Brújula -->
                <div class="bg-green-50 border-2 border-green-200 rounded-xl p-6 text-center transform hover:scale-105 transition-transform duration-300">
                    <div class="flex justify-center mb-4">
                        <svg class="h-16 w-16 text-green-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9 9 0 1 0 0-18 9 9 0 0 0 0 18Z" />
                            <path stroke-linecap="round" stroke-linejoin="round" d="M12 3v2.25m0 13.5V21M3.75 12H6m12 0h2.25M5.106 5.106l1.768 1.768m10.26 10.26 1.768 1.768M5.106 18.894l1.768-1.768m10.26-10.26 1.768-1.768" />
                            <path stroke-linecap="round" stroke-linejoin="round" d="m15 12-3 9-3-9 3-9 3 9Z" />
                        </svg>
                    </div>
                    <h2 class="text-2xl font-bold text-green-800 mb-2">La Brújula 🧭</h2>
                    <h3 class="text-lg font-semibold text-green-700 mb-4">Propósito y Audiencia (PA)</h3>
                    <p class="text-gray-700 mb-4">Nos ayuda a orientar la comunicación y mirar **HACIA ADELANTE**, definiendo **PARA QUÉ** creamos un mensaje y **PARA QUIÉN** es, adaptándolo para ser efectivo.</p>
                    <div class="bg-green-100 rounded-lg p-3 mt-3">
                        <p class="text-sm text-green-800 font-medium">Se activa al redactar una petición comunitaria, un correo formal, un informe académico o un guión.</p>
                    </div>
                </div>
    
                <!-- Lente 3: El Mapa -->
                <div class="bg-yellow-50 border-2 border-yellow-200 rounded-xl p-6 text-center transform hover:scale-105 transition-transform duration-300">
                    <div class="flex justify-center mb-4">
                           <svg class="h-16 w-16 text-yellow-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M9 6.75V15m6-6v8.25m.503-6.998 4.277-1.948a.75.75 0 0 1 .966.966l-1.948 4.277M6.75 18.25h8.25a.75.75 0 0 0 .75-.75V9a.75.75 0 0 0-.75-.75H6.75a.75.75 0 0 0-.75.75v8.5c0 .414.336.75.75.75Z" />
                            </svg>
                    </div>
                    <h2 class="text-2xl font-bold text-yellow-800 mb-2">El Mapa 🗺️</h2>
                    <h3 class="text-lg font-semibold text-yellow-700 mb-4">Contexto e Interpretación (CI)</h3>
                    <p class="text-gray-700 mb-4">Nos permite ver el panorama completo, mirando **ALREDEDOR** del texto para entender cómo la cultura, la época, el lugar y las perspectivas influyen en **QUÉ** significa.</p>
                    <div class="bg-yellow-100 rounded-lg p-3 mt-3">
                        <p class="text-sm text-yellow-800 font-medium">Permite interpretar noticias, discursos públicos, narrativas culturales e interacciones en redes sociales.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- GRANDES IDEAS -->
        <div id="grandes-ideas" class="bg-teal-50 border-2 border-teal-200 rounded-xl p-8 mb-12 md:mb-20">
            <header class="text-center mb-10">
                <h2 class="text-3xl sm:text-4xl font-bold text-teal-800 tracking-tight">GRANDES IDEAS</h2>
                <p class="mt-3 text-lg text-teal-700 max-w-3xl mx-auto">Son las comprensiones profundas que conectan las Grandes Ideas Institucionales con la disciplina del Lenguaje.</p>
            </header>
            <div class="grid grid-cols-1 gap-6">
                <!-- GI 1 -->
                <div class="bg-white p-6 rounded-lg border border-teal-200">
                    <div class="flex items-start">
                        <div class="flex-shrink-0 mr-4">
                            <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center">
                                <span class="text-blue-600 font-bold text-lg">GI 1</span>
                            </div>
                        </div>
                        <div>
                            <h3 class="font-bold text-gray-800 text-xl mb-3">El significado se construye mediante decisiones de autor y nuestras interpretaciones.</h3>
                            <p class="text-gray-700 mb-4">Comprender implica analizar cómo está hecho un texto y cómo distintos lectores interpretan ese significado desde sus experiencias, identidades y marcos culturales.</p>
                        </div>
                    </div>
                </div>

                <!-- GI 2 -->
                <div class="bg-white p-6 rounded-lg border border-teal-200">
                    <div class="flex items-start">
                        <div class="flex-shrink-0 mr-4">
                            <div class="w-12 h-12 bg-green-100 rounded-full flex items-center justify-center">
                                <span class="text-green-600 font-bold text-lg">GI 2</span>
                            </div>
                        </div>
                        <div>
                            <h3 class="font-bold text-gray-800 text-xl mb-3">Toda comunicación depende del propósito y la audiencia.</h3>
                            <p class="text-gray-700 mb-4">Los mensajes con impacto son el resultado de decisiones estratégicas y conscientes.</p>
                        </div>
                    </div>
                </div>

                <!-- GI 3 -->
                <div class="bg-white p-6 rounded-lg border border-teal-200">
                    <div class="flex items-start">
                        <div class="flex-shrink-0 mr-4">
                            <div class="w-12 h-12 bg-yellow-100 rounded-full flex items-center justify-center">
                                <span class="text-yellow-600 font-bold text-lg">GI 3</span>
                            </div>
                        </div>
                        <div>
                            <h3 class="font-bold text-gray-800 text-xl mb-3">Todo texto está situado en un contexto cultural que condiciona su significado.</h3>
                            <p class="text-gray-700 mb-4">Los textos nunca aparecen aislados: están atravesados por el tiempo, la cultura, los medios, las identidades y las relaciones de poder.</p>
                        </div>
                    </div>
                </div>

                <!-- GI 4 -->
                <div class="bg-white p-6 rounded-lg border border-teal-200">
                    <div class="flex items-start">
                        <div class="flex-shrink-0 mr-4">
                            <div class="w-12 h-12 bg-purple-100 rounded-full flex items-center justify-center">
                                <span class="text-purple-600 font-bold text-lg">GI 4</span>
                            </div>
                        </div>
                        <div>
                            <h3 class="font-bold text-gray-800 text-xl mb-3">El lenguaje es una herramienta para participar ética y críticamente en lo público.</h3>
                            <p class="text-gray-700 mb-4">Transformar con Ética: Les invita a usar el lenguaje como fuerza creadora y responsable.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- BANCO DE PROBLEMAS AUTÉNTICOS -->
        <div class="bg-gray-800 text-white rounded-xl p-8 mb-12 md:mb-20">
            <header class="text-center mb-10">
                <h2 class="text-3xl sm:text-4xl font-bold text-white tracking-tight">BANCO DE PROBLEMAS AUTÉNTICOS</h2>
                <p class="mt-3 text-lg text-gray-300 max-w-4xl mx-auto">Desafíos reales que conectan aprendizaje con impacto en diferentes escalas</p>
            </header>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                
                <!-- Problema E1 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-blue-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E1</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Comunicación y acción frente al ambiente</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos usar el periodismo para que las comunidades —locales, nacionales e internacionales— comprendan y actúen frente a problemas ambientales críticos?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E2 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-green-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E2</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Desinformación y convivencia democrática</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos educar al público para reconocer y frenar la desinformación que afecta la convivencia en comunidades locales y globales?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E3 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-yellow-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E3</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Preservación de memorias culturales</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos usar la narración, el lenguaje y la tecnología para preservar y difundir memorias culturales en riesgo?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E4 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-purple-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E4</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Narrativas para la convivencia escolar global</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos crear narrativas que transformen climas convivenciales en aulas de Colombia y del mundo?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E5 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-red-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E5</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Comunicación para la salud pública</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos convertirnos en comunicadores de la salud que generen cambios reales en hábitos comunitarios locales, nacionales e internacionales?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E6 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-indigo-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E6</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Redes de lectura y creación entre jóvenes</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos diseñar iniciativas de lectura y creación que conecten a jóvenes lectores de distintas regiones del país y del mundo?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E7 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-pink-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E7</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Mensajes persuasivos para el cambio ambiental</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos crear mensajes persuasivos capaces de cambiar conductas ambientales medibles en diferentes comunidades?</p>
                        </div>
                    </div>
                </div>

                <!-- Problema E8 -->
                <div class="bg-gray-700 p-6 rounded-lg transform hover:scale-105 transition-transform duration-300">
                    <div class="flex items-start mb-4">
                        <div class="flex-shrink-0 w-10 h-10 bg-teal-500 rounded-full flex items-center justify-center mr-4">
                            <span class="text-white font-bold">E8</span>
                        </div>
                        <div>
                            <h3 class="font-bold text-white text-lg mb-2">Vida digital y bienestar</h3>
                            <p class="text-gray-300 text-sm mb-4">¿Cómo podríamos diseñar medios juveniles que ayuden a jóvenes de Colombia y del mundo a equilibrar vida digital y vida real?</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- UNIDADES Y LECCIONES -->
        <div id="unidades" class="mb-20">
            <header class="text-center mb-12">
                <h2 class="text-3xl sm:text-4xl font-bold text-gray-800 tracking-tight">📚 UNIDADES Y LECCIONES</h2>
                <p class="mt-3 text-lg text-gray-600 max-w-3xl mx-auto">
                    Accede a los materiales completos de cada unidad organizados por grado
                </p>
            </header>

            <!-- Unidad 11° Grado -->
            <div class="bg-gradient-to-r from-red-50 to-orange-50 border-2 border-red-200 rounded-2xl p-8 mb-12 transform hover:scale-[1.01] transition-transform duration-300">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center mb-8">
                    <div class="w-full">
                        <!-- Banda y nivel -->
                        <div class="flex items-center mb-4">
                            <div class="inline-flex items-center px-4 py-1 bg-red-500 text-white rounded-full text-sm font-semibold mr-3">
                                <span class="mr-2">🟥</span>
                                Undécimo Grado - Banda 10-11
                            </div>
                            <div class="inline-block px-3 py-1 bg-red-100 text-red-700 rounded-full text-sm font-semibold">
                                Nivel abstracto y estratégico
                            </div>
                        </div>
                        
                        <!-- Título de la unidad -->
                        <h3 class="text-2xl md:text-3xl font-bold text-gray-800 mb-2">
                            Unidad 11°: Dos versiones, un hecho: ¿Quién controla lo que entiendes?
                        </h3>
                        
                        <!-- TDC -->
                        <div class="mb-4">
                            <div class="flex items-start">
                                <span class="font-bold text-red-700 mr-2">TDC:</span>
                                <p class="text-gray-700">Intervención pública con defensa retórica</p>
                            </div>
                            <div class="ml-6 mt-1">
                                <p class="text-gray-600 italic">"Dos versiones, un hecho: ¿Quién controla lo que entiendes?"</p>
                            </div>
                        </div>
                        
                        <!-- Lentes Conceptuales -->
                        <div class="mb-6">
                            <div class="flex items-start">
                                <span class="font-bold text-blue-700 mr-2">Lentes Conceptuales:</span>
                                <div class="flex items-center">
                                    <span class="px-3 py-1 bg-blue-100 text-blue-700 rounded-lg font-medium mr-2">
                                        Construcción de Significado (CS)
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Botón Ver Unidad Completa -->
                    <div class="mt-6 md:mt-0 md:ml-6">
                        <a href="#unidad11-detalle" 
                           class="px-6 py-3 bg-gradient-to-r from-red-500 to-orange-600 text-white rounded-lg font-bold hover:shadow-xl transition-all duration-300 inline-flex items-center whitespace-nowrap">
                            <i class="fas fa-external-link-alt mr-3 text-lg"></i>
                            Ver Unidad Completa
                        </a>
                    </div>
                </div>

                <!-- Criterios de Éxito -->
                <div class="mt-8 pt-6 border-t border-red-200">
                    <h4 class="text-xl font-bold text-gray-700 mb-6 flex items-center">
                        <i class="fas fa-check-circle text-red-500 mr-2"></i>
                        Criterios de Éxito - Niveles de Desarrollo
                    </h4>
                    
                    <!-- Grid de criterios -->
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                        <!-- Criterios de Adquisición -->
                        <div>
                            <h5 class="font-bold text-blue-700 mb-4 flex items-center">
                                <i class="fas fa-layer-group mr-2"></i>
                                Criterios de Adquisición
                            </h5>
                            <div class="criteria-grid">
                                <div class="criteria-item criteria-adquisicion">CEA1</div>
                                <div class="criteria-item criteria-adquisicion">CEA2</div>
                                <div class="criteria-item criteria-adquisicion">CEA3</div>
                                <div class="criteria-item criteria-adquisicion">CEA4</div>
                            </div>
                        </div>

                        <!-- Criterios de Profundización -->
                        <div>
                            <h5 class="font-bold text-green-700 mb-4 flex items-center">
                                <i class="fas fa-chart-line mr-2"></i>
                                Criterios de Profundización
                            </h5>
                            <div class="criteria-grid">
                                <div class="criteria-item criteria-profundizacion">CEP1</div>
                                <div class="criteria-item criteria-profundizacion">CEP2</div>
                                <div class="criteria-item criteria-profundizacion">CEP3</div>
                            </div>
                        </div>

                        <!-- Criterios de Transferencia -->
                        <div>
                            <h5 class="font-bold text-yellow-700 mb-4 flex items-center">
                                <i class="fas fa-exchange-alt mr-2"></i>
                                Criterios de Transferencia
                            </h5>
                            <div class="criteria-grid">
                                <div class="criteria-item criteria-transferencia">CET1</div>
                                <div class="criteria-item criteria-transferencia">CET2</div>
                                <div class="criteria-item criteria-transferencia">CET3</div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Enlace de acceso -->
                <div class="mt-8 pt-6 border-t border-red-200 text-center">
                    <a href="https://drive.google.com/drive/folders/unidad-11" 
                       target="_blank"
                       class="px-8 py-4 bg-gradient-to-r from-red-600 to-orange-700 text-white rounded-xl font-bold text-lg hover:shadow-2xl transition-all duration-300 inline-flex items-center mb-4">
                        <i class="fas fa-folder-open mr-4 text-2xl"></i>
                        Acceder a Materiales Completos de la Unidad
                        <i class="fas fa-arrow-right ml-4"></i>
                    </a>
                    
                    <!-- NUEVO: Cuadro de Asistente de Profesor -->
                    <div class="mt-6 bg-gradient-to-r from-purple-50 to-pink-50 border-2 border-purple-200 rounded-xl p-6">
                        <div class="flex flex-col md:flex-row items-center justify-between">
                            <div class="text-left mb-4 md:mb-0 md:mr-6">
                                <h4 class="text-xl font-bold text-purple-800 mb-2">💼 Asistente de Profesor</h4>
                                <p class="text-gray-700 mb-2">Accede a la planeación completa y recursos didácticos</p>
                                <div class="flex items-center">
                                    <i class="fas fa-link text-purple-500 mr-2"></i>
                                    <span class="text-sm text-gray-600">Disponible para docentes</span>
                                </div>
                            </div>
                            <div class="flex space-x-4">
                                <a href="https://docs.google.com/document/d/1dtDqBZcUFV6uA4jSDpLX5T__hsqVgL7swRVPbS8k5xM/edit?usp=sharing" 
                                   target="_blank"
                                   class="px-6 py-3 bg-gradient-to-r from-purple-500 to-pink-500 text-white rounded-lg font-bold hover:shadow-xl transition-all duration-300 inline-flex items-center">
                                    <i class="fas fa-file-alt mr-3"></i>
                                    Ver Planeación
                                </a>
                                <a href="https://react-j8lfxjrj.stackblitz.io/" 
                                   target="_blank"
                                   class="px-6 py-3 bg-gradient-to-r from-blue-500 to-teal-500 text-white rounded-lg font-bold hover:shadow-xl transition-all duration-300 inline-flex items-center">
                                    <i class="fas fa-chalkboard-teacher mr-3"></i>
                                    Asistente IA
                                </a>
                            </div>
                        </div>
                    </div>
                    
                    <p class="text-gray-500 text-sm mt-3">
                        Contiene: Plan de unidad, actividades, recursos, rúbricas y evaluaciones completas
                    </p>
                </div>
            </div>

        </div>

        <!-- Footer -->
        <footer class="mt-20 pt-8 border-t border-gray-200 text-center">
            <p class="text-gray-600 mb-2">IED Evelyn Abuchaibe de Daes - Departamento de Lengua Castellana</p>
            <p class="text-gray-500 text-sm">© 2024 Macro Currículo STEAM Bilingüe - Todos los derechos reservados</p>
        </footer>

    </div>

    <script>
        // Script para el efecto de flip cards
        document.querySelectorAll('.flip-card').forEach(card => {
            card.addEventListener('click', function() {
                this.classList.toggle('flipped');
            });
        });

        // Navegación suave
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Mostrar detalles de criterios
        document.querySelectorAll('.criteria-item').forEach(item => {
            item.addEventListener('click', function() {
                const criteriaCode = this.textContent;
                let description = '';
                
                if (criteriaCode.startsWith('CEA')) {
                    description = `Criterio de Adquisición ${criteriaCode.substring(3)}\n\nNivel básico de competencia. El estudiante demuestra comprensión inicial y aplicación guiada de los conceptos fundamentales.`;
                } else if (criteriaCode.startsWith('CEP')) {
                    description = `Criterio de Profundización ${criteriaCode.substring(3)}\n\nNivel intermedio de competencia. El estudiante aplica conocimientos en contextos variados con cierta autonomía.`;
                } else if (criteriaCode.startsWith('CET')) {
                    description = `Criterio de Transferencia ${criteriaCode.substring(3)}\n\nNivel avanzado de competencia. El estudiante transfiere conocimientos a situaciones nuevas y complejas con autonomía.`;
                }
                
                alert(`Detalles del criterio ${criteriaCode}:\n\n${description}\n\nConsulte la rúbrica completa para los descriptores específicos por nivel.`);
            });
        });
    </script>
</body>
</html>
