Aniverdario # BEN20
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aniversário de Max | Ben 10 Clássico</title>
<style>
body{
margin:0;
background:#000;
color:#fff;
font-family:Trebuchet MS, Arial, sans-serif;
text-align:center;
overflow-x:hidden;
background-image:
radial-gradient(circle at 20% 20%, rgba(57,255,20,.2), transparent 20%),
radial-gradient(circle at 80% 40%, rgba(57,255,20,.15), transparent 20%);
}
.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
padding:20px;
}
.logo{
font-size:4rem;
font-weight:bold;
color:#8cff00;
text-shadow:0 0 10px #39ff14,0 0 25px #39ff14;
}
.omnitrix{
width:280px;height:280px;border-radius:50%;
background:radial-gradient(circle,#a8ff60 0%,#39ff14 35%,#111 70%);
box-shadow:0 0 20px #39ff14,0 0 60px #39ff14,0 0 120px #39ff14;
animation:pulse 2s infinite;
cursor:pointer;
margin:25px 0;
}
@keyframes pulse{
0%,100%{transform:scale(1)}
50%{transform:scale(1.1)}
}
section{padding:70px 20px}
.title{
font-size:3rem;
color:#8cff00;
text-shadow:0 0 10px #39ff14;
}
.panel{
max-width:1000px;
margin:auto;
background:#101010;
border:4px solid #39ff14;
border-radius:20px;
padding:25px;
box-shadow:0 0 20px rgba(57,255,20,.5);
}
.aliens{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
margin-top:25px;
}
.card{
width:220px;
background:#1a1a1a;
border:3px solid #39ff14;
border-radius:20px;
padding:20px;
transition:.3s;
}
.card:hover{
transform:scale(1.08) rotate(-2deg);
}
.card h3{color:#8cff00}
.btn{
display:inline-block;
padding:18px 30px;
background:#39ff14;
color:#000;
font-weight:bold;
text-decoration:none;
border-radius:30px;
margin:10px;
}
#countdown{
font-size:2rem;
color:#8cff00;
font-weight:bold;
}
.blink{
animation:blink 1s infinite;
}
@keyframes blink{
50%{opacity:.4}
}
</style>
</head>
<body>

<div class="hero">
<div class="logo">BEN 10</div>
<h1>O ANIVERSÁRIO DE MAX</h1>
<p class="blink">⚠️ O OMNITRIX DETECTOU UMA MISSÃO ESPECIAL ⚠️</p>

<div class="omnitrix" onclick="document.getElementById('missao').scrollIntoView({behavior:'smooth'})"></div>

<h2>CLIQUE NO OMNITRIX PARA INICIAR A TRANSFORMAÇÃO</h2>
</div>

<section id="missao">
<div class="panel">
<div class="title">TRANSFORMAÇÃO CONCLUÍDA!</div>
<h2>VOCÊ FOI ESCOLHIDO PARA PARTICIPAR DO ANIVERSÁRIO DE MAX</h2>
<p>DNA ALIEN CARREGADO COM SUCESSO!</p>
</div>
</section>

<section>
<div class="panel">
<div class="title">MISSÃO 020</div>
<h2>📅 08/08/2026</h2>
<h2>🕢 19:30</h2>
<h2>📍 Rua José Elias Giuliari, 316<br>Boa Vista - Joinville/SC</h2>
</div>
</section>

<section>
<div class="panel">
<div class="title">ESCOLHA SEU ALIEN</div>

<div class="aliens">
<div class="card"><h3>🔥 CHAMA</h3><p>Chega incendiando a festa.</p></div>
<div class="card"><h3>⚡ XLR8</h3><p>Primeiro a chegar.</p></div>
<div class="card"><h3>💪 QUATRO BRAÇOS</h3><p>Força máxima.</p></div>
<div class="card"><h3>🧠 MASSA CINZENTA</h3><p>Gênio da equipe.</p></div>
<div class="card"><h3>👻 FANTASMÁTICO</h3><p>Mestre das surpresas.</p></div>
<div class="card"><h3>💎 DIAMANTE</h3><p>Brilha em qualquer missão.</p></div>
</div>

</div>
</section>

<section>
<div class="panel">
<div class="title">CONTAGEM REGRESSIVA</div>
<div id="countdown"></div>
</div>
</section>

<section>
<div class="panel">
<div class="title">VOCÊ ACEITA ESTA MISSÃO?</div>

<a class="btn" href="https://wa.me/5547997274703?text=Eu%20aceito%20a%20miss%C3%A3o!">🟢 SIM!</a>

<a class="btn" href="https://wa.me/5547997274703?text=Talvez!">🟡 TALVEZ!</a>

<a class="btn" href="https://wa.me/5547997274703?text=O%20Vilgax%20me%20capturou!">🔴 O VILGAX ME PEGOU!</a>

</div>
</section>

<section>
<div class="panel">
<div class="title blink">HERÓI REGISTRADO</div>
<h2>MISSÃO ACEITA</h2>
<h3>NOS VEMOS NO ANIVERSÁRIO DE MAX!</h3>
</div>
</section>

<script>
const target = new Date("2026-08-08T19:30:00");

function updateCountdown(){
const diff = target - new Date();
const d = Math.floor(diff/(1000*60*60*24));
const h = Math.floor((diff%(1000*60*60*24))/(1000*60*60));
const m = Math.floor((diff%(1000*60*60))/(1000*60));
document.getElementById("countdown").innerHTML =
d+" DIAS • "+h+" HORAS • "+m+" MINUTOS";
}
setInterval(updateCountdown,1000);
updateCountdown();
</script>

</body>
</html>
