<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Joyeux Anniversaire Princesse Kia 🎉</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #f6d365, #fda085);
      color: white;
      text-align: center;
    }
    section {
      padding: 60px 20px;
      max-width: 800px;
      margin: auto;
    }
    h1, h2 {
      margin-bottom: 20px;
    }
    p {
      font-size: 18px;
      line-height: 1.6;
    }
    .card {
      background: rgba(255, 255, 255, 0.15);
      padding: 30px;
      border-radius: 15px;
      margin-top: 30px;
    }
    button {
      margin-top: 20px;
      padding: 12px 25px;
      font-size: 16px;
      border: none;
      border-radius: 30px;
      background: #ffcc70;
      cursor: pointer;
    }
    button:hover {
      background: #ffd98e;
    }
    #secret {
      display: none;
      margin-top: 30px;
      font-size: 20px;
    }
    #secretContent {
      opacity: 0;
      transition: opacity 1.5s;
    }
    #bisous {
      margin-top: 20px;
      font-size: 28px;
    }
    footer {
      margin-top: 50px;
      font-size: 14px;
      opacity: 0.8;
    }
    .ingredient {
      display: inline-block;
      margin: 5px;
      font-size: 40px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <section>
    <h1>🎉 Joyeux 13 ans Princesse Kia 🎉</h1>
    <p>Bienvenue dans le royaume de Princesse Kia, 13 ans et déjà Première Ministre de son école 👑</p>
  </section>

  <!-- Super-pouvoirs interactifs -->
  <section class="card">
    <h2>Découvre tes super-pouvoirs ✨</h2>
    <button onclick="showPower('drôle')">Drôle 😂</button>
    <button onclick="showPower('créative')">Créative ✨</button>
    <button onclick="showPower('histoires')">Inventrice d’histoires 📖</button>
    <button onclick="showPower('pâtisserie')">Pâtissière 🍰</button>
    <p id="powerText" style="margin-top:20px;"></p>
  </section>

  <!-- Mini-jeu gâteau magique -->
  <section class="card">
    <h2>Crée ton gâteau magique 🍰</h2>
    <p>Choisis tes ingrédients :</p>
    <span class="ingredient" onclick="addIngredient('🍫')">🍫</span>
    <span class="ingredient" onclick="addIngredient('🍓')">🍓</span>
    <span class="ingredient" onclick="addIngredient('🥐')">🥐</span>
    <span class="ingredient" onclick="addIngredient('🍒')">🍒</span>
    <div id="cake" style="margin-top:20px;font-size:30px;"></div>
    <button onclick="finishCake()">Terminer le gâteau</button>
    <p id="cakeMessage" style="margin-top:20px;"></p>
  </section>

  <!-- 13 bisous -->
  <section class="card">
    <h2>13 bisous pour tes 13 ans 💋</h2>
    <button onclick="lancerBisous()">Clique pour les recevoir</button>
    <div id="bisous"></div>
  </section>

  <!-- Message final -->
  <section>
    <button onclick="showSecret()">Clique si t’es prête 👀</button>
    <div id="secret">
      <div id="secretContent">
        <p>
          Princesse Kia,<br><br>
          Tu es incroyable 💖<br>
          Je suis tellement fière de toi et de ton imagination ✨<br><br>
          Je t’aime fort 💙☺️<br>
          <em>De ta grande sœur qui t’adore et veille toujours sur toi 😄👑</em>
        </p>
      </div>
    </div>
  </section>

  <footer>
    Fait avec le cœur pour Princesse Kia 🎂
  </footer>

  <script>
    // Super-pouvoirs
    function showPower(power) {
      let message = '';
      if(power === 'drôle') message = "Ton humour est magique, tu fais rire tout le monde 😄";
      if(power === 'créative') message = "Ta créativité est incroyable, tu inventes toujours des histoires magiques ✨";
      if(power === 'histoires') message = "Tes histoires sont fascinantes, on pourrait les lire encore et encore 📖";
      if(power === 'pâtisserie') message = "Tes gâteaux sont délicieux… et ton sourire encore plus 🍰";
      document.getElementById('powerText').innerHTML = message;
    }

    // Mini-jeu gâteau magique
    let cakeIngredients = [];
    function addIngredient(ing) {
      cakeIngredients.push(ing);
      document.getElementById('cake').innerHTML = cakeIngredients.join('');
    }
    function finishCake() {
      if(cakeIngredients.length === 0) {
        document.getElementById('cakeMessage').innerHTML = "Ton gâteau est vide… mais tu restes parfaite 😄";
      } else {
        document.getElementById('cakeMessage').innerHTML = "Ton gâteau magique " + cakeIngredients.join('') + " est parfait, tout comme toi Princesse Kia 💖";
      }
      cakeIngredients = [];
      document.getElementById('cake').innerHTML = '';
    }

    // 13 bisous
    function lancerBisous() {
      const bisous = document.getElementById("bisous");
      bisous.innerHTML = "";
      let count = 0;
      const interval = setInterval(() => {
        if (count < 13) {
          bisous.innerHTML += "💋";
          count++;
        } else {
          clearInterval(interval);
        }
      }, 200);
    }

    // Message final fade-in
    function showSecret() {
      const secret = document.getElementById("secret");
      const content = document.getElementById("secretContent");
      secret.style.display = "block";
      setTimeout(() => {
        content.style.opacity = 1;
        content.scrollIntoView({ behavior: "smooth" });
      }, 500);
    }
  </script>

</body>
</html>
