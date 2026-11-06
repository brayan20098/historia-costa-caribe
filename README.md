<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Historia de la Costa Caribe</title>
<meta name="description" content="Conoce la historia, cultura, tradiciones y naturaleza de la Costa Caribe de Nicaragua.">

<style>
:root {
  --navy: #123b2b;
  --teal: #1f6846;
  --gold: #d7b765;
  --cream: #f3f7ef;
  --ink: #18382a;
  --muted: #647568;
  --leaf: #2f8051;
  --mint: #e4f0e4;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  background: var(--cream);
  color: var(--ink);
  font-family: Georgia, serif;
}

button, a {
  cursor: pointer;
}

a {
  text-decoration: none;
  color: inherit;
}

.sans {
  font-family: Arial, sans-serif;
}

/* NAVEGACIÓN */

.top {
  position: sticky;
  top: 0;
  z-index: 100;
  background: var(--navy);
  color: white;
  box-shadow: 0 3px 18px #0002;
}

.bar {
  max-width: 1200px;
  margin: auto;
  padding: 13px 22px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
}

.brand {
  display: flex;
  align-items: center;
  gap: 11px;
  font: 700 12px Arial, sans-serif;
  letter-spacing: 2px;
}

.logo {
  background: var(--gold);
  color: var(--navy);
  border-radius: 50%;
  width: 42px;
  height: 42px;
  display: grid;
  place-items: center;
  font-size: 25px;
}

.nav {
  display: flex;
  gap: 18px;
  flex-wrap: wrap;
}

.nav a {
  font: 700 11px Arial, sans-serif;
  letter-spacing: .6px;
  color: #dce7e2;
}

.nav a:hover {
  color: var(--gold);
}

.menu {
  display: none;
  background: none;
  border: 0;
  color: white;
  font-size: 27px;
}

/* PORTADA */

.hero {
  min-height: 590px;
  background:
    linear-gradient(90deg, #09252bf2 0%, #09252bbd 55%, #09252b55 100%),
    url("https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=2000&q=85");
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  color: white;
}

.hero-inner {
  max-width: 1200px;
  width: 100%;
  margin: auto;
  padding: 80px 25px;
}

.eyebrow {
  font: 700 11px Arial, sans-serif;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: #bd9148;
}

.hero .eyebrow {
  color: #e7c47d;
}

.hero h1 {
  font-size: clamp(42px, 7vw, 76px);
  font-weight: 500;
  line-height: 1.04;
  max-width: 780px;
  margin: 20px 0;
}

.hero h1 em {
  color: #e7c47d;
}

.hero p {
  font: 16px/1.8 Arial, sans-serif;
  max-width: 570px;
  color: #e1e9e5;
}

.btn {
  display: inline-block;
  border: 0;
  border-radius: 30px;
  background: var(--gold);
  color: #17383b;
  padding: 14px 22px;
  font: 700 12px Arial, sans-serif;
  letter-spacing: 1px;
  margin-top: 15px;
}

/* SECCIONES */

.wrap {
  max-width: 1150px;
  margin: auto;
  padding: 70px 24px;
}

.center {
  text-align: center;
  max-width: 720px;
  margin: 0 auto 40px;
}

.center h2,
.section-title {
  font-size: 38px;
  font-weight: 500;
  margin: 12px 0;
}

.lead {
  font: 15px/1.8 Arial, sans-serif;
  color: var(--muted);
}

.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.card {
  background: white;
  border: 1px solid #e9e3d8;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 8px 25px #163d3510;
  transition: .2s;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 15px 32px #163d3520;
}

.card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  display: block;
  background: var(--mint);
}

.card-body {
  padding: 22px;
}

.card h3 {
  font-size: 22px;
  margin: 0 0 10px;
}

.card p {
  font: 14px/1.8 Arial, sans-serif;
  color: var(--muted);
  margin: 0;
}

.band {
  background: #e7f0e3;
}

/* HISTORIA */

.timeline {
  border-left: 2px solid var(--gold);
  padding-left: 25px;
  margin: 35px 0;
}

.event {
  position: relative;
  margin-bottom: 32px;
}

.event:before {
  content: '';
  position: absolute;
  left: -32px;
  top: 5px;
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: var(--gold);
  border: 3px solid var(--cream);
}

.year {
  font: 700 11px Arial, sans-serif;
  letter-spacing: 2px;
  color: #ad813d;
}

