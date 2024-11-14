<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pedido Especial</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #fdf6e3;
            font-family: Arial, sans-serif;
            color: #333;
        }
        h1 {
            color: #e75480;
        }
        p {
            font-size: 1.2em;
            text-align: center;
            margin: 20px;
        }
        .buttons {
            display: flex;
            gap: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: 0.3s;
        }
        #btnSim {
            background-color: #e75480;
            color: #fff;
        }
        #btnNao {
            background-color: #ccc;
            color: #333;
        }
        button:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <h1>Tenho uma pergunta especial para ti!</h1>
    <p>Desde que te conheci, senti algo muito especial... Algo que cresce mais a cada momento. Por isso, criei coragem para te perguntar:</p>
    <p><strong>Quere namorar comigo?</strong></p>

    <div class="buttons">
        <button id="btnSim" onclick="responderSim()">Sim</button>
        <button id="btnNao" onclick="responderNao()">Não</button>
    </div>

    <script>
        function responderSim() {
            document.body.innerHTML = `
                <h1>Que felicidade! ❤️</h1>
                <p>Mal posso esperar para viver muitos momentos lindos ao teu lado!</p>
                <p>Obrigado por dizeres sim! 😊</p>
            `;
        }

        function responderNao() {
            document.body.innerHTML = `
                <h1>Entendo... 😔</h1>
                <p>Mesmo assim, continuarei a admirar a pessoa incrível que és. Desejo-te toda a felicidade do mundo.</p>
            `;
        }
    </script>

</body>
</html>
