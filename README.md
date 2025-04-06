<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>Carta de Amor con Animación de Corazones</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f9f1f1;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }
        .container {
            width: 80%;
            max-width: 600px;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            opacity: 0;
            transform: translateY(50px);
            animation: slideUp 1.5s ease-out forwards;
            position: relative;
            z-index: 1;
        }
        .header {
            text-align: center;
            font-size: 36px;
            color: #e91e63;
            margin-bottom: 30px;
        }
        .content {
            font-size: 18px;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        .footer {
            text-align: right;
            font-size: 16px;
            color: #555;
            margin-top: 30px;
        }

        /* Animación de deslizamiento */
        @keyframes slideUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Animación de corazones flotantes */
        .heart {
            position: absolute;
            color: #e91e63;
            font-size: 2rem;
            animation: floatHeart 5s ease-in-out infinite;
        }

        @keyframes floatHeart {
            0% {
                top: 100%;
                left: calc(100% * random());
                opacity: 0;
            }
            50% {
                opacity: 1;
                transform: scale(1.2);
            }
            100% {
                top: -10%;
                left: calc(100% * random());
                opacity: 0;
            }
        }

        /* Generar posición aleatoria para los corazones */
        .heart:nth-child(odd) {
            animation-delay: 0s;
        }
        .heart:nth-child(even) {
            animation-delay: 2s;
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">Para mi amiga</div>

    <div class="content">
        <p>Desde el primer momento en que te vi, supe que mi vida cambiaría para siempre. Tus ojos, tu sonrisa, tu manera de ser... todo en ti me cautivó, y hoy no puedo dejar de pensar en ti.</p>

        <p>Cada día a tu lado es un regalo que atesoro profundamente. Gracias por tu amor, por tu apoyo, por ser mi mejor amigo y mi compañero de vida. Estoy agradecido por cada instante que compartimos, y con cada momento que pasa, mi amor por ti crece más y más.</p>

        <p>Quiero que sepas que siempre estaré aquí para ti, en las buenas y en las malas, apoyándote en cada paso que tomes. Mi amor por ti no tiene límites, y no hay nada que desee más que pasar el resto de mi vida a tu lado.</p>
    </div>

    <div class="footer">Para mi mejor amiga, <br> Tu [Francis]</div>
</div>

<!-- Corazones flotantes -->
<div class="heart" style="top: 10%; left: 10%;">❤️</div>
<div class="heart" style="top: 20%; left: 30%;">❤️</div>
<div class="heart" style="top: 30%; left: 50%;">❤️</div>
<div class="heart" style="top: 40%; left: 70%;">❤️</div>
<div class="heart" style="top: 50%; left: 90%;">❤️</div>

</body>
</html>
