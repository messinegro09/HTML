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

    /* Estilos generales */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
    color: #333;
}

/* Encabezado */
header {
    background-color: #333;
    color: white;
    padding: 20px 0;
}

nav ul {
    list-style-type: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    font-size: 18px;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Sección de bienvenida */
#inicio {
    background-color: #007BFF;
    color: white;
    text-align: center;
    padding: 50px 20px;
}

#inicio h1 {
    font-size: 36px;
    margin-bottom: 20px;
}

#inicio p {
    font-size: 18px;
    margin-bottom: 30px;
}

#inicio button {
    background-color: #f8f9fa;
    color: #007BFF;
    border: none;
    padding: 10px 20px;
    font-size: 18px;
    cursor: pointer;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

#inicio button a {
    color: #007BFF;
    text-decoration: none;
}

#inicio button:hover {
    background-color: #0056b3;
    color: white;
}

/* Sección de cursos */
#cursos {
    background-color: white;
    padding: 50px 20px;
    text-align: center;
}

#cursos h2 {
    font-size: 30px;
    margin-bottom: 20px;
}

.curso {
    background-color: #f8f9fa;
    border: 1px solid #ddd;
    border-radius: 8px;
    margin: 20px 0;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.curso:hover {
    transform: translateY(-5px);
}

.curso h3 {
    font-size: 24px;
    margin-bottom: 10px;
}

.curso p {
    font-size: 16px;
    margin-bottom: 20px;
}

.curso button {
    background-color: #007BFF;
    color: white;
    padding: 10px 20px;
    font-size: 16px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.curso button a {
    color: white;
    text-decoration: none;
}

.curso button:hover {
    background-color: #0056b3;
}

/* Sección de contacto */
#contacto {
    background-color: #f4f4f4;
    padding: 50px 20px;
    text-align: center;
}

#contacto h2 {
    font-size: 30px;
    margin-bottom: 20px;
}

form {
    max-width: 600px;
    margin: 0 auto;
    text-align: left;
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

form label {
    font-size: 16px;
    margin-bottom: 8px;
    display: block;
}

form input, form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 16px;
}

form button {
    background-color: #007BFF;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 18px;
    transition: background-color 0.3s ease;
}

form button:hover {
    background-color: #0056b3;
}

/* Pie de página */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px;
    margin-top: 40px;
}

footer p {
    font-size: 14px;
}

/* Responsividad */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
    }

    .curso {
        width: 90%;
        margin: 20px auto;
    }

    form {
        width: 90%;
        margin: 0 auto;
    }
}
// Función para mostrar un mensaje de bienvenida personalizado
function mostrarBienvenida() {
    const nombreUsuario = prompt("¡Hola! ¿Cómo te llamas?");
    if (nombreUsuario) {
        alert("¡Bienvenido a Alura, " + nombreUsuario + "!");
    } else {
        alert("¡Bienvenido a Alura!");
    }
}

// Función para validar el formulario de contacto
function validarFormulario(event) {
    const nombre = document.getElementById('nombre').value;
    const email = document.getElementById('email').value;
    const mensaje = document.getElementById('mensaje').value;
    
    if (!nombre || !email || !mensaje) {
        event.preventDefault(); // Previene el envío del formulario si los campos están vacíos
        alert("Por favor, completa todos los campos del formulario.");
    } else {
        alert("¡Gracias por tu mensaje, " + nombre + "! Nos pondremos en contacto pronto.");
    }
}

// Función para el desplazamiento suave cuando se hace clic en los enlaces de navegación
function desplazamientoSuave(event) {
    event.preventDefault();
    const destino = document.querySelector(event.target.getAttribute('href'));
    window.scrollTo({
        top: destino.offsetTop,
        behavior: "smooth"
    });
}

// Agregar eventos a los enlaces de navegación
document.addEventListener("DOMContentLoaded", function() {
    // Mostrar mensaje de bienvenida cuando la página cargue
    mostrarBienvenida();
    
    // Agregar evento de desplazamiento suave a los enlaces
    const enlaces = document.querySelectorAll('nav ul li a');
    enlaces.forEach(enlace => {
        enlace.addEventListener('click', desplazamientoSuave);
    });
    
    // Validar el formulario de contacto al enviarlo
    const formulario = document.querySelector('form');
    formulario.addEventListener('submit', validarFormulario);
});

        <p>&copy; 2024 Alura - Todos los derechos reservados</p>
    </footer>
</body>
</html>
