<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GO-AWAY - Planifie ton voyage personnalisé</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #00b4d8;
      --secondary: #0077b6;
      --accent: #90e0ef;
      --light: #f1f1f1;
      --dark: #03045e;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f5f5f5;
      color: #333;
    }

    header {
      background: #f5f5f5;
      color: white;
      text-align: center;
      padding: 120px 20px;
    }

    header h1 {
      font-size: 3.5em;
      margin-bottom: 10px;
      font-weight: 700;
    }

    header p {
      font-size: 1.4em;
    }

    .container {
      max-width: 1200px;
      margin: 40px auto;
      padding: 0 20px;
    }

    .offers {
      display: flex;
      gap: 20px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .offer-card {
  border-radius: 10px;
  overflow: hidden;
  width: 300px;
  transition: transform 0.3s ease;
  background: none;
  box-shadow: none;
}

    .offer-card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .offer-content {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.5s ease-in-out, padding 0.3s ease-in-out;
      padding: 0 20px;
      background: transparent;
    }

    .offer-card:hover .offer-content {
      max-height: 400px;
      padding: 20px;
    }

    .offer-content h3 {
      margin-top: 0;
    }

    .option-boxes {
      display: flex;
      gap: 10px;
      margin: 10px 0;
      flex-wrap: wrap;
    }

    .option-box {
      padding: 8px 12px;
      border: none;
      border-radius: 6px;
      background-color: #f9f9f9;
      cursor: pointer;
      font-size: 0.9em;
      transition: background-color 0.2s ease;
    }

    .option-box:hover {
      background-color: var(--accent);
    }

    .price {
      font-weight: bold;
      margin-top: 10px;
      font-size: 1.1em;
      transition: color 0.3s ease, transform 0.3s ease;
    }

    .note {
      font-size: 0.9em;
      color: #555;
      margin-top: 4px;
    }
  .option-box.selected {
  background-color: #f5f5f5;
  color: white;
}
</style>
</head>
<body>
<header style="height: 100px; padding: 0 20px; display: flex; align-items: center; background-color: #f5f5f5;">
  <img src="https://i.imgur.com/zgUQoU5.png" alt="GO AWAY Logo" style="height: 100%;">
</header>
    <div class="container">
    <h2 style="text-align:center;">Voyages inoubliables à découvrir</h2>
    <div class="offers">

      <!-- Japon -->
      <div class="offer-card">
        <img src="https://images.unsplash.com/photo-1526481280693-3bfa7568e0f3" alt="Japon">
        <div class="offer-content">
          <h3>Japon - Entre Amis</h3>
          <p>✨ Tokyo, Kyoto et nuit dans un ryokan. 10 jours.</p>
          <div class="option-boxes">
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 1)">1</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 1.25)">2</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 1.5)">3</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 1.75)">4</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 2)">5</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 2.25)">6</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 2.5)">7</div>
            <div class="option-box" onmouseover="showPrice('japon-price', 1500, 2.75)">8</div>
          </div>
          <p class="price" id="japon-price">Passez votre souris pour voir le prix</p>
<button style="margin-top: 10px; padding: 10px 16px; background-color: var(--primary); color: white; border: none; border-radius: 6px; font-weight: bold; cursor: pointer; width: 100%;">Envoyer une demande</button>
        </div>
      </div>

      <!-- Tanzanie -->
      <div class="offer-card">
        <img src="https://images.unsplash.com/photo-1516426122078-c23e76319801" alt="Tanzanie">
        <div class="offer-content">
          <h3>Tanzanie - En Famille</h3>
          <p>✨ Safari 4x4 + détente à Zanzibar. 7 jours.</p>
          <div class="option-boxes">
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 1)">1</div>
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 1.2)">2</div>
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 1.4)">3</div>
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 1.6)">4</div>
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 1.8)">5</div>
            <div class="option-box" onmouseover="showPrice('tanzanie-price', 1800, 2.0)">6</div>
          </div>
          <p class="price" id="tanzanie-price">Passez votre souris pour voir le prix</p>   
