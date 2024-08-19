<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>C&K - Amor Eterno</title>
    <style>
        body {
            background-color: #ffdde1;
            color: #333;
            font-family: 'Arial', sans-serif;
            text-align: center;
            padding: 20px;
            overflow-x: hidden;
        }
        .hidden {
            display: none;
        }
        header {
            background-color: #ff6f61;
            padding: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        header h1 {
            color: white;
            font-size: 3em;
            margin: 0;
        }
        header::after {
            content: "♥";
            font-size: 5em;
            color: white;
            position: absolute;
            right: 20px;
            top: 10px;
        }
        .content {
            margin-top: 50px;
            max-width: 90%;
            padding: 20px;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .cta {
            margin-top: 30px;
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        .cta a {
            text-decoration: none;
            background-color: #ff6f61;
            color: white;
            padding: 15px 30px;
            border-radius: 30px;
            font-size: 1.2em;
            transition: background-color 0.3s;
        }
        .cta a:hover {
            background-color: #ff3b30;
        }
        .heart {
            font-size: 5em;
            cursor: pointer;
            transition: transform 0.3s;
        }
        .heart:hover {
            transform: scale(1.2);
        }
        footer {
            margin-top: 50px;
            font-size: 0.9em;
            color: #777;
        }
        .surprise {
            font-size: 3em;
            color: #ff6f61;
            display: none;
        }
        .funny-message {
            font-size: 1.5em;
            color: #ff6f61;
            margin: 20px;
        }
    </style>
</head>
<body>

    <!-- Música de fundo -->
    <audio autoplay loop>
        <source src="sua_musica.mp3" type="audio/mpeg">
        Seu navegador não suporta a reprodução de áudio.
    </audio>

    <header>
        <h1>C&K</h1>
    </header>

    <div class="content" id="page1">
        <h2>Bem-vinda ao nosso jogo de amor, Karol!</h2>
        <p>Cada clique em um coração revela uma razão pela qual eu te amo.</p>
        <div class="cta">
            <a href="#" onclick="goToPage('page2')">Começar</a>
        </div>
    </div>

    <div class="content hidden" id="page2">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(1)">💖</span>
        <p id="message1"></p>
        <a href="#" class="cta hidden" id="next1" onclick="goToPage('page3')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page3">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(2)">💖</span>
        <p id="message2"></p>
        <a href="#" class="cta hidden" id="next2" onclick="goToPage('page4')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page4">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(3)">💖</span>
        <p id="message3"></p>
        <a href="#" class="cta hidden" id="next3" onclick="goToPage('page5')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page5">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(4)">💖</span>
        <p id="message4"></p>
        <a href="#" class="cta hidden" id="next4" onclick="goToPage('page6')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page6">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(5)">💖</span>
        <p id="message5"></p>
        <a href="#" class="cta hidden" id="next5" onclick="goToPage('page7')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page7">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(6)">💖</span>
        <p id="message6"></p>
        <a href="#" class="cta hidden" id="next6" onclick="goToPage('page8')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page8">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(7)">💖</span>
        <p id="message7"></p>
        <a href="#" class="cta hidden" id="next7" onclick="goToPage('page9')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page9">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(8)">💖</span>
        <p id="message8"></p>
        <a href="#" class="cta hidden" id="next8" onclick="goToPage('page10')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page10">
        <h2>Clique no coração para descobrir o motivo</h2>
        <span class="heart" onclick="revealLove(9)">💖</span>
        <p id="message9"></p>
        <a href="#" class="cta hidden" id="next9" onclick="goToPage('page11')">Próxima Etapa</a>
    </div>

    <div class="content hidden" id="page11">
        <h2>Surpresa!</h2>
        <p class="funny-message">Você achou que acabou? Haha, ainda tem mais!</p>
        <p>Vou ser sincero: eu não posso te dizer o quanto você é importante para mim em apenas uma mensagem. Então, prepare-se para mais uma surpresa...</p>
        <span class="heart" onclick="revealFunny()">💖</span>
        <div id="funnyText" class="hidden">
            <p class="funny-message">Ah!!! Te peguei de novooooo hahahahah teeee amo minha garota , vamos à pergunta final!</p>
            <a href="#" class="cta" onclick="goToPage('finalPage')">Pergunta Final</a>
        </div>
    </div>

    <div class="content hidden" id="finalPage">
        <h2>Você aceita se casar comigo? lembre-se essa pergunta será única... Pois meu amor por você é verdadeiro!</h2>
        <div class="cta">
            <a href="https://wa.me/553198202782?text=Eu%20te%20amo" target="_blank">Sim</a>
            <a href="https://wa.me/553198202782?text=Aceito%20namorar%20contigo%20simmmm%20meu%20amor" target="_blank">Não</a>
        </div>
    </div>

    <footer>
        <p>Com todo o meu amor, para sempre seu, Cícero.</p>
    </footer>

    <script>
        const loveMessages = [
            "Porque você ilumina o meu dia!",
            "Porque seu sorriso é contagiante!",
            "Porque ao seu lado me sinto completo!",
            "Porque cada momento com você é mágico!",
            "Porque você é a pessoa mais incrível que já conheci!",
            "Porque meu amor por você é eterno!",
            "Porque você sempre sabe como me fazer sorrir!",
            "Porque te amo mais a cada dia que passa!",
            "Porque você é a minha paz e alegria!",
            "Porque a vida ao seu lado é um sonho realizado!"
        ];

        function revealLove(index) {
            document.getElementById('message' + index).textContent = loveMessages[index - 1];
            document.querySelectorAll('.heart')[index - 1].style.pointerEvents = "none";
            document.getElementById('next' + index).classList.remove('hidden');
        }

        function goToPage(pageId) {
            document.querySelectorAll('.content').forEach(page => page.classList.add('hidden'));
            document.getElementById(pageId).classList.remove('hidden');
        }

        function revealFunny() {
            document.getElementById('funnyText').classList.remove('hidden');
        }
    </script>

</body>
</html>
