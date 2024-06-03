<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flores en Movimiento</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(to bottom, #ffebcc, #ffccff);
            overflow: hidden;
            font-family: 'Arial', sans-serif;
        }

        .container {
            text-align: center;
            position: relative;
        }

        h1 {
            font-size: 2em;
            color: #663399;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }

        .flower {
            position: absolute;
            width: 50px;
            height: 50px;
            background-image: url('https://i.imgur.com/Jnp5wyj.png'); /* URL de una imagen de flor */
            background-size: cover;
            animation: float 10s infinite;
        }

        @keyframes float {
            0% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-100px);
            }
            100% {
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>La belleza de la naturaleza en movimiento</h1>
        <div class="flower" style="top: 50px; left: 100px; animation-duration: 6s;"></div>
        <div class="flower" style="top: 150px; left: 200px; animation-duration: 8s;"></div>
        <div class="flower" style="top: 100px; left: 300px; animation-duration: 5s;"></div>
        <div class="flower" style="top: 200px; left: 400px; animation-duration: 7s;"></div>
        <div class="flower" style="top: 250px; left: 500px; animation-duration: 9s;"></div>
    </div>
</body>
</html>

