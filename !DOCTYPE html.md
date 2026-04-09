<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<title>For Kalila ❤️</title>  
  
<style>  
body {  
  margin: 0;  
  height: 100vh;  
  overflow: hidden;  
  font-family: Arial;  
  background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);  
  color: white;  
  display: flex;  
  justify-content: center;  
  align-items: center;  
  text-align: center;  
}  
  
.container {  
  background: rgba(255,255,255,0.1);  
  padding: 35px;  
  border-radius: 20px;  
  backdrop-filter: blur(15px);  
  max-width: 320px;  
}  
  
button {  
  margin-top: 15px;  
  padding: 10px 20px;  
  border: none;  
  border-radius: 20px;  
  background: #ff4d6d;  
  color: white;  
}  
  
.hidden {  
  display: none;  
  margin-top: 15px;  
  font-size: 14px;  
}  
  
.heart {  
  position: absolute;  
  color: #ff4d6d;  
  animation: fall linear infinite;  
}  
  
@keyframes fall {  
  0% { transform: translateY(-10vh); }  
  100% { transform: translateY(110vh); }  
}  
</style>  
</head>  
  
<body onclick="love(event)">  
  
<div class="container">  
  <h2>Kalila Anishah ❤️</h2>  
  
  <p>  
    i don’t really know where to start…<br><br>  
    but ever since i met you,<br>  
    something slowly changed in me.<br><br>  
    little things started to matter,<br>  
    ordinary days felt different,<br>  
    and somehow…<br>  
    you became someone i don’t want to lose.  
  </p>  
  
  <button onclick="show()">keep reading 💌</button>  
  
  <div id="msg" class="hidden">  
    i’m not perfect,<br>  
    i still have so many flaws…<br><br>  
    but one thing i’m sure about is:<br>  
    what i feel for you is real.<br><br>  
    i don’t want something temporary…<br>  
    i want something that lasts.<br><br>  
    and honestly…<br>  
    i want that with you.  
  </div>  
  
  <button onclick="music()">play our song 🎶</button>  
  
  <br><br>  
  
  <p>will you stay with me?</p>  
  
  <button onclick="yes()">YES 💖</button>  
  <button id="noBtn" onmouseover="run()">NO 😭</button>  
  
  <div id="yesMsg" class="hidden">  
    thank you for choosing me 🫶<br>  
    i’ll take care of this, i promise.  
  </div>  
</div>  
  
<!-- A Thousand Years (reff) -->  
<iframe id="m" width="0" height="0"  
src=""  
allow="autoplay">  
</iframe>  
  
<script>  
function show(){  
  document.getElementById("msg").style.display="block";  
}  
  
function music(){  
  document.getElementById("m").src =  
  "https://www.youtube.com/embed/rtOvBOTyX00?start=60&autoplay=1&loop=1&playlist=rtOvBOTyX00";  
}  
  
function yes(){  
  document.getElementById("yesMsg").style.display="block";  
}  
  
function run(){  
  const b=document.getElementById("noBtn");  
  b.style.position="absolute";  
  b.style.left=Math.random()*80+"vw";  
  b.style.top=Math.random()*80+"vh";  
}  
  
function createHeart(){  
  const h=document.createElement("div");  
  h.className="heart";  
  h.innerHTML="❤";  
  h.style.left=Math.random()*100+"vw";  
  h.style.animationDuration=(Math.random()*3+2)+"s";  
  document.body.appendChild(h);  
  setTimeout(()=>h.remove(),5000);  
}  
setInterval(createHeart,300);  
  
function love(e){  
  const h=document.createElement("div");  
  h.innerHTML="💖";  
  h.style.position="absolute";  
  h.style.left=e.clientX+"px";  
  h.style.top=e.clientY+"px";  
  document.body.appendChild(h);  
  setTimeout(()=>h.remove(),1000);  
}  
</script>  
  
</body>  
</html>  
