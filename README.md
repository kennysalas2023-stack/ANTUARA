<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ANTUARA — El Tiempo Esculpido en los Andes</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Fuentes Editoriales de Lujo -->
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600&family=Plus+Jakarta+Sans:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #0d0c0a;
      color: #f5f2eb;
      font-family: 'Plus Jakarta Sans', sans-serif;
      overflow-x: hidden;
    }
    .font-serif-luxury {
      font-family: 'Cormorant Garamond', serif;
    }
    /* Canvas fijo de fondo como en el video */
    #webgl-canvas {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      object-fit: cover;
      z-index: -2;
    }
    /* Degradado lateral para asegurar lectura de textos */
    .vignette-overlay {
      position: fixed;
      inset: 0;
      background: linear-gradient(90deg, rgba(13,12,10,0.75) 0%, rgba(13,12,10,0.2) 55%, rgba(13,12,10,0.4) 100%);
      z-index: -1;
      pointer-events: none;
    }
    .step-section {
      height: 100vh;
      display: flex;
      align-items: flex-end;
      padding: 4rem 5rem;
      opacity: 0;
      filter: blur(10px);
      transform: translateY(30px);
      transition: all 0.8s cubic-bezier(0.16, 1, 0.3, 1);
    }
    .step-section.active {
      opacity: 1;
      filter: blur(0px);
      transform: translateY(0px);
    }
  </style>
