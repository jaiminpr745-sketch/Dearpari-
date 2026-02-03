dear pari 
 <!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For My Love 💕</title>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Poppins:wght@300;500&display=swap" rel="stylesheet">
<style>
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  overflow: hidden;
  text-align: center;
  color: white;
}

/* GIF BACKGROUND */
body::before {
  content: "";
  position: fixed;
  width: 100%;
  height: 100%;
  background: url("https://media.giphy.com/media/3oriO0OEd9QIDdllqo/giphy.gif") center/cover no-repeat;
  z-index: -1;
  filter: brightness(0.5);
}

/* Pages */
.page {
  display: none;
  height: 100vh;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 20px;
  animation: fadeIn 1s ease;
}
.active { display: flex; }

/* Animations */
@keyframes fadeIn {
  from {opacity:0;}
  to {opacity:1;}
}

h1 {
  font-family: 'Pacifico', cursive;
  font-size: 32px;
  margin: 10px 0;
}

p {
  font-size: 20px;
  margin: 5px 0;
}

button {
  margin-top: 20px;
  padding: 12px 30px;
  border: none;
  border-radius: 25px;
  font-size: 18px;
  background: #ff4d6d;
  color: white;
  cursor: pointer;
  transition: transform 0.2s;
}
button:hover { transform: scale(1.1); }
</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="page active" id="p1">
  <h1>Hey My Pari 💖</h1>
  <p>Mera Pyara Bacha, tum meri duniya ho 🥰</p>
  <button onclick="next(2)">Tap</button>
</div>

<!-- PAGE 2 -->
<div class="page" id="p2">
  <h1>My Cute Baby 🐻💕</h1>
  <p>Har pal tumhare saath hona chahta hoon ✨</p>
  <button onclick="next(3)">Next</button>
</div>

<!-- PAGE 3 -->
<div class="page" id="p3">
  <h1>My Love Paru Baby 💘</h1>
  <p>Tum meri life ki sabse pyari cheez ho 😘</p>
  <button onclick="next(4)">Next</button>
</div>

<!-- PAGE 4 -->
<div class="page" id="p4">
  <h1>I Love You Forever ❤️</h1>
  <p>Har din tumhari muskaan dekhna chahta hoon 😍</p>
  <button onclick="next(5)">Next</button>
</div>

<!-- PAGE 5 -->
<div class="page" id="p5">
  <h1>Tum Ho Meri Pari ✨</h1>
  <p>Meri duniya tumse hi roshan hai 💫</p>
  <button onclick="next(6)">Next</button>
</div>

<!-- PAGE 6 -->
<div class="page" id="p6">
  <h1>Forever Yours 💍💖</h1>
  <p>Bas tum aur mai 💕</p>
  <button onclick="yes()">Yes</button>
</div>

<script>
function next(page) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.getElementById('p' + page).classList.add('active');
}

function yes() {
  alert("I Love You My Baby Paru 💖✨");
}
</script>

</body>
</html>
