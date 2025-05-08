<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Untuk Kamu yang Aku Sayang</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: #fbe9e7;
      color: #4e342e;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
      text-align: center;
      padding: 20px;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2em;
      max-width: 600px;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #ffab91;
      border: none;
      border-radius: 10px;
      font-size: 1em;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Sayangku Cintaku, Maafkan Aku...</h1>
  <p id="message">Aku tahu mungkin aku membuatmu kecewa, tapi percayalah, hatiku tak pernah ingin menyakitimu. Aku hanya manusia biasa yang sedang belajar menjadi lebih baik untukmu. Jangan marah terus ya, senyummu adalah hal yang paling aku rindukan setiap hari.</p>
  <button onclick="nextMessage()">Coba kamu pencet cantik</button>

  <script>
    const messages = [
      "Maafin akuu yahh Cantik,maaf kalo akuu suka bikin kamu ngambek,badmood.",
      "Aku ingin bersamamu, memperbaiki semuanya, dan membuat kenangan indah bersama.",
      "Marahmu melukai hatiku, tapi aku mengerti... karena kamu peduli.",
      "Aku rela menunggu, memperbaiki diri, asalkan kamu tetap di sisiku.",
      "Jangan biarkan marah sesaat menghapus cinta yang kita bangun perlahan.",
      "Kamu adalah anugerah terindah dalam hidupku. Jangan pergi, ya?",
      "Aku mencintaimu bukan karena siapa kamu, tapi karena siapa aku ketika bersamamu."
    ];

    let index = 0;
    function nextMessage() {
      if (index < messages.length) {
        document.getElementById("message").innerText = messages[index];
        index++;
      } else {
        document.getElementById("message").innerText = "Terima kasih sudah membaca sampai akhir. Aku sayang kamu, selalu.";
      }
    }
  </script>
</body>
</html>
