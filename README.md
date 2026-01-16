
<html lang="en">
<head>
<meta charset="UTF-8">
<title>VelCrowny | Standoff 2 Clan</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
/* ===== RESET ===== */
*{box-sizing:border-box;}
body{
  margin:0;
  font-family:Segoe UI, sans-serif;
  background:#040611;
  color:#fff;
  overflow-x:hidden;
}

/* ===== BACKGROUND EFFECT ===== */
.bg-glow{
  position:fixed;
  inset:0;
  background:
    radial-gradient(circle at 20% 30%, #6f00ff44, transparent 40%),
    radial-gradient(circle at 80% 70%, #00f6ff33, transparent 45%);
  animation:moveBg 10s infinite alternate;
  z-index:-1;
}
@keyframes moveBg{
  from{filter:hue-rotate(0deg);}
  to{filter:hue-rotate(40deg);}
}

/* ===== HEADER ===== */
header{
  text-align:center;
  padding:70px 20px;
}
header h1{
  font-size:clamp(36px,8vw,52px);
  letter-spacing:4px;
  color:#00f6ff;
  text-shadow:
    0 0 10px #00f6ff,
    0 0 30px #6f00ff;
  animation:neonPulse 2s infinite alternate;
}
@keyframes neonPulse{
  from{text-shadow:0 0 10px #00f6ff;}
  to{text-shadow:0 0 25px #00f6ff,0 0 50px #6f00ff;}
}
header p{opacity:.8}

/* ===== NAV ===== */
nav{
  display:flex;
  justify-content:center;
  gap:20px;
  padding:14px;
  backdrop-filter:blur(10px);
}
nav a{
  color:#aaa;
  text-decoration:none;
  font-weight:600;
}
nav a:hover{color:#00f6ff}

/* ===== SECTION ===== */
section{
  max-width:1000px;
  margin:auto;
  padding:30px 20px;
}
.card{
  background:rgba(255,255,255,.04);
  border:1px solid #00f6ff44;
  box-shadow:0 0 25px #00f6ff22;
  border-radius:18px;
  padding:25px;
  margin-bottom:25px;
  transition:.3s;
}
.card:hover{
  box-shadow:0 0 35px #00f6ff55;
}
.card h2{
  color:#ff00ea;
  margin-bottom:15px;
}

/* ===== MEMBERS ===== */
.members{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(160px,1fr));
  gap:16px;
}
.member{
  background:#080b20;
  border:1px solid #00f6ff55;
  border-radius:14px;
  padding:18px;
  text-align:center;
  transition:.3s;
}
.member:hover{
  transform:translateY(-5px);
  box-shadow:0 0 20px #00f6ff66;
}

/* ===== FORM ===== */
form input, form select{
  width:100%;
  padding:14px;
  margin-bottom:12px;
  border-radius:10px;
  border:none;
  background:#0c1025;
  color:#fff;
}
form button{
  width:100%;
  padding:15px;
  border:none;
  border-radius:12px;
  background:#00f6ff;
  color:#000;
  font-weight:700;
  cursor:pointer;
  box-shadow:0 0 20px #00f6ff88;
}
form button:hover{
  background:#6f00ff;
  color:#fff;
}

/* ===== MOBILE FIX ===== */
@media(max-width:600px){
  nav{gap:14px;font-size:14px;}
  .card{padding:20px;}
}
</style>
</head>

<body>
<div class="bg-glow"></div>

<header>
  <h1>VELCROWNY</h1>
  <p>Standoff 2 | Cyberpunk Esport Clan</p>
</header>

<nav>
  <a href="#about">About</a>
  <a href="#members">Members</a>
  <a href="#join">Join</a>
</nav>

<section id="about" class="card">
  <h2>About</h2>
  <p>VelCrowne бол Standoff 2 дээр төвлөрсөн rank up хэв маягтай esport clan.</p>
</section>

<section id="members" class="card">
  <h2>Members</h2>
  <div class="members">
    <div class="member">👑 Leader<br>Xyp3x_4k</div>
    <div class="member">⚔️ Sniper<br>Crow</div>
    <div class="member">🔥 Rusher<br>Nyx</div>
  </div>
</section>

<section id="join" class="card">
  <h2>Join Clan</h2>
  <form>
    <input type="text" placeholder="Nickname" required>
    <select>
      <option>Rank</option>
      <option>Gold</option>
      <option>Phoenix</option>
      <option>Ranger</option>
      <option>Champion</option>
    </select>
    <button type="submit">Apply</button>
  </form>
</section>

</body>
</html>
