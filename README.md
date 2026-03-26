<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Oxygène Restaurant & Lounge</title>

<style>
body {
  margin:0;
  font-family: Arial;
  background:#0c0c0c;
  color:white;
}

header {
  background:url('https://images.unsplash.com/photo-1552566626-52f8b828add9') center/cover;
  height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
}

h1 {
  font-size:3em;
  color:#d4af37;
}

button {
  padding:15px 30px;
  border:none;
  background:#d4af37;
  color:black;
  font-weight:bold;
  cursor:pointer;
}

section {
  padding:40px;
}

.menu {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:20px;
}

.card {
  background:#1a1a1a;
  padding:20px;
  border-radius:10px;
}

input, select {
  width:100%;
  padding:10px;
  margin:10px 0;
}

footer {
  text-align:center;
  padding:20px;
  background:black;
}
</style>
</head>

<body>

<header>
  <h1>Oxygène Restaurant & Lounge</h1>
  <p>Expérience culinaire unique à Abidjan</p>
  <button onclick="scrollToReservation()">Réserver maintenant</button>
</header>

<section>
<h2>Notre Menu</h2>
<div class="menu">
  <div class="card">
    <h3>Grillades</h3>
    <p>À partir de 5000 FCFA</p>
  </div>
  <div class="card">
    <h3>Plats africains</h3>
    <p>À partir de 3000 FCFA</p>
  </div>
  <div class="card">
    <h3>Cocktails</h3>
    <p>À partir de 4000 FCFA</p>
  </div>
</div>
</section>

<section id="reservation">
<h2>Réserver une table</h2>

<input type="text" placeholder="Nom">
<input type="tel" placeholder="Téléphone">
<input type="date">
<input type="time">
<select>
  <option>Nombre de personnes</option>
  <option>1</option>
  <option>2</option>
  <option>3</option>
  <option>4+</option>
</select>

<button onclick="payer()">Payer & Réserver</button>
</section>

<section>
<h2>Contact</h2>
<p>📍 Angré CNPS 9ème tranche, Abidjan</p>
<p>📞 07 89 89 70 70</p>
</section>

<footer>
<p>© 2026 Oxygène Restaurant</p>
</footer>

<script>
function scrollToReservation() {
  document.getElementById("reservation").scrollIntoView({behavior:"smooth"});
}

function payer() {
  alert("Redirection vers paiement Mobile Money / Carte...");
  window.location.href = "https://paydunya.com"; // à remplacer
}
</script>

</body>
</html>
