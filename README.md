<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Birthday Trap Night</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      font-family: Arial;
      background: black;
      color: white;
    }

    .banner {
      background: url('SEU-FLYER-AQUI.jpg') center/cover no-repeat;
      height: 300px;
    }

    .container {
      max-width: 500px;
      margin: -60px auto 20px;
      background: #111;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 0 20px rgba(255,0,0,0.3);
    }

    h1 {
      text-align: center;
      color: #ff0033;
    }

    .info {
      margin: 15px 0;
      line-height: 1.6;
    }

    .highlight {
      color: #ff0033;
      font-weight: bold;
    }

    input {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border-radius: 8px;
      border: none;
    }

    button {
      width: 100%;
      padding: 15px;
      background: #ff0033;
      color: white;
      border: none;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #cc0029;
    }

    .footer {
      text-align: center;
      font-size: 14px;
      opacity: 0.7;
      margin-top: 20px;
    }
  </style>
</head>

<body>

  <!-- COLOQUE SUA IMAGEM AQUI -->
  <div class="banner"></div>

  <div class="container">

    <h1>🔥 Birthday Trap Night</h1>

    <div class="info">
      <p>📅 <span class="highlight">02 de Maio</span></p>
      <p>📍 <span class="highlight">Soma Galeria</span></p>
      <p>💸 <span class="highlight">R$ 25,00</span></p>
    </div>

    <div class="info">
      🎤 Artistas locais de trap<br>
      🎭 Festa fantasia / terror<br>
      🔊 Trap + Funk liberado
    </div>

    <h2>🎟 Garantir ingresso</h2>

    <input type="text" id="nome" placeholder="Seu nome">
    <input type="tel" id="whatsapp" placeholder="Seu WhatsApp">

    <button onclick="comprar()">Comprar agora</button>

    <div class="footer">
      Evento exclusivo • Vagas limitadas
    </div>

  </div>

  <script>
    function comprar() {
      let nome = document.getElementById("nome").value;
      let zap = document.getElementById("whatsapp").value;

      if(nome === "" || zap === "") {
        alert("Preencha tudo!");
        return;
      }

      let mensagem = `🔥 Birthday Trap Night 🔥
Quero meu ingresso!

Nome: ${nome}
WhatsApp: ${zap}`;

      let numero = "5541995448318";

      let link = `https://wa.me/${numero}?text=${encodeURIComponent(mensagem)}`;

      window.location.href = link;
    }
  </script>

</body>
</html>
