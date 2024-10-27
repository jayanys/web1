<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Los Beneficios de la Lectura</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background: #35424a;
            color: #ffffff;
            padding: 10px 0;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            color: #ffffff;
            text-decoration: none;
        }

        section {
            padding: 20px;
            margin: 10px;
            background: #ffffff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background: #35424a;
            color: #ffffff;
            position: relative;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Los Beneficios de la Lectura</h1>
        <nav>
            <ul>
                <li><a href="#benefits">Beneficios</a></li>
                <li><a href="#quotes">Citas</a></li>
                <li><a href="#contact">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <section id="benefits">
        <h2>Beneficios de Leer</h2>
        <ul>
            <li>Mejora la concentración.</li>
            <li>Aumenta el vocabulario.</li>
            <li>Estimula la imaginación.</li>
            <li>Reduce el estrés.</li>
        </ul>
    </section>

    <section id="quotes">
        <h2>Citas Inspiradoras</h2>
        <blockquote id="quote"></blockquote>
        <button onclick="newQuote()">Nueva Cita</button>
    </section>

    <footer id="contact">
        <h2>Contacto</h2>
        <p>Email: ejemplo@correo.com</p>
    </footer>

    <script>
        const quotes = [
            "La lectura es a la mente lo que el ejercicio es al cuerpo.",
            "Un libro es un sueño que tienes en tus manos.",
            "La lectura es una forma de viajar sin salir de casa.",
            "Hoy es el mañana que tanto temías ayer."
        ];

        function newQuote() {
            const randomIndex = Math.floor(Math.random() * quotes.length);
            document.getElementById("quote").innerText = quotes[randomIndex];
        }

        // Cargar una cita al iniciar la página
        window.onload = newQuote;
    </script>
</body>
</html>
