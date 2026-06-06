<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Álvaro García M.</title>

  <style>
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, sans-serif;
      color: #111;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;

      /* Fondo suave con toque azul/rojo */
      background: radial-gradient(circle at top left, #e8f0ff, transparent 40%),
                  radial-gradient(circle at bottom right, #ffe8e8, transparent 40%),
                  #ffffff;
    }

    .container {
      max-width: 680px;
      padding: 60px 20px;
      animation: fadeUp 0.8s ease-out;
    }

    @keyframes fadeUp {
      from {
        opacity: 0;
        transform: translateY(15px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .profile {
      text-align: center;
      margin-bottom: 40px;
    }

    img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #2b6fff; /* azul */
      box-shadow: 0 8px 20px rgba(0,0,0,0.08);
    }

    h1 {
      margin: 15px 0 5px;
      font-size: 30px;
      letter-spacing: -0.5px;
    }

    p.bio {
      color: #444;
      font-size: 16px;
      max-width: 520px;
      margin: 0 auto;
    }

    h2 {
      margin-top: 40px;
      font-size: 18px;
      position: relative;
    }

    h2::after {
      content: "";
      display: block;
      width: 40px;
      height: 3px;
      background: linear-gradient(to right, #2b6fff, #ff3b3b);
      margin-top: 6px;
      border-radius: 2px;
    }

    a {
      display: block;
      margin: 12px 0;
      color: #2b6fff;
      text-decoration: none;
      transition: color 0.2s ease;
    }

    a:hover {
      color: #ff3b3b;
    }

    .links {
      margin-top: 20px;
    }

    /* Animación escalonada suave */
    .links a {
      opacity: 0;
      animation: linkFade 0.6s ease forwards;
    }

    .links a:nth-child(1) { animation-delay: 0.2s; }
    .links a:nth-child(2) { animation-delay: 0.3s; }
    .links a:nth-child(3) { animation-delay: 0.4s; }
    .links a:nth-child(4) { animation-delay: 0.5s; }

    @keyframes linkFade {
      from {
        opacity: 0;
        transform: translateY(8px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

  </style>
</head>

<body>

  <div class="container">

    <div class="profile">
      <img src="https://i.blogs.es/322f86/blob/288_288.jpeg" alt="Foto">
      <h1>Álvaro García M.</h1>
      <p class="bio">
        Periodista tecnológico. Escribo sobre Apple, Android y cultura digital en medios como Applesfera y Xataka.
      </p>
    </div>

    <h2>Mis trabajos</h2>

    <div class="links">
      <a href="https://www.applesfera.com/autor/alvaro-garcia">Applesfera</a>
      <a href="https://www.xataka.com/autor/alvaro-garcia">Xataka</a>
      <a href="https://www.xatakamovil.com/autor/alvaro-garcia">Xataka Móvil</a>
      <a href="https://www.xatakandroid.com/autor/alvaro-garcia">Xataka Android</a>
    </div>

  </div>

</body>
</html>
