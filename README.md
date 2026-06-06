<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Álvaro García M.</title>

  <style>
    :root {
      --bg: #ffffff;
      --text: #111;
      --muted: #555;
      --primary: #2b6fff;
      --accent: #ff3b3b;
      --card: rgba(0,0,0,0.04);
      --border: rgba(0,0,0,0.1);
    }

    @media (prefers-color-scheme: dark) {
      :root {
        --bg: #0f1115;
        --text: #f2f2f2;
        --muted: #b5b5b5;
        --card: rgba(255,255,255,0.06);
        --border: rgba(255,255,255,0.12);
      }
    }

    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, sans-serif;
      background: radial-gradient(circle at top left, rgba(43,111,255,0.15), transparent 40%),
                  radial-gradient(circle at bottom right, rgba(255,59,59,0.12), transparent 40%),
                  var(--bg);
      color: var(--text);
      display: flex;
      justify-content: center;
    }

    .container {
      max-width: 720px;
      width: 100%;
      padding: 60px 20px;
    }

    .profile {
      text-align: center;
      margin-bottom: 40px;
    }

    .profile img {
      width: 110px;
      height: 110px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid var(--primary);
    }

    h1 {
      margin: 15px 0 5px;
      font-size: 30px;
    }

    p {
      color: var(--muted);
      max-width: 520px;
      margin: 0 auto;
    }

    h2 {
      margin-top: 40px;
      font-size: 18px;
    }

    h2::after {
      content: "";
      display: block;
      width: 40px;
      height: 3px;
      margin-top: 6px;
      background: linear-gradient(to right, var(--primary), var(--accent));
      border-radius: 2px;
    }

    /* CARDS */
    .grid {
      display: grid;
      gap: 12px;
      margin-top: 20px;
    }

    .card {
      display: flex;
      align-items: center;
      gap: 14px;
      padding: 16px;
      border-radius: 16px;
      text-decoration: none;
      background: var(--card);
      border: 1px solid var(--border);
      transition: all 0.25s ease;
    }

    .card img {
      width: 48px;
      height: 48px;
      border-radius: 12px;
      object-fit: cover;
    }

    .card strong {
      display: block;
      font-size: 15px;
      color: var(--text);
    }

    .card span {
      display: block;
      font-size: 13px;
      color: var(--muted);
      margin-top: 2px;
    }

    .card div {
      display: flex;
      flex-direction: column;
    }

    .card:hover {
      transform: translateY(-4px);
      border-color: var(--accent);
      box-shadow: 0 10px 30px rgba(0,0,0,0.15);
    }

    /* MOBILE */
    @media (max-width: 600px) {
      h1 {
        font-size: 26px;
      }

      .container {
        padding: 40px 16px;
      }
    }

  </style>
</head>

<body>

  <div class="container">

    <div class="profile">
      <img src="https://i.blogs.es/322f86/blob/288_288.jpeg" alt="Foto">
      <h1>Álvaro García M.</h1>
      <p>Periodista tecnológico especializado en Apple, Android y cultura digital.</p>
    </div>

    <h2>Mis trabajos</h2>

    <div class="grid">

      <a class="card" href="https://www.applesfera.com/autor/alvaro-garcia">
        <img src="https://yt3.googleusercontent.com/AchftUgiT2t0fzQtg091oMaLSUv0PHweWArc8qvI5CD5-EyIMFkWrs5V969b9Wf5cr6gPsFtug=s900-c-k-c0x00ffffff-no-rj">
        <div>
          <strong>Applesfera</strong>
          <span>Artículos sobre Apple y ecosistema</span>
        </div>
      </a>

      <a class="card" href="https://www.xataka.com/autor/alvaro-garcia">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTGUuJ47JpfkIJcMmSD85KKMkIGSVjz3xO2jw&s">
        <div>
          <strong>Xataka</strong>
          <span>Tecnología, análisis y actualidad</span>
        </div>
      </a>

      <a class="card" href="https://www.xatakamovil.com/autor/alvaro-garcia">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSlIQhgviqLt-EXM7LHVnNRc8OjkdJUhA8ceA&s">
        <div>
          <strong>Xataka Móvil</strong>
          <span>Smartphones y movilidad</span>
        </div>
      </a>

      <a class="card" href="https://www.xatakandroid.com/autor/alvaro-garcia">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTqoMNSiupnhdY1NZjORyh2jCctivdCoEI-7w&s">
        <div>
          <strong>Xataka Android</strong>
          <span>Android, apps y ecosistema Google</span>
        </div>
      </a>

    </div>

  </div>

</body>
</html>
