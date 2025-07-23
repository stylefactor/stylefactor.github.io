<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>STYLE FACTOR DANCE CHAMBELANES</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display&display=swap" rel="stylesheet">
    <style>
       :root {
    --primary-color: #000000;
    --secondary-color: #008000;
    --accent-color: #ffffff;
    --neon-green: #39ff14; /* Color neón verde */
    --neon-white: #ffffff; /* Color neón blanco */
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    background-color: #f8f8f8;
    color: #333;
}

/* Importar fuentes desde Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Brusher&family=Charmonman:wght@400;700&display=swap');

header {
    background-color: var(--primary-color);
    padding: 1.5rem 0;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

header.scrolled {
    transform: translateY(-20px);
}

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
}

.logo-container {
    display: flex;
    justify-content: center;
    margin-bottom: 1rem;
}

.logo-placeholder {
    width: 200px;
    height: 100px;
    background-color: rgba(255, 255, 255, 0.1);
    border: 2px dashed var(--secondary-color);
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--secondary-color);
    font-weight: bold;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
    gap: 2rem;
}

nav a {
    color: var(--accent-color);
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    font-size: 1rem;
}

nav a:hover {
    color: var(--neon-green);
    text-shadow: 0 0 5px var(--neon-green), 0 0 10px var(--neon-green);
}

.hero {
    background: linear-gradient(-45deg,#068706 , #0d6a0d , #299c29 , #068706 );
    background-size: 400% 400%;
    height: 80vh;
    animation: gradient 15s ease infinite;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: var(--accent-color);
}

.hero-content h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
    text-shadow: 
        0 0 10px var(--neon-green), 
        0 0 20px var(--neon-green), 
        0 0 5px var(--neon-white), 
        0 0 10px var(--neon-white);
    font-family: 'Brusher', cursive; /* Tipografía Brusher */
}

.hero-content h1 span.style {
    font-style: italic;
    font-family: 'Charmonman', cursive; /* Tipografía Chambonman */
    color: var(--secondary-color);
    text-shadow: 0 0 5px var(--neon-white), 0 0 10px var(--neon-white);
}

.hero-content h1 span.dance {
    font-style: italic;
    font-family: 'Charmonman', cursive; /* Tipografía Chambonman */
    color: var(--accent-color);
}

.hero-content p {
    font-size: 1.2rem;
    max-width: 800px;
    margin: 0 auto 2rem;
}

.btn {
    display: inline-block;
    background-color: var(--secondary-color);
    color: var(--accent-color);
    padding: 0.8rem 2rem;
    border-radius: 30px;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    border: none;
    cursor: pointer;
    box-shadow: 0 0 5px var(--neon-green), 0 0 10px var(--neon-green);
}

.btn:hover {
    background-color: #006600;
    transform: translateY(-3px);
    animation: pulse 1s infinite;
    box-shadow: 0 0 10px var(--neon-green), 0 0 20px var(--neon-green);
}

@keyframes pulse {
    0% { box-shadow: 0 0 0 0 rgba(0, 128, 0, 0.4); }
    70% { box-shadow: 0 0 0 15px rgba(0, 128, 0, 0); }
    100% { box-shadow: 0 0 0 0 rgba(0, 128, 0, 0); }
}

section {
    padding: 4rem 0;
}

.section-title {
    text-align: center;
    margin-bottom: 3rem;
}

.section-title h2 {
    font-size: 2.5rem;
    color: #FFF7F8;
    position: relative;
    display: inline-block;
}

.section-title h2::after {
    content: '';
    position: absolute;
    width: 50%;
    height: 3px;
    background-color: var(--secondary-color);
    bottom: -10px;
    left: 25%;
}

.about-content {
    display: flex;
    align-items: center;
    gap: 3rem;
}

.about-text {
    flex: 1;
     font-family: 'Comic Sans', serif;
      font-size: 22px;
      color: #333333; /* Gris oscuro elegante */
}

.about-image {
    flex: 1;
}

