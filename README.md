<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Arnav ❤️ Anushka</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:linear-gradient(135deg,#ff758c,#ff7eb3);
overflow-x:hidden;
color:white;
text-align:center;
}

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
padding:20px;
}

.hero h1{
font-size:3rem;
margin-bottom:10px;
}

.hero p{
font-size:1.2rem;
max-width:700px;
}

.gallery{
padding:40px 20px;
}

.gallery h2{
margin-bottom:20px;
}

.photos{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:15px;
}

.photos img{
width:100%;
height:350px;
object-fit:cover;
border-radius:20px;
box-shadow:0 5px 20px rgba(0,0,0,0.2);
}

.letter{
padding:50px 20px;
}

.box{
background:white;
color:#333;
max-width:800px;
margin:auto;
padding:30px;
border-radius:20px;
line-height:1.8;
box-shadow:0 5px 25px rgba(0,0,0,0.2);
}

button{
margin-top:25px;
padding:14px 28px;
border:none;
border-radius:30px;
font-size:1rem;
cursor:pointer;
background:white;
color:#ff4f81;
font-weight:bold;
}

#secret{
display:none;
margin-top:20px;
font-size:1.2rem;
}

.footer{
padding:40px;
font-size:1.1rem;
}

.heart{
position:fixed;
top:-20px;
font-size:24px;
animation:fall linear infinite;
pointer-events:none;
}

@keyframes fall{
to{
transform:translateY(110vh);
}
}
</style>
</head>

<body>

<section class="hero">
<h1>❤️ Arnav & Anushka ❤️</h1>
<p>
Every picture tells a story, every memory holds a smile,
and every moment with you becomes my favorite.
</p>

<button onclick="showSecret()">Open My Heart 💌</button>

<div id="secret">
🫂🤍🧿<br><br>
IM GRATEFUL TO HAVE YOU BABE
</div>
</section>

<section class="gallery">
<h2>📸 Our Beautiful Memories</h2>

<div class="photos">
<img src="photo1.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">
<img src="photo4.jpg">
</div>
</section>

<section class="letter">
<div class="box">
<h2>💌 A Letter For You</h2>
<br>

<p>
Dear Anushka,
<br><br>
I don't always find the perfect words,
but I hope you know how much you mean to me.
Thank you for your smile, your support,
your laughter and all the memories we have created together.
<br><br>
You make ordinary days feel special,
and even the smallest moments become unforgettable when they're with you.
<br><br>
No matter where life takes us,
I will always cherish every memory we've shared.
<br><br>
❤️ Forever Yours,<br>
Arnav
</p>

</div>
</section>

<div class="footer">
Made with ❤️ by Arnav
</div>

<script>

function showSecret(){
document.getElementById("secret").style.display="block";
}

for(let i=0;i<50;i++){
let heart=document.createElement("div");
heart.innerHTML="❤️";
heart.classList.add("heart");
heart.style.left=Math.random()*100+"vw";
heart.style.animationDuration=(Math.random()*5+5)+"s";
document.body.appendChild(heart);
}

</script>

</body>
</html>
