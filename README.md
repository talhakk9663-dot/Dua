
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Dua 💗</title>
<style>
*{box-sizing:border-box}
body{
 margin:0;min-height:100vh;padding:25px 14px;
 display:flex;align-items:center;justify-content:center;
 overflow-x:hidden;
 background:linear-gradient(145deg,#270d29,#8c356d,#ffc1df);
 color:#8e285a;font-family:Georgia,serif;text-align:center;
}
.card{
 position:relative;z-index:2;width:100%;max-width:450px;
 padding:30px 20px;border-radius:30px;
 background:#fff6f9ed;border:2px solid #fff;
 box-shadow:0 0 45px #ffb4db75;
 animation:appear 1.3s ease;
}
@keyframes appear{
 from{opacity:0;transform:translateY(35px) scale(.94)}
 to{opacity:1;transform:translateY(0) scale(1)}
}
.top{font-size:25px;letter-spacing:5px}
h1{font-size:clamp(38px,10vw,52px);line-height:1.2;margin:20px 0}
.name{color:#ed4d99;font-style:italic;text-shadow:0 0 15px #ffb0d7}
.subtitle{font-size:12px;letter-spacing:3px}
.teddy{
 display:inline-block;font-size:105px;margin:12px;
 transform-origin:bottom center;
 animation:dance 2s ease-in-out infinite;
 filter:drop-shadow(0 8px 7px #cf73a455);
}
@keyframes dance{
 0%,100%{transform:rotate(-9deg) translateY(0)}
 50%{transform:rotate(9deg) translateY(-13px)}
}
.cake{font-size:60px;animation:bounce 1.5s infinite}
@keyframes bounce{50%{transform:translateY(-9px)}}
p{font-size:16px;line-height:1.9}
.letter{
 background:#ffe8f2;border:1px dashed #e887b6;
 border-radius:20px;padding:18px;margin-top:20px;
}
button{
 border:0;border-radius:30px;padding:14px 19px;
 margin:8px 3px;background:linear-gradient(90deg,#ed579c,#ba69ce);
 color:white;font-size:15px;cursor:pointer;
 box-shadow:0 5px 15px #d35b9b40;
}
#letter{display:none;animation:appear .7s ease}
.float{
 position:fixed;bottom:-50px;z-index:1;pointer-events:none;
 animation:rise linear forwards;
}
@keyframes rise{
 0%{transform:translateY(0) rotate(0);opacity:0}
 15%{opacity:1}
 100%{transform:translateY(-115vh) rotate(360deg);opacity:0}
}
footer{font-size:12px;letter-spacing:2px;margin-top:25px}
</style>
</head>
<body>
<main class="card">
 <div class="top">🌸 💗 🧸 💗 🌸</div>
 <p class="subtitle">A LITTLE SURPRISE FOR SOMEONE SPECIAL</p>

 <h1>Happy Birthday<br><span class="name">Dua</span> 🎀</h1>

 <div class="teddy">🧸💝</div>

 <p>
  A cute teddy, a thousand hearts,<br>
  and the sweetest birthday wishes just for you! 💕<br>
  May your special day be full of smiles,<br>
  beautiful memories and magical moments. ✨
 </p>

 <div class="cake">🎂</div>
 <p>🌷 May all your wishes come true 🌷</p>

 <button onclick="openLetter()">💌 Open Your Letter</button>
 <button onclick="party()">💖 Send Love</button>

 <div id="letter" class="letter">
  <div style="font-size:48px">🧸🌹💗</div>
  <h2>Dear Dua, 💕</h2>
  Happy Birthday to you! 🎂

  <p>
   I hope your day is as beautiful as your smile
   and your year is filled with happiness.
   May Allah bless you with peace, success,
   good health and countless reasons to smile.
   Always stay happy and keep shining. 🌙✨
  </p>

  <p>
   Sending you this little teddy with lots of
   birthday wishes and a heart full of kindness. 🧸💝
  </p>

  <h3>With lots of love,<br>Talha 💗</h3>
  🎀 Happy Birthday, Dua! 🎀
 </div>

 <footer>MADE WITH ♡ BY TALHA, JUST FOR DUA</footer>
</main>

<script>
function floatItem(symbol){
 const el=document.createElement("div");
 el.className="float";
 el.textContent=symbol;
 el.style.left=Math.random()*100+"vw";
 el.style.fontSize=(18+Math.random()*24)+"px";
 const duration=4+Math.random()*5;
 el.style.animationDuration=duration+"s";
 document.body.appendChild(el);
 setTimeout(()=>el.remove(),duration*1000);
}
setInterval(()=>{
 floatItem(["💗","💕","🌸","✨","🧸","🎀"][
 Math.floor(Math.random()*6)]);
},450);

function openLetter(){
 const box=document.getElementById("letter");
 box.style.display=box.style.display==="block"?"none":"block";
 if(box.style.display==="block")party();
}
function party(){
 for(let i=0;i<35;i++){
  setTimeout(()=>floatItem(["💖","💗","🧸","🌹","✨","🎀"][
  Math.floor(Math.random()*6)]),i*90);
 }
}
</script>
</body>
</html>