.event h3 {
  font-size: 22px;
  margin: 7px 0;
}

.event p {
  font: 14px/1.8 Arial, sans-serif;
  color: var(--muted);
  max-width: 850px;
}

/* BLOQUES CON IMAGEN */

.split {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 42px;
  align-items: center;
}

.split img {
  width: 100%;
  height: 370px;
  object-fit: cover;
  border-radius: 16px;
}

.split p {
  font: 15px/1.9 Arial, sans-serif;
  color: var(--muted);
}

.quote {
  background: var(--navy);
  color: white;
  padding: 35px;
  border-radius: 17px;
  margin-top: 45px;
  font-size: 25px;
  line-height: 1.5;
}

.quote small {
  display: block;
  color: #d9bd85;
  font: 11px Arial, sans-serif;
  letter-spacing: 2px;
  margin-top: 16px;
}

/* GALERÍA */

.gallery {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}

.gallery img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 12px;
  transition: .3s;
}

.gallery img:hover {
  transform: scale(1.02);
}

.gallery img:first-child {
  grid-column: span 2;
  grid-row: span 2;
  height: 452px;
}

/* CUESTIONARIO */

.quiz {
  max-width: 700px;
  margin: auto;
  background: white;
  border-radius: 16px;
  padding: 28px;
  border: 1px solid #e5dfd3;
}

.quiz h3 {
  font-size: 23px;
}

.answers {
  display: grid;
  gap: 10px;
  margin-top: 20px;
}

.answers button {
  padding: 14px;
  border: 1px solid #ddd5c8;
  border-radius: 9px;
  text-align: left;
  background: white;
  font: 14px Arial, sans-serif;
}

.answers button:hover {
  background: #e8f2e7;
}

.answers button:disabled {
  cursor: default;
}

#resultado {
  font: 15px/1.7 Arial, sans-serif;
  margin-top: 20px;
  font-weight: bold;
}

/* PIE DE PÁGINA */

.foot {
  background: var(--navy);
  color: white;
  padding: 45px 24px;
}

.foot-inner {
  max-width: 1150px;
  margin: auto;
}

.foot p {
  font: 13px/1.8 Arial, sans-serif;
  color: #c4d0ca;
  max-width: 700px;
}

.foot a {
  color: #e7c47d;
}

.notice {
  font: 12px/1.7 Arial, sans-serif;
  color: #778;
  padding-top: 15px;
}

@media(max-width:850px) {
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .split {
    grid-template-columns: 1fr;
  }

  .gallery {
    grid-template-columns: repeat(2, 1fr);
  }

  .gallery img:first-child {
    height: 300px;
  }
}

@media(max-width:650px) {
  .bar {
    padding: 12px 16px;
  }

  .menu {
    display: block;
  }

  .nav {
    display: none;
    position: absolute;
    top: 65px;
    left: 0;
    right: 0;
    background: var(--navy);
    padding: 20px;
    flex-direction: column;
    gap: 20px;
  }

  .nav.active {
    display: flex;
  }

  .hero {
    min-height: 540px;
  }

  .hero-inner {
    padding: 65px 22px;
  }

  .grid {
    grid-template-columns: 1fr;
  }

  .center h2,
  .section-title {
    font-size: 31px;
  }

  .wrap {
    padding: 55px 19px;
  }

  .gallery {
    grid-template-columns: 1fr 1fr;
  }

  .gallery img,
  .gallery img:first-child {
    height: 180px;
  }

  .gallery img:first-child {
    grid-column: span 2;
  }
}
</style>
</head>

<body>

<header class="top">
  <div class="bar">

    <div class="brand">
      <div class="logo">✺</div>
      <div>
        HISTORIA DE LA<br>
        <span style="color:#d5ad68">COSTA CARIBE</span>
      </div>
    </div>

    <button class="menu" id="menu" aria-label="Abrir menú">☰</button>

    <nav class="nav" id="nav">
      <a href="#inicio">INICIO</a>
      <a href="#historia">HISTORIA</a>
      <a href="#cultura">CULTURA</a>
      <a href="#naturaleza">NATURALEZA</a>
      <a href="#gastronomia">GASTRONOMÍA</a>
      <a href="#galeria">GALERÍA</a>
    </nav>

  </div>
</header>

<!-- PORTADA -->

