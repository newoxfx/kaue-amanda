<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kauê & Amanda: Nosso Amor Infinito ❤️</title>
    <!-- Importando fontes bonitas do Google Fonts para um visual profissional -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Montserrat:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet">
    
    <style>
        /* 
           ======================================================
           1. Variáveis CSS para Cores e Fontes (Fácil Personalização)
           ======================================================
        */
        :root {
            --primary-color: #d63384;      /* Rosa vibrante (títulos secundários, detalhes) */
            --secondary-color: #e65c9f;    /* Rosa médio (linhas, detalhes) */
            --light-pink-bg: #ffe0e6;      /* Rosa muito claro para fundo inicial */
            --soft-pink-bg: #fff0f5;       /* Rosa quase branco para cards/seções */
            --dark-pink-text: #c2185b;     /* Rosa escuro para títulos principais, poesia */
            --text-color-main: #333;       /* Cor padrão do texto */
            --text-color-light: #555;      /* Cor de texto mais suave */
            --bg-gradient-start: #fce4ec;  /* Gradiente de fundo mais suave */
            --bg-gradient-end: #fff0f5;    /* Gradiente de fundo mais suave */

            --font-display: 'Dancing Script', cursive; /* Fonte para títulos maiores e assinatura */
            --font-heading: 'Playfair Display', serif; /* Fonte para subtítulos e destaques */
            --font-body: 'Montserrat', sans-serif;     /* Fonte para o corpo do texto */

            --shadow-light: 0 4px 15px rgba(0, 0, 0, 0.08);
            --shadow-medium: 0 8px 25px rgba(0, 0, 0, 0.12);
        }

        /* 
           ======================================================
           2. Estilos Globais e Reset Básico
           ======================================================
        */
        body {
            font-family: var(--font-body);
            background: linear-gradient(135deg, var(--bg-gradient-start) 0%, var(--bg-gradient-end) 100%); /* Gradiente suave de fundo */
            color: var(--text-color-main);
            margin: 0;
            padding: 0;
            line-height: 1.6;
            scroll-behavior: smooth; /* Rolagem suave para navegação (se houvesse) */
            overflow-x: hidden; /* Evita rolagem horizontal */
            min-height: 100vh; /* Ocupa a altura total da viewport */
            display: flex;
            flex-direction: column; /* Para empurrar o footer para o final */
            align-items: center; /* Centraliza o conteúdo principal horizontalmente */
        }

        .container {
            width: 100%;
            max-width: 960px; /* Largura maior para o site */
            margin: 0 auto;
            padding: 20px;
            box-sizing: border-box;
            z-index: 10; /* Garante que o conteúdo fique acima das decorações de fundo */
            position: relative; /* Necessário para z-index */
        }

        /* 
           ======================================================
           3. Estilos de Títulos e Parágrafos
           ======================================================
        */
        h1, h2, h3 {
            font-family: var(--font-heading);
            color: var(--primary-color);
            margin-bottom: 20px;
            text-align: center;
        }

        h1 {
            font-family: var(--font-display); /* Fonte cursiva para o título principal */
            font-size: 4.2em; /* Título bem grande */
            color: var(--dark-pink-text);
            text-shadow: 2px 2px 5px rgba(0,0,0,0.05); /* Sombra sutil no texto */
            margin-top: 40px;
            margin-bottom: 10px;
            letter-spacing: 1.8px;
            line-height: 1.2;
        }

        h2 {
            font-size: 2.5em; /* Subtítulo grande */
            color: var(--secondary-color);
            margin-bottom: 30px;
            letter-spacing: 1px;
            font-weight: 500;
        }

        h3 {
            font-size: 1.8em;
            color: var(--primary-color);
            margin-top: 40px;
            margin-bottom: 25px;
            font-weight: 600;
        }

        p {
            font-size: 1.15em; /* Tamanho padrão do parágrafo */
            margin-bottom: 20px;
            color: var(--text-color-light);
            text-align: center;
            max-width: 780px;
            margin-left: auto;
            margin-right: auto;
        }

        /* 
           ======================================================
           4. Estilos de Seções (Cartões)
           ======================================================
        */
        section {
            background-color: var(--soft-pink-bg);
            border-radius: 25px; /* Bordas mais arredondadas */
            padding: 50px 60px;
            margin-bottom: 40px;
            box-shadow: var(--shadow-medium);
            text-align: center;
            position: relative;
            opacity: 0; /* Começa invisível para a animação */
            transform: translateY(40px); /* Move para baixo para a animação */
            animation: fadeInAndSlideUp 1s ease-out forwards; /* Animação de entrada */
            animation-delay: var(--delay-offset, 0s); /* Atraso personalizado para cada seção */
        }

        /* Atrasos específicos para cada seção */
        #hero-section { --delay-offset: 0s; }
        #poetry-section { --delay-offset: 0.5s; }
        #memories-section { --delay-offset: 1s; }
        #amanda-world-section { --delay-offset: 1.5s; } /* NOVO ATRASO PARA A NOVA SEÇÃO */
        #final-message-section { --delay-offset: 2s; } /* AJUSTADO O ATRASO */

        /* 
           ======================================================
           5. Estilos da Poesia
           ======================================================
        */
        .poesia {
            font-family: var(--font-heading); /* Fonte de destaque para a poesia */
            font-size: 1.9em;
            font-style: italic;
            color: var(--dark-pink-text);
            margin: 40px auto;
            padding: 30px 40px;
            background-color: #fffafc; /* Fundo muito claro para a poesia */
            border-left: 6px solid var(--secondary-color); /* Borda decorativa */
            border-right: 6px solid var(--secondary-color);
            border-radius: 12px;
            max-width: 650px;
            box-shadow: inset 0 0 15px rgba(0,0,0,0.05); /* Sombra interna sutil */
            line-height: 1.8;
        }

        .poesia span {
            display: block; /* Cada linha em seu próprio bloco */
            margin-bottom: 12px;
            opacity: 0; /* Começa invisível para a animação de texto */
            transform: translateY(15px);
            animation: fadeInText 0.9s ease-out forwards; /* Animação de entrada para cada linha */
            animation-delay: calc(var(--delay-offset-line) + 0.3s); /* Atraso progressivo */
        }
        /* Atrasos para cada linha da poesia */
        .poesia span:nth-child(1) { --delay-offset-line: 0.2s; }
        .poesia span:nth-child(2) { --delay-offset-line: 0.4s; }
        .poesia span:nth-child(3) { --delay-offset-line: 0.6s; }
        .poesia span:nth-child(4) { --delay-offset-line: 0.8s; }
        .poesia span:nth-child(5) { --delay-offset-line: 1.0s; }
        .poesia span:nth-child(6) { --delay-offset-line: 1.2s; }
        .poesia span:nth-child(7) { --delay-offset-line: 1.4s; }
        .poesia span:nth-child(8) { --delay-offset-line: 1.6s; }


        /* 
           ======================================================
           6. Estilos da Seção de Momentos (Cards)
           ======================================================
        */
        .memory-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Layout responsivo com grid */
            gap: 30px; /* Espaçamento entre os cards */
            margin-top: 35px;
        }

        .memory-card {
            background-color: #fff;
            padding: 25px;
            border-radius: 18px;
            box-shadow: var(--shadow-light);
            transition: transform 0.3s ease, box-shadow 0.3s ease; /* Transições suaves para hover */
            cursor: pointer;
            position: relative;
            overflow: hidden; /* Garante que pseudo-elementos fiquem dentro */
            text-align: center;
        }

        .memory-card:hover {
            transform: translateY(-10px) scale(1.03); /* Efeito de elevação e leve aumento */
            box-shadow: var(--shadow-medium); /* Sombra mais proeminente no hover */
        }

        .memory-card::before {
            content: '💖'; /* Ícone decorativo (emoji) */
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 2.2em;
            opacity: 0.15;
            z-index: 0;
            transform: rotate(-25deg);
        }

        .memory-card h4 {
            font-family: var(--font-heading);
            color: var(--primary-color);
            margin-bottom: 12px;
            font-size: 1.4em;
            z-index: 1; /* Garante que o texto fique acima do pseudo-elemento */
            position: relative;
        }

        .memory-card p {
            font-size: 1em;
            color: var(--text-color-light); /* Ajustado para consistência com as variáveis */
            text-align: center;
            z-index: 1;
            position: relative;
            max-width: none; /* Remove a limitação de largura para os cards */
        }

        /* 
           ======================================================
           7. Estilos da Nova Seção "O Universo da Minha Amanda"
           ======================================================
        */
        .amanda-favorites-list {
            list-style: none; /* Remove marcadores de lista padrão */
            padding: 0;
            margin: 30px auto;
            max-width: 600px;
            text-align: left; /* Alinha o texto da lista à esquerda */
        }

        .amanda-favorites-list li {
            background-color: #fffafc;
            border-left: 5px solid var(--secondary-color);
            margin-bottom: 15px;
            padding: 15px 25px;
            border-radius: 10px;
            box-shadow: var(--shadow-light);
            font-size: 1.1em;
            color: var(--text-color-main);
            display: flex; /* Para alinhar o ícone e o texto */
            align-items: center;
            gap: 15px; /* Espaçamento entre ícone e texto */
        }

        .amanda-favorites-list li strong {
            color: var(--dark-pink-text);
            font-family: var(--font-heading);
            font-weight: 700;
        }

        .amanda-favorites-list li .icon {
            font-size: 1.5em;
            color: var(--primary-color);
        }

        /*
           Estilo para o container da imagem principal (se for adicionada)
           (Este estilo é opcional e só será aplicado se você adicionar a imagem conforme a resposta anterior)
        */
        .main-image-container {
            margin: 30px auto; /* Centraliza e adiciona margem */
            max-width: 80%; /* Limita a largura da imagem */
            overflow: hidden; /* Garante que a borda arredondada funcione bem */
            border-radius: 20px; /* Bordas arredondadas para a imagem */
            box-shadow: var(--shadow-medium); /* Sombra elegante */
            animation: fadeInAndScale 1.2s ease-out forwards; /* Animação de entrada */
            animation-delay: 0.8s; /* Atraso para aparecer depois da seção */
            display: block; /* Para garantir que as margens funcionem */
        }

        .featured-image {
            width: 100%; /* A imagem ocupa 100% da largura do seu container */
            height: auto; /* Mantém a proporção da imagem */
            display: block; /* Remove espaço extra abaixo da imagem */
            transition: transform 0.5s ease; /* Transição suave para o hover */
        }

        .featured-image:hover {
            transform: scale(1.05); /* Efeito de zoom sutil ao passar o mouse */
        }

        @keyframes fadeInAndScale {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }

        /* 
           ======================================================
           8. Estilos de Assinatura e Coração
           ======================================================
        */
        .assinatura {
            font-family: var(--font-display);
            font-size: 3em; /* Assinatura maior */
            color: var(--dark-pink-text);
            margin-top: 50px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.04);
            animation: pulseText 2.5s infinite alternate ease-in-out; /* Animação de pulsar */
            display: block;
            line-height: 1.2;
        }

        .heart {
            color: var(--secondary-color);
            font-size: 3.5em; /* Coração bem grande */
            margin-top: 30px;
            animation: pulse 1.8s infinite alternate; /* Animação de pulsar do coração */
            display: block;
        }

        /* 
           ======================================================
           9. Estilos do Rodapé (Footer)
           ======================================================
        */
        footer {
            margin-top: 60px;
            padding: 40px;
            text-align: center;
            font-size: 0.95em;
            color: #777;
            background-color: #fcf4f7; /* Fundo suave para o rodapé */
            border-top: 1px solid #f0e6eb;
            width: 100%;
            box-sizing: border-box;
            line-height: 1.5;
            z-index: 10;
            position: relative;
        }
        footer p {
            font-size: 0.9em;
            margin-top: 15px;
            color: #999;
        }

        /* 
           ======================================================
           10. Animações Keyframes
           ======================================================
        */
        @keyframes fadeInAndSlideUp {
            from { opacity: 0; transform: translateY(40px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInText {
            from { opacity: 0; transform: translateY(15px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.18); opacity: 0.9; }
            100% { transform: scale(1); opacity: 1; }
        }

        @keyframes pulseText {
            0% { transform: scale(1); }
            50% { transform: scale(1.03); }
            100% { transform: scale(1); }
        }

        /* 
           ======================================================
           11. Efeito de Confete (Decoração de Fundo)
           ======================================================
        */
        body::before, body::after,
        .confetti-1, .confetti-2, .confetti-3 {
            content: '';
            position: fixed;
            background-color: var(--secondary-color);
            border-radius: 50%;
            opacity: 0.4;
            animation: confettiFall 12s infinite linear;
            z-index: 0; /* Fica atrás do conteúdo principal */
        }

        body::before { /* Pequeno confete rosa claro */
            width: 10px; height: 10px;
            left: 10%; top: -10%;
            animation-delay: 0s;
            background-color: #f7cac9; 
            box-shadow: 0 0 8px #f7cac9;
        }
        body::after { /* Pequeno confete rosa médio */
            width: 8px; height: 8px;
            left: 80%; top: -20%;
            animation-delay: 5s;
            background-color: #f9d5e5;
            box-shadow: 0 0 8px #f9d5e5;
        }
        .confetti-1 { /* Maior e mais escuro */
            width: 12px; height: 12px;
            left: 30%; top: -5%;
            animation-delay: 2s;
            background-color: var(--primary-color);
            box-shadow: 0 0 10px var(--primary-color);
        }
        .confetti-2 { /* Médio e vibrante */
            width: 9px; height: 9px;
            left: 60%; top: -15%;
            animation-delay: 7s;
            background-color: var(--dark-pink-text);
            box-shadow: 0 0 8px var(--dark-pink-text);
        }
        .confetti-3 { /* Pequeno e discreto */
            width: 7px; height: 7px;
            left: 20%; top: -25%;
            animation-delay: 9s;
            background-color: #f0e6eb;
            box-shadow: 0 0 6px #f0e6eb;
        }

        @keyframes confettiFall {
            0% { transform: translateY(-10vh) translateX(0) rotate(0deg); opacity: 0.7; }
            25% { transform: translateY(20vh) translateX(30px) rotate(90deg); opacity: 0.6; }
            50% { transform: translateY(50vh) translateX(-20px) rotate(180deg); opacity: 0.5; }
            75% { transform: translateY(80vh) translateX(10px) rotate(270deg); opacity: 0.6; }
            100% { transform: translateY(110vh) translateX(-10px) rotate(360deg); opacity: 0.7; }
        }

        /* 
           ======================================================
           12. Responsividade (Media Queries)
           ======================================================
        */
        @media (max-width: 992px) {
            .container {
                max-width: 768px;
            }
            h1 { font-size: 3.5em; }
            h2 { font-size: 2em; }
            h3 { font-size: 1.6em; }
            section {
                padding: 40px;
                margin-bottom: 35px;
            }
            .poesia {
                font-size: 1.6em;
                margin: 35px auto;
                padding: 25px 30px;
            }
            .assinatura {
                font-size: 2.5em;
            }
            .heart {
                font-size: 3em;
            }
            .amanda-favorites-list li {
                font-size: 1.05em;
                padding: 12px 20px;
            }
        }

        @media (max-width: 768px) {
            .container {
                max-width: 100%;
                padding: 15px;
            }
            h1 { font-size: 2.8em; }
            h2 { font-size: 1.6em; }
            h3 { font-size: 1.4em; }
            p { font-size: 1em; }
            section {
                padding: 30px;
                margin-bottom: 30px;
                border-radius: 18px;
            }
            .poesia {
                font-size: 1.3em;
                margin: 30px auto;
                padding: 20px 25px;
                border-left-width: 4px;
                border-right-width: 4px;
            }
            .memory-grid {
                grid-template-columns: 1fr; /* Uma coluna em telas menores */
                gap: 20px;
            }
            .memory-card {
                padding: 20px;
                border-radius: 15px;
            }
            .memory-card h4 {
                font-size: 1.2em;
            }
            .assinatura {
                font-size: 2em;
            }
            .heart {
                font-size: 2.5em;
            }
            footer {
                padding: 30px 15px;
            }
            .amanda-favorites-list {
                max-width: 90%;
            }
            .amanda-favorites-list li {
                font-size: 1em;
                padding: 10px 15px;
                gap: 10px;
            }
        }

        @media (max-width: 480px) {
            h1 { font-size: 2.2em; }
            h2 { font-size: 1.3em; margin-bottom: 20px; }
            h3 { font-size: 1.2em; margin-top: 30px; margin-bottom: 15px; }
            p { font-size: 0.95em; }
            section {
                padding: 20px;
                margin-bottom: 20px;
                border-radius: 15px;
            }
            .poesia {
                font-size: 1.1em;
                margin: 20px auto;
                padding: 15px 20px;
                border-left-width: 3px;
                border-right-width: 3px;
            }
            .assinatura {
                font-size: 1.6em;
                margin-top: 30px;
            }
            .heart {
                font-size: 2em;
                margin-top: 20px;
            }
            .memory-card::before {
                font-size: 1.8em;
                top: 10px;
                right: 15px;
            }
            .amanda-favorites-list li {
                font-size: 0.9em;
                flex-direction: column; /* Ícone e texto em linhas separadas em telas muito pequenas */
                align-items: flex-start;
                padding: 10px 15px;
            }
            .amanda-favorites-list li .icon {
                margin-bottom: 5px;
            }
        }
    </style>
</head>
<body>
    <!-- Decorações de Confete no Fundo -->
    <div class="confetti-1"></div>
    <div class="confetti-2"></div>
    <div class="confetti-3"></div>

    <div class="container">
        <header>
            <h1>Kauê & Amanda</h1>
            <h2>Para a mulher que amo, com os detalhes da nossa história ✨</h2>
        </header>

        <main>
            <section id="hero-section">
                <h3>A Mensagem do Meu Coração</h3>
                <p>
                    Minha amada Amanda, cada dia ao seu lado é uma página de um livro encantado, repleto de risos, cumplicidade e um amor que só cresce. Desde que nossos caminhos se cruzaram, meu mundo ganhou novas cores, uma melodia mais suave e um propósito ainda mais lindo. Este espaço é uma pequena janela para a imensidão do que sinto por você.
                </p>
                <p>
                    Saber que você gosta de mim, que seus olhos brilham ao ver minhas fotos e que seu cabelo lindo é uma de suas paixões, me enche de alegria. Você é a minha inspiração, o abraço que acalma, o olhar que compreende sem palavras. Com você, até os dias cinzentos ganham um brilho especial. Obrigado por ser você, por me escolher e por construirmos juntos essa linda jornada. Meu coração transborda de gratidão e carinho por ter você na minha vida.
                </p>
            </section>

            <section id="poetry-section">
                <h3>Nossa Poesia, Nosso Eterno Cantar</h3>
                <div class="poesia">
                    <span>Em cada amanhecer, Amanda, meu sol,</span>
                    <span>Seu nome sussurra, meu mais doce farol.</span>
                    <span>Com você, o tempo é brisa, o amor é canção,</span>
                    <span>Um porto seguro para o meu coração.</span>
                    <br>
                    <span>Teu riso me veste, teu carinho me guia,</span>
                    <span>A cada passo, nova e pura magia.</span>
                    <span>Kauê para Amanda, promessa no ar,</span>
                    <span>Um para sempre que vamos sonhar.</span>
                </div>
                <p>
                    Que estes versos sejam um espelho do carinho, da admiração e da paixão que sinto por você, meu amor. Você me completa de um jeito que nunca imaginei ser possível.
                </p>
            </section>

            <section id="memories-section">
                <h3>Nossos Momentos Inesquecíveis</h3>
                <p>
                    Cada momento ao seu lado é um tesouro, e alguns deles moldaram nossa linda história.
                </p>
                <div class="memory-grid">
                    <div class="memory-card">
                        <h4>Onde Tudo Começou: Nossa Call</h4>
                        <p>Foi em uma call, em meio a vozes e risadas, que nossos olhares (e corações) se encontraram pela primeira vez. Quem diria que o amor nasceria ali?</p>
                    </div>
                    <div class="memory-card">
                        <h4>Meu Protetor, Minha Leoa!</h4>
                        <p>Eu sempre estarei aqui para te proteger, livrando você de qualquer assédio. E sua força é linda, como naquele dia que você brigou por mim. Somos um time!</p>
                    </div>
                    <div class="memory-card">
                        <h4>Nossa Canção Secreta</h4>
                        <p>A melodia que virou trilha sonora do nosso amor. Cada nota, uma história, cada refrão, um "eu te amo" em segredo.</p>
                    </div>
                    <div class="memory-card">
                        <h4>A Viagem Especial</h4>
                        <p>Explorar novos lugares ao seu lado é sempre a melhor aventura. As paisagens se tornam mais bonitas com a sua presença.</p>
                    </div>
                    <div class="memory-card">
                        <h4>As Maratona no Sofá</h4>
                        <p>Nossos filmes e séries, as risadas, as pipocas... Cada momento simples ao seu lado se torna extraordinário.</p>
                    </div>
                    <div class="memory-card">
                        <h4>Os Planos para o Futuro</h4>
                        <p>Sonhar e planejar a vida ao seu lado é a parte mais emocionante de todas. Mal posso esperar para viver cada um deles contigo.</p>
                    </div>
                </div>
                <p style="margin-top: 40px;">
                    Que venham muitos e muitos momentos para preencher ainda mais nosso álbum de memórias!
                </p>
            </section>

            <section id="amanda-world-section">
                <h3>O Universo da Minha Amanda</h3>
                <p>
                    Cada detalhe seu me encanta. Conhecer seus gostos e sonhos é mergulhar ainda mais fundo no mundo da pessoa mais incrível que já conheci.
                </p>
                <ul class="amanda-favorites-list">
                    <li><span class="icon">🎶</span> <strong>Música Favorita:</strong> Sanguessuga - Orochi</li>
                    <li><span class="icon">🍝</span> <strong>Comida Favorita:</strong> Strogonoff</li>
                    <li><span class="icon">💖</span> <strong>O que você mais ama (além de mim!):</strong> Ver minhas fotos e seu lindo cabelo.</li>
                    <li><span class="icon">✈️</span> <strong>Lugares dos Sonhos Juntos:</strong> Fernando de Noronha e Dubai</li>
                    <li><span class="icon">🎬</span> <strong>Hobbies e Atividades:</strong> Assistir filmes/séries, cozinhar juntos (escolhendo uma receita e fazendo!), passear e conhecer lugares novos na cidade.</li>
                </ul>
                <p>
                    E o maior de todos os nossos sonhos, o que mais me move e me faz querer construir um futuro eterno ao seu lado:
                </p>
                <p class="poesia" style="font-size: 1.6em; padding: 20px 30px; margin-top: 20px;">
                    <span>Nosso Sonho de Família:</span>
                    <span>Criar e amar os filhos que teremos juntos.</span>
                </p>
                <p>
                    Mal posso esperar para viver cada um desses momentos e sonhos com você, minha vida.
                </p>
            </section>

            <section id="final-message-section">
                <h3>Eternamente Seu</h3>
                <p>
                    Amanda, cada dia que passa, meu amor e admiração por você só aumentam. Você é a estrela que ilumina meu céu, a flor mais linda do meu jardim, a paz que encontro no meu coração. Que a nossa jornada continue sendo repleta de amor incondicional, companheirismo, respeito, cumplicidade e muitas, muitas alegrias.
                </p>
                <p>
                    Estarei sempre aqui, pronto para te amar, te apoiar, te proteger e te fazer a pessoa mais feliz do mundo, com a certeza de que nosso amor é um presente divino.
                </p>
            </section>
        </main>

        <footer>
            <span class="assinatura">Com todo o meu amor eterno, <br>Seu Kauê</span>
            <div class="heart">&#10084;&#65039;</div> <!-- Emoji de coração -->
            <p>&copy; 2025 - Feito com o coração para Amanda. Todos os direitos de amar reservados. ❤️</p>
        </footer>
    </div>
</body>
</html>
