PROYECTO FINAL
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zona Gaming</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        <ins> 
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            position: relative;
            overflow: hidden;
            animation: fadeIn 1s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        video {
            position: fixed;
            top: 50%;
            left: 50%;
            min-width: 100%;
            min-height: 100%;
            width: auto;
            height: auto;
            z-index: -1;
            transform: translate(-50%, -50%);
            background: no-repeat;
            background-size: cover;
            opacity: 0.6;
        }

        header {
            background-color: rgba(0, 0, 0, 0.8);
            color: #ffffff;
            padding: 10px 0;
            text-align: center;
            text-shadow: 0 0 20px #ffffff;
            animation: slideIn 0.5s ease;
        }

        @keyframes slideIn {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        nav {
            background-color: rgba(0, 0, 0, 0.8);
            overflow: hidden;
            padding: 10px 0;
            animation: slideIn 0.5s ease;
        }

        nav a {
            float: left;
            display: block;
            color: #ffffff;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
            transition: color 0.3s, transform 0.3s;
        }

        nav a:hover {
            color: #ffffff;
            text-shadow: 0 0 10px #ffffff;
            transform: scale(1.1);
        }

        .dropdown {
            float: left;
            overflow: hidden;
        }

        .dropdown .dropbtn {
            cursor: pointer;
            padding: 14px 16px;
            background-color: #333;
            color: #ffffff;
            border: none;
            outline: none;
            font-size: 16px;
            transition: color 0.3s;
        }

        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #222;
            min-width: 160px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.5);
            z-index: 1;
        }

        .dropdown-content a {
            float: none;
            color: #ffffff;
            padding: 12px 16px;
            text-decoration: none;
            text-align: left;
            transition: background-color 0.3s;
        }

        .dropdown-content a:hover {
            background-color: rgba(255, 0, 255, 0.5);
            text-shadow: 0 0 10px #ff00ff;
        }

        .dropdown.show .dropdown-content {
            display: block;
            animation: fadeIn 0.3s ease;
        }

        main {
            padding: 20px;
            color: white;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            animation: fadeIn 0.5s ease;
        }

        th, td {
            border: 1px solid #ffffff;
            padding: 8px;
            text-align: center;
            transition: background-color 0.3s;
        }

        th {
            background-color: rgba(0, 0, 0, 0.8);
            color: #ffffff;
            text-shadow: 0 0 10px #ffffff;
        }

        tr:nth-child(even) {
            background-color: rgba(0, 0, 0, 0.1);
        }

        tr:nth-child(odd) {
            background-color: rgba(255, 255, 255, 0.2);
        }

        tr:hover {
            background-color: rgba(0, 0, 0, 0.2);
        }

        section {
            margin: 20px 0;
            border: 1px solid #ffffff;
            padding: 10px;
            border-radius: 5px;
            background-color: rgba(0, 0, 0, 0.7);
            color: #00ffcc;
            text-shadow: 0 0 10px #00ffcc;
            transition: transform 0.3s;
        }

        section:hover {
            transform: scale(1.02);
        }
    </style>
</head>
<body>

<video autoplay muted loop>
    <source src="https://addons-media.operacdn.com/media/themes/14/278014/1.0-rev1/animations/video_preview.webm" type="video/webm">
    Tu navegador no soporta el video.
</video>

<header>
    <h1>Zona Gaming</h1>
</header>

<nav>
    <a href="#home">Inicio</a>
    <a href="#about">Acerca de</a>
    <div class="dropdown" id="dropdown">
        <button class="dropbtn" onclick="toggleDropdown()">Servicios</button>
        <div class="dropdown-content">
            <a href="#LO ULTIMO DEL GAMING">LO ULTIMO DEL GAMING</a>
            <a href="#LOS JUEGOS MAS POPULARES DE ESTE 2024">LOS JUEGOS MAS POPULARES DE ESTE 2024</a>
            <a href="#JUEGOS PARA PC DE GAMA BAJA">JUEGOS PARA PC DE GAMA BAJA</a>
        </div>
    </div>
    <a href="#contact">Contacto</a>
</nav>

