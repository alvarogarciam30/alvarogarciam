<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Alvaro García</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 700px;
      margin: 60px auto;
      line-height: 1.6;
      padding: 0 20px;
      color: #111;
    }

    img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
    }

    h1 {
      margin-top: 20px;
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
  </style>
</head>

<body>

  <img src="TU_FOTO_AQUI" alt="Foto">
  
  <h1>Alvaro García</h1>

  <p>
    Periodista tecnológico especializado en Apple, software y cultura digital. Escribo sobre tecnología en distintos medios.
  </p>

  <h2>Artículos</h2>

  <a href="https://ejemplo.com">Artículo 1</a>
  <a href="https://ejemplo.com">Artículo 2</a>
  <a href="https://ejemplo.com">Artículo 3</a>

  <h2>Random</h2>

  <a href="#" onclick="window.location.href=randomArticle()">Leer artículo aleatorio</a>

  <script>
    const articles = [
      "https://ejemplo.com",
      "https://ejemplo.com",
      "https://ejemplo.com"
    ];

    function randomArticle() {
      return articles[Math.floor(Math.random() * articles.length)];
    }
  </script>

</body>
</html>