<section class="hero" id="inicio">
  <div class="hero-inner">

    <div class="eyebrow">Nicaragua · Región Autónoma de la Costa Caribe Sur</div>

    <h1>
      Historia y cultura de la
      <em>Costa Caribe</em>
    </h1>

    <p>
      Un recorrido por nuestras raíces, nuestra historia, nuestras
      tradiciones y la riqueza natural de una región donde conviven
      diferentes culturas y pueblos.
    </p>

    <a href="#historia" class="btn">DESCUBRIR NUESTRA HISTORIA</a>

  </div>
</section>

<!-- INTRODUCCIÓN -->

<section class="wrap">

  <div class="center">
    <div class="eyebrow">Nuestra identidad</div>
    <h2>Una región llena de historia y diversidad</h2>

    <p class="lead">
      La Costa Caribe de Nicaragua es una región de gran riqueza
      cultural, histórica y natural. Sus comunidades conservan
      tradiciones, lenguas, conocimientos y costumbres que forman
      parte de la identidad del país.
    </p>
  </div>

  <div class="grid">

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=900&q=85"
        alt="Bosque tropical"
        loading="lazy">

      <div class="card-body">
        <h3>Naturaleza</h3>
        <p>
          Bosques tropicales, ríos, lagunas, playas y una gran variedad
          de especies forman parte del patrimonio natural caribeño.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?auto=format&fit=crop&w=900&q=85"
        alt="Mar y costa"
        loading="lazy">

      <div class="card-body">
        <h3>Territorio</h3>
        <p>
          El mar Caribe, las comunidades costeras y los paisajes
          naturales han influido en la vida y las actividades
          de sus habitantes.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://s3.laprensani.com/wp-content/uploads/2026/09/Herencia-Nicaraguense-Miami-Marlins-celebracion-1000x600.jpg"
        alt="Celebración de la herencia nicaragüense"
        loading="lazy">

      <div class="card-body">
        <h3>Identidad cultural</h3>
        <p>
          La música, las celebraciones, las expresiones artísticas
          y las tradiciones mantienen viva la identidad de los
          pueblos caribeños.
        </p>
      </div>
    </article>

  </div>

</section>

<!-- HISTORIA -->

<section class="band" id="historia">
  <div class="wrap">

    <div class="center">
      <div class="eyebrow">Memoria histórica</div>
      <h2>Historia de la Costa Caribe</h2>

      <p class="lead">
        La historia de la Costa Caribe nicaragüense está marcada
        por la presencia de pueblos originarios, la llegada de
        europeos, la influencia africana y el desarrollo de sus
        propias comunidades.
      </p>
    </div>

    <div class="split">

      <div>
        <img
          src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=1100&q=85"
          alt="Paisaje natural de Centroamérica"
          loading="lazy">
      </div>

      <div>
        <div class="eyebrow">Un pasado que nos identifica</div>

        <h2 class="section-title">Raíces de nuestra región</h2>

        <p>
          Antes de la llegada de los europeos, diferentes pueblos
          indígenas habitaban el territorio caribeño. Entre ellos
          se encontraban comunidades miskitas, mayangnas y ramas,
          con sus propias formas de organización, conocimientos
          y tradiciones.
        </p>

        <p>
          Con el paso del tiempo, la región recibió influencias
          europeas y africanas. Estas relaciones históricas
          contribuyeron a formar una sociedad multicultural
          con características propias.
        </p>
      </div>

    </div>

    <div class="timeline">

      <div class="event">
        <div class="year">ANTES DEL SIGLO XVI</div>
        <h3>Los pueblos originarios</h3>
        <p>
          Diferentes comunidades indígenas habitaban la región.
          Desarrollaron conocimientos sobre la naturaleza,
          la pesca, la agricultura y la vida comunitaria.
        </p>
      </div>

      <div class="event">
        <div class="year">SIGLOS XVI AL XVIII</div>
        <h3>Contacto con europeos</h3>
        <p>
          La presencia europea y las relaciones comerciales
          transformaron distintos aspectos de la vida regional.
          También aumentaron los contactos entre pueblos
          indígenas, europeos y africanos.
        </p>
      </div>

      <div class="event">
        <div class="year">SIGLO XIX</div>
        <h3>El desarrollo de la región caribeña</h3>
        <p>
          La Costa Caribe vivió importantes cambios políticos,
          sociales y económicos. Las relaciones entre la región
          y el resto de Nicaragua continuaron transformándose.
        </p>
      </div>

      <div class="event">
        <div class="year">1894</div>
        <h3>Reincorporación de la Mosquitia</h3>
        <p>
          El gobierno de Nicaragua incorporó el territorio
          de la Mosquitia al Estado nicaragüense, en un proceso
          histórico que produjo cambios en la organización
          política y administrativa de la región.
        </p>
      </div>

      <div class="event">
        <div class="year">1987</div>
        <h3>Autonomía de la Costa Caribe</h3>
        <p>
          Se aprobó el Estatuto de Autonomía mediante la Ley 28,
          que reconoce derechos políticos, sociales, económicos
          y culturales de los pueblos de las regiones autónomas.
        </p>
      </div>

      <div class="event">
        <div class="year">ACTUALIDAD</div>
        <h3>Una región multicultural</h3>
        <p>
          La Costa Caribe continúa desarrollándose y conservando
          sus tradiciones, lenguas, conocimientos y diversidad
          cultural.
        </p>
      </div>

    </div>

    <div class="quote">
      “Conocer nuestra historia es valorar nuestras raíces
      y comprender la riqueza de nuestra identidad.”
      <small>HISTORIA DE LA COSTA CARIBE</small>
    </div>

  </div>
