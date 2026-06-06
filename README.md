<style>
  :root {
    --bg: #ffffff;
    --text: #111;
    --muted: #444;
    --primary: #2b6fff;
    --accent: #ff3b3b;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --bg: #0f1115;
      --text: #f2f2f2;
      --muted: #b5b5b5;
    }
  }

  body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, sans-serif;
    color: var(--text);
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;

    background: radial-gradient(circle at top left, rgba(43,111,255,0.15), transparent 40%),
                radial-gradient(circle at bottom right, rgba(255,59,59,0.12), transparent 40%),
                var(--bg);

    transition: background 0.3s ease, color 0.3s ease;
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
    border: 3px solid var(--primary);
    box-shadow: 0 8px 20px rgba(0,0,0,0.15);
  }

  h1 {
    margin: 15px 0 5px;
    font-size: 30px;
    letter-spacing: -0.5px;
  }

  p.bio {
    color: var(--muted);
    font-size: 16px;
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
    background: linear-gradient(to right, var(--primary), var(--accent));
    margin-top: 6px;
    border-radius: 2px;
  }

  .links {
    margin-top: 20px;
  }

  /* HOVER CARDS */
  .links a {
    display: block;
    margin: 12px 0;
    padding: 12px 14px;
    border-radius: 10px;
    text-decoration: none;
    color: var(--primary);
    background: rgba(127,127,127,0.05);
    border: 1px solid rgba(127,127,127,0.15);
    transition: all 0.2s ease;
  }

  .links a:hover {
    transform: translateY(-2px);
    border-color: var(--accent);
    color: var(--accent);
    background: rgba(255,59,59,0.06);
  }
</style>
