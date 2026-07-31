# Lahey
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Declaração de Amor ❤️</title>
    <style>
        body {
            background-color: #ffe6eb;
            font-family: 'Arial', sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        .card {
            background-color: #ffffff;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(255, 77, 109, 0.2);
            border: 2px solid #ff4d6d;
        }

        h1 {
            color: #ff4d6d;
            font-size: 3rem;
            margin-bottom: 10px;
            animation: pulsar 1.5s infinite;
            display: none; /* Esconde a mensagem no início */
        }

        .beijos {
            font-size: 2rem;
            margin-top: 20px;
            min-height: 50px;
        }

        button {
            background-color: #ff4d6d;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2rem;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, background-color 0.2s;
            margin-top: 20px;
        }

        button:hover {
            background-color: #ff758f;
            transform: scale(1.05);
        }

        @keyframes pulsar {
            0% { transform: scale(1); }
            50% { transform: scale(1.08); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>

    <div class="card">
        <h1 id="mensagem-amor">❤️ EU TE AMO! ❤️</h1>
        <div class="beijos" id="area-beijos">💋 💋 💋</div>
        <button id="btn-acao" onclick="revelarEBeijar()">Clique aqui para uma surpresa! 🎁</button>
    </div>

    <script>
        function revelarEBeijar() {
            const mensagem = document.getElementById('mensagem-amor');
            const area = document.getElementById('area-beijos');
            const botao = document.getElementById('btn-acao');

            // Exibe a mensagem de amor
            mensagem.style.display = 'block';

            // Adiciona mais um beijo a cada clique
            area.innerHTML += " 💋";

            // Altera o texto do botão após a primeira revelação
            botao.textContent = "Mandar mais beijos! 💋";
        }
    </script>

</body>
</html>