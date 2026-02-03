<!DOCTYPE html>  
<html lang="en">  
<head>  
  <meta charset="UTF-8" />  
  <title>MidwestChemo — Official Artist Site</title>  
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />  
  
  <link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">  
  
  <style>  
    :root {  
      --bg: #0f141a;  
      --fg: #eae7df;  
      --muted: #9ca3af;  
      --accent: #7da2c8;  
      --grain-opacity: 0.08;  
    }  
  
    * {  
      box-sizing: border-box;  
    }  
  
    body {  
      margin: 0;  
      background: linear-gradient(180deg, #0f141a, #141b24);  
      color: var(--fg);  
      font-family: "Inter", sans-serif;  
      min-height: 100vh;  
      overflow-x: hidden;  
    }  
  
    .grain {  
      pointer-events: none;  
      position: fixed;  
      inset: 0;  
      background-image: url("https://grainy-gradients.vercel.app/noise.svg");  
      opacity: var(--grain-opacity);  
      z-index: 100;  
    }  
  
    .container {  
      max-width: 900px;  
      margin: auto;  
      padding: 4rem 2rem;  
      display: flex;  
      flex-direction: column;  
      gap: 4rem;  
    }  
  
    .hero {  
      min-height: 70vh;  
      display: flex;  
      flex-direction: column;  
      justify-content: center;  
    }  
  
    .title {  
      font-family: "Space Mono", monospace;  
      font-size: clamp(3rem, 8vw, 6rem);  
      letter-spacing: 0.15em;  
      text-transform: uppercase;  
      position: relative;  
      color: var(--fg);  
    }  
  
    .title::after {  
      content: "MIDWESTCHEMO";  
      position: absolute;  
      left: 3px;  
      top: 3px;  
      color: var(--accent);  
      opacity: 0.4;  
      z-index: -1;  
    }  
  
    .tagline {  
      margin-top: 1.5rem;  
      color: var(--muted);  
      max-width: 500px;  
      line-height: 1.6;  
    }  
  
    .divider {  
      width: 100%;  
      height: 1px;  
      background: linear-gradient(to right, transparent, var(--accent), transparent);  
      opacity: 0.5;  
    }  
  
    .section {  
      display: flex;  
      flex-direction: column;  
      gap: 1rem;  
    }  
  
    .section h2 {  
      font-family: "Space Mono", monospace;  
      letter-spacing: 0.1em;  
      font-size: 1rem;  
      color: var(--accent);  
      text-transform: uppercase;  
    }  
  
    .bio {  
      max-width: 600px;  
      line-height: 1.8;  
      color: var(--fg);  
    }  
  
    .links {  
      display: flex;  
      flex-wrap: wrap;  
      gap: 1.5rem;  
    }  
  
    .links a {  
      text-decoration: none;  
      color: var(--fg);  
      border: 1px solid rgba(255,255,255,0.2);  
      padding: 0.75rem 1.5rem;  
      border-radius: 4px;  
      transition: all 0.2s ease;  
      font-size: 0.9rem;  
      letter-spacing: 0.1em;  
    }  
  
    .links a:hover {  
      border-color: var(--accent);  
      color: var(--accent);  
      transform: translateY(-2px);  
    }  
  
    .footer {  
      margin-top: 4rem;  
      font-size: 0.75rem;  
      color: var(--muted);  
      letter-spacing: 0.15em;  
      text-transform: uppercase;  
      opacity: 0.7;  
    }  
  
    .vhs {  
      animation: drift 6s ease-in-out infinite;  
    }  
  
    @keyframes drift {  
      0% { transform: translateX(0px); }  
      50% { transform: translateX(2px); }  
      100% { transform: translateX(0px); }  
    }  
  </style>  
</head>  
<body>  
  
  <div class="grain"></div>  
  
  <main class="container">  
    <section class="hero">  
      <h1 class="title vhs">MidwestChemo</h1>  
      <p class="tagline">  
        Soft distortion. Quiet rooms. Long drives home.  
        <br>  
        Midwest emo from the in-between.  
      </p>  
    </section>  
  
    <div class="divider"></div>  
  
    <section class="section">  
      <h2>About</h2>  
      <p class="bio">  
        MidwestChemo is a lo-fi Midwest emo project built on grainy guitars,  
        quiet breakdowns, and the feeling of staring out a basement window  
        while the world keeps moving without you.  
        <br><br>  
        Inspired by American Football, Free Throw, and Camping in Alaska —  
        this space exists to document what hurts, what heals, and what  
        lingers in between.  
      </p>  
    </section>  
  
    <section class="section">  
      <h2>Listen / Follow</h2>  
      <div class="links">  
        <a href="#" target="_blank">Spotify</a>  
        <a href="#" target="_blank">Apple Music</a>  
        <a href="#" target="_blank">YouTube</a>  
        <a href="#" target="_blank">Instagram</a>  
      </div>  
    </section>  
  
    <footer class="footer">  
      Official Artist Website — MidwestChemo © 2026  
    </footer>  
  </main>  
  
</body>  
</html>  