.about-image img {
    width: 100%;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

.packages {
    background-color: var(--primary-color);
    color: var(--accent-color);
}

.package-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.package-card {
    background-color: rgba(255, 255, 255, 0.1);
    padding: 2rem;
    border-radius: 10px;
    transition: all 0.3s ease;
    text-align: center;
}

.package-card:hover {
    transform: translateY(-15px) scale(1.03);
    box-shadow: 0 15px 30px rgba(0, 128, 0, 0.3);
    background-color: rgba(0, 128, 0, 0.1);
    border: 2px solid var(--secondary-color);
}

.package-card h3 {
    color: var(--secondary-color);
    font-size: 1.5rem;
    margin-bottom: 1rem;
}

.package-card .price {
    font-size: 2rem;
    font-weight: bold;
    margin-bottom: 1.5rem;
    color: var(--accent-color);
}

.package-card ul {
    list-style: none;
    margin-bottom: 2rem;
}

.package-card ul li {
    margin-bottom: 0.8rem;
    position: relative;
    padding-left: 20px;
}

.package-card ul li::before {
    content: '✓';
    color: var(--secondary-color);
    position: absolute;
    left: 0;
}

.contact-info {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.contact-card {
    background-color: var(--accent-color);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.contact-card i {
    font-size: 2rem;
    color: var(--secondary-color);
    margin-bottom: 1rem;
}

.map-container {
    margin-top: 3rem;
}

.map-container iframe {
    width: 100%;
    height: 450px;
    border: none;
    border-radius: 10px;
}

.social-media {
    background-color: var(--primary-color);
    padding: 3rem 0;
    text-align: center;
}

.social-icons {
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    margin-top: 1.5rem;
}

.social-icons a {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50px;
    height: 50px;
    background-color: var(--secondary-color);
    color: var(--accent-color);
    border-radius: 50%;
    font-size: 1.5rem;
    transition: all 0.3s ease;
    text-decoration: none;
}

.social-icons a:hover {
    transform: translateY(-5px) rotate(10deg) scale(1.2);
    background-color: var(--accent-color);
    color: var(--secondary-color);
    box-shadow: 0 10px 20px rgba(0, 128, 0, 0.3);
}

.testimonials {
    background-color: #f0f0f0;
    padding-bottom: 4rem;
}

.testimonial-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin-bottom: 3rem;
}

.testimonial-card {
    background-color: var(--accent-color);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    position: relative;
}

.rating {
    color: #ffcc00;
    margin-bottom: 1rem;
    font-size: 1.5rem;
}

.testimonial-card .quote {
    font-style: italic;
    margin-bottom: 1.5rem;
    color: #555;
}

.testimonial-card .author {
    font-weight: bold;
    color: var(--secondary-color);
}

.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1rem;
}

.gallery-item {
    overflow: hidden;
    border-radius: 10px;
    position: relative;
    height: 250px;
}

.gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
}

.gallery-item {
    transition: all 0.5s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.gallery-item:hover {
    transform: scale(1.05);
    z-index: 10;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
}

.gallery-item:hover img {
    transform: scale(1.2);
    filter: brightness(1.1);
}

footer {
    background-color: var(--primary-color);
    color: var(--accent-color);
    padding: 3rem 0 1.5rem;
    text-align: center;
}

.footer-logo {
    margin-bottom: 1rem;
}

.footer-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 1.5rem;
    margin-bottom: 2rem;
}

.footer-links a {
    color: var(--accent-color);
    text-decoration: none;
    transition: all 0.3s ease;
}

.footer-links a:hover {
    color: var(--secondary-color);
}

.copyright {
    margin-top: 2rem;
    font-size: 0.9rem;
    color: #aaa;
}

@keyframes gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

