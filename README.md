<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Colorimetría y Huerto Escolar</title>

  <!-- AOS Animation Library -->
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet" />
  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>

  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f9;
      color: #333;
    }
    header {
      background: #4CAF50;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    /* Menu */
    .menu-toggle {
      display: none;
      flex-direction: column;
      cursor: pointer;
    }
    .menu-toggle span {
      background: white;
      height: 4px;
      width: 25px;
      margin: 4px 0;
      border-radius: 2px;
    }
    nav {
      background: #2e7d32;
      color: white;
      padding: 0.5rem 1rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .nav-links {
      display: flex;
      gap: 1rem;
    }
    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    @media (max-width: 600px) {
      .menu-toggle {
        display: flex;
      }
      .nav-links {
        display: none;
        flex-direction: column;
        background: #2e7d32;
        width: 100%;
        text-align: center;
      }
      .nav-links.active {
        display: flex;
      }
    }

    section {
      padding: 2rem;
    }
    h2 {
      color: #4CAF50;
    }
    .container {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
    }
    .card {
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      padding: 1rem;
      flex: 1 1 300px;
    }
    .card img {
      max-width: 100%;
      border-radius: 5px;
      margin-top: 0.5rem;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card img:hover {
      transform: scale(1.05);
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #333;
      color: white;
      margin-top: 2rem;
    }
  </style>
</head>
<body>

<header>
  <h1>Colorimetría y Huerto Escolar</h1>
</header>

<nav>
  <div class="menu-toggle" onclick="toggleMenu()">
    <span></span>
    <span></span>
    <span></span>
  </div>
  <div class="nav-links" id="menu">
    <a href="#colorimetria">Colorimetría</a>
    <a href="#huerto">Huerto</a>
  </div>
</nav>

<section id="colorimetria">
  <h2>1. Colorimetría</h2>
  <p>Se analizan las prendas típicas de tres regiones mexicanas según sus gamas cromáticas: colores fríos y cálidos.</p>

  <div class="container">
    <div class="card" data-aos="fade-up">
      <h3>Mocorito, Sinaloa</h3>
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/86/Traje_t%C3%ADpico_de_Sinaloa.jpg" alt="Prenda típica de Sinaloa">
      <p><strong>Colores cálidos:</strong> Rojo, amarillo, naranja.<br>
      <strong>Colores fríos:</strong> Verde, azul marino.</p>
    </div>

    <div class="card" data-aos="fade-up">
      <h3>Minatitlán, Veracruz</h3>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Traje_tipico_veracruz.jpg/800px-Traje_tipico_veracruz.jpg" alt="Prenda típica de Veracruz">
      <p><strong>Colores cálidos:</strong> Rojo cereza, rosa mexicano.<br>
      <strong>Colores fríos:</strong> Azul turquesa, verde esmeralda.</p>
    </div>

    <div class="card" data-aos="fade-up">
      <h3>Choapam, Oaxaca</h3>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/Traje_tipico_de_Oaxaca.jpg/800px-Traje_tipico_de_Oaxaca.jpg" alt="Prenda típica de Oaxaca">
      <p><strong>Colores cálidos:</strong> Amarillo oro, fucsia, rojo.<br>
      <strong>Colores fríos:</strong> Azul cobalto, verde botella.</p>
    </div>
  </div>
</section>

<section id="huerto">
  <h2>2. Huerto Escolar</h2>
  <p>Simulación de actividades realizadas en un huerto escolar con cultivo de <strong>cilantro</strong> y otros cultivos complementarios como lechuga y rábano.</p>

  <div class="container">
    <div class="card" data-aos="fade-up">
      <h3>Datos de germinación</h3>
      <ul>
        <li><strong>Cilantro</strong> - <em>Coriandrum sativum</em><br>Germinación: 7-10 días | Temp: 18°C-25°C</li>
        <li><strong>Lechuga</strong> - <em>Lactuca sativa</em><br>Germinación: 4-7 días | Temp: 15°C-22°C</li>
        <li><strong>Rábano</strong> - <em>Raphanus sativus</em><br>Germinación: 3-6 días | Temp: 16°C-28°C</li>
      </ul>
    </div>

    <div class="card" data-aos="fade-up">
      <h3>Tiempo de cosecha</h3>
      <p><strong>Cilantro:</strong> 45-70 días<br>
         <strong>Lechuga:</strong> 55-70 días<br>
         <strong>Rábano:</strong> 25-35 días</p>
      <img src="https://upload.wikimedia.org/wikipedia/commons/f/f6/Lettuce_leaves.jpg" alt="Lechuga">
      <img src="https://upload.wikimedia.org/wikipedia/commons/5/56/Radishes.jpg" alt="Rábanos">
    </div>

    <div class="card" data-aos="fade-up">
      <h3>Actividades realizadas</h3>
      <ul>
        <li>Preparación del terreno con herramientas manuales</li>
        <li>Distribución de camas de cultivo</li>
        <li>Siembra directa de semillas</li>
        <li>Rotulación y monitoreo semanal</li>
        <li>Uso de fertilizantes orgánicos</li>
        <li>Evaluación de crecimiento y registro de datos</li>
      </ul>
      <img src="https://upload.wikimedia.org/wikipedia/commons/4/40/School_garden_Melbourne.jpg" alt="Huerto escolar">
    </div>
  </div>
</section>

<footer>
  <p>Créditos: José Antonio López Bartolo</p>
</footer>

<script>
  AOS.init();
  function toggleMenu() {
    const menu = document.getElementById('menu');
    menu.classList.toggle('active');
  }
</script>

</body>
</html>
