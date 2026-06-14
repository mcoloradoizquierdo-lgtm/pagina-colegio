

body {
    font-family: Arial;
    margin: 0;
    background-color: #f4f4f4;
}

/* ENCABEZADO */
header {
    background-color: #1a5276;
    color: white;
    text-align: center;
    padding: 20px;
}

/* MENÚ */
nav {
    background-color: #154360;
    text-align: center;
    padding: 10px;
}

nav a {
    color: white;
    margin: 10px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: yellow;
}

/* CONTENIDO */
section {
    background: white;
    margin: 20px;
    padding: 20px;
    border-radius: 10px;
}

/* PIE DE PÁGINA */
footer {
    background-color: #1a5276;
    color: white;
    text-align: center;
    padding: 10px;
}
.imagenes img {
    width: 400px;
    height: 250px;
    object-fit: cover;
    object-position: center;
        /* SOMBRA ELEGANTE */
    box-shadow: 0px 4px 10px rgba(0,0,0,0.4);

    /* ANIMACIÓN SUAVE */
    transition: transform 0.3s, box-shadow 0.3s;
    
}
.imagenes {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
}
.valores {
    list-style: none;
    padding: 0;
    text-align: center;
}

.valores li {
    background-color: #1a5276;
    color: white;
    margin: 10px auto;
    padding: 10px;
    width: 200px;
    border-radius: 8px;
    font-weight: bold;
}
.valores-movimiento {
    overflow: hidden;
    white-space: nowrap;
    background-color: #1a5276;
    color: white;
    padding: 15px;
    margin-top: 10px;
}

.valores-movimiento p {
    display: inline-block;
    animation: mover 10s linear infinite;
}

@keyframes mover {
    from {
        transform: translateX(100%);
    }
    to {
        transform: translateX(-100%);
    }
}
.valores-pro {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 20px;
    flex-wrap: wrap;
}

/* TARJETAS */
.valor {
    background: #1a5276;
    color: white;
    padding: 20px;
    width: 180px;
    text-align: center;
    border-radius: 10px;
    font-weight: bold;

    /* ANIMACIÓN DE ENTRADA */
    opacity: 0;
    transform: translateY(50px);
    animation: aparecer 1s forwards;
}

/* RETARDO PARA CADA TARJETA */
.valor:nth-child(1) { animation-delay: 0.2s; }
.valor:nth-child(2) { animation-delay: 0.4s; }
.valor:nth-child(3) { animation-delay: 0.6s; }
.valor:nth-child(4) { animation-delay: 0.8s; }
.valor:nth-child(5) { animation-delay: 1s; }

/* EFECTO AL PASAR EL MOUSE */
.valor:hover {
    transform: scale(1.1);
    background: #154360;
    transition: 0.3s;
}

/* ANIMACIÓN */
@keyframes aparecer {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}


<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>I.E.I.P N° 11118 - Kañaris</title>

    <link rel="stylesheet" href="estilos.css">
</head>
<body>

<header>
    <img src="imagenes/logo.png.jpeg" width="80">
    <h1>I.E.I.P N° 11118 - KAÑARIS</h1>
    <p>"EDUCACIÓN, DISCIPLINA Y TRABAJO"</p>
    
</header>

<nav>
    <a href="#">BIENVENIDOS</a>
    <section>
    <h2>Inicio</h2>

    <p>
        En la Institución Educativa N.° 11118 - Kañaris formamos más que estudiantes, formamos personas con valores, metas y visión de futuro. Somos una comunidad educativa pública ubicada en el caserío San Cristobal, que apuesta por una educación de calidad, inclusiva y conectada con la realidad de nuestros estudiantes.
    </p>

    <p>
        Creemos en el talento de cada alumno y en su capacidad para transformar su entorno.
    </p>

</section>
    <a href="#">NOSOTROS</a>
    <section>
        Brindamos educación de calidad en Kañaris, formando estudiantes con valores, disciplina y trabajo.
    <h2>Misión</h2>
    <p>
        La Institución Educativa N.° 11118 del caserío de San Cristóbal brinda una educación integral y de calidad a los estudiantes de los niveles de inicial y primaria, promoviendo el desarrollo de competencias, capacidades y valores. Forma estudiantes creativos, críticos y responsables, comprometidos con su aprendizaje, su identidad cultural y el cuidado de su entorno, fortaleciendo la participación activa de la comunidad para contribuir al desarrollo sostenible de una sociedad justa y solidaria.
    </p>
</section>

<section>
    <h2>Visión</h2>
    <p>
        Al año 2030, la Institución Educativa N.° 11118 de la comunidad de San Cristóbal será reconocida por la comunidad educativa y las autoridades del sector educación por brindar una educación rural de calidad, formando estudiantes competentes, críticos, creativos y con sólidos valores, comprometidos con su identidad cultural, el cuidado del ambiente y el desarrollo de su comunidad, con la participación activa de las familias.
    </p>
</section>
    <a href="#">NUESTROS VALORES</a>
<section>
    <h2>Nuestros Valores</h2>

    <div class="valores-pro">
        <div class="valor">Respeto</div>
        <div class="valor">Responsabilidad</div>
        <div class="valor">Honestidad</div>
        <div class="valor">Solidaridad</div>
        <div class="valor">Compromiso</div>
    </div>
</section>
    <section>
        <h2>DIRECTOR</h2>
<div class="valores-movimiento">
    <p>Prof. Jorge Bello ZAVALETA JULCA.</p>
</div>
</section>
</nav>
<div class="imagenes">
    <img src="imagenes/colegio1.jpg.jpeg">
    <img src="imagenes/colegio2.jpg.jpeg">
</div>
</section>

<section>
    <h2>CONTACTO</h2>
    <p><strong>.</strong></p>
</section>

<footer>
    <p>© 2026 I.E.I.P N° 11118 - Kañaris</p>
</footer>

</body>
</html>



console.log("Página cargada correctamente");