</section>

<!-- BLUEFIELDS -->

<section class="wrap">

  <div class="split">

    <div>
      <div class="eyebrow">Nuestra ciudad</div>

      <h2 class="section-title">Bluefields, corazón del Caribe Sur</h2>

      <p>
        Bluefields es la cabecera de la Región Autónoma de la
        Costa Caribe Sur de Nicaragua. Es una ciudad reconocida
        por su diversidad cultural, su historia y su relación
        con el mar Caribe.
      </p>

      <p>
        En sus comunidades conviven diferentes expresiones
        culturales y lingüísticas. Sus habitantes mantienen
        tradiciones que se reflejan en la música, la gastronomía,
        las celebraciones y la vida cotidiana.
      </p>

      <p>
        Su ubicación costera ha influido en el comercio,
        la pesca y las actividades económicas de la región.
      </p>

    </div>

    <div>
      <img
        src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21?auto=format&fit=crop&w=1100&q=85"
        alt="Paisaje de costa tropical"
        loading="lazy">
    </div>

  </div>

</section>

<!-- CULTURA -->

<section class="band" id="cultura">
  <div class="wrap">

    <div class="center">
      <div class="eyebrow">Tradiciones y raíces</div>
      <h2>La riqueza de nuestra cultura</h2>

      <p class="lead">
        La cultura de la Costa Caribe se caracteriza por
        su diversidad de pueblos, lenguas, expresiones
        artísticas y costumbres.
      </p>
    </div>

    <div class="grid">

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1504609813442-a8924e83f76e?auto=format&fit=crop&w=900&q=85"
          alt="Celebración cultural"
          loading="lazy">

        <div class="card-body">
          <h3>Celebraciones</h3>
          <p>
            Las fiestas comunitarias reúnen a las familias
            y permiten compartir costumbres, música, bailes
            y expresiones tradicionales.
          </p>
        </div>
      </article>

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1516280440614-37939bbacd81?auto=format&fit=crop&w=900&q=85"
          alt="Música y expresión artística"
          loading="lazy">

        <div class="card-body">
          <h3>Música y danza</h3>
          <p>
            La música y la danza son importantes formas
            de expresión cultural. Reflejan la historia,
            la convivencia y la identidad de los pueblos.
          </p>
        </div>
      </article>

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1528605248644-14dd04022da1?auto=format&fit=crop&w=900&q=85"
          alt="Personas compartiendo alimentos"
          loading="lazy">

        <div class="card-body">
          <h3>Vida comunitaria</h3>
          <p>
            La convivencia, la solidaridad y el respeto
            a las costumbres de cada comunidad son parte
            de la identidad caribeña.
          </p>
        </div>
      </article>

    </div>

    <div class="quote">
      La diversidad cultural es una de las mayores riquezas
      de la Costa Caribe de Nicaragua.
      <small>IDENTIDAD Y PATRIMONIO</small>
    </div>

  </div>
</section>

<!-- PUEBLOS -->

