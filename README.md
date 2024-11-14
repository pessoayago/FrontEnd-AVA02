<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cristiano Ronaldo - Carreira e Vida Pessoal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background: #4CAF50;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        .tab {
            display: flex;
            justify-content: center;
            margin: 10px 0;
        }
        .tab button {
            background: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            margin: 0 5px;
            border-radius: 5px;
        }
        .tab button.active {
            background: #45a049;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
            background: white;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: none;
        }
        .container.active {
            display: block;
        }
        img {
            max-width: 100%;
            border-radius: 5px;
        }
        footer {
            text-align: center;
            padding: 10px 0;
            background: #333;
            color: white;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        .club {
            margin: 20px 0;
        }
        .club img {
            width: 150px; /* Ajuste o tamanho da imagem conforme necessário */
            display: block;
            margin: 10px auto;
        }
        @media (max-width: 600px) {
            .tab {
                flex-direction: column;
            }
            .tab button {
                margin: 5px 0;
                width: 100%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Cristiano Ronaldo</h1>
</header>

<div class="tab">
    <button class="active" onclick="showTab('carreira')">Carreira</button>
    <button onclick="showTab('vida-pessoal')">Vida Pessoal</button>
</div>

<div id="carreira" class="container active">
    <h2>Carreira</h2>
    <p>Cristiano Ronaldo dos Santos Aveiro, nascido em 5 de fevereiro de 1985, é um jogador de futebol português considerado um dos melhores da história. Ele jogou em vários clubes, onde deixou sua marca indelével. Aqui estão os clubes que Ronaldo representou:</p>

    <div class="club">
        <h3>Sporting CP</h3>
        <img src="https://via.placeholder.com/150?text=Sporting+CP" alt="Cristiano Ronaldo no Sporting CP">
    </div>

    <div class="club">
        <h3>Manchester United (2003-2009)</h3>
        <img src="https://via.placeholder.com/150?text=Manchester+United" alt="Cristiano Ronaldo no Manchester United">
    </div>

    <div class="club">
        <h3>Real Madrid (2009-2018)</h3>
        <img src="https://via.placeholder.com/150?text=Real+Madrid" alt="Cristiano Ronaldo no Real Madrid">
    </div>

    <div class="club">
        <h3>Juventus (2018-2021)</h3>
        <img src="https://via.placeholder.com/150?text=Juventus" alt="Cristiano Ronaldo na Juventus">
    </div>

    <div class="club">
        <h3>Manchester United (2021-2022)</h3>
        <img src="https://via.placeholder.com/150?text=Manchester+United+2" alt="Cristiano Ronaldo no Manchester United novamente">
    </div>

    <div class="club">
        <h3>Al Nassr (2023-presente)</h3>
        <img src="https://via.placeholder.com/150?text=Al+Nassr" alt="Cristiano Ronaldo no Al Nassr">
    </div>
</div>

<div id="vida-pessoal" class="container">
    <h2>Vida Pessoal</h2>
    <p>Cristiano Ronaldo nasceu na Ilha da Madeira, Portugal. É pai de quatro filhos e é conhecido por seu envolvimento em várias obras de caridade. Ronaldo também é um empresário de sucesso, com sua própria linha de roupas e perfumes.</p>
    <img src="https://via.placeholder.com/800x400?text=Cristiano+Ronaldo+com+seus+filhos" alt="Cristiano Ronaldo com seus filhos">
    <p>Além de sua carreira esportiva, ele é uma figura pública influente, com milhões de seguidores nas redes sociais, onde compartilha sua vida e seus treinos.</p>
</div>

<footer>
    <p>&copy; 2024 Cristiano Ronaldo. Todos os direitos reservados.</p>
</footer>

<script>
    function showTab(tabName) {
        // Esconde todas as abas
        const tabs = document.querySelectorAll('.container');
        tabs.forEach(tab => {
            tab.classList.remove('active');
        });

        // Remove a classe ativa de todos os botões
        const buttons = document.querySelectorAll('.tab button');
        buttons.forEach(button => {
            button.classList.remove('active');
        });

        // Exibe a aba selecionada
        document.getElementById(tabName).classList.add('active');
        // Adiciona a classe ativa ao botão correspondente
        const activeButton = Array.from(buttons).find(button => button.textContent.toLowerCase() === tabName);
        if (activeButton) {
            activeButton.classList.add('active');
        }
    }
</script>

</body>
</html>
