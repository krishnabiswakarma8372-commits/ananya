<!DOCTYPE html>
<html>
<head>
<title>For Ananya – From Krishna</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
    margin: 0;
    padding: 0;
    background: url('https://images.unsplash.com/photo-1448375240586-882707db888b?auto=format&fit=crop&w=1400&q=60') no-repeat center center fixed;
    background-size: cover;
    font-family: 'Poppins', sans-serif;
    color: white;
    scroll-behavior: smooth;
}

/* Content box */
.section {
    width: 85%;
    max-width: 700px;
    margin: 80px auto;
    padding: 25px;
    background: rgba(0,0,0,0.45);
    border-radius: 18px;
    backdrop-filter: blur(8px);
}

h1, h2, h3, p {
    text-shadow: 0 0 10px rgba(255,255,255,0.7);
}

/* Fade-in */
.fade-in {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUp 1.2s forwards;
}
@keyframes fadeInUp {
    to { opacity: 1; transform: translateY(0); }
}

/* Next button */
.next-btn {
    display: inline-block;
    padding: 12px 25px;
    margin-top: 30px;
    background: #ffcb4b;
    color: black;
    font-weight: bold;
    text-decoration: none;
    border-radius: 50px;
    box-shadow: 0 0 20px #ffcb4b;
}

/* Particle effects */
.star, .heart {
    position: fixed;
    width: 6px;
    height: 6px;
    pointer-events: none;
    border-radius: 50%;
    animation: floatUp 1.5s linear;
}
.star { background:white; }
.heart { background:pink; }

@keyframes floatUp {
    0% { opacity: 1; transform: translateY(0); }
    100% { opacity: 0; transform: translateY(-40px); }
}

/* Floating quotes */
.quote {
    position: absolute;
    font-size: 18px;
    color: rgba(255,255,255,0.35);
    white-space: nowrap;
    animation: drift 30s linear infinite;
}
@keyframes drift {
    0% { transform: translateX(110vw); }
    100% { transform: translateX(-110vw); }
}

/* Sparkles at final */
.spark {
    position: absolute;
    width: 4px;
    height: 4px;
    background: gold;
    border-radius: 50%;
    opacity: 0;
    animation: sparkle 2s infinite;
}
@keyframes sparkle {
    0% {opacity:0; transform: scale(0);}
    50% {opacity:1; transform: scale(1);}
    100% {opacity:0; transform: scale(0);}
}
</style>
</head>


<body>

<!-- 🎵 Background Music -->
<audio id="bg-music" autoplay loop>
  <source src="YOUR_AUDIO_URL_HERE" type="audio/mpeg">
</audio>

<button id="music-btn" style="position:fixed;top:20px;right:20px;padding:10px 15px;border-radius:50px;border:none;background:#ffcb4b;font-weight:bold;cursor:pointer;z-index:999;">
  Pause Music
</button>

<script>
const music = document.getElementById('bg-music');
const btn = document.getElementById('music-btn');
btn.addEventListener('click', () => {
    if(music.paused){
        music.play();
        btn.innerText = 'Pause Music';
    } else {
        music.pause();
        btn.innerText = 'Play Music';
    }
});
</script>


<!-- Floating Quotes -->
<div class="quote" style="top:20px;">You feel like peace.</div>
<div class="quote" style="top:120px;">Some connections happen quietly.</div>
<div class="quote" style="top:220px;">A soft voice can change a tough day.</div>


<!-- ========== SECTION 1 ========== -->
<div class="section fade-in" id="sec1">
<h2>Krishna Says:</h2>
<p>Every story begins somewhere…<br>
And ours started unexpectedly.</p>
<a href="#sec2" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 2 ========== -->
<div class="section fade-in" id="sec2">
<h2>Krishna Says:</h2>
<p>Ananya...<br><br>
Here is a small letter for you.<br>
Not to impress you,<br>
but to express what my heart feels.</p>
<a href="#sec3" class="next-btn">Open Letter »</a>
</div>


