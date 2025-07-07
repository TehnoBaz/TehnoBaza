# TehnoBaza
TehnoBaza
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>ТехноБаза — Побутова техніка Grifon у Харкові</title>
<style>
  /* Reset */
  * {
    margin: 0; padding: 0; box-sizing: border-box;
  }
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #f4f7f9;
    color: #333;
    line-height: 1.6;
  }
  header {
    background: #0078d7;
    color: white;
    padding: 20px 0;
    text-align: center;
    box-shadow: 0 3px 6px rgba(0,0,0,0.1);
  }
  header h1 {
    font-weight: 700;
    font-size: 2.2rem;
    letter-spacing: 1px;
  }
  nav {
    background: #005a9e;
    display: flex;
    justify-content: center;
    padding: 15px 0;
  }
  nav a {
    color: white;
    text-decoration: none;
    font-weight: 600;
    margin: 0 25px;
    font-size: 1.1rem;
    transition: color 0.3s ease;
  }
  nav a:hover {
    color: #ffcc00;
  }
  .hero {
    background: url('https://images.unsplash.com/photo-1580587771525-78b9dba3b914?auto=format&fit=crop&w=1350&q=80') no-repeat center/cover;
    color: white;
    padding: 100px 20px;
    text-align: center;
  }
  .hero h2 {
    font-size: 3rem;
    margin-bottom: 15px;
    text-shadow: 0 2px 6px rgba(0,0,0,0.7);
  }
  .hero p {
    font-size: 1.4rem;
    margin-bottom: 30px;
    text-shadow: 0 1px 3px rgba(0,0,0,0.6);
  }
  .hero button {
    background: #ffcc00;
    border: none;
    padding: 15px 40px;
    font-size: 1.2rem;
    font-weight: 700;
    border-radius: 30px;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  .hero button:hover {
    background: #e6b800;
  }
  main {
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
  }
  section {
    margin-bottom: 60px;
  }
  h2.section-title {
    text-align: center;
    font-size: 2rem;
    margin-bottom: 40px;
    color: #0078d7;
  }
  /* Catalog */
  .catalog {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
    gap: 30px;
  }
  .product-card {
    background: white;
    border-radius: 12px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    transition: transform 0.3s ease;
  }
  .product-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.15);
  }
  .product-image {
    height: 180px;
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
  }
  .product-info {
    padding: 20px;
    flex-grow: 1;
  }
  .product-info h3 {
    margin-bottom: 10px;
    font-size: 1.25rem;
    color: #0078d7;
  }
  .product-info p {
    font-size: 0.95rem;
    color: #555;
    margin-bottom: 15px;
  }
  .product-info strong {
    display: block;
    font-size: 1.1rem;
    margin-bottom: 15px;
    color: #222;
  }
  .product-info button {
    background: #0078d7;
    color: white;
    border: none;
    padding: 12px 25px;
    font-size: 1rem;
    font-weight: 600;
    border-radius: 30px;
    cursor: pointer;
    transition: background 0.3s ease;
    width: 100%;
  }
  .product-info button:hover {
    background: #005a9e;
  }
  /* Features */
  .features-list {
    display: flex;
    justify-content: center;
    gap: 50px;
    flex-wrap: wrap;
  }
  .feature-item {
    max-width: 220px;
    text-align: center;
    color: #0078d7;
  }
  .feature-item svg {
    width: 60px;
    height: 60px;
    margin-bottom: 15px;
    fill: #0078d7;
  }
  .feature-item p {
    font-weight: 600;
    font-size: 1.1rem;
  }
  /* Reviews */
  .reviews p {
    max-width: 700px;
    margin: 20px auto;
    font-style: italic;
    color: #444;
    font-size: 1.1rem;
    border-left: 4px solid #0078d7;
    padding-left: 15px;
  }
  /* Contact Form */
  form {
    max-width: 480px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  input, textarea {
    padding: 12px 15px;
    border-radius: 8px;
    border: 1.5px solid #ccc;
    font-size: 1rem;
    resize: vertical;
    transition: border-color 0.3s ease;
  }
  input:focus, textarea:focus {
    border-color: #0078d7;
    outline: none;
  }
  button[type="submit"] {
    background: #0078d7;
    color: white;
    padding: 15px;
    border: none;
    font-size: 1.1rem;
    font-weight: 700;
    border-radius: 30px;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  button[type="submit"]:hover {
    background: #005a9e;
  }
  footer {
    background: #003963;
    color: white;
    padding: 25px 20px;
    text-align: center;
    font-size: 0.9rem;
  }
  footer p {
    margin: 5px 0;
  }
  @media(max-width: 600px) {
    nav {
      flex-direction: column;
      gap: 10px;
    }
    .features-list {
      gap: 30px;
    }
  }
</style>
</head>
<body>
<header>
  <h1>ТехноБаза — Grifon</h1>
  <p>Офіційна техніка Grifon у Харкові. Без вихідних</p>
</header>
<nav>
  <a href="#catalog">Каталог</a>
  <a href="#why">Переваги</a>
  <a href="#reviews">Відгуки</a>
  <a href="#contact">Контакти</a>
</nav>

<section class="hero">
  <h2>Якісна побутова техніка Grifon за доступною ціною</h2>
  <p>Швидка доставка по Харкову. Гарантія до 12 місяців</p>
  <button onclick="document.getElementById('catalog').scrollIntoView({behavior:'smooth'})">Перейти до каталогу</button>
</section>

<main>
  <section id="catalog">
    <h2 class="section-title">Наш каталог</h2>
    <div class="catalog">
      <div class="product-card">
        <div class="product-image" style="background-image: url('https://grifon.ua/image/cache/catalog/products/washing-machines/gwm7123dd-500x500.jpg');"></div>
        <div class="product-info">
          <h3>Пральна машина Grifon GWM‑7123DD</h3>
          <p>7 кг · Інвертор · 14 програм · A+++ · 1200 об/хв · LED · Гарантія 10 років</p>
          <strong>12 999 грн</strong>
          <button>Купити</button>
        </div>
      </div>
      <div class="product-card">
        <div class="product-image" style="background-image: url('https://grifon.ua/image/cache/catalog/products/refrigerators/dfn180w-500x500.jpg');"></div>
        <div class="product-info">
          <h3>Холодильник Grifon DFN‑180W</h3>
          <p>254 л (191+63) · A+ · Механічне керування · Габарити: 180×55×56 см</p>
          <strong>10 499 грн</strong>
          <button>Купити</button>
        </div>
      </div>
      <div class="product-card">
        <div class="product-image" style="background-image: url('https://grifon.ua/image/cache/catalog/products/refrigerators/nfn185bg-500x500.jpg');"></div>
        <div class="product-info">
          <h3>Холодильник Grifon NFN‑185BG</h3>
          <p>No Frost · 290 л (201+89) · A+ · Електронне керування · Гарантія 30 міс</p>
          <strong>15 999 грн</strong>
          <button>Купити</button>
        </div>
      </div>
    </div>
  </section>

  <section id="why">
    <h2 class="section-title">Чому обирають ТехноБазу</h2>
    <div class="features-list">
      <div class="feature-item">
        <svg viewBox="0 0 64 64"><path d="M32 0a32 32 0 1032 32A32 32 0 0032 0zm0 60A28 28 0 1159.999 32 28 28 0 0132 60z"/><path d="M44.242 20.485l-18 18a2 2 0 01-2.828 0l-8-8a2 2 0 112.828-2.828L26 33.172l16.485-16.485a2 2 0 112.828 2.828z"/></svg>
        <p>Офіційна техніка з гарантією</p>
      </div>
      <div class="feature-item">
        <svg viewBox="0 0 64 64"><path d="M32 4a28 28 0 1028 28A28 28 0 0032 4zm0 52a24 24 0 1124-24 24 24 0 01-24 24z"/><path d="M32 12a2 2 0 012 2v16a2 2 0 11-4 0V14a2 2 0 012-2zm-8 8a2 2 0 012-2h8a2 2 0 110 4h-8a2 2 0 01-2-2zm16 12a2 2 0 11-4 0v-4a2 2 0 114 0z"/></svg>
        <p>Без передоплати</p>
      </div>
      <div class="feature-item">
        <svg viewBox="0 0 64 64"><path d="M32 2a30 30 0 1030 30A30 30 0 0032 2zm0 56a26 26 0 1126-26 26 26 0 01-26 26z"/><path d="M44.586 18.586l-15 15a2 2 0 01-2.828-2.828l15-15a2 2 0 012.828 2.828z"/></svg>
        <p>Доставка по місту за 1 день</p>
      </div>
      <div class="feature-item">
        <svg viewBox="0 0 64 64"><circle cx="32" cy="32" r="30" fill="none" stroke="#0078d7" stroke-width="4"/><path d="M16 36l8 8 16-24" fill="none" stroke="#0078d7" stroke-width="4"/></svg>
        <p>Працюємо без вихідних</p>
      </div>
    </div>
  </section>

  <section id="reviews" class="reviews">
    <h2 class="section-title">Відгуки клієнтів</h2>
    <p>«Холодильник привезли за кілька годин, сервіс — супер!» — Анна</p>
    <p>«Grifon працює як швейцарський годинник!» — Володимир</p>
  </section>

  <section class="delivery section">
    <h2 class="section-title">Доставка та оплата</h2>
    <ul style="max-width: 600px; margin: 0 auto; list-style:none; padding:0; color:#555;">
      <li style="margin-bottom: 10px; font-weight: 600;">🚚 Доставка по Харкову  — від 400 грн</li>
      <li style="margin-bottom: 10px; font-weight: 600;">💳 Оплата: готівка, картка або при отриманні</li>
      <li style="margin-bottom: 10px; font-weight: 600;">🔧 Установка техніки — за запитом</li>
    </ul>
  </section>

  <section id="contact">
    <h2 class="section-title">Залишити заявку</h2>
    <form>
      <input type="text" placeholder="Ваше ім’я" required />
      <input type="tel" placeholder="Телефон" required />
      <textarea placeholder="Яка техніка цікавить?" rows="4"></textarea>
      <button type="submit">Надіслати</button>
    </form>
  </section>
</main>

<footer>
  <p>Контакти: +38 (063) 136-95-38 | м. Харків, ст.м Академіка Павлова</p>
  <p>Працюємо щодня, без вихідних: 09:00 – 20:00</p>
  <p>Instagram / Facebook / OLX</p>
</footer>
</body>
</html>
