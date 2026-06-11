<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agro Futuro Sustentável</title>
<style>
/* Reset e fontes */
* {margin:0; padding:0; box-sizing:border-box; font-family:Arial, sans-serif;}
body {background:black; color:white; line-height:1.6;}

/* Header futurista */
header {
    text-align:center;
    padding:50px 20px;
    background: linear-gradient(90deg, #32CD32, #000);
    color:white;
    animation: glow 2s infinite alternate;
}
header h1 {font-size:3em; font-weight:bold; letter-spacing:2px;}
header p.slogan {font-size:1.2em; font-style:italic; color:#BFFF00; margin-top:10px;}

/* Navegação */
nav ul {
    display:flex;
    justify-content:center;
    margin-top:20px;
    list-style:none;
    gap:30px;
}
nav ul li a {
    color:#BFFF00;
    text-decoration:none;
    font-weight:bold;
    transition:0.3s;
}
nav ul li a:hover {
    color:white;
    text-shadow:0 0 10px #BFFF00;
}

/* Seções */
main {padding:40px 20px;}
section {margin-bottom:60px; text-align:center;}
section h2 {color:#BFFF00; margin-bottom:20px; font-size:2em; text-transform:uppercase;}

/* Botões futuristas */
button {
    padding:15px 30px;
    border:none;
    background-color:#32CD32;
    color:black;
    font-weight:bold;
    cursor:pointer;
    transition:0.3s;
    border-radius:5px;
}
button:hover {background-color:#BFFF00; transform:scale(1.1);}

/* Formulário */
form input, form textarea {
    display:block;
    width:100%;
    max-width:400px;
    margin:10px auto;
    padding:12px;
    border-radius:5px;
    border:none;
    outline:none;
}
form button {margin-top:10px;}

/* Footer */
footer {background-color:#111; color:white; text-align:center; padding:20px;}

/* Animações */
@keyframes glow {
    from {box-shadow:0 0 10px #32CD32;}
    to {box-shadow:0 0 30px #BFFF00;}
}
</style>
</head>
<body>
<header>
    <h1>Agro Futuro Sustentável</h1>
    <p class="slogan">Cultivando o amanhã com força, tecnologia e respeito à natureza</p>
    <nav>
        <ul>
            <li><a href="#sobre">Sobre</a></li>
            <li><a href="#sustentabilidade">Sustentabilidade</a></li>
            <li><a href="#contato">Contato</a></li>
        </ul>
    </nav>
</header>

<main>
<section id="sobre">
    <h2>Nosso Agro</h2>
    <p>Unimos tecnologia, inovação e sustentabilidade para transformar o campo brasileiro em referência mundial.</p>
    <button id="learnMoreBtn">Saiba Mais</button>
    <p id="extraInfo"></p>
</section>

<section id="sustentabilidade">
    <h2>Sustentabilidade em Ação</h2>
    <p>Práticas agroecológicas, uso eficiente de recursos naturais e inovação tecnológica são a base do nosso trabalho.</p>
</section>

<section id="contato">
    <h2>Contato</h2>
    <form id="contactForm">
        <input type="text" placeholder="Seu nome" required>
        <input type="email" placeholder="Seu email" required>
        <textarea placeholder="Mensagem" required></textarea>
        <button type="submit">Enviar</button>
    </form>
    <p id="formMessage"></p>
</section>
</main>

<footer>
    <p>&copy; 2026 Agro Futuro Sustentável. Todos os direitos reservados.</p>
</footer>

<script>
// Botão "Saiba Mais"
document.getElementById('learnMoreBtn').addEventListener('click', function() {
    const info = document.getElementById('extraInfo');
    info.textContent = "Nossa missão é integrar inovação tecnológica com práticas agroecológicas para um futuro sustentável e próspero.";
    info.style.color = "#BFFF00";
});

// Envio do formulário (simulação)
document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();
    const message = document.getElementById('formMessage');
    message.textContent = "Mensagem enviada! Obrigado por entrar em contato.";
    message.style.color = "#32CD32";
    this.reset();
});
</script>
</body>
</html>
