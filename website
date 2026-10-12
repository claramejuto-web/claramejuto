<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Clara Mejuto | Música en Spotify</title>

  <style>
    /* =========================
       Paleta pastel (verano/otoño)
       ========================= */
    :root{
      --bg0: #fbf3ef;     /* crema cálida */
      --bg1: #f3f7ff;     /* nube fría */
      --card: rgba(255,255,255,.62);
      --card2: rgba(255,255,255,.48);
      --text: #1f2430;   /* tinta suave */
      --muted: rgba(31,36,48,.70);

      --border: rgba(31,36,48,.12);
      --shadow: 0 22px 70px rgba(31,36,48,.12);

      --peach: #ffb4a2;
      --lav: #cbb7ff;
      --mint: #9fe8dd;
      --sand: #f3d2b3;

      --radius: 18px;
      --radius2: 26px;
      --focus: 0 0 0 4px rgba(203,183,255,.35);

      --serif: ui-serif, "Iowan Old Style", "Palatino Linotype", Palatino, "Book Antiqua", Georgia, serif;
      --sans: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Apple Color Emoji","Segoe UI Emoji";
    }

    *{ box-sizing: border-box; }
    html, body{ height: 100%; }

    body{
      margin: 0;
      font-family: var(--sans);
      color: var(--text);
      background:
        radial-gradient(900px 420px at 15% 0%, rgba(255,180,162,.35), transparent 60%),
        radial-gradient(720px 380px at 90% 10%, rgba(203,183,255,.32), transparent 55%),
        radial-gradient(900px 520px at 50% 110%, rgba(159,232,221,.30), transparent 60%),
        linear-gradient(180deg, var(--bg0), var(--bg1));
    }

    a{ color: inherit; text-decoration: none; }
    a:focus-visible, button:focus-visible{
      outline: none;
      box-shadow: var(--focus);
      border-radius: 14px;
    }

    .wrap{
      max-width: 1040px;
      margin: 0 auto;
      padding: 24px 16px 54px;
    }

    /* =========================
       Header
       ========================= */
    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap: 14px;
      padding: 6px 0 18px;
      flex-wrap: wrap;
    }

    .brand{
      display:flex; align-items:center; gap: 12px;
      min-width: 240px;
    }

    .monogram{
      width: 44px; height: 44px;
      border-radius: 16px;
      border: 1px solid var(--border);
      background:
        linear-gradient(135deg, rgba(255,180,162,.45), rgba(203,183,255,.35)),
        rgba(255,255,255,.55);
      display:flex; align-items:center; justify-content:center;
      font-weight: 900;
      letter-spacing: .3px;
    }

    .brand h1{
      margin:0;
      font-family: var(--serif);
      font-size: 1.08rem;
      letter-spacing: -0.01em;
    }
    .brand p{
      margin: 2px 0 0;
      color: var(--muted);
      font-size: .95rem;
    }

    nav{
      display:flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content:flex-end;
    }

    .pill{
      border: 1px solid var(--border);
      background: rgba(255,255,255,.55);
      padding: 10px 12px;
      border-radius: 999px;
      font-weight: 750;
      font-size: .95rem;
      color: rgba(31,36,48,.92);
      transition: transform .18s ease, background .18s ease, border-color .18s ease;
      display:inline-flex; align-items:center; gap: 8px;
      user-select: none;
      backdrop-filter: blur(6px);
    }
    .pill:hover{
      transform: translateY(-1px);
      border-color: rgba(31,36,48,.18);
      background: rgba(255,255,255,.72);
    }

    /* =========================
       Hero
       ========================= */
    .hero{
      display:grid;
      grid-template-columns: 1.15fr .85fr;
      gap: 16px;
      align-items: stretch;
      margin-top: 10px;
    }

    .card{
      border-radius: var(--radius2);
      border: 1px solid var(--border);
      background: linear-gradient(180deg, var(--card), var(--card2));
      box-shadow: var(--shadow);
      overflow: hidden;
    }

    .hero-main{
      position: relative;
      padding: 22px 22px 18px;
      min-height: 240px;
      display:flex;
      flex-direction: column;
      justify-content: flex-end;
    }

    /* Foto (la tuya) como capa sutil */
    .hero-main::before{
      content:"";
      position:absolute;
      inset:0;
      background:
        linear-gradient(120deg, rgba(251,243,239,.70), rgba(243,247,255,.40)),
        radial-gradient(600px 260px at 18% 10%, rgba(255,180,162,.40), transparent 60%),
        radial-gradient(620px 260px at 88% 25%, rgba(203,183,255,.35), transparent 58%),
        radial-gradient(620px 260px at 50% 110%, rgba(159,232,221,.35), transparent 60%),
        url("tu_foto.jpg");
      background-size: cover;
      background-position: center;
      filter: saturate(1.05) contrast(.98);
      opacity: .95;
      transform: scale(1.02);
    }
    .hero-main > *{ position: relative; }

    .kicker{
      display:flex; flex-wrap: wrap; gap: 10px; align-items:center;
      margin-bottom: 10px;
    }

    .dot{
      width: 10px; height: 10px;
      border-radius: 999px;
      background: linear-gradient(135deg, var(--lav), var(--mint));
      box-shadow: 0 0 0 4px rgba(203,183,255,.25);
    }

    .kicker span{
      font-weight: 780;
      color: rgba(31,36,48,.72);
      font-size: .98rem;
    }

    .hero-main h2{
      margin: 0;
      font-family: var(--serif);
      font-size: clamp(1.5rem, 2.6vw, 2.25rem);
      letter-spacing: -0.02em;
      line-height: 1.12;
    }

    .hero-main p{
      margin: 10px 0 0;
      color: rgba(31,36,48,.78);
      font-size: 1.05rem;
      max-width: 62ch;
    }

    .hero-side{
      padding: 18px;
      display:flex;
      flex-direction: column;
      gap: 12px;
    }

    .side-title{
      display:flex; justify-content:space-between; align-items:center; gap: 10px;
      margin-bottom: 2px;
    }

    .side-title strong{
      font-family: var(--serif);
      font-size: 1.08rem;
      letter-spacing: -0.01em;
    }

    .tag{
      border: 1px solid var(--border);
      background: rgba(255,255,255,.55);
      border-radius: 999px;
      padding: 8px 10px;
      font-weight: 820;
      font-size: .92rem;
      color: rgba(31,36,48,.88);
      white-space: nowrap;
    }

    .socials{
      display:flex; flex-direction:column; gap: 10px;
      margin-top: 4px;
    }

    .social-row{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap: 12px;
      border: 1px solid var(--border);
      background: rgba(255,255,255,.48);
      border-radius: 18px;
      padding: 12px 12px;
      transition: transform .18s ease, background .18s ease, border-color .18s ease;
      backdrop-filter: blur(6px);
    }
    .social-row:hover{
      transform: translateY(-1px);
      background: rgba(255,255,255,.68);
      border-color: rgba(31,36,48,.18);
    }

    .left{
      display:flex; align-items:center; gap: 10px;
      min-width: 180px;
    }

    .icon{
      width: 36px; height: 36px;
      border-radius: 14px;
      display:flex; align-items:center; justify-content:center;
      border: 1px solid var(--border);
      background: rgba(255,255,255,.55);
      flex: 0 0 auto;
    }

    .handle strong{
      display:block;
      font-size: .98rem;
      font-weight: 900;
      letter-spacing: -0.01em;
    }
    .handle span{
      display:block;
      color: var(--muted);
      font-size: .92rem;
      margin-top: 2px;
    }

    .arrow{
      font-weight: 900;
      color: rgba(31,36,48,.66);
      padding-left: 6px;
    }

    /* =========================
       Singles
       ========================= */
    .section{
      margin-top: 18px;
    }

    .section-head{
      display:flex;
      align-items: flex-end;
      justify-content: space-between;
      gap: 12px;
      margin: 18px 2px 12px;
      flex-wrap: wrap;
    }

    .section-head h3{
      margin:0;
      font-family: var(--serif);
      font-size: 1.45rem;
      letter-spacing: -0.02em;
    }

    .section-head p{
      margin:0;
      color: var(--muted);
      font-size: .98rem;
    }

    .grid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }

    .single{
      padding: 14px;
      border-radius: var(--radius);
      border: 1px solid var(--border);
      background: rgba(255,255,255,.45);
      transition: transform .18s ease, background .18s ease, border-color .18s ease;
      display:flex;
      flex-direction: column;
      gap: 10px;
      min-height: 185px;
      backdrop-filter: blur(6px);
    }

    .single:hover{
      transform: translateY(-2px);
      background: rgba(255,255,255,.65);
      border-color: rgba(31,36,48,.18);
    }

    .single .title{
      font-weight: 950;
      letter-spacing: -0.01em;
      font-size: 1.06rem;
    }

    .single .sub{
      color: var(--muted);
      font-size: .95rem;
      margin-top: -6px;
    }

    .spacer{ flex: 1; }

    .cta{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap: 9px;
      border-radius: 16px;
      padding: 11px 12px;
      border: 1px solid rgba(31,36,48,.14);
      background:
        linear-gradient(135deg, rgba(255,180,162,.35), rgba(203,183,255,.26), rgba(159,232,221,.22));
      font-weight: 920;
      transition: transform .18s ease, background .18s ease, border-color .18s ease;
    }
    .cta:hover{
      transform: translateY(-1px);
      border-color: rgba(31,36,48,.20);
      background:
        linear-gradient(135deg, rgba(255,180,162,.45), rgba(203,183,255,.32), rgba(159,232,221,.26));
    }

    /* =========================
       Bio + Contacto
       ========================= */
    .bio{
      margin-top: 18px;
      padding: 20px;
    }

    .bio h3{
      margin:0 0 10px;
      font-family: var(--serif);
      font-size: 1.45rem;
      letter-spacing: -0.02em;
    }

    blockquote{
      margin: 0;
      font-size: 1.06rem;
      color: rgba(31,36,48,.86);
      font-family: var(--serif);
    }

    blockquote p{ margin: 0 0 12px; line-height: 1.6; }

    blockquote footer{
      color: var(--muted);
      font-size: .97rem;
      margin-top: 12px;
      font-family: var(--sans);
      font-weight: 700;
    }

    .contact{
      margin-top: 12px;
      display:flex;
      gap: 10px;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .contact .mail{
      display:flex; gap: 10px; align-items:center;
      border: 1px solid var(--border);
      background: rgba(255,255,255,.5);
      border-radius: 18px;
      padding: 12px 14px;
      backdrop-filter: blur(6px);
      font-weight: 850;
    }

    .mail a{
      font-weight: 950;
      text-decoration: underline;
      text-decoration-thickness: 2px;
      text-decoration-color: rgba(203,183,255,.7);
      text-underline-offset: 4px;
    }

    footer{
      margin-top: 22px;
      color: var(--muted);
      font-size: .95rem;
      display:flex;
      justify-content:space-between;
      gap: 12px;
      flex-wrap: wrap;
      padding-top: 14px;
      border-top: 1px solid rgba(31,36,48,.10);
    }

    /* =========================
       Responsive
       ========================= */
    @media (max-width: 920px){
      .hero{ grid-template-columns: 1fr; }
      .grid{ grid-template-columns: 1fr; }
    }

    @media (max-width: 520px){
      .hero-main{ min-height: 260px; }
      .grid{ gap: 10px; }
      .single{ min-height: 170px; }
    }
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <a class="brand" href="#inicio" aria-label="Ir al inicio">
        <div class="monogram">CM</div>
        <div>
          <h1>Clara Mejuto</h1>
          <p>Singles en Spotify • Insta & TikTok</p>
        </div>
      </a>

      <nav aria-label="Enlaces">
        <a class="pill" href="https://open.spotify.com/" target="_blank" rel="noreferrer noopener">🎧 Spotify</a>
        <a class="pill" href="https://www.instagram.com/claramejutomsc/" target="_blank" rel="noreferrer noopener">📸 Instagram</a>
        <a class="pill" href="https://www.tiktok.com/@claramejuto" target="_blank" rel="noreferrer noopener">🎵 TikTok</a>
        <a class="pill" href="mailto:claramejuto@icloud.com">✉️ Contacto</a>
      </nav>
    </header>

    <section id="inicio" class="hero" aria-label="Portada">
      <div class="card hero-main">
        <div class="kicker">
          <div class="dot" aria-hidden="true"></div>
          <span>Pastel • poético • para escuchar bajito</span>
        </div>
        <h2>“cerca de mi piel”, “enemigos” y “solo una vez más”</h2>
        <p>
          Tres singles para conectar con lo que late: intimidad, tensión y esa luz que vuelve.
          Dale play y quédate.
        </p>
      </div>

      <aside class="card hero-side" aria-label="Redes y contacto">
        <div class="side-title">
          <strong>Encuéntrame</strong>
          <span class="tag">✨ @claramejuto</span>
        </div>

        <div class="socials">
          <a class="social-row" href="https://www.instagram.com/claramejutomsc/" target="_blank" rel="noreferrer noopener">
            <div class="left">
              <div class="icon" aria-hidden="true">📸</div>
              <div class="handle">
                <strong>Instagram</strong>
                <span>@claramejutomsc</span>
              </div>
            </div>
            <div class="arrow" aria-hidden="true">→</div>
          </a>

          <a class="social-row" href="https://www.tiktok.com/@claramejuto" target="_blank" rel="noreferrer noopener">
            <div class="left">
              <div class="icon" aria-hidden="true">🎵</div>
              <div class="handle">
                <strong>TikTok</strong>
                <span>@claramejuto</span>
              </div>
            </div>
            <div class="arrow" aria-hidden="true">→</div>
          </a>

          <div class="social-row" role="group" aria-label="Correo de contacto" style="cursor: default;">
            <div class="left">
              <div class="icon" aria-hidden="true">✉️</div>
              <div class="handle">
                <strong>Correo</strong>
                <span>claramejuto@icloud.com</span>
              </div>
            </div>
            <div class="arrow" aria-hidden="true">↗</div>
          </div>
        </div>
      </aside>
    </section>

    <section class="section" id="singles" aria-label="Singles">
      <div class="section-head">
        <h3>Singles</h3>
        <p>Escucha directa en Spotify ▶️</p>
      </div>

      <div class="grid">
        <article class="single">
          <div>
            <div class="title">enemigos</div>
            <div class="sub">Single • Spotify</div>
          </div>
          <div class="spacer"></div>
          <a class="cta" href="https://open.spotify.com/intl-es/track/46xW1mMopiyJzQGX3Qf6s7?si=7ed4e97de1a34a1f" target="_blank" rel="noreferrer noopener">
            🎧 Abrir en Spotify
          </a>
        </article>

        <article class="single">
          <div>
            <div class="title">cerca de mi piel</div>
            <div class="sub">Single • Spotify</div>
          </div>
          <div class="spacer"></div>
          <a class="cta" href="https://open.spotify.com/intl-es/track/1hQjW1pCk0JvOxqUjGNJLT?si=9372267734a54d4d" target="_blank" rel="noreferrer noopener">
            🎧 Abrir en Spotify
          </a>
        </article>

        <article class="single">
          <div>
            <div class="title">solo una vez más</div>
            <div class="sub">Single • Spotify</div>
          </div>
          <div class="spacer"></div>
          <a class="cta" href="https://open.spotify.com/intl-es/track/7e379zpw2ENlUWH2fRqgW6?si=b948c2197e494b9c" target="_blank" rel="noreferrer noopener">
            🎧 Abrir en Spotify
          </a>
        </article>
      </div>
    </section>

    <section class="card bio" aria-label="Biografía">
      <h3>Biografía</h3>
      <blockquote>
        <p>“We don’t read and write poetry because it’s cute. We read and write poetry because we are members of the human race.”</p>
        <p>“And the human race is filled with passion. Medicine, law, business, engineering — these are noble pursuits and necessary to sustain life. But poetry, beauty, romance, love — these are what we stay alive for.”</p>
        <footer>— John Keating (Robin Williams) from <em>death poets society</em></footer>
      </blockquote>

      <div class="contact" aria-label="Contacto">
        <div class="mail">
          <span aria-hidden="true">📩</span>
          <span>Escríbeme:</span>
          <a href="mailto:claramejuto@icloud.com">claramejuto@icloud.com</a>
        </div>

        <div style="color: var(--muted); font-weight: 750;">
          Disponible para colaboraciones y prensa ✨
        </div>
      </div>
    </section>

    <footer aria-label="Pie de página">
      <div>© <span id="year"></span> • Clara Mejuto</div>
      <div>Hecho para escuchar y sentir 💛</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

  <!--
    ✅ IMPORTANTE: Cambia "tu_foto.jpg" por el nombre real del archivo de la imagen subida.
    En tu caso, dime el nombre del archivo (por ejemplo: "IMG_1234.jpg") y te lo dejo perfecto.
  -->
</body>
</html>
