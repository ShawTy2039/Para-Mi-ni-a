# Para-Mi-niña
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Ghisline ❤️</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            background: linear-gradient(to bottom, #ff99cc, #ff3366);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            font-family: 'Arial', sans-serif;
            color: white;
        }

        .container {
            position: relative;
            z-index: 10;
        }

        h1 {
            font-size: 3em;
            animation: fadeIn 2s ease-in-out;
        }

        p {
            font-size: 1.5em;
            margin: 20px;
            animation: fadeIn 3s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: red;
            clip-path: polygon(50% 0%, 100% 35%, 80% 100%, 50% 80%, 20% 100%, 0% 35%);
            opacity: 0.7;
            animation: fall 4s linear infinite;
        }

        @keyframes fall {
            from { transform: translateY(-100px); opacity: 1; }
            to { transform: translateY(100vh); opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Para Ghisline ❤️</h1>
        <p>Desde el momento en que entraste en mi vida, cada día se ha llenado de luz y alegría.  
        Eres la razón por la que sonrío, el latido de mi corazón y el sueño más hermoso que jamás hubiera imaginado.</p>
        <p>Hoy, en este día especial, quiero recordarte lo mucho que significas para mí.  
        No hay palabras suficientes para describir lo increíble que eres, pero sí hay algo que puedo decir con certeza:  
        <strong>te quiero con todo mi corazón.</strong></p>
        <p>Gracias por ser mi inspiración, mi felicidad y mi mejor historia de amor.</p>
        <p><strong>Feliz San Valentín, Ghisline.</strong></p>
    </div>

    <audio autoplay loop>
        <source src="https://www.bensound.com/bensound-music/bensound-love.mp3" type="audio/mp3">
        Tu navegador no soporta el audio.
    </audio>

    <script>
        function createHeart() {
            const heart = document.createElement("div");
            heart.classList.add("heart");
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = Math.random() * 2 + 3 + "s";
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 4000);
        }

        setInterval(createHeart, 300);

        document.addEventListener("click", createHeart);
    </script>
</body>
</html>
