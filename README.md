<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gadhaa Janata Party</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins;
}

body{
background:#f7f7f7;
color:#111;
}

/* HEADER */
header{
display:flex;
justify-content:space-between;
align-items:center;
padding:18px 10%;
background:#fff;
position:sticky;
top:0;
border-bottom:1px solid #eee;
}

.logo{
font-size:20px;
font-weight:800;
}

.logo span{
color:#e60023;
}

nav a{
color:#e60023;
font-weight:800;
text-decoration:none;
}

/* HERO */
.hero{
text-align:center;
padding:60px 10%;
}

.hero h1{
font-size:50px;
font-weight:800;
}

.hero h1 span{
color:#e60023;
}

.hero p{
margin-top:10px;
color:#555;
line-height:1.7;
}

.tag{
margin-top:10px;
display:inline-block;
background:#ffe3e6;
color:#e60023;
padding:8px 15px;
border-radius:50px;
font-weight:700;
font-size:12px;
}

/* COUNTER */
.counter{
text-align:center;
margin-top:30px;
font-size:60px;
font-weight:900;
}

.counter small{
display:block;
font-size:13px;
color:#777;
}

/* SECTION */
.section{
padding:50px 10%;
}

.card{
background:#fff;
padding:25px;
border-radius:15px;
box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

/* GRID */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:15px;
margin-top:15px;
}

.box{
background:#fafafa;
padding:15px;
border-radius:12px;
text-align:center;
font-weight:600;
}

/* FORM */
input{
width:100%;
padding:12px;
margin-top:10px;
border:1px solid #ddd;
border-radius:10px;
}

input:focus{
border-color:#e60023;
outline:none;
}

button{
width:100%;
padding:12px;
background:#e60023;
color:#fff;
border:none;
border-radius:10px;
font-weight:800;
cursor:pointer;
margin-top:10px;
}

/* SUCCESS */
#success{
display:none;
margin-top:15px;
padding:15px;
background:#eaffea;
border:2px solid #22c55e;
border-radius:10px;
text-align:center;
font-weight:800;
color:#166534;
}

/* FOOTER */
footer{
text-align:center;
padding:25px;
color:#888;
border-top:1px solid #eee;
margin-top:40px;
}

.bottom{
text-align:center;
font-size:12px;
color:#aaa;
margin-bottom:10px;
}

</style>
</head>

<body>

<header>
<div class="logo">🫏 <span>GJP</span> Party</div>

<nav>
<a href="https://instagram.com/gadhaajanataparty" target="_blank">📸 Instagram</a>
</nav>
</header>

<!-- HERO -->
<div class="hero">

<h1>Voice of <span>Overworked People</span></h1>

<p>
A meme-driven political satire movement for daily life struggles 😭🫏
</p>

<div class="tag">
NATION'S MOST OVERWORKED PARTY 🫏
</div>

<div class="counter">
👥 <span id="count">0</span>
<small>LIVE MEMBERS</small>
</div>

</div>

<!-- PROBLEMS -->
<div class="section">
<div class="card">
<h2>Today's Problems 💀</h2>

<div class="grid">
<div class="box">🚧 Roads never finish</div>
<div class="box">📡 Network issues</div>
<div class="box">💰 Salary delay</div>
<div class="box">🏛 No results meetings</div>
<div class="box">🗳 Election promises</div>
<div class="box">📈 Inflation rise</div>
</div>

</div>
</div>

<!-- FUN -->
<div class="section">
<div class="card">
<h2>Fun Questions 😂</h2>

<div class="grid">
<div class="box">Roads? → Next election</div>
<div class="box">Salary? → Processing</div>
<div class="box">Network? → Weather issue</div>
<div class="box">Results? → 1947 pending</div>
<div class="box">Promises? → Update pending</div>
<div class="box">Prices? → System bug</div>
</div>

</div>
</div>

<!-- FORM -->
<div class="section">
<div class="card">

<h2>Join The Party 🫏</h2>

<form name="gjp-form" method="POST" data-netlify="true">

<input type="hidden" name="form-name" value="gjp-form">

<input name="name" placeholder="Name" required>
<input name="age" placeholder="Age" required>
<input name="email" placeholder="Email" required>
<input name="city" placeholder="City" required>
<input name="district" placeholder="District" required>
<input name="state" placeholder="State" required>
<input name="reason" placeholder="Why joining?" required>
<input name="instagram" placeholder="@Instagram ID" required>

<button type="submit">JOIN NOW</button>

</form>

<div id="success">
🎉 Successfully Joined! Welcome to GJP 🫏
</div>

</div>
</div>

<footer>
Powered by 🫏 Gadhaa Janata Party
</footer>

<p class="bottom">Built with satire 😭🫏</p>

<script>

/* LIVE COUNTER */
let count = localStorage.getItem("gjp_count") || 0;
document.getElementById("count").innerText = count;

/* FORM */
document.querySelector("form").addEventListener("submit",function(){

count++;
localStorage.setItem("gjp_count",count);
document.getElementById("count").innerText = count;

/* SUCCESS MESSAGE */
setTimeout(()=>{
document.getElementById("success").style.display="block";
},300);

});

</script>

</body>
</html>