<!-- ========== SECTION 3 ========== -->
<div class="section fade-in" id="sec3">
<h2>Krishna Says:</h2>
<p>
When I asked you for that dressing on my hand…  
That was the moment I truly *saw you*.  
Your calmness, innocence, and soft voice — like a little baby —  
changed something inside me.
</p>
<a href="#sec4" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 4 ========== -->
<div class="section fade-in" id="sec4">
<h2>Krishna Says:</h2>
<p>
From one-word replies…  
To late-night conversations…  
To voice notes…  
Somewhere between all that,  
you became the reason my phone felt alive.
</p>
<a href="#sec5" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 5 ========== -->
<div class="section fade-in" id="sec5">
<h2>Krishna Says:</h2>
<p>You don’t just look beautiful.<br>
You *are* beautiful — in your thoughts, behavior, and kindness.</p>

<canvas id="constellation" width="700" height="300" style="display:block;margin:30px auto;"></canvas>

<a href="#sec6" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 6 ========== -->
<div class="section fade-in" id="sec6">
<h2>Krishna Says:</h2>
<p>
10 reasons why you're special:<br><br>
Your voice, innocence, courage, smile,<br>
honesty, patience, kindness, strength,<br>
simplicity, and the comfort you bring.
</p>
<a href="#sec7" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 7 ========== -->
<div class="section fade-in" id="sec7">
<h2>Krishna Says:</h2>
<p>
I didn’t expect it…  
but my heart softened whenever your name appeared on my screen.
</p>
<a href="#sec8" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 8 ========== -->
<div class="section fade-in" id="sec8">
<h2>Krishna Says:</h2>
<p>A small song… that reminds me of you.</p>

<iframe width="100%" height="240" 
src="https://www.youtube.com/embed/VEAfV9V5kAE" 
frameborder="0" allowfullscreen></iframe>

<a href="#sec9" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 9 ========== -->
<div class="section fade-in" id="sec9">
<h2>Krishna Says:</h2>
<p>
I don't want to make you uncomfortable.  
I don’t expect anything from you.  
I just want you to know what my heart truly feels.
</p>
<a href="#sec10" class="next-btn">Next »</a>
</div>


<!-- ========== SECTION 10 (FINAL) ========== -->
<div class="section fade-in" id="sec10">
<h2>Krishna Says:</h2>
<p>
No pressure. No expectations.<br><br>
If someday… even a small part of your heart feels the same,<br>
I’ll be the happiest person under this entire Milky Way.
</p>

<p style="text-align:center;margin-top:40px;">
With Respect & Care,<br><b>Krishna</b>
</p>
</div>

<script>
/* Floating particles (mouse + touch) */
document.addEventListener("mousemove", e => createParticle(e.x, e.y));
document.addEventListener("touchmove", e => {
    if(e.touches.length > 0){ 
        createParticle(e.touches[0].clientX, e.touches[0].clientY); 
    }
});

function createParticle(x, y){
    let heart = document.createElement("div");
    heart.classList.add("heart");
    heart.style.left = (x + (Math.random()*20-10)) + "px";
    heart.style.top = (y + (Math.random()*20-10)) + "px";
    heart.style.width = (4 + Math.random()*4) + "px";
    heart.style.height = heart.style.width;
    document.body.appendChild(heart);
    setTimeout(()=>{ heart.remove(); }, 1200);
}

/* ANANYA Constellation */
const canvas = document.getElementById('constellation');
if(canvas){
const ctx = canvas.getContext('2d');
let pts = [
  {x:50,y:200},{x:100,y:100},{x:150,y:200}, 
  {x:200,y:200},{x:250,y:100},{x:300,y:200}, 
  {x:350,y:200},{x:400,y:100},{x:450,y:200}, 
  {x:500,y:200},{x:550,y:100},{x:600,y:200}, 
  {x:650,y:200},{x:700,y:100}
];
let i=0;
(function draw(){
  if(i < pts.length-1){
    ctx.beginPath();
    ctx.moveTo(pts[i].x, pts[i].y);
    ctx.lineTo(pts[i+1].x, pts[i+1].y);
    ctx.strokeStyle='gold';
    ctx.lineWidth=2;
    ctx.stroke();
    i++;
    requestAnimationFrame(draw);
  }
})();
}

/* Final page sparkles */
setInterval(()=>{
    let s = document.createElement('div');
    s.classList.add('spark');
    s.style.left = Math.random()*innerWidth + "px";
    s.style.top = Math.random()*innerHeight + "px";
    document.body.appendChild(s);
    setTimeout(()=>s.remove(),2000);
},300);
</script>

</body>
</html>
