<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flashcards — Parasitologia</title>
<style>
:root{
  --bg:#0a0e1a; --card:#ffffff; --ink:#18212b; --muted:#66717d;
  --accent:#315f8a; --accent2:#e8f0f7; --line:#dfe5eb; --ok:#287a4b; --warn:#b23b3b;
  --neon:#00e5ff; --neon2:#a855f7; --neon3:#22d3ee;
}
*{box-sizing:border-box}
body{margin:0;font-family:Arial,Helvetica,sans-serif;background:var(--bg);color:#e8f0f7;line-height:1.55}
header{background:linear-gradient(135deg,#0a0e1a,#0f1d3d,#0a0e1a);color:white;padding:26px 20px;border-bottom:1px solid rgba(0,229,255,.15)}
header .wrap{max-width:900px;margin:auto}
h1{margin:0 0 6px;font-size:26px;background:linear-gradient(90deg,var(--neon),var(--neon2),var(--neon3));
  -webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;font-weight:900;letter-spacing:.5px}
header p{margin:0;opacity:.75;font-size:14px}
.wrap{max-width:900px;margin:auto;padding:24px 20px}
.screen{display:none}
.screen.active{display:block}

/* ============ INTRO FUTURISTA ============ */
.intro{
  position:relative;
  background:linear-gradient(160deg,#0a0e1a 0%,#0d1430 45%,#0a0e1a 100%);
  border:1px solid rgba(0,229,255,.25);
  border-radius:24px;
  padding:44px 30px 38px;
  text-align:center;
  overflow:hidden;
  box-shadow:
    0 0 0 1px rgba(0,229,255,.08) inset,
    0 0 40px rgba(0,229,255,.18),
    0 20px 60px rgba(0,0,0,.5);
}
.intro::before{
  content:"";
  position:absolute;inset:-50%;
  background:
    linear-gradient(rgba(0,229,255,.06) 1px, transparent 1px) 0 0/40px 40px,
    linear-gradient(90deg, rgba(0,229,255,.06) 1px, transparent 1px) 0 0/40px 40px;
  transform:perspective(600px) rotateX(60deg) translateY(30%);
  pointer-events:none;
  opacity:.7;
  mask-image:linear-gradient(to bottom, transparent 40%, #000 100%);
  -webkit-mask-image:linear-gradient(to bottom, transparent 40%, #000 100%);
}
.intro::after{
  content:"";
  position:absolute;top:-40%;left:-20%;right:-20%;height:300px;
  background:radial-gradient(closest-side, rgba(168,85,247,.35), transparent 70%);
  filter:blur(40px);pointer-events:none;
}
.intro > *{position:relative;z-index:2}

.intro-svg{
  width:140px;height:140px;display:block;margin:0 auto 14px;
  filter:drop-shadow(0 0 12px rgba(0,229,255,.55)) drop-shadow(0 0 26px rgba(168,85,247,.35));
  animation:floatY 3.5s ease-in-out infinite;
}
@keyframes floatY{0%,100%{transform:translateY(0)}50%{transform:translateY(-6px)}}

.intro h2{
  margin:0 0 14px;font-size:26px;letter-spacing:1px;font-weight:900;
  background:linear-gradient(90deg,var(--neon),var(--neon3),var(--neon2));
  -webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;
  text-shadow:0 0 22px rgba(0,229,255,.25);
}
.intro .tag{
  display:inline-block;font-size:11px;letter-spacing:3px;font-weight:800;
  color:var(--neon);border:1px solid rgba(0,229,255,.4);border-radius:999px;
  padding:5px 14px;margin-bottom:18px;text-transform:uppercase;
  background:rgba(0,229,255,.06);
  box-shadow:0 0 18px rgba(0,229,255,.2) inset;
}
.intro .autor{
  font-size:16px;color:#cbd5e1;margin:0 auto 8px;max-width:620px;line-height:1.7;
}
.intro .autor b{
  color:var(--neon);
  text-shadow:0 0 10px rgba(0,229,255,.6);
}
.intro .wish{
  font-size:15px;color:#94a3b8;margin:18px auto 26px;max-width:620px;line-height:1.75;
  border-left:3px solid var(--neon2);
  border-right:3px solid var(--neon);
  padding:14px 20px;
  background:linear-gradient(90deg, rgba(168,85,247,.08), rgba(0,229,255,.08));
  border-radius:12px;
  font-style:italic;
}
.intro .wish b{color:var(--neon3);font-style:normal}

.big-btn{
  position:relative;
  border:0;border-radius:14px;
  padding:15px 34px;
  background:linear-gradient(135deg,#00e5ff,#a855f7);
  color:#0a0e1a;font-weight:900;font-size:15px;letter-spacing:1.5px;text-transform:uppercase;
  cursor:pointer;
  box-shadow:0 0 24px rgba(0,229,255,.5), 0 0 50px rgba(168,85,247,.3);
  transition:transform .2s, box-shadow .2s;
  overflow:hidden;
}
.big-btn:hover{
  transform:translateY(-2px) scale(1.02);
  box-shadow:0 0 34px rgba(0,229,255,.8), 0 0 70px rgba(168,85,247,.5);
}
.big-btn:active{transform:translateY(0) scale(.99)}

/* ============ CARD ============ */
.topbar{display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;font-size:13px;color:#94a3b8;font-weight:700}
.progress{background:#1e293b;border-radius:999px;height:8px;flex:1;margin:0 14px;overflow:hidden}
.progress > div{height:100%;background:linear-gradient(90deg,var(--neon),var(--neon2));width:0;transition:width .3s}

.flash{background:#0d1430;border:1px solid rgba(0,229,255,.2);border-radius:18px;overflow:hidden;box-shadow:0 0 30px rgba(0,229,255,.15),0 10px 40px rgba(0,0,0,.5)}
.photo{height:340px;background:#0a0e1a;display:flex;align-items:center;justify-content:center;position:relative}
.photo img{width:100%;height:100%;object-fit:contain;background:#f5f7fa}
.timer{
  position:absolute;top:12px;right:12px;background:rgba(10,14,26,.9);color:var(--neon);
  border:1px solid rgba(0,229,255,.4);
  border-radius:999px;padding:8px 14px;font-weight:800;font-size:14px;min-width:64px;text-align:center;transition:background .3s,color .3s,border-color .3s;
  box-shadow:0 0 14px rgba(0,229,255,.35);
}
.timer.low{background:rgba(178,59,59,.95);color:#fff;border-color:#ff5c5c;animation:pulse .6s infinite;box-shadow:0 0 18px rgba(255,92,92,.6)}
@keyframes pulse{0%{transform:scale(1)}50%{transform:scale(1.15)}100%{transform:scale(1)}}
.timer.done{background:var(--ok);color:#fff;border-color:#3ddc84;box-shadow:0 0 18px rgba(61,220,132,.6)}

.prompt{padding:16px 20px;background:rgba(0,229,255,.05);border-top:1px solid rgba(0,229,255,.15);font-weight:700;color:var(--neon3);font-size:14px;text-align:center}
.answer{padding:0 22px;max-height:0;overflow:hidden;transition:max-height .5s ease, padding .3s ease}
.answer.show{max-height:800px;padding:20px 22px}
.answer h2{margin:0 0 14px;font-size:22px;color:var(--neon);text-shadow:0 0 12px rgba(0,229,255,.4)}
.row{padding:9px 0;border-top:1px solid rgba(0,229,255,.12);font-size:15px;color:#cbd5e1}
.row:first-of-type{border-top:0}
.label{font-weight:800;color:var(--neon3)}
.badge{display:inline-block;background:rgba(168,85,247,.18);color:#d8b4fe;border:1px solid rgba(168,85,247,.4);border-radius:999px;padding:3px 10px;font-size:13px;font-weight:700}

.actions{padding:16px 20px 22px;display:flex;gap:10px;justify-content:center;flex-wrap:wrap;border-top:1px solid rgba(0,229,255,.15)}
.btn{border:0;border-radius:10px;padding:11px 22px;font-weight:800;cursor:pointer;font-size:14px;transition:opacity .2s, transform .15s}
.btn:not(:disabled):hover{transform:translateY(-1px)}
.btn-primary{background:linear-gradient(135deg,#00e5ff,#a855f7);color:#0a0e1a;box-shadow:0 0 16px rgba(0,229,255,.45)}
.btn-ghost{background:transparent;color:var(--neon);border:1px solid rgba(0,229,255,.4)}
.btn-ghost:not(:disabled):hover{background:rgba(0,229,255,.08)}
.btn:disabled{opacity:.3;cursor:not-allowed}

/* ============ FIM ============ */
.end{
  background:linear-gradient(160deg,#0a0e1a,#0d1430,#0a0e1a);
  border:1px solid rgba(0,229,255,.25);
  border-radius:24px;padding:40px 30px;text-align:center;
  box-shadow:0 0 40px rgba(0,229,255,.2),0 20px 60px rgba(0,0,0,.5);
  position:relative;overflow:hidden;
}
.end::before{
  content:"";position:absolute;top:-50%;left:-20%;right:-20%;height:300px;
  background:radial-gradient(closest-side, rgba(0,229,255,.35), transparent 70%);
  filter:blur(40px);pointer-events:none;
}
.end > *{position:relative;z-index:2}
.end h2{margin-top:0;font-size:28px;
  background:linear-gradient(90deg,var(--neon),var(--neon2));
  -webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;
  text-shadow:0 0 20px rgba(0,229,255,.3);
}
.end .fontes{
  margin-top:24px;background:rgba(0,229,255,.05);border-left:4px solid var(--neon);border-radius:8px;
  padding:14px 16px;font-size:13px;color:#94a3b8;text-align:left;
}
.end .fontes b{color:var(--neon3)}
footer{color:#64748b;font-size:12px;padding:24px 20px;text-align:center}

@media(max-width:600px){
  h1{font-size:22px}
  .photo{height:250px}
  .intro-svg{width:110px;height:110px}
  .intro h2{font-size:21px}
  .intro .autor{font-size:14px}
  .intro .wish{font-size:13px}
}
</style>
</head>
<body>

<header>
  <div class="wrap">
    <h1>Flashcards — Parasitologia</h1>
    <p>Fiz para você revisar no caminho para a faculdade.</p>
  </div>
</header>

<main class="wrap">

  <!-- INTRO FUTURISTA -->
  <section id="screen-start" class="screen active">
    <div class="intro">
      <svg class="intro-svg" viewBox="0 0 160 160" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
        <defs>
          <linearGradient id="gradCap" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0%" stop-color="#00e5ff"/>
            <stop offset="100%" stop-color="#a855f7"/>
          </linearGradient>
          <linearGradient id="gradBook" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0%" stop-color="#22d3ee"/>
            <stop offset="100%" stop-color="#a855f7"/>
          </linearGradient>
        </defs>
        <polygon points="80,22 145,52 80,82 15,52" fill="url(#gradCap)" stroke="#00e5ff" stroke-width="2.5" stroke-linejoin="round"/>
        <path d="M50 62 L50 88 Q50 98 80 98 Q110 98 110 88 L110 62" fill="url(#gradCap)" stroke="#00e5ff" stroke-width="2.5" opacity=".9"/>
        <line x1="145" y1="52" x2="145" y2="80" stroke="#00e5ff" stroke-width="2.5" stroke-linecap="round"/>
        <circle cx="145" cy="86" r="4.5" fill="#a855f7"/>
        <path d="M22 108 L80 120 L138 108 L138 132 L80 144 L22 132 Z" fill="url(#gradBook)" stroke="#00e5ff" stroke-width="2.5" stroke-linejoin="round"/>
        <line x1="80" y1="120" x2="80" y2="144" stroke="#00e5ff" stroke-width="2.5"/>
        <circle cx="62" cy="105" r="3" fill="#0a0e1a"/>
        <circle cx="98" cy="105" r="3" fill="#0a0e1a"/>
      </svg>

      <div class="tag">▸ Revisão de Parasitologia ◂</div>
      <h2>PREPARAÇÃO INTENSIVA</h2>

      <p class="autor">
        Material criado por Aluno <b>Wesley Coutinho</b> para revisar na ida até a faculdade —
        identificação rápida de parasitos por imagem, forma evolutiva e morfologia.
      </p>

      <div class="wish">
        <b>Desejo uma boa prova a todos!</b><br>
        Estudem com calma, confiem no que aprenderam e vão com tudo.
        Este material foi feito com muita dedicação — aproveitem cada card. 🚀
      </div>

      <button class="big-btn" id="btn-start">Iniciar Missão</button>
    </div>
  </section>

  <!-- CARD -->
  <section id="screen-card" class="screen">
    <div class="topbar">
      <span id="counter">1 / 7</span>
      <div class="progress"><div id="bar"></div></div>
      <span id="status">Pense!</span>
    </div>

    <article class="flash">
      <div class="photo">
        <img id="img" src="" alt="Parasito">
        <div class="timer" id="timer">15</div>
      </div>
      <div class="prompt">Qual é o parasito, a forma evolutiva e as características morfológicas?</div>
      <div class="answer" id="answer">
        <h2 id="ans-name">—</h2>
        <div class="row"><span class="label">Gênero/Espécie:</span> <span id="ans-gen">—</span></div>
        <div class="row"><span class="label">Forma evolutiva:</span> <span class="badge" id="ans-form">—</span></div>
        <div class="row"><span class="label">Características morfológicas:</span> <span id="ans-morph">—</span></div>
      </div>
      <div class="actions">
        <button class="btn btn-ghost" id="btn-reveal" disabled>Revelar</button>
        <button class="btn btn-primary" id="btn-next" disabled>Próximo →</button>
      </div>
    </article>
  </section>

  <!-- FIM -->
  <section id="screen-end" class="screen">
    <div class="end">
      <h2>MISSÃO CUMPRIDA! 🎉</h2>
      <p style="color:#cbd5e1;font-size:16px">Você revisou todos os flashcards deste bloco.<br>
      Bons estudos <b style="color:#00e5ff">e</b> boa prova — você consegue. 💪</p>
      <div class="fontes">
        <b>Sobre as imagens:</b> todas as fontes foram retiradas da internet (sites educacionais, CDC DPDx, bancos de imagens e materiais de aula), usadas aqui apenas para fins de estudo e revisão acadêmica.
      </div>
      <div style="margin-top:24px">
        <button class="big-btn" id="btn-restart">Recomeçar</button>
      </div>
    </div>
  </section>

</main>

<footer>Material de revisão acadêmica · Fontes das imagens: internet · Feito com dedicação por Aluno Wesley Coutinho.</footer>

<script>
/* ============================================================
   SONS HOSPEDADOS (URLs diretas)
   ============================================================ */
const somMensagem = new Audio("https://www.myinstants.com/media/sounds/nao-vou-revelar-online-audio-converter.mp3");
const somAlerta   = new Audio("https://www.myinstants.com/media/sounds/nudge.mp3");
const somEnvio    = new Audio("https://www.myinstants.com/media/sounds/msn-sound_1.mp3");
const somFinal    = new Audio("https://www.myinstants.com/media/sounds/eu-finjo-q-n-percebo_1uWXjKL.mp3");

[somMensagem, somAlerta, somEnvio, somFinal].forEach(a => {
  a.preload = 'auto';
  a.volume = 0.9;
});

function tocar(audio){
  try{
    audio.currentTime = 0;
    audio.play().catch(()=>{});
  }catch(e){}
}

/* ============================================================
   TICK DE CONTAGEM — gerado no navegador (sempre funciona)
   ============================================================ */
let audioCtx = null;
function getCtx(){
  if(!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
  if(audioCtx.state === 'suspended') audioCtx.resume();
  return audioCtx;
}

function tocarTick(){
  try{
    const ctx = getCtx();
    const t0  = ctx.currentTime;

    const osc  = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.type = 'square';
    osc.frequency.setValueAtTime(1800, t0);
    gain.gain.setValueAtTime(0.0001, t0);
    gain.gain.exponentialRampToValueAtTime(0.12, t0 + 0.002);
    gain.gain.exponentialRampToValueAtTime(0.0001, t0 + 0.06);
    osc.connect(gain).connect(ctx.destination);
    osc.start(t0);
    osc.stop(t0 + 0.07);

    const osc2  = ctx.createOscillator();
    const gain2 = ctx.createGain();
    osc2.type = 'sine';
    osc2.frequency.setValueAtTime(3200, t0);
    gain2.gain.setValueAtTime(0.0001, t0);
    gain2.gain.exponentialRampToValueAtTime(0.06, t0 + 0.001);
    gain2.gain.exponentialRampToValueAtTime(0.0001, t0 + 0.03);
    osc2.connect(gain2).connect(ctx.destination);
    osc2.start(t0);
    osc2.stop(t0 + 0.04);
  }catch(e){}
}

/* ============================================================
   DADOS DOS FLASHCARDS
   ============================================================ */
const cards = [
  { img:"https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjyh_RmxJYkX01LenvU4zyG0vSXd4MWiolRwxVXb5iqVEIqplMvc46YRGhvdprFZSQ8Zaf5IRArdnZ2f9iqRgyS8afnqPGbq2lcerLfx6ew3k00URvPdyzagqXVbRkuZ2Dm9SqCGb8gODMp/s1600/Tenia_solium_scolex.jpg",
    fallback:"https://www.cdc.gov/dpdx/images/taeniasis/Taenia_solium_scolex1.jpg",
    name:"Taenia solium", genero:"Taenia solium", forma:"Cisticerco",
    morph:"Vesícula translúcida; escólex invaginado; 4 ventosas; rostelo com acúleos." },
  { img:"https://cdn.lecturio.com/assets/Trophozoites-of-Giardia-lamblia.jpg",
    name:"Giardia lamblia", genero:"Giardia lamblia (G. duodenalis)", forma:"Trofozoíto",
    morph:"Formato piriforme; 2 núcleos; corpos medianos; 4 pares de flagelos." },
  { img:"https://www.researchgate.net/profile/Dennis-Mans/publication/316191566/figure/fig7/AS:492772266639360@1494460283301/Macrophage-infected-with-Leishmania-spp-clearly-showing-nuclei-and-kinetoplasts.png",
    name:"Leishmania sp.", genero:"Leishmania sp.", forma:"Amastigota",
    morph:"Formas arredondadas intracelulares em macrófago, com núcleo e cinetoplasto." },
  { img:"https://www.cdc.gov/dpdx/images/ascariasis/Ascaris_egg_fert_embryo.jpg",
    name:"Ascaris lumbricoides", genero:"Ascaris lumbricoides", forma:"Ovo",
    morph:"Ovo arredondado; casca espessa; camada mamilonada; conteúdo embrionário." },
  { img:"https://static.mundoeducacao.uol.com.br/mundoeducacao/2021/08/schistosoma-mansoni.jpg",
    name:"Schistosoma mansoni", genero:"Schistosoma mansoni", forma:"Vermes adultos",
    morph:"Macho mais robusto; fêmea mais fina e longa alojada no canal ginecóforo; ventosas oral e ventral." },
  { img:"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSEUb0H6odQikkbbh9XDwSmXEN2PjSZU98wF_Y6kaLNbMePKr6xOmmj9Vgk&s=10",
    name:"Entamoeba coli", genero:"Entamoeba coli", forma:"Cisto",
    morph:"Cisto arredondado; parede cística definida; mais de 4 núcleos — frequentemente até 8." },
  { img:"https://files.cercomp.ufg.br/weby/up/486/o/P_falciparum_2.jpg",
    name:"Plasmodium sp.", genero:"Plasmodium sp.", forma:"Trofozoíto",
    morph:"Parasito dentro da hemácia; formato de anel ('anel de sinete'); cromatina periférica." }
];

/* ============================================================
   ESTADO
   ============================================================ */
const TEMPO = 15;
let index = 0, timeLeft = TEMPO, timerId = null, revelado = false, ultimoTickSom = -1;

const screenStart = document.getElementById('screen-start');
const screenCard  = document.getElementById('screen-card');
const screenEnd   = document.getElementById('screen-end');
const imgEl     = document.getElementById('img');
const timerEl   = document.getElementById('timer');
const counterEl = document.getElementById('counter');
const barEl     = document.getElementById('bar');
const statusEl  = document.getElementById('status');
const answerEl  = document.getElementById('answer');
const ansName   = document.getElementById('ans-name');
const ansGen    = document.getElementById('ans-gen');
const ansForm   = document.getElementById('ans-form');
const ansMorph  = document.getElementById('ans-morph');
const btnReveal = document.getElementById('btn-reveal');
const btnNext   = document.getElementById('btn-next');

function showScreen(id){
  document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
}

function carregarCard(){
  const c = cards[index];
  revelado = false; ultimoTickSom = -1;
  imgEl.src = c.img;
  imgEl.onerror = () => { if(c.fallback) imgEl.src = c.fallback; };
  answerEl.classList.remove('show');
  timerEl.classList.remove('low','done');
  timerEl.textContent = TEMPO;
  statusEl.textContent = 'Pense!';
  btnReveal.disabled = true; btnNext.disabled = true;
  btnNext.textContent = (index === cards.length - 1) ? 'Finalizar' : 'Próximo →';
  counterEl.textContent = (index+1) + ' / ' + cards.length;
  barEl.style.width = ((index)/cards.length*100) + '%';
  timeLeft = TEMPO;
  clearInterval(timerId);
  timerId = setInterval(tick, 1000);
}

function tick(){
  timeLeft--;
  timerEl.textContent = timeLeft;

  if(timeLeft <= 10 && timeLeft > 0){
    if(!timerEl.classList.contains('low')) timerEl.classList.add('low');
    if(timeLeft !== ultimoTickSom){
      tocarTick();
      ultimoTickSom = timeLeft;
    }
  }

  if(timeLeft <= 0){
    clearInterval(timerId);
    timerEl.classList.remove('low');
    timerEl.classList.add('done');
    timerEl.textContent = '✓';
    statusEl.textContent = 'Escolha: Revelar ou Próximo';
    tocar(somAlerta);
    btnReveal.disabled = false;
    btnNext.disabled = false;
  }
}

function revelar(){
  if(revelado) return;
  revelado = true;
  clearInterval(timerId);
  const c = cards[index];
  ansName.textContent  = c.name;
  ansGen.textContent   = c.genero;
  ansForm.textContent  = c.forma;
  ansMorph.textContent = c.morph;
  timerEl.classList.remove('low'); timerEl.classList.add('done');
  timerEl.textContent = '✓';
  statusEl.textContent = 'Revelado';
  tocar(somMensagem);
  answerEl.classList.add('show');
  btnReveal.disabled = true; btnNext.disabled = false;
  btnNext.textContent = (index === cards.length - 1) ? 'Finalizar' : 'Próximo →';
  barEl.style.width = ((index+1)/cards.length*100) + '%';
}

function proximo(){
  clearInterval(timerId);
  tocar(somEnvio);
  index++;
  if(index >= cards.length){
    showScreen('screen-end');
    // 🔊 toca automaticamente ao finalizar todos os cards
    setTimeout(()=> tocar(somFinal), 400);
    return;
  }
  carregarCard();
}

document.getElementById('btn-start').addEventListener('click', ()=>{
  getCtx();
  // Pré-carrega o som final para não atrasar
  try{ somFinal.load(); }catch(e){}
  index = 0;
  showScreen('screen-card');
  carregarCard();
});

btnReveal.addEventListener('click', revelar);
btnNext.addEventListener('click', proximo);

document.getElementById('btn-restart').addEventListener('click', ()=>{
  try{ somFinal.pause(); somFinal.currentTime = 0; }catch(e){}
  index = 0;
  showScreen('screen-card');
  carregarCard();
});
</script>

</body>
</html>