</head>
<body>

  <!-- Fondo de Video / Secuencia de Imágenes -->
  <canvas id="webgl-canvas"></canvas>
  <div class="vignette-overlay"></div>

  <!-- Header Fijo (HUD Minimalista) -->
  <header class="fixed top-0 left-0 w-full flex justify-between items-center px-12 py-6 z-50 text-xs tracking-[0.25em] uppercase border-b border-white/10 backdrop-blur-sm">
    <div class="font-semibold text-sm tracking-[0.35em]">ANTUARA</div>
    <nav class="hidden md:flex gap-8 text-white/70">
      <a href="#s1" class="hover:text-white transition">Origen</a>
      <a href="#s2" class="hover:text-white transition">Santuario</a>
      <a href="#s3" class="hover:text-white transition">Artesanía</a>
      <a href="#s4" class="hover:text-white transition">Colección</a>
    </nav>
    <div class="text-white/60">13°31′S 71°58′W • CUSCO</div>
  </header>

  <!-- Contenedor de Scroll (4 Estaciones) -->
  <main class="relative z-10">

    <!-- ESTACIÓN 1: HERO (Equivalente a "VILLA MARAVILHA") -->
    <section id="s1" class="step-section active">
      <div class="max-w-2xl">
        <p class="text-xs uppercase tracking-[0.3em] text-amber-200/80 mb-2">Alta Relojería Artesanal • Cusco, Perú</p>
        <h1 class="font-serif-luxury text-6xl md:text-8xl tracking-wide leading-none mb-4">ANTUARA<br>ANDES</h1>
        <p class="text-sm text-white/75 font-light max-w-md">
          Piezas únicas talladas en maderas nobles certificadas, diseñadas para quienes valoran el tiempo con historia e identidad.
        </p>
      </div>
    </section>

    <!-- ESTACIÓN 2: VISTA AÉREA (Equivalente a "BETWEEN SEA AND CENOTE") -->
    <section id="s2" class="step-section">
      <div class="max-w-xl">
        <p class="text-xs uppercase tracking-[0.3em] text-amber-200/80 mb-2">01 / Origen Sostenible</p>
        <h2 class="font-serif-luxury text-5xl md:text-7xl leading-none mb-6">ENTRE EL BOSQUE<br>Y LA PIEDRA INCA</h2>
        <div class="space-y-3 text-xs tracking-widest uppercase border-t border-white/20 pt-4">
          <div class="flex justify-between py-2 border-b border-white/10"><span>Material</span><span class="text-amber-200">100% Hipoalergénico (Libre de Níquel)</span></div>
          <div class="flex justify-between py-2 border-b border-white/10"><span>Grabado Láser</span><span class="text-amber-200">Iconografía de Sacsayhuamán</span></div>
          <div class="flex justify-between py-2 border-b border-white/10"><span>Peso en Muñeca</span><span class="text-amber-200">Ultraligero — 35 Gramos</span></div>
        </div>
      </div>
    </section>

    <!-- ESTACIÓN 3: ACERCAMIENTO (Equivalente a "THE GARDEN ARRIVAL") -->
    <section id="s3" class="step-section">
      <div class="w-full flex flex-col md:flex-row justify-between items-end gap-8">
        <div class="max-w-xl">
          <p class="text-xs uppercase tracking-[0.3em] text-amber-200/80 mb-2">02 / Ingeniería & Precisión</p>
          <h2 class="font-serif-luxury text-5xl md:text-7xl leading-none mb-4">EL CORAZÓN<br>DEL TALLER</h2>
          <p class="text-sm text-white/75 font-light">
            Maquinaria de cuarzo japonés ensamblada a mano en Cusco, protegida dentro de un estuche de madera tallada de colección.
          </p>
        </div>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-6 text-xs border-t border-white/20 pt-4 w-full md:w-auto">
          <div><span class="block text-white/50">MOVIMIENTO</span>Cuarzo Japonés</div>
          <div><span class="block text-white/50">RETIRO EN TIENDA</span>Click & Collect Cusco</div>
          <div><span class="block text-white/50">CAMBIOS</span>Sistema BORIS</div>
          <div><span class="block text-white/50">GARANTÍA</span>Logística Inversa</div>
        </div>
      </div>
    </section>

    <!-- ESTACIÓN 4: INTERIOR Y PALETA DE MATERIALES (Equivalente a "NOON INTERIOR") -->
    <section id="s4" class="step-section">
      <div class="w-full flex flex-col md:flex-row justify-between items-end gap-8">
        <div class="max-w-xl">
          <p class="text-xs uppercase tracking-[0.3em] text-amber-200/80 mb-2">03 / Paleta de Maderas Nobles</p>
          <h2 class="font-serif-luxury text-5xl md:text-7xl leading-none mb-4">DISEÑO<br>BUSINESS-QUARTZ</h2>
          <p class="text-sm text-white/75 font-light mb-6">
            Cada veta es irrepetible. Selecciona el tono de madera y personaliza el reverso con grabado láser.
          </p>
          <!-- Selector de Materiales como en el segundo 0:14 del video -->
          <div class="flex gap-3">
            <div class="w-16 h-16 rounded bg-[#3b281e] border border-white/40 p-2 flex items-end text-[10px] cursor-pointer hover:scale-105 transition">Nogal</div>
            <div class="w-16 h-16 rounded bg-[#c8a165] border border-white/20 p-2 flex items-end text-[10px] text-black font-medium cursor-pointer hover:scale-105 transition">Bambú</div>
            <div class="w-16 h-16 rounded bg-[#7a3b2e] border border-white/20 p-2 flex items-end text-[10px] cursor-pointer hover:scale-105 transition">Caspi</div>
            <div class="w-16 h-16 rounded bg-[#1c1917] border border-white/20 p-2 flex items-end text-[10px] cursor-pointer hover:scale-105 transition">Ébano</div>
          </div>
        </div>

        <a href="https://wa.me/51900000000" target="_blank" class="px-8 py-4 bg-[#f5f2eb] text-black text-xs uppercase tracking-[0.25em] font-medium hover:bg-amber-200 transition">
          Reservar Pieza • S/. 500.00
        </a>
      </div>
    </section>

  </main>

  <!-- Librerías GSAP + ScrollTrigger + Lenis -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/gsap.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/ScrollTrigger.min.js"></script>
  <script src="https://unpkg.com/@studio-freight/lenis@1.0.42/dist/lenis.min.js"></script>

  <script>
    // 1. Inicializar Scroll Suave (Lenis)
    const lenis = new Lenis({ duration: 1.4, smoothWheel: true });
    function raf(time) {
      lenis.raf(time);
      requestAnimationFrame(raf);
    }
    requestAnimationFrame(raf);

    // 2. Activar las secciones con efecto Blur al hacer Scroll
    const sections = document.querySelectorAll('.step-section');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('active');
        } else {
          entry.target.classList.remove('active');
        }
      });
    }, { threshold: 0.45 });

    sections.forEach(section => observer.observe(section));
  </script>
</body>
</html>