<section class="wrap">

  <div class="center">
    <div class="eyebrow">Diversidad humana</div>
    <h2>Pueblos y comunidades</h2>

    <p class="lead">
      La Costa Caribe es hogar de diferentes pueblos
      y comunidades que conservan su identidad,
      sus conocimientos y sus tradiciones.
    </p>
  </div>

  <div class="grid">

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1517849845537-4d257902454a?auto=format&fit=crop&w=900&q=85"
        alt="Retrato de una comunidad"
        loading="lazy">

      <div class="card-body">
        <h3>Pueblo Miskitu</h3>
        <p>
          El pueblo Miskitu posee una historia y una lengua
          propias. Sus tradiciones están relacionadas con
          la vida comunitaria y el entorno natural.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=900&q=85"
        alt="Bosque tropical"
        loading="lazy">

      <div class="card-body">
        <h3>Pueblo Mayangna</h3>
        <p>
          El pueblo Mayangna conserva conocimientos
          tradicionales y una estrecha relación con
          los bosques y territorios donde habita.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=900&q=85"
        alt="Paisaje natural"
        loading="lazy">

      <div class="card-body">
        <h3>Pueblo Rama</h3>
        <p>
          El pueblo Rama forma parte de la diversidad
          histórica y cultural del Caribe nicaragüense.
          Su identidad está vinculada a sus territorios
          y tradiciones.
        </p>
      </div>
    </article>

  </div>

  <p class="notice">
    También forman parte de la diversidad cultural regional
    las comunidades afrodescendientes, creoles y garífunas.
  </p>

</section>

<!-- NATURALEZA -->

<section class="band" id="naturaleza">
  <div class="wrap">

    <div class="center">
      <div class="eyebrow">Patrimonio natural</div>
      <h2>La naturaleza del Caribe</h2>

      <p class="lead">
        La región cuenta con ecosistemas de gran importancia
        para la biodiversidad y el bienestar de las comunidades.
      </p>
    </div>

    <div class="grid">

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1448375240586-882707db888b?auto=format&fit=crop&w=900&q=85"
          alt="Bosque tropical"
          loading="lazy">

        <div class="card-body">
          <h3>Bosques</h3>
          <p>
            Los bosques tropicales albergan numerosas especies
            de plantas y animales. También ayudan a proteger
            los suelos y las fuentes de agua.
          </p>
        </div>
      </article>

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1473116763249-2faaef81ccda?auto=format&fit=crop&w=900&q=85"
          alt="Río entre vegetación"
          loading="lazy">

        <div class="card-body">
          <h3>Ríos y lagunas</h3>
          <p>
            Los ríos y lagunas son importantes para el transporte,
            la pesca, la biodiversidad y las actividades
            cotidianas de las comunidades.
          </p>
        </div>
      </article>

      <article class="card">
        <img
          src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21?auto=format&fit=crop&w=900&q=85"
          alt="Mar y playa"
          loading="lazy">

        <div class="card-body">
          <h3>Playas y costas</h3>
          <p>
            Las zonas costeras son espacios naturales de gran
            valor ambiental, social y económico para la región.
          </p>
        </div>
      </article>

    </div>

  </div>
</section>

<!-- GASTRONOMÍA -->

<section class="wrap" id="gastronomia">

  <div class="center">
    <div class="eyebrow">Sabores del Caribe</div>
    <h2>Gastronomía tradicional</h2>

    <p class="lead">
      La cocina caribeña se distingue por sus sabores,
      ingredientes locales y recetas transmitidas
      entre generaciones.
    </p>
  </div>

  <div class="grid">

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1515003197210-e0cd7184f8b5?auto=format&fit=crop&w=900&q=85"
        alt="Plato de comida"
        loading="lazy">

      <div class="card-body">
        <h3>Rundown</h3>
        <p>
          Es una preparación tradicional caribeña que suele
          combinar leche de coco, pescado o mariscos y otros
          ingredientes según la receta familiar.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1547592180-85f173990554?auto=format&fit=crop&w=900&q=85"
        alt="Comida tradicional"
        loading="lazy">

      <div class="card-body">
        <h3>Rice and Beans</h3>
        <p>
          Arroz y frijoles preparados tradicionalmente
          con leche de coco y condimentos que aportan
          un sabor característico.
        </p>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?auto=format&fit=crop&w=900&q=85"
        alt="Preparación de alimentos"
        loading="lazy">

      <div class="card-body">
        <h3>Patí</h3>
        <p>
          Es una preparación de masa rellena, conocida
          por su sabor condimentado y su presencia
          en la tradición gastronómica caribeña.
        </p>
      </div>
    </article>

  </div>

</section>

<!-- IMPORTANCIA -->

