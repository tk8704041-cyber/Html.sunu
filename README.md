<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday My Love ❤️</sultana>

<style>
body {
  margin: 0;
  height: 100vh;
  background: linear-gradient(120deg, #ff758c, #ff7eb3);
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: 'Segoe UI', sans-serif;
  color: white;
  overflow: hidden;
}

.card {
  background: rgba(0,0,0,0.3);
  padding: 35px;
  border-radius: 25px;
  text-align: center;
  max-width: 350px;
  box-shadow: 0 15px 40px rgba(0,0,0,0.4);
  animation: fadeIn 1.5s ease;
}

h1 {
  font-size: 2.6rem;
  margin-bottom: 10px;
}

p {
  font-size: 1.1rem;
  line-height: 1.6;
}

button {
  margin-top: 20px;
  padding: 12px 28px;
  font-size: 16px;
  border: none;
  border-radius: 30px;
  background: #ff2d55;
  color: white;
  cursor: pointer;
  box-shadow: 0 5px 15px rgba(0,0,0,0.3);
}

button:hover {
  background: #ff1744;
}

@keyframes fadeIn {
  from {opacity: 0; transform: scale(0.7);}
  to {opacity: 1; transform: scale(1);}
}

/* Floating hearts */
.heart {
  position: absolute;
  bottom: -20px;
  font-size: 20px;
  animation: float 6s infinite;
}

@keyframes float {
  0% {transform: translateY(0); opacity: 1;}
  100% {transform: translateY(-700px); opacity: 0;}
}
</style>
</head>

<body>

<div class="card">
  <h1>🎂 Happy Birthday ❤️</h1>
  <p>
    To the girl who makes my life brighter ✨<br>
    Your smile is my favorite thing in the world 💕<br>
    I’m so lucky to have you 🥺❤️
  </p>
  <button onclick="surprise()">💖 Click for Surprise</button>
</div>

<audio id="music">
  <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3">
</audio>

<script>
function surprise() {
  document.getElementById("music").play();
  alert("I love you more than words can say ❤️");
}

function createHeart() {
  const heart = document.createElement("div");
  heart.className = "heart";
  heart.innerHTML = "❤️";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.animationDuration = (Math.random() * 3 + 3) + "s";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 6000);
}

setInterval(createHeart, 300);
</script>

</body>
</html>
