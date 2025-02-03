# maluu
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Malu</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: black;
            color: white;
            display: flex;
            justify-content: center;
            flex-direction: column;
            align-items: center;
        }

        .content {
            width: 80%; /* Área principal do conteúdo */
            padding: 20px;
            text-align: center;
        }

        .sidebar {
            position: fixed;
            top: 0;
            height: 100%;
            width: 50px; /* Largura do painel lateral mais fino */
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }

        .sidebar img {
            width: 100%; /* A imagem do anúncio ocupa toda a largura do painel */
            height: 100%; /* A imagem ocupa toda a altura do painel */
            object-fit: cover; /* Faz a imagem cobrir todo o espaço */
            border-radius: 10px;
        }

        .left-sidebar {
            left: 0; /* Lado esquerdo */
        }

        .right-sidebar {
            right: 0; /* Lado direito */
        }

        .header {
            padding: 20px;
            background: black;
            font-size: 24px;
            font-weight: bold;
            text-align: center;
        }

        .button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 18px;
            background: red;
            color: white;
            border: none;
            cursor: pointer;
        }

        .scary-img {
            margin-top: 20px;
            width: 300px;
            border: 5px solid red;
            display: none; /* A imagem começa oculta */
            margin-left: auto;
            margin-right: auto;
        }

        .top-image {
            margin-bottom: 20px; /* Espaçamento entre a imagem e o botão */
            width: 300px; /* Tamanho da imagem */
            display: block;
            margin-left: auto;
            margin-right: auto;
        }
    </style>
    <script>
        function toggleScaryImage() {
            var image = document.getElementById("scaryImage");
            if (image.style.display === "none") {
                image.style.display = "block"; // Exibe a imagem
                image.src = "https://i.imgur.com/AtK197Y.jpeg"; // Atualiza a imagem
            } else {
                image.style.display = "none"; // Esconde a imagem
            }
        }
    </script>
</head>
<body>

    <div class="content">
        <div class="header">
            ⚠️ Bem-vindo ao mundo de Malu ⚠️
        </div>
        <p>Você ousou entrar... Agora é tarde demais...</p>

        <!-- Imagem acima do botão -->
        <img class="top-image" src="https://i.imgur.com/SCLyNkk.jpeg" alt="Imagem assustadora">

        <button class="button" onclick="toggleScaryImage()">NAO APERTE!</button>

        <!-- Imagem assustadora que será exibida ao apertar o botão -->
        <img id="scaryImage" class="scary-img" src="https://via.placeholder.com/300/000000/ff0000?text=BOO!" alt="Imagem assustadora">
    </div>

    <!-- Lado esquerdo -->
    <div class="sidebar left-sidebar">
        <a href="https://www.roblox.com/pt/users/1441346019/profile" target="_blank">
            <img src="https://i.imgur.com/eQEEntM.jpeg" alt="Anúncio">
        </a>
    </div>

    <!-- Lado direito -->
    <div class="sidebar right-sidebar">
        <a href="https://www.roblox.com/pt/users/1441346019/profile" target="_blank">
            <img src="https://i.imgur.com/eQEEntM.jpeg" alt="Anúncio">
        </a>
    </div>

</body>
</html>