<section class="band">
  <div class="wrap">

    <div class="split">

      <div>
        <img
          src="https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?auto=format&fit=crop&w=1100&q=85"
          alt="Naturaleza y biodiversidad"
          loading="lazy">
      </div>

      <div>
        <div class="eyebrow">Nuestro compromiso</div>

        <h2 class="section-title">
          Cuidar nuestro patrimonio
        </h2>

        <p>
          La historia, la cultura y la naturaleza de la Costa
          Caribe forman parte del patrimonio de Nicaragua.
          Protegerlas es una responsabilidad compartida
          entre las comunidades y las nuevas generaciones.
        </p>

        <p>
          Es importante promover el respeto a las culturas,
          conservar los recursos naturales y transmitir
          los conocimientos tradicionales.
        </p>

        <p>
          Conocer nuestra región nos ayuda a valorar
          su diversidad y a construir un futuro
          donde las tradiciones sigan vivas.
        </p>

      </div>

    </div>

  </div>
</section>

<!-- GALERÍA -->

<section class="wrap" id="galeria">

  <div class="center">
    <div class="eyebrow">Un recorrido visual</div>
    <h2>Galería de la Costa Caribe</h2>

    <p class="lead">
      Imágenes ilustrativas de paisajes, naturaleza,
      mar y cultura caribeña.
    </p>
  </div>

  <div class="gallery">

    <img
      src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?auto=format&fit=crop&w=1200&q=85"
      alt="Mar Caribe"
      loading="lazy">

    <img
      src="https://images.unsplash.com/photo-1448375240586-882707db888b?auto=format&fit=crop&w=900&q=85"
      alt="Bosque tropical"
      loading="lazy">

    <img
      src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21?auto=format&fit=crop&w=900&q=85"
      alt="Costa tropical"
      loading="lazy">

    <img
      src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=900&q=85"
      alt="Paisaje natural"
      loading="lazy">

    <img
      src="https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=900&q=85"
      alt="Vegetación tropical"
      loading="lazy">

    <img
      src="https://images.unsplash.com/photo-1473116763249-2faaef81ccda?auto=format&fit=crop&w=900&q=85"
      alt="Río y vegetación"
      loading="lazy">

  </div>

</section>

<!-- CUESTIONARIO -->

<section class="band">
  <div class="wrap">

    <div class="center">
      <div class="eyebrow">Pon a prueba tus conocimientos</div>
      <h2>¿Cuánto aprendiste?</h2>

      <p class="lead">
        Responde estas preguntas sobre la historia
        y cultura de la Costa Caribe.
      </p>
    </div>

    <div class="quiz">

      <h3 id="pregunta">1. ¿Cuál es la cabecera de la Costa Caribe Sur?</h3>

      <div class="answers" id="respuestas">

        <button onclick="responder(0)">A. Bluefields</button>
        <button onclick="responder(1)">B. Managua</button>
        <button onclick="responder(2)">C. León</button>

      </div>

      <div id="resultado"></div>

      <button class="btn" id="siguiente" onclick="siguientePregunta()" style="display:none">
        SIGUIENTE PREGUNTA
      </button>

    </div>

  </div>
</section>

<!-- PIE DE PÁGINA -->

<footer class="foot">
  <div class="foot-inner">

    <div class="brand">
      <div class="logo">✺</div>
      <div>
        HISTORIA DE LA<br>
        <span style="color:#d5ad68">COSTA CARIBE</span>
      </div>
    </div>

    <h2>Conocer nuestras raíces es valorar nuestra identidad.</h2>

    <p>
      Este sitio web es un proyecto educativo dedicado
      a compartir información sobre la historia, cultura,
      tradiciones y naturaleza de la Costa Caribe
      de Nicaragua.
    </p>

    <p>
      <strong>Fuentes de consulta:</strong><br>
      Estatuto de Autonomía de las Regiones de la Costa Caribe
      de Nicaragua, Ley No. 28.<br>
      Información histórica y cultural de las comunidades
      de la Costa Caribe.<br>
      Materiales educativos y fuentes institucionales
      de Nicaragua.
    </p>

    <p>
      <strong>Créditos de imágenes:</strong><br>
      Fotografías ilustrativas alojadas en
      <a href="https://unsplash.com/" target="_blank" rel="noopener">Unsplash</a>.<br>
      Imagen de herencia nicaragüense:
      <a href="https://www.laprensani.com/" target="_blank" rel="noopener">La Prensa</a>.
      El uso de imágenes de terceros debe respetar sus licencias
      y condiciones de autorización.
    </p>

    <p class="notice" style="color:#c4d0ca">
      Las fotografías ilustrativas no representan necesariamente
      lugares específicos de Bluefields. El contenido de esta
      página tiene fines educativos.
    </p>

    <p>© 2026 Historia de la Costa Caribe · Nicaragua</p>

  </div>
