# -
Мемные звуки
<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Meme Soundboard</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: white;
      text-align: center;
      padding: 30px;
    }h1 {
  margin-bottom: 20px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 15px;
  max-width: 800px;
  margin: auto;
}

button {
  padding: 20px;
  font-size: 16px;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  background: #ff4757;
  color: white;
  transition: 0.2s;
}

button:hover {
  background: #ff6b81;
  transform: scale(1.05);
}

  </style>
</head>
<body>
  <h1>🎵 Мем-звуки (жми и страдай)</h1>  <div class="grid">
    <button onclick="playSound('bruh')">Bruh</button>
    <button onclick="playSound('vine')">Vine Boom</button>
    <button onclick="playSound('laugh')">Evil Laugh</button>
    <button onclick="playSound('wow')">Wow</button>
  </div><audio id="bruh" src="sounds/bruh.mp3"></audio> <audio id="vine" src="sounds/vine-boom.mp3"></audio> <audio id="laugh" src="sounds/evil-laugh.mp3"></audio> <audio id="wow" src="sounds/wow.mp3"></audio>

  <script>
    function playSound(id) {
      const audio = document.getElementById(id);
      audio.currentTime = 0;
      audio.play();
    }
  </script></body>
</html>
