<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>New Year Surprise 🎉</title>
<link rel="stylesheet" href="style.css">
</head>
<body>

<!-- Fireworks canvas -->
<canvas id="fireworks"></canvas>

<!-- Heart container (floating hearts) -->
<div id="heart-container" aria-hidden="true"></div>

<!-- Screens wrapper -->
<main id="app">
  <!-- Screen 1 -->
  <section id="screen1" class="screen active">
    <div class="left">
      <img src="shinchan.jpeg.jpeg" alt="Shinchan" class="side-img">
    </div>
    <div class="right text-container">
      <h1>🎉 Happy New Year, Sis 💖</h1>
      <p>May this year be full of smiles, peace, and laughter!</p>
      <div class="controls"><button onclick="showScreen('like')">Next</button></div>
    </div>
  </section>

  <!-- Screen 2: Do you like me -->
  <section id="screenLike" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>Do you like me? 💖</h1>
      <div class="controls">
        <button onclick="showScreen('goodGirl')">Yes</button>
        <button onclick="showScreen('please')">No</button>
      </div>
    </div>
  </section>

  <!-- Good girl page (after Yes) -->
  <section id="screenGoodGirl" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>😄 I thought you'd click No!</h1>
      <p>Good girl 💖 You actually clicked Yes — that made my day!</p>
      <div class="controls"><button onclick="showScreen('thank')">Next</button></div>
    </div>
  </section>

  <!-- "Please" page (No / alternate) -->
  <section id="screenPlease" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>Please, my cute bestie! 😘</h1>
      <p>Click Yes! I promise a special message is waiting for you 🎉</p>
      <div class="controls"><button onclick="showScreen('thank')">Yes</button></div>
    </div>
  </section>

  <!-- Thank you -->
  <section id="screenThank" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>❤️ Thank you for staying with me ❤️</h1>
      <div class="controls"><button onclick="showScreen('bond')">Next</button></div>
    </div>
  </section>

  <!-- Bond -->
  <section id="screenBond" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>💞 Please don’t leave me 💞</h1>
      <p>I want this bond forever — you’re my world 🥺💖</p>
      <div class="controls"><button onclick="showScreen('sorry')">Next</button></div>
    </div>
  </section>

  <!-- Sorry -->
  <section id="screenSorry" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>🙏 Sorry madam 🙏</h1>
      <p>If I ever hurt you, please forgive me 💖</p>
      <div class="controls"><button onclick="showScreen('trust')">Next</button></div>
    </div>
  </section>

  <!-- Trust (new) -->
  <section id="screenTrust" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>🤝 The trust you have on me 🤝</h1>
      <p>Your trust means the world to me. I’ll always value it 🌟</p>
      <div class="controls"><button onclick="showScreen('heartfelt')">Next</button></div>
    </div>
  </section>

  <!-- Heartfelt / Madam -->
  <section id="screenHeartfelt" class="screen">
    <div class="left"><img src="heart png.png" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>🌸 Madam 🌸</h1>
      <p>You’re my first priority, always 💖</p>
      <div class="controls"><button onclick="showScreen('princess')">Next</button></div>
    </div>
  </section>

  <!-- Princess -->
  <section id="screenPrincess" class="screen">
    <div class="left"><img src="princess.png" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>👑 You’re my princess 👑</h1>
      <p>Your smile brightens my world ✨</p>
      <div class="controls"><button onclick="showScreen('memories')">Next</button></div>
    </div>
  </section>

  <!-- Memories (slideshow single-photo with Prev/Next) -->
  <section id="screenMemories" class="screen">
    <div class="text-container memories-wrap">
      <h1>📸 Our Memories 📸</h1>

      <div class="memory-stage">
        <img id="memDisplay" src="mem1.jpg" alt="memory" class="memories-img slide-active">
      </div>

      <div class="controls memory-controls">
        <button id="prevBtn" onclick="prevMemory()">Previous</button>
        <span id="memCounter">1 / 10</span>
        <button id="nextBtn" onclick="nextMemory()">Next</button>
      </div>
    </div>
  </section>

  <!-- Final -->
  <section id="screenFinal" class="screen">
    <div class="left"><img src="shinchan.jpeg.jpeg" alt="" class="side-img"></div>
    <div class="right text-container">
      <h1>🎆 Happy New Year again! 🎆</h1>
      <p>May this new year bring endless joy and love 💖</p>
    </div>
  </section>
</main>

<script src="script.js"></script>
</body>
</html>
