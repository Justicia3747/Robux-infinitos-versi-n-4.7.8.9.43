<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>¡Caiste!</title>
  <style>
    body {
      background-color: #000;
      color: #fff;
      text-align: center;
      font-family: sans-serif;
      padding-top: 50px;
    }
    img {
      width: 300px;
      margin-top: 20px;
    }
    h1 {
      font-size: 3em;
      color: #ff4444;
    }
  </style>
</head>
<body>
  <h1>¡Caiste!</h1>
  <img src="https://media.tenor.com/UnFx-k_lSckAAAAC/kitty-cat.gif" alt="Gato riendo" id="cat">

  <!-- Sonido de risa (puedes cambiar el enlace si tienes otro audio) -->
  <audio id="laugh" autoplay loop>
    <source src="https://www.myinstants.com/media/sounds/trollolololololol.mp3" type="audio/mpeg">
    Tu navegador no soporta audio.
  </audio>

  <script>
    const voz = new SpeechSynthesisUtterance("¡Pendejo!");
    voz.lang = "es-MX"; // Español mexicano

    setInterval(() => {
      speechSynthesis.speak(voz);
      alert("¡Pendejo!");
    }, 3000);
  </script>
</body>
</html>
