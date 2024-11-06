# HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Bienvenido a Alura</title>
    <link rel="stylesheet" href="estilos.css">
</head>
<body>
    <!-- Encabezado -->
    <header>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#cursos">Cursos</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <!-- Sección de bienvenida -->
    <section id="inicio">
        <h1>¡Bienvenido a Alura!</h1>
        <p>Alura es la plataforma de aprendizaje online donde puedes mejorar tus habilidades tecnológicas. ¡Explora nuestros cursos y lleva tu conocimiento al siguiente nivel!</p>
        <button><a href="#cursos">Ver Cursos</a></button>
    </section>

    <!-- Sección de cursos -->
    <section id="cursos">
        <h2>Cursos disponibles</h2>
        <div class="curso">
            <h3>Curso de Desarrollo Web</h3>
            <p>Aprende desde lo más básico hasta avanzado en desarrollo web.</p>
            <button><a href="#">Más información</a></button>
        </div>
        <div class="curso">
            <h3>Curso de Python</h3>
            <p>Adquiere las habilidades necesarias para programar con Python.</p>
            <button><a href="#">Más información</a></button>
        </div>
        <!-- Puedes agregar más cursos aquí -->
    </section>

    <!-- Sección de contacto -->
    <section id="contacto">
        <h2>Contacto</h2>
        <p>Si tienes preguntas, no dudes en contactarnos.</p>
        <form action="enviar_mensaje.php" method="post">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre" required>

            <label for="email">Correo electrónico:</label>
            <input type="email" id="email" name="email" required>

            <label for="mensaje">Mensaje:</label>
            <textarea id="mensaje" name="mensaje" required></textarea>

            <button type="submit">Enviar mensaje</button>
        </form>
    </section>

    <!-- Pie de página -->
    <footer>
        <p>&copy; 2024 Alura - Todos los derechos reservados</p>
    </footer>
</body>
</html>
