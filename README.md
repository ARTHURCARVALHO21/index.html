<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AGRO NEXUS 2050 | O Futuro Brota da Terra</title>

<style>
:root{
    --lime:#BFFF00;
    --green:#32CD32;
    --black:#050505;
    --white:#ffffff;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:var(--black);
    color:var(--white);
    overflow-x:hidden;
}

/* Fundo animado */
body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
    radial-gradient(circle at 20% 20%, rgba(191,255,0,.15), transparent 25%),
    radial-gradient(circle at 80% 30%, rgba(50,205,50,.15), transparent 25%),
    radial-gradient(circle at 50% 80%, rgba(191,255,0,.08), transparent 30%);
    animation:bgMove 10s infinite alternate;
    z-index:-1;
}

@keyframes bgMove{
    from{transform:scale(1);}
    to{transform:scale(1.2);}
}

/* Header */
.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    flex-direction:column;
    padding:20px;
}

.logo{
    font-size:5rem;
    font-weight:900;
    color:var(--lime);
    text-shadow:
    0 0 10px var(--lime),
    0 0 30px var(--lime),
    0 0 60px var(--green);
    animation:pulse 2s infinite;
}

@keyframes pulse{
    50%{
        transform:scale(1.05);
    }
}

.slogan{
    font-size:1.5rem;
    max-width:800px;
    margin:25px auto;
    color:white;
}

.highlight{
    color:var(--lime);
}

.btn{
    padding:15px 35px;
    border:none;
    background:var(--lime);
    color:black;
    font-size:1rem;
    font-weight:bold;
    border-radius:50px;
    cursor:pointer;
    transition:.4s;
    box-shadow:0 0 20px var(--lime);
}

.btn:hover{
    transform:translateY(-5px) scale(1.05);
    box-shadow:0 0 40px var(--lime);
}

/* Menu */
nav{
    position:fixed;
    width:100%;
    top:0;
    backdrop-filter:blur(10px);
    background:rgba(0,0,0,.6);
    z-index:1000;
}

nav ul{
    display:flex;
    justify-content:center;
    gap:40px;
    list-style:none;
    padding:20px;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:600;
    transition:.3s;
}

nav a:hover{
    color:var(--lime);
}

/* Seções */
section{
    padding:100px 10%;
}

.section-title{
    text-align:center;
    font-size:3rem;
    margin-bottom:50px;
    color:var(--lime);
    text-shadow:0 0 15px var(--lime);
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:30px;
}

.card{
    background:#111;
    border:1px solid rgba(191,255,0,.2);
    border-radius:20px;
    padding:30px;
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 0 25px rgba(191,255,0,.5);
}

.card h3{
    color:var(--lime);
    margin-bottom:15px;
}

/* Estatísticas */
.stats{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:40px;
    margin-top:50px;
}

.stat{
    text-align:center;
}

.number{
    font-size:4rem;
    font-weight:900;
    color:var(--lime);
}

.label{
    color:white;
}

