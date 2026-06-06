<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Álvaro García M.</title>

  <style>
    body {
      font-family: -apple-system, BlinkMacSystemFont, sans-serif;
      max-width: 680px;
      margin: 70px auto;
      padding: 0 20px;
      line-height: 1.6;
      color: #111;
      background: #fff;
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
    }

    h1 {
      margin: 15px 0 5px;
      font-size: 28px;
    }

    p.bio {
      color: #444;
      font-size: 16px;
    }

    h2 {
      margin-top: 40px;
      font-size: 18px;
    }

    a {
      display: block;
      margin: 10px 0;
      color: #0a66c2;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .button {
      display: inline-block;
      margin-top: 15px;
      padding: 10px 14px;
      border: 1px solid #111;
      border-radius: 8px;
      cursor: pointer;
      font-size: 14px;
      background: transparent;
    }

    .button:hover {
      background: #111;
      color: white;
    }
  </style>
</head>

<body>

  <div class="profile">
    <img src="https://i.blogs.es/322f86/blob/288_288.jpeg" alt="Foto">
    <h1>Álvaro García</h1>
    <p class="bio">
      Periodista tecnológico. Escribo sobre Apple, Android y cultura digital en medios como Applesfera y Xataka.
    </p>
  </div>

  <h2>Mis trabajos</h2>

  <a href="https://www.applesfera.com/autor/alvaro-garcia">Applesfera</a>
  <a href="https://www.xataka.com/autor/alvaro-garcia">Xataka</a>
  <a href="https://www.xatakamovil.com/autor/alvaro-garcia">Xataka Móvil</a>
  <a href="https://www.xatakandroid.com/autor/alvaro-garcia">Xataka Android</a>

  <h2>Leer un artículo aleatorio</h2>

  <button class="button" onclick="randomArticle()">Abrir artículo random</button>

  <script>
    const articles = [
      "https://www.applesfera.com/autor/alvaro-garcia",
      "https://www.xataka.com/autor/alvaro-garcia"
    ];

    function randomArticle() {
      const url = articles[Math.floor(Math.random() * articles.length)];
      window.location.href = url;
    }
  </script>

</body>
</html>