<main>
    <section id="home">
        <h2>Inicio</h2>
        <p>Bienvenido a Zona Gaming. Aquí, la diversión y la aventura nunca tienen fin. Te traemos las últimas novedades del mundo gamer, desde lanzamientos esperados hasta sorpresas inesperadas. Además, hemos seleccionado los mejores juegos para que encuentres fácilmente tu próxima aventura. Ya seas un jugador casual o un experto en busca de desafíos, aquí hay algo para todos. También encontrarás reseñas, guías y consejos para mejorar tu experiencia. ¡Prepárate para sumergirte en un mundo de diversión en Zona Gaming y descubrir todo lo que tenemos para ofrecerte! A continuación, te mostramos una tabla con algunas categorías de juegos y los juegos que te pueden interesar de ellas.</p>
        
        <table>
            <tr>
                <th>Battle Royale</th>
                <th>Zombies</th>
                <th>Survival</th>
                <th>Mundo Abierto</th>
            </tr>
            <tr>
                <td>Free Fire</td>
                <td>The Last of Us</td>
                <td>Minecraft</td>
                <td>GTA V</td>
            </tr>
            <tr>
                <td>Fortnite</td>
                <td>Call of Duty: BO2</td>
                <td>The Forest</td>
                <td>GTA San Andreas</td>
            </tr>
            <tr>
                <td>Warzone</td>
                <td>Plantas vs Zombies</td>
                <td>The Last of Us Part II</td>
                <td>GTA Vice City</td>
            </tr>
            <tr>
                <td>Call of Duty</td>
                <td>DayZ</td>
                <td>Red Reminiscence</td>
                <td>Horizon Zero Dawn</td>
            </tr>
        </table>
    </section>
    
    <section id="about">
        <h2>Acerca de</h2>
        <p>Esta es una página especializada en el mundo de los juegos y nada más. Nosotros te actualizamos de cualquier noticia sobre los videojuegos y a la vez te damos reseñas de estos mismos. En esta página encontrarás desde links para descargar juegos, las mejores ofertas que haya en el momento y lo que más esté en tendencia y en jugabilidad en los últimos días.</p>
    </section>
    
    <section id="LO ULTIMO DEL GAMING">
        <h2>LO ULTIMO DEL GAMING:</h2>
        <ul>
            <li><strong>Spider-Man 2:</strong> Lanzado el 20 de octubre, este juego ha sido uno de los más esperados del año. Desarrollado por Insomniac Games, continúa la historia de Peter Parker y Miles Morales en un mundo abierto de Nueva York. Los críticos han elogiado la narrativa, la jugabilidad y la integración de ambos personajes, cada uno con habilidades únicas.</li>
            
            <li><strong>Alan Wake II:</strong> Programado para lanzarse el 27 de octubre, este juego es la secuela del título original de 2010. Se centra en el escritor Alan Wake, quien lucha contra las fuerzas oscuras mientras busca a su esposa desaparecida. El juego ofrece una jugabilidad basada en la narrativa y la exploración, combinada con mecánicas de supervivencia y acción en tercera persona.</li>
        </ul>
    </section>

    <section id="LOS JUEGOS MAS POPULARES DE ESTE 2024">
        <h2>LOS JUEGOS MAS POPULARES DE ESTE 2024</h2>
        <ul>
            <li>Free Fire</li>
            <li>Fortnite</li>
            <li>Call of Duty</li>
            <li>Warzone</li>
            <li>Fall Guys</li>
        </ul>
    </section>

    <section id="JUEGOS PARA PC DE GAMA BAJA">
        <h2>JUEGOS PARA PC DE GAMA BAJA</h2>
        <ul>
            <li><strong>League of Legends:</strong> Un juego de estrategia en línea de ritmo rápido donde dos equipos de cinco jugadores compiten para destruir la base del enemigo.</li>
            <li><strong>Counter-Strike: Global Offensive:</strong> Un juego de disparos en primera persona donde los jugadores luchan en equipos de terroristas contra fuerzas especiales.</li>
            <li><strong>Stardew Valley:</strong> Un juego de rol de simulación en el que los jugadores se convierten en granjeros, cultivando y criando animales mientras interactúan con los habitantes del pueblo.</li>
            <li><strong>Portal 2:</strong> Un juego de puzzles y plataformas en primera persona, donde los jugadores deben resolver acertijos usando portales para avanzar.</li>
        </ul>
    </section>
</main>

<footer>
    <p>&copy; Lopez cervera angel saul contactanos: +52 985 112 2176</p>
</footer>

<script>
    function toggleDropdown() {
        document.getElementById("dropdown").classList.toggle("show");
    }
</script>

</body>
</html>
