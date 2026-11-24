<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Main Yuk! Demo Gratis</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&display=swap">
<style>
:root{
  --bg:#CDEEF3; --ink:#26214A; --back:#6C4DF6; --back-ink:#B9AAFF; --front:#FFFFFF;
  --match:#B8F0C8; --bad:#FFB3B3; --btn:#FF8A3D; --chip:#FFFFFF; color-scheme:light;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){--bg:#1B1740;--ink:#F3F0FF;--back:#8C74FF;--back-ink:#D6CCFF;--front:#2B2660;--match:#2F7A52;--bad:#8A3A4A;--chip:#2B2660;color-scheme:dark}
}
:root[data-theme="dark"]{--bg:#1B1740;--ink:#F3F0FF;--back:#8C74FF;--back-ink:#D6CCFF;--front:#2B2660;--match:#2F7A52;--bad:#8A3A4A;--chip:#2B2660;color-scheme:dark}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;min-height:100vh;background:var(--bg);color:var(--ink);display:flex;justify-content:center;
  font-family:"Fredoka","Nunito",ui-rounded,"Comic Sans MS",system-ui,sans-serif}
main{width:100%;max-width:460px;padding:18px 16px 28px;text-align:center}
h1{font-size:clamp(32px,10vw,46px);margin:6px 0 4px}
h2{font-size:24px;margin:0;flex:1}
.sub{margin:0 0 18px;font-size:18px}
button{font:inherit;color:var(--ink);cursor:pointer;-webkit-tap-highlight-color:transparent}
button:focus-visible{outline:4px solid var(--btn);outline-offset:3px}
.menu{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.tile-m{border:4px solid var(--ink);border-radius:26px;padding:18px 8px;color:#26214A;font-weight:700;font-size:19px;min-height:150px;
  display:flex;flex-direction:column;align-items:center;justify-content:center;gap:8px}
.tile-m span{font-size:56px;line-height:1}
.top{display:flex;align-items:center;gap:10px;margin-bottom:12px}
.back{border:3px solid var(--ink);background:var(--chip);border-radius:999px;padding:8px 14px;font-weight:600;font-size:16px;min-height:44px}
.stats{display:flex;justify-content:center;flex-wrap:wrap;gap:8px;margin-bottom:14px;font-size:17px;font-weight:600;min-height:36px}
.stats span{background:var(--chip);padding:5px 14px;border-radius:999px}
.board{display:grid;gap:10px}.c4{grid-template-columns:repeat(4,1fr)}.c3{grid-template-columns:repeat(3,1fr);gap:8px}
.card{position:relative;aspect-ratio:1;border:0;padding:0;background:none;perspective:600px}
.inner{position:absolute;inset:0;transition:transform .4s;transform-style:preserve-3d}
.card.open .inner{transform:rotateY(180deg)}
.face{position:absolute;inset:0;border-radius:18px;display:flex;align-items:center;justify-content:center;
  backface-visibility:hidden;-webkit-backface-visibility:hidden;border:3px solid var(--ink)}
.back-f{background:var(--back);color:var(--back-ink);font-size:clamp(26px,8vw,38px)}
.front{background:var(--front);transform:rotateY(180deg);font-size:clamp(34px,12vw,56px)}
.card.done .front{background:var(--match)}
.tile{aspect-ratio:1;border:4px solid var(--ink);border-radius:20px;font-weight:700;font-size:clamp(36px,13vw,56px);color:#26214A}
.tile.blank{visibility:hidden}
.prompt{background:var(--chip);border:3px solid var(--ink);border-radius:24px;padding:18px 12px;margin-bottom:16px}
.emo{font-size:clamp(40px,12vw,56px);line-height:1.25;word-break:break-all}
.word{font-size:clamp(36px,11vw,50px);font-weight:700;letter-spacing:.12em}
.prompt p{margin:6px 0 0;font-size:19px;font-weight:600}
.opts{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.opt{border:4px solid var(--ink);border-radius:22px;background:var(--front);font-weight:700;font-size:clamp(32px,10vw,44px);min-height:84px}
.opt.good{background:var(--match)}.opt.bad{background:var(--bad)}
.big-btn{font-weight:700;font-size:20px;margin-top:16px;padding:12px 28px;border-radius:999px;border:3px solid var(--ink);background:var(--btn);color:#26214A;min-height:48px}
#win,#lock{position:fixed;inset:0;background:rgba(20,15,50,.6);display:flex;align-items:center;justify-content:center;padding:20px}
#win[hidden],#lock[hidden]{display:none}
.box{background:var(--bg);border:4px solid var(--ink);border-radius:28px;padding:24px 26px;max-width:340px}
.box .e{font-size:60px;line-height:1}.box h2{margin:8px 0 4px;font-size:32px}.box p{margin:0;font-size:19px}
.box button{margin:14px 4px 0}
.tile-m{position:relative}.lk{position:absolute;top:10px;right:12px;font-size:26px;font-style:normal}
a.big-btn{display:inline-block;text-decoration:none}.note{font-size:16px;margin:14px 0 0;font-weight:600}
@media (prefers-reduced-motion:reduce){.inner{transition:none}}
</style>
</head>
<body>
<main id="view"></main>
<div id="win" hidden role="dialog" aria-live="polite">
  <div class="box"><div class="e">🎉</div><h2>Hebat!</h2><p id="winText"></p><p class="note">Suka? Masih ada 2 game lagi di paket lengkap.</p>
    <button class="big-btn" id="again">Main lagi</button><button class="big-btn" id="menuBtn" style="background:var(--chip)">Menu</button><a class="big-btn" data-buy target="_blank" rel="noopener">Beli paket lengkap</a></div>
</div>
<div id="lock" hidden role="dialog"><div class="box"><div class="e">🔒</div><h2 id="lockT"></h2><p>Game ini ada di paket lengkap bersama 2 game lainnya.</p><a class="big-btn" data-buy target="_blank" rel="noopener">Beli paket lengkap</a><button class="big-btn" id="lockX" style="background:var(--chip)">Nanti dulu</button></div></div>
<script>
const BUY_URL="https://lynk.id/GANTI-DENGAN-LINK-KAMU"; // ganti dengan link produk di lynk.id
const $=s=>document.querySelector(s), view=$("#view"), win=$("#win");
const rand=n=>Math.floor(Math.random()*n), pick=a=>a[rand(a.length)];
const shuffle=a=>{for(let i=a.length-1;i>0;i--){const j=rand(i+1);[a[i],a[j]]=[a[j],a[i]]}return a};
const ANIMALS=["🐶","🐱","🐰","🐼","🦁","🐸","🐵","🐘"];

function screen(title,cls){
  view.innerHTML='<div class="top"><button class="back" id="back">← Menu</button><h2>'+title+'</h2></div><div class="stats" id="stats"></div><div id="body" class="'+(cls||"")+'"></div>';
  $("#back").onclick=menu; return $("#body");
}
const stat=(...a)=>{$("#stats").innerHTML=a.map(x=>"<span>"+x+"</span>").join("")};
function won(text,again){
  $("#winText").textContent=text; win.hidden=false;
  $("#again").onclick=()=>{win.hidden=true;again()}; $("#menuBtn").onclick=()=>{win.hidden=true;menu()};
}

const GAMES=[
  {t:"Cocokkan Hewan",e:"🐼",c:"#FFB347",f:memory},
  {t:"Susun Angka",e:"🔢",c:"#7ED9A0",f:slide},
  {t:"Hitung Hewan",e:"🐥",c:"#7FC8FF",lock:1},
  {t:"Tebak Huruf",e:"🔤",c:"#FF9EC4",lock:1}
];
function menu(){
  win.hidden=true;$("#lock").hidden=true;
  view.innerHTML='<h1>Main Yuk!</h1><p class="sub">Pilih game kesukaanmu</p><div class="menu"></div><p class="note">Versi demo gratis: 2 dari 4 game</p><a class="big-btn" data-buy target="_blank" rel="noopener">Beli paket lengkap</a>';
  GAMES.forEach(g=>{const b=document.createElement("button");b.className="tile-m";b.style.background=g.c;
    b.innerHTML="<span>"+g.e+"</span>"+g.t+(g.lock?'<i class="lk">🔒</i>':"");
    b.onclick=g.lock?()=>{$("#lockT").textContent=g.t;$("#lock").hidden=false}:g.f;view.querySelector(".menu").appendChild(b)});
  document.querySelectorAll("a[data-buy]").forEach(a=>{a.href=BUY_URL});
}

/* Game 1: memory */
function memory(){
  const b=screen("Cocokkan Hewan","board c4"); const P=6; let first=null,lock=false,moves=0,found=0;
  stat("Langkah: 0","Pasangan: 0/"+P);
  shuffle(shuffle(ANIMALS.slice()).slice(0,P).flatMap(a=>[a,a])).forEach(a=>{
    const c=document.createElement("button"); c.className="card"; c.dataset.a=a; c.setAttribute("aria-label","Kartu tertutup");
    c.innerHTML='<div class="inner"><div class="face back-f">🐾</div><div class="face front">'+a+'</div></div>';
    c.onclick=()=>{
      if(lock||c===first||c.classList.contains("open"))return;
      c.classList.add("open"); c.setAttribute("aria-label","Kartu "+a);
      if(!first){first=c;return}
      moves++;
      if(first.dataset.a===a){first.classList.add("done");c.classList.add("done");first=null;found++;
        if(found===P)setTimeout(()=>won("Kamu selesai dalam "+moves+" langkah.",memory),700)}
      else{lock=true;const f=first;first=null;setTimeout(()=>{f.classList.remove("open");c.classList.remove("open");lock=false},900)}
      stat("Langkah: "+moves,"Pasangan: "+found+"/"+P);
    };
    b.appendChild(c);
  });
}

/* Game 2: sliding number puzzle */
function slide(){
  const b=screen("Susun Angka","board c3");
  const nb=i=>{const r=Math.floor(i/3),c=i%3,o=[];if(r>0)o.push(i-3);if(r<2)o.push(i+3);if(c>0)o.push(i-1);if(c<2)o.push(i+1);return o};
  const solved=t=>t.every((v,k)=>v===(k<8?k+1:0));
  let t,m=0;
  do{t=[1,2,3,4,5,6,7,8,0];let z=8;for(let k=0;k<80;k++){const j=pick(nb(z));[t[z],t[j]]=[t[j],t[z]];z=j}}while(solved(t));
  stat("Langkah: 0","Urutkan 1 sampai 8");
  function draw(){
    b.innerHTML="";
    t.forEach((v,i)=>{const e=document.createElement("button");e.className="tile"+(v?"":" blank");
      if(v){e.textContent=v;e.style.background="hsl("+(v*42)+" 85% 72%)"}else e.disabled=true;
      e.onclick=()=>{const z=t.indexOf(0);if(!nb(z).includes(i))return;
        [t[z],t[i]]=[t[i],t[z]];m++;stat("Langkah: "+m,"Urutkan 1 sampai 8");draw();
        if(solved(t))setTimeout(()=>won("Angkanya sudah urut dalam "+m+" langkah.",slide),400)};
      b.appendChild(e)});
  }
  draw();
}

$("#lockX").onclick=()=>{$("#lock").hidden=true};
menu();
</script>
</body>
</html>
