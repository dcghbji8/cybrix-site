# cybrix
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cybrix — Продвижение и Рейтинг</title>
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
  <script src="https://unpkg.com/scrollreveal"></script>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #000;
      color: #0f0;
      scroll-behavior: smooth;
      overflow-x: hidden;
      position: relative;
    }
    #particles-js {
      position: fixed;
      width: 100%;
      height: 100%;
      z-index: -1;
    }
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: radial-gradient(circle, rgba(0,255,0,0.2) 1px, transparent 1px);
      background-size: 40px 40px;
      z-index: -2;
    }
    header {
      background-color: #050505;
      padding: 60px 20px 40px;
      text-align: center;
      border-bottom: 1px solid #0f0;
    }
    header h1 {
      font-size: 2.5em;
      font-family: 'Press Start 2P', cursive;
      color: #0f0;
      animation: glow 2s ease-in-out infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 5px #0f0; }
      to { text-shadow: 0 0 20px #0f0, 0 0 30px #0f0; }
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    h2 {
      font-size: 1.8em;
      border-left: 4px solid #0f0;
      padding-left: 10px;
      margin-bottom: 20px;
    }
    .card, .tariff-card, .review, .contact {
      background: #111;
      border: 1px solid #0f0;
      border-radius: 12px;
      padding: 20px;
      margin: 20px 0;
      box-shadow: 0 0 15px #0f0;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover, .tariff-card:hover {
      transform: scale(1.02);
      box-shadow: 0 0 25px #0f0;
    }
    .tariff-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .review {
      font-style: italic;
      border-left: 3px solid #0f0;
      padding-left: 10px;
    }
    .contact input,
    .contact textarea {
      width: 100%;
      margin: 10px 0;
      padding: 10px;
      background: #000;
      border: 1px solid #0f0;
      color: #0f0;
    }
    .contact button {
      background: #0f0;
      color: #000;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      font-weight: bold;
      transition: transform 0.3s;
    }
    .contact button:hover {
      transform: scale(1.05);
    }
    .btn-scroll, .btn-telegram {
      position: fixed;
      right: 20px;
      background: #0f0;
      color: #000;
      padding: 10px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      box-shadow: 0 0 10px #0f0;
      z-index: 100;
    }
    .btn-scroll { bottom: 80px; }
    .btn-telegram { bottom: 20px; }
    footer {
      text-align: center;
      padding: 30px 20px;
      background: #000;
      border-top: 1px solid #0f0;
    }
    .footer-content {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
    }
    .footer-logo {
      height: 50px;
      animation: neon-glow 2s infinite alternate;
    }
    .planet-icon {
      font-size: 32px;
      animation: rotate 10s linear infinite;
      filter: drop-shadow(0 0 5px #00ff00);
    }
    @keyframes rotate {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    @keyframes neon-glow {
      from { filter: drop-shadow(0 0 5px #00ff00); }
      to { filter: drop-shadow(0 0 20px #00ff00); }
    }
    .credits {
      text-align: center;
      font-size: 0.8em;
      margin-top: 20px;
      color: #0f0;
      opacity: 0.6;
    }
    .credits a {
      color: #0f0;
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div id="particles-js"></div>
  <header>
    <h1>Cybrix</h1>
    <p>ПРОДВИЖЕНИЕ, ОТЗЫВЫ, РЕЙТИНГИ</p>
  </header>

  <section id="about">
    <h2>О нас</h2>
    <div class="card">
      <p>Мы — команда Cybrix, эксперты в области цифрового продвижения. Наша миссия — сделать ваш бизнес заметным через отзывы, рейтинги и профессиональный подход.</p>
    </div>
  </section>

  <section id="services">
    <h2>Услуги</h2>
    <div class="tariff-grid">
      <div class="tariff-card">
        <h3>Отзывы</h3>
        <p>Создание и размещение позитивных отзывов о вашем бизнесе.</p>
      </div>
      <div class="tariff-card">
        <h3>Рейтинг</h3>
        <p>Повышение рейтингов в каталогах и на популярных площадках.</p>
      </div>
      <div class="tariff-card">
        <h3>Комплексное продвижение</h3>
        <p>Индивидуальные стратегии для увеличения вашей онлайн-репутации.</p>
      </div>
    </div>
  </section>

  <section id="faq">
    <h2>Часто задаваемые вопросы</h2>
    <div class="card">
      <h3>Как быстро появляются отзывы?</h3>
      <p>Обычно в течение 24–48 часов после оформления заказа.</p>
    </div>
    <div class="card">
      <h3>Безопасно ли это?</h3>
      <p>Да, мы соблюдаем все правила платформ и используем проверенные методы.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Связаться с нами</h2>
    <div class="card contact">
      <input type="text" id="name" placeholder="Ваше имя">
      <input type="email" id="email" placeholder="Ваш email">
      <textarea id="message" rows="5" placeholder="Ваше сообщение..."></textarea>
      <button onclick="submitForm()">Отправить</button>
      <p id="status"></p>
    </div>
  </section>

  <footer>
    <div class="footer-content">
      <img src="cybrix-logo.png" alt="Cybrix" class="footer-logo">
      <p>© 2025 Cybrix — Продвижение, отзывы, рейтинг. Мы делаем ваш бизнес заметным!</p>
      <div class="planet-icon">🪐</div>
      <div class="credits">
        Разработка дизайна — <a href="https://t.me/Cybrix7" target="_blank">@Cybrix7</a>
      </div>
    </div>
  </footer>

  <button class="btn-scroll" onclick="document.getElementById('contact').scrollIntoView({ behavior: 'smooth' })">Связаться</button>
  <a href="https://t.me/Cybrix7" target="_blank"><button class="btn-telegram">Telegram</button></a>

  <script>
    particlesJS("particles-js", {
      particles: {
        number: { value: 80 },
        color: { value: "#00ff00" },
        shape: { type: "star" },
        opacity: { value: 0.5 },
        size: { value: 3 },
        line_linked: {
          enable: true,
          distance: 150,
          color: "#00ff00",
          opacity: 0.4,
          width: 1
        },
        move: { enable: true, speed: 1 }
      },
      interactivity: {
        events: { onhover: { enable: true, mode: "repulse" } }
      },
      retina_detect: true
    });

    ScrollReveal().reveal('.card, .tariff-card, .review, .contact', {
      delay: 100,
      duration: 1000,
      reset: true,
      opacity: 0,
      scale: 0.9,
      distance: '20px'
    });

    function submitForm() {
      const name = document.getElementById("name").value.trim();
      const email = document.getElementById("email").value.trim();
      const message = document.getElementById("message").value.trim();
      const status = document.getElementById("status");

      if (!name || !email || !message) {
        status.innerText = "Пожалуйста, заполните все поля.";
        status.style.color = "red";
        return;
      }

      status.innerText = "Спасибо! Ваше сообщение отправлено.";
      status.style.color = "lime";

      document.getElementById("name").value = "";
      document.getElementById("email").value = "";
      document.getElementById("message").value = "";
    }
  </script>
</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cybrix — Продвижение и Рейтинг</title>
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js"></script>
  <script src="https://unpkg.com/scrollreveal"></script>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #000;
      color: #0f0;
      scroll-behavior: smooth;
      overflow-x: hidden;
      position: relative;
    }
    #particles-js {
      position: fixed;
      width: 100%;
      height: 100%;
      z-index: -1;
    }
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: radial-gradient(circle, rgba(0,255,0,0.2) 1px, transparent 1px);
      background-size: 40px 40px;
      z-index: -2;
    }
    header {
      background-color: #050505;
      padding: 60px 20px 40px;
      text-align: center;
      border-bottom: 1px solid #0f0;
    }
    header h1 {
      font-size: 2.5em;
      font-family: 'Press Start 2P', cursive;
      color: #0f0;
      animation: glow 2s ease-in-out infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 5px #0f0; }
      to { text-shadow: 0 0 20px #0f0, 0 0 30px #0f0; }
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    h2 {
      font-size: 1.8em;
      border-left: 4px solid #0f0;
      padding-left: 10px;
      margin-bottom: 20px;
    }
    .card, .tariff-card, .review, .contact {
      background: #111;
      border: 1px solid #0f0;
      border-radius: 12px;
      padding: 20px;
      margin: 20px 0;
      box-shadow: 0 0 15px #0f0;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover, .tariff-card:hover {
      transform: scale(1.02);
      box-shadow: 0 0 25px #0f0;
    }
    .tariff-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .review {
      font-style: italic;
      border-left: 3px solid #0f0;
      padding-left: 10px;
    }
    .contact input,
    .contact textarea {
      width: 100%;
      margin: 10px 0;
      padding: 10px;
      background: #000;
      border: 1px solid #0f0;
      color: #0f0;
    }
    .contact button {
      background: #0f0;
      color: #000;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      font-weight: bold;
      transition: transform 0.3s;
    }
    .contact button:hover {
      transform: scale(1.05);
    }
    .btn-scroll, .btn-telegram {
      position: fixed;
      right: 20px;
      background: #0f0;
      color: #000;
      padding: 10px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      box-shadow: 0 0 10px #0f0;
      z-index: 100;
    }
    .btn-scroll { bottom: 80px; }
    .btn-telegram { bottom: 20px; }
    footer {
      text-align: center;
      padding: 30px 20px;
      background: #000;
      border-top: 1px solid #0f0;
    }
    .footer-content {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
    }
    .footer-logo {
      height: 50px;
      animation: neon-glow 2s infinite alternate;
    }
    .planet-icon {
      font-size: 32px;
      animation: rotate 10s linear infinite;
      filter: drop-shadow(0 0 5px #00ff00);
    }
    @keyframes rotate {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    @keyframes neon-glow {
      from { filter: drop-shadow(0 0 5px #00ff00); }
      to { filter: drop-shadow(0 0 20px #00ff00); }
    }
    .credits {
      text-align: center;
      font-size: 0.8em;
      margin-top: 20px;
      color: #0f0;
      opacity: 0.6;
    }
    .credits a {
      color: #0f0;
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div id="particles-js"></div>
  <header>
    <h1>Cybrix</h1>
    <p>ПРОДВИЖЕНИЕ, ОТЗЫВЫ, РЕЙТИНГИ</p>
  </header>

  <section id="about">
    <h2>О нас</h2>
    <div class="card">
      <p>Мы — команда Cybrix, эксперты в области цифрового продвижения. Наша миссия — сделать ваш бизнес заметным через отзывы, рейтинги и профессиональный подход.</p>
    </div>
  </section>

  <section id="services">
    <h2>Услуги</h2>
    <div class="tariff-grid">
      <div class="tariff-card">
        <h3>Отзывы</h3>
        <p>Создание и размещение позитивных отзывов о вашем бизнесе.</p>
      </div>
      <div class="tariff-card">
        <h3>Рейтинг</h3>
        <p>Повышение рейтингов в каталогах и на популярных площадках.</p>
      </div>
      <div class="tariff-card">
        <h3>Комплексное продвижение</h3>
        <p>Индивидуальные стратегии для увеличения вашей онлайн-репутации.</p>
      </div>
    </div>
  </section>

  <section id="faq">
    <h2>Часто задаваемые вопросы</h2>
    <div class="card">
      <h3>Как быстро появляются отзывы?</h3>
      <p>Обычно в течение 24–48 часов после оформления заказа.</p>
    </div>
    <div class="card">
      <h3>Безопасно ли это?</h3>
      <p>Да, мы соблюдаем все правила платформ и используем проверенные методы.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Связаться с нами</h2>
    <div class="card contact">
      <input type="text" id="name" placeholder="Ваше имя">
      <input type="email" id="email" placeholder="Ваш email">
      <textarea id="message" rows="5" placeholder="Ваше сообщение..."></textarea>
      <button onclick="submitForm()">Отправить</button>
      <p id="status"></p>
    </div>
  </section>

  <footer>
    <div class="footer-content">
      <img src="cybrix-logo.png" alt="Cybrix" class="footer-logo">
      <p>© 2025 Cybrix — Продвижение, отзывы, рейтинг. Мы делаем ваш бизнес заметным!</p>
      <div class="planet-icon">🪐</div>
      <div class="credits">
        Разработка дизайна — <a href="https://t.me/Cybrix7" target="_blank">@Cybrix7</a>
      </div>
    </div>
  </footer>

  <button class="btn-scroll" onclick="document.getElementById('contact').scrollIntoView({ behavior: 'smooth' })">Связаться</button>
  <a href="https://t.me/Cybrix7" target="_blank"><button class="btn-telegram">Telegram</button></a>

  <script>
    particlesJS("particles-js", {
      particles: {
        number: { value: 80 },
        color: { value: "#00ff00" },
        shape: { type: "star" },
        opacity: { value: 0.5 },
        size: { value: 3 },
        line_linked: {
          enable: true,
          distance: 150,
          color: "#00ff00",
          opacity: 0.4,
          width: 1
        },
        move: { enable: true, speed: 1 }
      },
      interactivity: {
        events: { onhover: { enable: true, mode: "repulse" } }
      },
      retina_detect: true
    });

    ScrollReveal().reveal('.card, .tariff-card, .review, .contact', {
      delay: 100,
      duration: 1000,
      reset: true,
      opacity: 0,
      scale: 0.9,
      distance: '20px'
    });

    function submitForm() {
      const name = document.getElementById("name").value.trim();
      const email = document.getElementById("email").value.trim();
      const message = document.getElementById("message").value.trim();
      const status = document.getElementById("status");

      if (!name || !email || !message) {
        status.innerText = "Пожалуйста, заполните все поля.";
        status.style.color = "red";
        return;
      }

      status.innerText = "Спасибо! Ваше сообщение отправлено.";
      status.style.color = "lime";

      document.getElementById("name").value = "";
      document.getElementById("email").value = "";
      document.getElementById("message").value = "";
    }
  </script>
</body>
</html>
