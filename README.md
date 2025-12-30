
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Мир котиков</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      min-height: 100vh;
    }
    
    .c { max-width: 700px; margin: 0 auto; padding: 15px; }
    h1 {
      text-align: center;
      font-size: 2rem;
      color: white;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
      animation: b 1s ease infinite;
    }
    @keyframes b {
      0%, 50%, 100% { transform: translateY(0); }
      25% { transform: translateY(-8px); }
      75% { transform: translateY(-4px); }
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 10px;
      margin: 15px 0;
      flex-wrap: wrap;
    }
    nav a {
      color: white;
      text-decoration: none;
      padding: 6px 12px;
      border-radius: 20px;
      background: rgba(255,255,255,0.2);
      transition: 0.2s;
    }
    nav a:hover {
      background: rgba(255,255,255,0.4);
      transform: scale(1.05);
    }
    .g {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 12px;
      margin: 20px 0;
    }
    .crd {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: 0.2s;
    }
    .crd:hover { transform: translateY(-4px); box-shadow: 0 8px 16px rgba(0,0,0,0.12); }
    .img { width: 100%; height: 140px; object-fit: cover; transition: 0.2s; }
    .crd:hover .img { transform: scale(1.02); }
    .inf { padding: 10px; text-align: center; }
    .ttl {
      font-size: 1rem;
      margin-bottom: 5px;
      color: #ff6b6b;
    }
    section { margin: 25px 0; }
    h2 {
      text-align: center;
      color: #ff6b6b;
      margin-bottom: 15px;
    }
    .bx {
      background: #fff9;
      border-left: 3px solid #ff6b6b;
      padding: 10px;
      margin: 10px 0;
      border-radius: 0 4px 4px 0;
      animation: s 0.5s forwards;
      opacity: 0;
    }
    @keyframes s {
      from { transform: translateX(-8px); opacity: 0; }
      to { transform: translateX(0); opacity: 1; }
    }
    footer {
      text-align: center;
      padding: 15px 0;
      color: white;
      font-size: 0.7rem;
      margin-top: 20px;
      border-top: 1px solid rgba(255,255,255,0.2);
    }
    .paw {
      position: fixed;
      top: -8px;
      left: 50%;
      transform: translateX(-50%);
      color: rgba(255,255,255,0.5);
      font-size: 1.2rem;
      z-index: -1;
      animation: f 2.5s linear infinite;
      pointer-events: none;
    }
    @keyframes f { to { top: 110vh; opacity: 0; } }
  </style>
</head>
<body>
  <div class="paw">🐾</div>
  <div class="paw" style="left: 5%; animation-delay: 0.3s;">🐾</div>
  <div class="paw" style="left: 95%; animation-delay: 0.6s;">🐾</div>

  <div class="c">
    <h1>🐱 Мир котиков 🐱</h1>

    <nav>
    <a href="#photos">Фото</a>
      <a href="#facts">Факты</a>
      <a href="#care">Уход</a>
    </nav>

    <section id="photos">
      <h2>Фотогалерея</h2>
      <div class="g">
        <div class="crd">
          <img src="https://i.pinimg.com/originals/9c/bd/08/9cbd08888096d19518eff45ea96a3b23.jpg" alt="Кот" class="img">
          <div class="inf">
            <h3 class="ttl">Дворовые (Легенды)</h3>
            <p>Любит коробки</p>
          </div>
        </div>
        <div class="crd">
          <img src="https://i.pinimg.com/736x/d9/40/a0/d940a045153d7234a11ef1b801f93682.jpg" alt="Кошка" class="img">
          <div class="inf">
            <h3 class="ttl">Манчкины</h3>
            <p>Тёплый и ласковый</p>
          </div>
        </div>
        <div class="crd">
          <img src="https://avatars.mds.yandex.net/i?id=ea48879eff783969909e4f804eee3f278bc798e3-4571079-images-thumbs&n=13" alt="Котёнок" class="img">
          <div class="inf">
            <h3 class="ttl">Мэйн Кун</h3>
            <p>Большые пушистые</p>
          </div>
        </div>
      </div>
    </section>

    <section id="facts">
      <h2>Интересные факты</h2>
      <div class="bx"><strong>Сон 12–16 ч</strong> — экономия энергии</div>
      <div class="bx"><strong>32 мышцы в ухе</strong> — поворот на 180°</div>
      <div class="bx"><strong>Мурлыканье</strong> — заживляет ткани</div>
      <div class="bx"><strong>Уникальный нос</strong> — как отпечатки</div>
      <div class="bx"><strong>Обоняние ×14</strong> лучше человеческого</div>
      <div class="bx"><strong>Потеют через лапы</strong></div>
      <div class="bx"><strong>Видят в темноте ×6</strong> лучше людей</div>
      <div class="bx"><strong>Не чувствуют сладкое</strong></div>
    </section>

    <section id="care">
      <h2>Советы по уходу</h2>
      <div class="bx"><strong>Кормление:</strong> качественный корм, вода, режим</div>
      <div class="bx"><strong>Гигиена:</strong> расчёсывание, чистка ушей, когти</div>
      <div class="bx"><strong>Активность:</strong> игрушки, прогулки</div>
      <div class="bx"><strong>Здоровье:</strong> прививки, осмотр у ветеринара</div>
      <div class="bx"><strong>Комфорт:</strong> лоток, спальное место</div>
    </section>

    <footer>© 2025 Мир котиков. Все права защищены.</footer>
  </div>
</body>
</html>