</footer>

<script>
/* MENÚ MÓVIL */

const menu = document.getElementById("menu");
const nav = document.getElementById("nav");

menu.addEventListener("click", function() {
  nav.classList.toggle("active");
});

document.querySelectorAll(".nav a").forEach(function(link) {
  link.addEventListener("click", function() {
    nav.classList.remove("active");
  });
});

/* CUESTIONARIO */

const preguntas = [
  {
    pregunta: "1. ¿Cuál es la cabecera de la Costa Caribe Sur?",
    respuestas: ["A. Bluefields", "B. Managua", "C. León"],
    correcta: 0
  },
  {
    pregunta: "2. ¿En qué año se aprobó el Estatuto de Autonomía?",
    respuestas: ["A. 1979", "B. 1987", "C. 1995"],
    correcta: 1
  },
  {
    pregunta: "3. ¿Cuál de estos pueblos forma parte de la diversidad cultural caribeña?",
    respuestas: ["A. Miskitu", "B. Inca", "C. Azteca"],
    correcta: 0
  },
  {
    pregunta: "4. ¿Qué ingrediente es característico de muchos platos caribeños?",
    respuestas: ["A. Leche de coco", "B. Chocolate", "C. Manzana"],
    correcta: 0
  },
  {
    pregunta: "5. ¿Qué debemos hacer para proteger nuestro patrimonio?",
    respuestas: ["A. Dañar los bosques", "B. Respetar la cultura y cuidar la naturaleza", "C. Contaminar los ríos"],
    correcta: 1
  }
];

let numeroPregunta = 0;
let puntuacion = 0;
let contestada = false;

function cargarPregunta() {
  contestada = false;

  const actual = preguntas[numeroPregunta];

  document.getElementById("pregunta").textContent = actual.pregunta;

  const contenedor = document.getElementById("respuestas");
  contenedor.innerHTML = "";

  actual.respuestas.forEach(function(respuesta, indice) {
    const boton = document.createElement("button");

    boton.textContent = respuesta;

    boton.addEventListener("click", function() {
      responder(indice);
    });

    contenedor.appendChild(boton);
  });

  document.getElementById("resultado").textContent = "";
  document.getElementById("siguiente").style.display = "none";
}

function responder(indice) {
  if (contestada) return;

  contestada = true;

  const actual = preguntas[numeroPregunta];
  const botones = document.querySelectorAll("#respuestas button");

  if (indice === actual.correcta) {
    puntuacion++;
    document.getElementById("resultado").textContent =
      "¡Correcto! Muy bien.";
  } else {
    document.getElementById("resultado").textContent =
      "Respuesta incorrecta. La respuesta correcta es: " +
      actual.respuestas[actual.correcta];
  }

  botones.forEach(function(boton) {
    boton.disabled = true;
  });

  document.getElementById("siguiente").style.display = "inline-block";

  if (numeroPregunta === preguntas.length - 1) {
    document.getElementById("siguiente").textContent = "VER RESULTADO";
  }
}

function siguientePregunta() {
  if (numeroPregunta < preguntas.length - 1) {
    numeroPregunta++;
    cargarPregunta();
  } else {
    mostrarResultado();
  }
}

function mostrarResultado() {
  document.getElementById("pregunta").textContent =
    "¡Has terminado el cuestionario!";

  document.getElementById("respuestas").innerHTML = "";

  document.getElementById("resultado").textContent =
    "Tu puntuación fue de " + puntuacion + " de " +
    preguntas.length + " respuestas correctas.";

  const boton = document.getElementById("siguiente");
  boton.textContent = "VOLVER A INTENTAR";
  boton.onclick = reiniciar;
}

function reiniciar() {
  numeroPregunta = 0;
  puntuacion = 0;

  const boton = document.getElementById("siguiente");
  boton.textContent = "SIGUIENTE PREGUNTA";
  boton.onclick = siguientePregunta;

  cargarPregunta();
}

</script>

</body>
</html>