/* Review Form Styles */
.review-form {
    max-width: 600px;
    margin: 0 auto;
    background: var(--accent-color);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

.form-group {
    margin-bottom: 1.5rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 600;
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 0.8rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 1rem;
}

.form-group textarea {
    min-height: 120px;
}

.star-rating {
    display: flex;
    direction: rtl;
    unicode-bidi: bidi-override;
}

.star-rating input {
    display: none;
}

.star-rating label {
    font-size: 2rem;
    padding: 0 5px;
    cursor: pointer;
    color: #ddd;
}

.star-rating input:checked ~ label,
.star-rating label:hover,
.star-rating label:hover ~ label {
    color: #ffcc00;
}

/* Responsive Styles */
@media (max-width: 758px) {
    .hero-content h1 {
        font-size: 1.5rem;
    }
    
    .about-content {
        flex-direction: column;
    }
    
    nav ul {
        flex-direction: column;
        gap: 1rem;
        align-items: center;
    }

            height: 300px; /* Ajusta la altura según sea necesario */
            background-color: #ffffff; /* Color de fondo */
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .video-item:hover {
            transform: scale(1.05);
            z-index: 10;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        .video-item iframe {
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 10px;
        }
        @media (max-width: 1024px) {
            .video-grid {
                grid-template-columns: repeat(2, 1fr); /* Dos columnas en pantallas más pequeñas */
            }
        }
        @media (max-width: 600px) {
            .video-grid {
                grid-template-columns: 1fr; /* Una columna en pantallas muy pequeñas */
            }
        }
</style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="logo-container">
                <img src="style factor.jpeg">
            </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#inicio">Inicio</a></li>
                    <li><a href="#nosotros">Nosotros</a></li>
                    <li><a href="#paquetes">Paquetes</a></li>
                    <li><a href="#galeria">Galería</a></li>
                    <li><a href="#contacto">Contacto</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="nosotros">
        <div class="container">
            <div class="section-title">
                <h2 style="color:#121313";>Sobre Nosotros</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <p>
<strong>STYLE FACTOR DANCE CHAMBELANES</strong> es la agencia líder en servicios para eventos sociales, especializada en <strong>chambelanes profesionales</strong>, <strong>coreografías personalizadas para bodas y quinceañeras</strong>, y espectáculos visuales que marcan diferencia.
<br>
<li>Nos dedicamos a crear momentos inolvidables con elegancia, estilo y profesionalismo, ofreciendo <strong>pistas iluminadas</strong>, <strong>letras gigantes con luz LED</strong>, y presentaciones que fusionan danza y ambientación para elevar cualquier celebración.
<br>
<li>Nuestro equipo está formado por bailarines altamente capacitados, con años de experiencia en bodas, quinceañeras, festivales y todo tipo de eventos especiales.
<br>
<li>Lo que nos diferencia es nuestra pasión por el arte escénico, nuestro compromiso con la calidad y nuestra habilidad para personalizar cada espectáculo según la visión de nuestros clientes.</p>
                </div>
                <div class="about-image">
                    <img src="foto1.jpeg" alt="Grupo de chambelanes profesionales vestidos de negro con detalles verdes, realizando una coreografía sincronizada en un evento elegante">
                </div>
            </div>
        </div>
    </section>

    <section class="packages" id="paquetes">
        <div class="container">
            <div class="section-title">
                <h2>Nuestros Paquetes</h2>
            </div>
            <div class="package-grid">
                <div class="package-card">
                    <h3>Plata</h3>
                    <div class="price">$6,200 MXN</div>
                    <ul>
                        <li> Vals de Entrada</li>
                        <li> Vals Principal</li>
                        <li>Vals de Salida</li>
                        <li>Vals Muñeca</li>
                        <li>Brindis</li>
			<li>Vals Familiar</li>
			<li>Baile sorpresa (2-3 minutos)
			<li>Show Style Factor
			<li>Coreógrafo personal (Vals y show sorpresa)</li>
			<li>Maestra de ceremonia</li>
			<li>4 chambelanes Show Sorpresa</li>
			<li>4 chambelanes Vals</li>
                        <br>
			<div class="price">Incluye:</div>
			<br>
			<li>3 Disparos de pirotecnia fría</li>
			<li>3 Bazucas de papel picado </li>
			
                    </ul>
                    <a href="#contacto" class="btn">Reservar</a>
                </div>
                <div class="package-card">
                    <h3>Oro</h3>
                    <div class="price">$7,400 MXN</div>
                    <ul>
                        <li> Vals de Entrada</li>
                        <li> Vals Principal</li>
                        <li>Vals de Salida</li>
                        <li>Vals Muñeca, Corona y Zapatillas</li>
                        <li>Brindis</li>
			<li>Vals Familiar</li>
			<li>Baile sorpresa (3-4 minutos)</li>
			<li>Show Style Factor</li>
			<li>Coreógrafo personal (Vals y show sorpresa)</li>
			<li>Vestuario a elegir(Show Sorpresa)</li>
			<li>Maestra de ceremonia</li>
			<li>6 chambelanes Show Sorpresa</li>
			<li>4 chambelanes Vals</li>
			<br>
			<div class="price">Incluye:</div>
			<br>
			<li>¡Acompañamiento desde Misa!</li>
			<li>2 Maquinas de efectos especiales (Humo o Fuego) </li>
			<li>4 Disparos de pirotecnia fría</li>
			<li>4 Bazucas de papel picado </li>
                    </ul>
                    <a href="#contacto" class="btn">Reservar</a>
                </div>
                <div class="package-card">
                    <h3>Diamante</h3>
                    <div class="price">$8,200 MXN</div>
                    <ul>
			<li>Presentación</li>
                       <li> Vals de Entrada</li>
                        <li> Vals Principal</li>
                        <li>Vals de Salida</li>
			<li>Vals Sorpresa</li>
                        <li>Vals Muñeca, Corona y Zapatillas</li>
                        <li>Brindis</li>
			<li>Vals Familiar</li>
			<li>Baile sorpresa (4-5 minutos)</li>
			<li>Show Style Factor</li>
			<li>Coreógrafo personal (Vals y show sorpresa)</li>
			<li>Vestuario a elegir(Show Sorpresa)</li>
			<li>Maestra de ceremonia</li>
			<li>8 chambelanes Show Sorpresa</li>
			<li>4 chambelanes Vals</li>
			<br>
			<div class="price">Incluye:</div>
			<br>
			<li>¡Acompañamiento desde Misa!</li>
			<li>2 Maquinas de Humo vertical </li>
			<li>2 Maquinas de Fuego Vertical</li>
			<li>5 Disparos de pirotecnia fría</li>
			<li>5 Bazucas 80cm de papel picado </li>


                    </ul>
                    <a href="#contacto" class="btn">Reservar</a>
                </div>
            </div>
        </div>
    </section>

    <section id="galeria">
        <div class="container">
            <div class="section-title">
                <h2 style="color:#000302";>Galería</h2>
            </div>
            <div class="gallery">
                <div class="gallery-item">
                    <img src="foto14.heic" alt="Grupo de chambelanes realizando una formación triangular durante una presentación nocturna con luces de colores">
                </div>
                <div class="gallery-item">
                    <img src="foto3.jpeg" alt="Chambelán realizando un giro espectacular con la capa ondeando al viento en una puesta en escena">
                </div>
                <div class="gallery-item">
                    <img src="foto4.jpeg" alt="Equipo completo de Style Factor Dance Chambelanes posando para foto grupal con trajes elegantes negros y verdes">
                </div>
                <div class="gallery-item">
                    <img src="foto5.jpeg" alt="Momento emotivo donde los chambelanes acompañan a la quinceañera en su vals">
                </div>
                <div class="gallery-item">
                    <img src="foto6.jpeg" alt="Coreografía sincronizada con elementos de humo y luces durante un evento grande">
                </div>
                <div class="gallery-item">
                    <img src="foto7.jpeg" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
	        <div class="gallery-item">
                    <img src="foto8.jpeg" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
		<div class="gallery-item">
                    <img src="foto9.jpeg" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
		<div class="gallery-item">
                    <img src="foto10.jpeg" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
		<div class="gallery-item">
                    <img src="foto11.jpeg" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
		<div class="gallery-item">
                    <img src="foto12.heic" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
		</div>
		<div class="gallery-item">
                    <img src="foto13.heic" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
                </div>
                </div>
            </div>
        </div>
    </section>
  
  <blockquote class="tiktok-embed" cite="https://www.tiktok.com/@stylefactordance/video/7492273597302541574" data-video-id="7492273597302541574" style="max-width: 605px;min-width: 325px;" > <section> <a target="_blank" title="@stylefactordance" href="https://www.tiktok.com/@stylefactordance?refer=embed">@stylefactordance</a> ¡El mejor baile sorpresa para tus XV! 🔥😱  <a title="xvaños" target="_blank" href="https://www.tiktok.com/tag/xva%C3%B1os?refer=embed">#xvaños</a> <a title="quinceaños" target="_blank" href="https://www.tiktok.com/tag/quincea%C3%B1os?refer=embed">#quinceaños</a> <a title="quinceañeras" target="_blank" href="https://www.tiktok.com/tag/quincea%C3%B1eras?refer=embed">#quinceañeras</a> <a title="quinceañera" target="_blank" href="https://www.tiktok.com/tag/quincea%C3%B1era?refer=embed">#quinceañera</a> <a title="quinceañeraviral" target="_blank" href="https://www.tiktok.com/tag/quincea%C3%B1eraviral?refer=embed">#quinceañeraviral</a> <a title="misquinceaños" target="_blank" href="https://www.tiktok.com/tag/misquincea%C3%B1os?refer=embed">#misquinceaños</a> <a title="misxvaños💙" target="_blank" href="https://www.tiktok.com/tag/misxva%C3%B1os%F0%9F%92%99?refer=embed">#misxvaños💙</a> <a title="rauwalejandro" target="_blank" href="https://www.tiktok.com/tag/rauwalejandro?refer=embed">#rauwalejandro</a> <a title="bailesorpresa" target="_blank" href="https://www.tiktok.com/tag/bailesorpresa?refer=embed">#bailesorpresa</a> <a title="bailesorpresaxv" target="_blank" href="https://www.tiktok.com/tag/bailesorpresaxv?refer=embed">#bailesorpresaxv</a> <a title="punto40rauwalejandro" target="_blank" href="https://www.tiktok.com/tag/punto40rauwalejandro?refer=embed">#punto40rauwalejandro</a> <a title="punto40" target="_blank" href="https://www.tiktok.com/tag/punto40?refer=embed">#punto40</a> <a title="carolinarauwalejandro" target="_blank" href="https://www.tiktok.com/tag/carolinarauwalejandro?refer=embed">#carolinarauwalejandro</a> <a title="bailereggaeton" target="_blank" href="https://www.tiktok.com/tag/bailereggaeton?refer=embed">#bailereggaeton</a> <a title="regatones" target="_blank" href="https://www.tiktok.com/tag/regatones?refer=embed">#regatones</a> <a title="stylefactorchambelanes" target="_blank" href="https://www.tiktok.com/tag/stylefactorchambelanes?refer=embed">#stylefactorchambelanes</a> <a target="_blank" title="♬ sonido original - Style Factor Dance Oficial" href="https://www.tiktok.com/music/sonido-original-7492273614097566470?refer=embed">♬ sonido original - Style Factor Dance Oficial</a> </section> </blockquote> <script async src="https://www.tiktok.com/embed.js"></script>  <blockquote class="tiktok-embed" cite="https://www.tiktok.com/@stylefactordance/video/7477311455356800262" data-video-id="7477311455356800262" style="max-width: 605px;min-width: 325px;" > <section> <a target="_blank" title="@stylefactordance" href="https://www.tiktok.com/@stylefactordance?refer=embed">@stylefactordance</a> <p></p> <a target="_blank" title="♬ sonido original - Style Factor Dance Oficial" href="https://www.tiktok.com/music/sonido-original-7477311483530644279?refer=embed">♬ sonido original - Style Factor Dance Oficial</a> </section> </blockquote> <script async src="https://www.tiktok.com/embed.js"></script>


        
    </div>
</section>

    <section id="contacto">
        <div class="container">
            <div class="section-title">
                <h2 style="color:#000302";>Contacto</h2>
            </div>
            <div class="contact-info">
                <div class="contact-card">
                    <i class="fas fa-map-marker-alt"></i>
                    <h3>Ubicación</h3>
                    <p>C. Uranga 38, Barrio del Calvario, 72700 San Juan Cuautlancingo, Pue.</p>
                </div>
                <div class="contact-card">
                    <i class="fas fa-phone-alt"></i>
                    <h3>Teléfono</h3>
                    <p>+52 222 154 8706</p>
		    <a href="https://w.app/stylefactor"class="btn" target="_blank">Mensaje Directo</a>


                </div>
                <div class="contact-card">
                    <i class="fas fa-clock"></i>
                    <h3>Horario</h3>
                    <p>Lunes a Viernes<br>5:00 PM - 8:30 PM</p>
                </div>
            </div>
            <div class="map-container">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4483.73858066705!2d-98.27395762783392!3d19.091869740311306!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85cfc7174b366ff1%3A0xe8d61f1abf2a4269!2sSTYLE%20FACTOR%20grupo%20valsistico!5e0!3m2!1ses-419!2smx!4v1753140993728!5m2!1ses-419!2smx" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>
    </section>

    <section class="social-media">
        <div class="container">
            <h2 style="color:#ffffff";>Síguenos en Redes Sociales</h2>
            <div class="social-icons">
                <a href="https://www.facebook.com/StyleFactorDance/"><i class="fab fa-facebook-f"></i></a>
                <a href="https://www.instagram.com/style.factor.dance/"><i class="fab fa-instagram"></i></a>
                <a href="https://www.tiktok.com/@stylefactordance"><i class="fab fa-tiktok"></i></a>
                <a href="https://www.youtube.com/@stylefactordanceoficial4822"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
                    <img src="tarjeta.jpeg" width="500" height="300" alt="Detalle del vestuario premium con acabados en verde sobre fondo negro de alta calidad">
            
    </section>

<section class="testimonials">
    <div class="container">
        <div class="section-title">
            <h2 style="color:#000302;">Deja tu opinión</h2>
        </div>
        <form class="review-form" id="reviewForm">
            <div class="form-group">
                <label for="name">Nombre:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div class="form-group">
                <label for="rating">Calificación:</label>
                <div class="star-rating">
                    <input type="radio" id="star5" name="rating" value="5" required>
                    <label for="star5">★</label>
                    <input type="radio" id="star4" name="rating" value="4">
                    <label for="star4">★</label>
                    <input type="radio" id="star3" name="rating" value="3">
                    <label for="star3">★</label>
                    <input type="radio" id="star2" name="rating" value="2">
                    <label for="star2">★</label>
                    <input type="radio" id="star1" name="rating" value="1">
                    <label for="star1">★</label>
                </div>
            </div>
            <div class="form-group">
                <label for="comment">Comentario:</label>
                <textarea id="comment" name="comment" required></textarea>
            </div>
            <button type="submit" class="btn">Enviar opinión</button>
        </form>
<br>
<br>

        <div class="section-title">
            <h2 style="color:#000302;">Comentarios</h2>
        </div>
        <div class="testimonial-grid" id="testimonialGrid">
            <!-- Los testimonios se cargarán aquí -->
        </div>
    </div>
</section>

<script>
    // Cargar testimonios del almacenamiento local al cargar la página
    document.addEventListener('DOMContentLoaded', function() {
        const testimonials = JSON.parse(localStorage.getItem('testimonials')) || [];
        testimonials.forEach(testimonial => {
            addTestimonialToDOM(testimonial.name, testimonial.rating, testimonial.comment);
        });
    });

    document.getElementById('reviewForm').addEventListener('submit', function(event) {
        event.preventDefault(); // Evita el envío del formulario

        // Captura los valores del formulario
        const name = document.getElementById('name').value;
        const rating = document.querySelector('input[name="rating"]:checked').value;
        const comment = document.getElementById('comment').value;

        // Crea un objeto para el testimonio
        const testimonial = { name, rating, comment };

        // Agrega el testimonio al almacenamiento local
        const testimonials = JSON.parse(localStorage.getItem('testimonials')) || [];
        testimonials.push(testimonial);
        localStorage.setItem('testimonials', JSON.stringify(testimonials));

        // Agrega el testimonio al DOM
        addTestimonialToDOM(name, rating, comment);

        // Limpia el formulario
        document.getElementById('reviewForm').reset();
    });

    function addTestimonialToDOM(name, rating, comment) {
        const testimonialCard = document.createElement('div');
        testimonialCard.classList.add('testimonial-card');
        testimonialCard.innerHTML = `
            <div class="rating">${'★'.repeat(rating)}</div>
            <p class="quote">"${comment}"</p>
            <p class="author">- ${name}</p>
            <button class="delete-btn" onclick="deleteTestimonial('${name}', this)">🗑️</button>
        `;
        document.getElementById('testimonialGrid').prepend(testimonialCard);
    }

    function deleteTestimonial(name, button) {
        const testimonials = JSON.parse(localStorage.getItem('testimonials')) || [];
        const updatedTestimonials = testimonials.filter(testimonial => testimonial.name !== name);
        localStorage.setItem('testimonials', JSON.stringify(updatedTestimonials));
        button.parentElement.remove(); // Elimina el testimonio del DOM
    }
</script>

<style>
    .testimonial-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
        margin-bottom: 3rem;
    }

    .testimonial-card {
        background-color: var(--accent-color);
        padding: 2rem;
        border-radius: 10px;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        position: relative;
    }

    .rating {
        color: #ffcc00;
        margin-bottom: 1rem;
        font-size: 1.5rem;
    }

    .quote {
        font-style: italic;
        margin-bottom: 1.5rem;
        color: #555;
    }

    .author {
        font-weight: bold;
        color: var(--secondary-color);
    }

    .delete-btn {
        margin-top: 1rem;
        cursor: pointer;
        background: none;
        border: none;
        color: #ff0000; /* Color rojo para el botón de eliminar */
        font-size: 1.2rem;
    }
</style>


    <footer>
        <div class="container">
            <div class="footer-logo">
                <h2><span style="color: var(--secondary-color);">STYLE FACTOR</span> <span style="color: var(--accent-color); font-style: italic;">DANCE CHAMBELANES</span></h2>
            </div>
            <div class="footer-links">
                <a href="#inicio">Inicio</a>
                <a href="#nosotros">Nosotros</a>
                <a href="#paquetes">Paquetes</a>
                <a href="#galeria">Galería</a>
                <a href="#contacto">Contacto</a>
                
            </div>
            <div class="copyright">
                <p>&copy; 2025 STYLE FACTOR DANCE CHAMBELANES. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>
    <script>
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });
    </script>
</body>
</html>