/* CTA */
.cta{
    text-align:center;
    background:linear-gradient(135deg,#0d0d0d,#1a1a1a);
    border-top:1px solid rgba(191,255,0,.2);
}

.cta p{
    max-width:800px;
    margin:20px auto;
    font-size:1.2rem;
}

/* Footer */
footer{
    text-align:center;
    padding:30px;
    background:#000;
    border-top:1px solid rgba(191,255,0,.2);
}

footer span{
    color:var(--lime);
}

/* Responsivo */
@media(max-width:768px){
    .logo{
        font-size:3rem;
    }

    .slogan{
        font-size:1.1rem;
    }

    nav ul{
        gap:15px;
        font-size:.9rem;
    }
}
</style>
</head>
<body>

<nav>
    <ul>
        <li><a href="#sobre">Sobre</a></li>
        <li><a href="#tecnologia">Tecnologia</a></li>
        <li><a href="#impacto">Impacto</a></li>
        <li><a href="#futuro">Futuro</a></li>
    </ul>
</nav>

<header class="hero">
    <h1 class="logo">AGRO NEXUS 2050</h1>

    <p class="slogan">
        <span class="highlight">Produzir mais.</span>
        Preservar melhor.
        Conectar tecnologia, sustentabilidade e inovação para alimentar o futuro do planeta.
    </p>

    <button class="btn" onclick="mostrarMensagem()">
        Descubra o Futuro
    </button>

    <p id="mensagem" style="margin-top:25px;color:#BFFF00;font-weight:bold;"></p>
</header>

<section id="sobre">
    <h2 class="section-title">Agro Forte e Sustentável</h2>

    <div class="cards">
        <div class="card">
            <h3>🌱 Produção Inteligente</h3>
            <p>
                Agricultura moderna baseada em dados, eficiência e redução de desperdícios.
            </p>
        </div>

        <div class="card">
            <h3>🚜 Tecnologia Avançada</h3>
            <p>
                Máquinas conectadas, sensores, drones e automação impulsionando resultados.
            </p>
        </div>

        <div class="card">
            <h3>🌎 Sustentabilidade Real</h3>
            <p>
                Crescimento econômico aliado à preservação dos recursos naturais.
            </p>
        </div>
    </div>
</section>

<section id="tecnologia">
    <h2 class="section-title">O Campo Conectado</h2>

    <div class="cards">
        <div class="card">
            <h3>🤖 Inteligência Artificial</h3>
            <p>
                Previsão climática, monitoramento de safras e decisões estratégicas em tempo real.
            </p>
        </div>

        <div class="card">
            <h3>📡 Agricultura Digital</h3>
            <p>
                Sensores inteligentes aumentam produtividade e reduzem impactos ambientais.
            </p>
        </div>

        <div class="card">
            <h3>🔋 Energia Limpa</h3>
            <p>
                Soluções renováveis para tornar o agro ainda mais eficiente e sustentável.
            </p>
        </div>
    </div>
</section>

<section id="impacto">
    <h2 class="section-title">Impacto Positivo</h2>

    <div class="stats">
        <div class="stat">
            <div class="number" id="n1">0</div>
            <div class="label">Eficiência</div>
        </div>

        <div class="stat">
            <div class="number" id="n2">0</div>
            <div class="label">Inovação</div>
        </div>

        <div class="stat">
            <div class="number" id="n3">0</div>
            <div class="label">Sustentabilidade</div>
        </div>
    </div>
</section>

<section id="futuro" class="cta">
    <h2 class="section-title">O Futuro Está Plantado Hoje</h2>

    <p>
        O agronegócio do futuro não é apenas produtivo. É inteligente,
        conectado, sustentável e preparado para alimentar uma população global
        crescente sem comprometer o planeta.
    </p>

    <button class="btn" onclick="window.scrollTo({top:0,behavior:'smooth'})">
        Voltar ao Topo
    </button>
</section>

<footer>
    © 2026 <span>AGRO NEXUS 2050</span> — Cultivando a próxima geração do planeta.
</footer>

<script>
function mostrarMensagem(){
    document.getElementById("mensagem").innerHTML =
    "🚀 O futuro do agro já começou: mais tecnologia, mais produtividade e mais sustentabilidade.";
}

function animarNumero(id, alvo){
    let atual = 0;
    const elemento = document.getElementById(id);

    const intervalo = setInterval(()=>{
        atual++;
        elemento.textContent = atual + "%";

        if(atual >= alvo){
            clearInterval(intervalo);
        }
    },20);
}

const observer = new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
        if(entry.isIntersecting){
            animarNumero("n1",95);
            animarNumero("n2",98);
            animarNumero("n3",100);
            observer.disconnect();
        }
    });
});

observer.observe(document.querySelector("#impacto"));
</script>

</body>
</html>
