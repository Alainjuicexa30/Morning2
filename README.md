<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Buenos Días</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(to bottom, #FFDEE9, #B5FFFC);
            color: #333;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            animation: sky-color 10s linear;
        }

        @keyframes sky-color {
            0% { background: linear-gradient(to bottom, #FF4500, #FF6347); }
            5% { background: linear-gradient(to bottom, #FF6347, #FF7F50); }
            10% { background: linear-gradient(to bottom, #FF7F50, #FF8C00); }
            15% { background: linear-gradient(to bottom, #FF8C00, #FFA500); }
            20% { background: linear-gradient(to bottom, #FFA500, #FFB347); }
            25% { background: linear-gradient(to bottom, #FFB347, #FFD700); }
            30% { background: linear-gradient(to bottom, #FFD700, #FFE4B5); }
            35% { background: linear-gradient(to bottom, #FFE4B5, #E0FFFF); }
            40% { background: linear-gradient(to bottom, #E0FFFF, #B0E0E6); }
            45% { background: linear-gradient(to bottom, #B0E0E6, #87CEEB); }
            50% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            55% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            60% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            65% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            70% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            75% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            80% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            85% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            90% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            95% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
            100% { background: linear-gradient(to bottom, #87CEEB, #B5FFFC); }
        }

        .message {
            text-align: center;
            position: relative;
            z-index: 10;
            padding: 20px;
        }

        .sun {
            position: absolute;
            bottom: -150px;
            left: 50%;
            width: 150px;
            height: 150px;
            background-color: #FFD700;
            border-radius: 50%;
            box-shadow: 0 0 20px #FFD700;
            transform: translateX(-50%);
            animation: sunrise 10s linear forwards;
        }

        @keyframes sunrise {
            0% { bottom: 30px; }
            100% { bottom: 65%; }
        }

        .cloud {
            position: absolute;
            top: 30%;
            left: 30%;
            width: 200px;
            height: 60px;
            background: #fff;
            border-radius: 50px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: cloud-moving 40s linear infinite;
        }

        .cloud:before,
        .cloud:after {
            content: '';
            position: absolute;
            background: #fff;
            width: 100px;
            height: 60px;
            border-radius: 50px;
        }

        .cloud:before {
            top: -30px;
            left: 10px;
        }

        .cloud:after {
            top: -20px;
            left: 120px;
            width: 80px;
            height: 80px;
        }

        @keyframes cloud-moving {
            0% { transform: translateX(0); }
            100% { transform: translateX(200px); }
        }
    </style>
</head>
<body>
    <div class="message">
        <h1>Buenos Días</h1>
        <h2>Que el sol brille tanto como tú</h2>
    </div>
    <div class="sun"></div>
    <div class="cloud"></div>
</body>
</html>
