<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Cashback App</title>
  <style>
    body {
      font-family: sans-serif;
      margin: 20px;
      background-color: #f7f7f7;
    }
    h1 {
      text-align: center;
    }
    input, button {
      padding: 10px;
      margin: 5px 0;
      width: 100%;
      box-sizing: border-box;
    }
    .angebot {
      background: #fff;
      border: 1px solid #ccc;
      padding: 10px;
      margin: 10px 0;
      border-radius: 8px;
    }
  </style>
</head>
<body>
  <h1>Cashback-Angebote</h1>

  <input id="produkt" placeholder="Produktname">
  <input id="marke" placeholder="Marke">
  <input id="ablauf" type="date">
  <input id="link" placeholder="Link zum Angebot (optional)">
  <button onclick="hinzufügen()">Angebot speichern</button>

  <h2>Aktive Angebote</h2>
  <div id="liste"></div>

  <script>
    let angebote = JSON.parse(localStorage.getItem("angebote")) || [];

    function speichern() {
      localStorage.setItem("angebote", JSON.stringify(angebote));
    }

    function anzeigen() {
      const liste = document.getElementById("liste");
      liste.innerHTML = "";

      const heute = new Date().toISOString().split("T")[0];
      angebote = angebote.filter(a => a.ablauf >= heute);
      speichern();

      angebote.forEach((a, index) => {
        const div = document.createElement("div");
        div.className = "angebot";
        div.innerHTML = `
          <strong>${a.produkt}</strong> von <em>${a.marke}</em><br>
          Läuft ab: ${a.ablauf}<br>
          ${a.link ? `<a href="${a.link}" target="_blank">Zum Angebot</a><br>` : ""}
          <button onclick="löschen(${index})">Löschen</button>
        `;
        liste.appendChild(div);
      });
    }

    function hinzufügen() {
      const produkt = document.getElementById("produkt").value;
      const marke = document.getElementById("marke").value;
      const ablauf = document.getElementById("ablauf").value;
      const link = document.getElementById("link").value;

      if (!produkt || !marke || !ablauf) {
        alert("Bitte Produkt, Marke und Ablaufdatum angeben.");
        return;
      }

      angebote.push({ produkt, marke, ablauf, link });
      speichern();
      anzeigen();

      document.getElementById("produkt").value = "";
      document.getElementById("marke").value = "";
      document.getElementById("ablauf").value = "";
      document.getElementById("link").value = "";
    }

    function löschen(index) {
      angebote.splice(index, 1);
      speichern();
      anzeigen();
    }

    anzeigen();
  </script>
</body>
</html>