<button style="margin-top: 10px; padding: 10px 16px; background-color: var(--primary); color: white; border: none; border-radius: 6px; font-weight: bold; cursor: pointer; width: 100%;">Envoyer une demande</button>
        </div>
      </div>

      <!-- Bali -->
      <div class="offer-card">
        <img src="https://images.unsplash.com/photo-1577949269674-517f978815cf" alt="Bali">
        <div class="offer-content">
          <h3>Bali - Solo/Duo</h3>
          <p>✨ Yoga, plages, temples et rizières. 8 jours.</p>
          <div class="option-boxes">
            <div class="option-box" onmouseover="showPrice('bali-price', 1300, 1)">Seul</div>
            <div class="option-box" onmouseover="showPrice('bali-price', 1300, 1.35)">Accompagné</div>
          </div>
          
<button style="margin-top: 10px; padding: 10px 16px; background-color: var(--primary); color: white; border: none; border-radius: 6px; font-weight: bold; cursor: pointer; width: 100%;">Envoyer une demande</button>
        </div>
      </div>

    </div>
  </div>

  <script>
    function showPrice(id, base, multiplier) {
      const el = document.getElementById(id);
      el.textContent = `Budget : ${Math.round(base * multiplier)} €`;
      el.style.color = '#0077b6';
      el.style.transform = 'scale(1.1)';
      setTimeout(() => {
        el.style.transform = 'scale(1)';
      }, 200);
    }
  </script>
<section class="form-section" style="background-color: #ffffffcc; padding: 40px; border-radius: 16px; box-shadow: 0 8px 30px rgba(0,0,0,0.08); max-width: 700px; margin: 60px auto;">
  <h2>Crée ton voyage personnalisé</h2>
  <p>Dis-nous ce que tu veux, on s’occupe du reste.</p>
  <form style="display: grid; gap: 16px;">
    <label for="destination">Destination souhaitée :</label>
<select id="destination" name="destination">
  <option>France</option>
  <option>Japon</option>
  <option>Tanzanie</option>
  <option>Bali</option>
  <option>Italie</option>
  <option>Canada</option>
  <option>Mexique</option>
  <option>Espagne</option>
</select>

    <label for="start-date">Date de départ :</label>
<input type="date" id="start-date" name="start-date">

<label for="end-date">Date de retour :</label>
<input type="date" id="end-date" name="end-date">

    <label for="budget">Budget (€) :</label>
    <input type="number" id="budget" name="budget">

    <label for="type">Type de voyage :</label>
<div class="option-boxes">
  <div class="option-box" onclick="selectOption(this, 'type')">Solo</div>
  <div class="option-box" onclick="selectOption(this, 'type')">Couple</div>
  <div class="option-box" onclick="selectOption(this, 'type')">Famille</div>
  <div class="option-box" onclick="selectOption(this, 'type')">Amis</div>
</div>
<input type="hidden" id="type" name="type">

    <label for="themes">Thèmes préférés :</label>
    <input type="text" id="themes" name="themes" placeholder="plage, nature, ville...">

    <label for="transport">Transport préféré :</label>
    <select id="transport" name="transport">
      <option>Avion</option>
      <option>Train</option>
      <option>Voiture</option>
      <option>Peu importe</option>
    </select>

    <label for="hebergement">Type d’hébergement :</label>
    <select id="hebergement" name="hebergement">
      <option>Hôtel</option>
      <option>Auberge</option>
      <option>Appartement</option>
      <option>Surprise</option>
    </select>

    <label for="email">Ton adresse email :</label>
    <input type="email" id="email" name="email">

    <button type="submit">Envoyer une demande</button>
  </form>
</section>
<script>
function selectOption(element, inputId) {
  const boxes = element.parentElement.querySelectorAll('.option-box');
  boxes.forEach(b => b.classList.remove('selected'));
  element.classList.add('selected');
  document.getElementById(inputId).value = element.textContent;
}
</script>
</body>
</html>
