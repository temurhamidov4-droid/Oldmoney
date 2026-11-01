
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#f7f4ed">
<meta name="description" content="OLD MONEY — премиальный барбершоп в Ташкенте. Искусство мужского стиля. Проспект Шарафа Рашидова, 40.">
<title>OLD MONEY — Barber House | Tashkent</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Manrope:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
:root {
  --cream: #f7f4ed;
  --white: #fffefa;
  --sand: #e9e0d1;
  --gold: #b69b6c;
  --dark: #30291f;
  --muted: #8d8375;
  --line: rgba(87,72,51,.17);
  --serif: 'Cormorant Garamond', serif;
  --sans: 'Manrope', sans-serif;
}

* {margin:0;padding:0;box-sizing:border-box}
html {scroll-behavior:smooth}
body {
  background:var(--cream);
  color:var(--dark);
  font-family:var(--sans);
  overflow-x:hidden;
}
a {color:inherit;text-decoration:none}
button {font-family:inherit}
::selection {background:var(--gold);color:white}

/* PRELOADER */
.loader {
 position:fixed;inset:0;background:var(--cream);
 display:flex;align-items:center;justify-content:center;
 z-index:9999;transition:.8s;
}
.loader span {
 font-family:var(--serif);font-size:45px;
 letter-spacing:12px;animation:pulse 1.5s infinite;
}
.loader.hide {opacity:0;visibility:hidden}
@keyframes pulse {50%{opacity:.35}}

/* NAVIGATION */
header {
 position:absolute;top:0;left:0;width:100%;
 padding:28px 7%;display:flex;
 align-items:center;justify-content:space-between;
 z-index:10;border-bottom:1px solid rgba(255,255,255,.2);
 color:white;
}
.logo {
 font-family:var(--serif);font-size:31px;
 letter-spacing:6px;font-weight:500;
}
.logo small {
 display:block;font-family:var(--sans);
 font-size:8px;letter-spacing:6px;
 text-align:center;margin-top:-3px;
}
nav {display:flex;gap:35px;align-items:center}
nav a {
 font-size:10px;letter-spacing:2px;
 text-transform:uppercase;transition:.3s;
}
nav a:hover {color:var(--gold)}
.nav-book {
 border:1px solid rgba(255,255,255,.7);
 padding:13px 23px;
}
.menu-btn {display:none;background:none;border:0;color:white;font-size:25px}

/* HERO */
.hero {
 min-height:790px;height:100svh;max-height:1050px;
 position:relative;display:flex;align-items:center;
 background:
 linear-gradient(90deg,rgba(21,18,14,.75),rgba(21,18,14,.15)),
 url('https://images.unsplash.com/photo-1503951914875-452162b0f3f1?auto=format&fit=crop&w=2200&q=90') center/cover;
 color:white;
}
.hero-content {padding:0 12%;max-width:850px;margin-top:70px}
.eyebrow {
 font-size:10px;letter-spacing:5px;text-transform:uppercase;
 color:#ddc9a4;display:flex;align-items:center;gap:15px;
}
.eyebrow:before {content:"";width:35px;height:1px;background:var(--gold)}
.hero h1 {
 font-family:var(--serif);font-size:clamp(75px,12vw,155px);
 line-height:.8;font-weight:400;letter-spacing:7px;
 margin:35px 0;
}
.hero h1 span {display:block;font-style:italic;font-size:.65em;letter-spacing:10px}
.hero p {
 font-size:12px;line-height:2.1;letter-spacing:2px;
 color:#e3ddd2;max-width:390px;
}
.hero-actions {display:flex;gap:15px;margin-top:40px;flex-wrap:wrap}
.btn {
 display:inline-flex;align-items:center;justify-content:center;
 padding:17px 29px;font-size:10px;letter-spacing:2px;
 text-transform:uppercase;transition:.3s;
}
.btn-gold {background:#c0a77b;color:#251f17}
.btn-gold:hover {background:#e0c99e;transform:translateY(-3px)}
.btn-outline {border:1px solid rgba(255,255,255,.6);color:white}
.btn-outline:hover {background:white;color:var(--dark)}
.hero-bottom {
 position:absolute;bottom:35px;left:7%;right:7%;
 display:flex;justify-content:space-between;
 font-size:9px;letter-spacing:3px;color:#ddd1bf;
}
.scroll {writing-mode:vertical-rl}

/* COMMON */
section {padding:120px 8%}
.section-label {
 color:var(--gold);font-size:10px;letter-spacing:4px;
 text-transform:uppercase;margin-bottom:23px;
}
.section-title {
 font-family:var(--serif);font-size:clamp(43px,6vw,76px);
 line-height:.95;font-weight:400;
}
.section-title em {color:#a58d68;font-weight:400}
.section-desc {
 color:var(--muted);font-size:12px;line-height:2.1;
 max-width:450px;margin-top:25px;
}

/* INTRO */
.intro {
 display:grid;grid-template-columns:1fr 1fr;
 gap:10%;align-items:center;
}
.intro-image {position:relative;padding:0 25px 25px 0}
.intro-image img {
 width:100%;height:570px;object-fit:cover;
 filter:sepia(12%);
}
.intro-image:after {
 content:"";position:absolute;right:0;bottom:0;
 width:75%;height:75%;border:1px solid var(--gold);
 z-index:-1;
}
.intro-copy {padding:30px 0}
.signature {
 font-family:var(--serif);font-size:38px;
 font-style:italic;color:#9f8864;margin-top:35px;
}
.intro-note {
 margin-top:35px;padding-top:25px;border-top:1px solid var(--line);
 font-size:10px;letter-spacing:2px;color:var(--muted);
}

/* VALUES */
.values {
 background:#eae3d7;
 text-align:center;
}
.values .section-desc {margin:25px auto 65px}
.values-grid {
 display:grid;grid-template-columns:repeat(3,1fr);
 border-top:1px solid rgba(87,72,51,.2);
 border-bottom:1px solid rgba(87,72,51,.2);
}
.value {padding:45px 25px}
.value+.value {border-left:1px solid rgba(87,72,51,.2)}
.value-number {
 font-family:var(--serif);font-size:40px;
 color:var(--gold);margin-bottom:15px;
}
.value h3 {
 font-family:var(--serif);font-size:28px;
 font-weight:500;margin-bottom:12px;
}
.value p {font-size:11px;line-height:2;color:var(--muted)}

/* SERVICES */
.services-head {
 display:flex;justify-content:space-between;
 align-items:end;gap:30px;margin-bottom:65px;
}
.service-list {border-top:1px solid var(--line)}
.service {
 display:grid;grid-template-columns:70px 1fr auto;
 align-items:center;gap:25px;padding:30px 5px;
 border-bottom:1px solid var(--line);
 transition:.3s;
}
.service:hover {padding-left:18px;background:rgba(255,255,255,.4)}
.service-num {font-family:var(--serif);font-size:27px;color:var(--gold)}
.service h3 {font-family:var(--serif);font-size:30px;font-weight:500}
.service p {font-size:10px;color:var(--muted);margin-top:5px}
.price {font-family:var(--serif);font-size:27px;white-space:nowrap}
.price small {font-family:var(--sans);font-size:10px;color:var(--muted)}

/* GALLERY */
.gallery {background:#eae3d7}
.gallery-top {display:flex;justify-content:space-between;align-items:end;margin-bottom:45px}
.gallery-grid {
 display:grid;grid-template-columns:1.2fr .8fr 1fr;
 grid-template-rows:270px 270px;gap:15px;
}
.gallery-grid img {
 width:100%;height:100%;object-fit:cover;
 filter:sepia(10%);transition:.7s;
}
.gallery-grid img:hover {filter:none;transform:scale(1.02)}
.gallery-item {overflow:hidden}
.gallery-item:first-child {grid-row:span 2}
.gallery-item:nth-child(2) {grid-column:span 2}

/* EXPERIENCE */
.experience {
 min-height:520px;display:flex;align-items:center;
 justify-content:center;text-align:center;color:white;
 background:
 linear-gradient(rgba(31,25,18,.67),rgba(31,25,18,.67)),
 url('https://images.unsplash.com/photo-1599351431202-1e0f0137899a?auto=format&fit=crop&w=1800&q=85') center/cover fixed;
}
.experience .section-title {font-size:clamp(55px,8vw,95px)}
.experience p {
 font-size:11px;letter-spacing:3px;
 margin-top:30px;color:#e4d7c2;
}

/* LOCATION */
.location-grid {
 display:grid;grid-template-columns:1fr 1fr;
 gap:9%;align-items:center;
}
.location-image img {width:100%;height:500px;object-fit:cover}
.contact-item {
 padding:23px 0;border-bottom:1px solid var(--line);
 display:flex;justify-content:space-between;gap:15px;
}
.contact-item span:first-child {
 font-size:10px;color:var(--muted);letter-spacing:2px;
 text-transform:uppercase;
}
.contact-item span:last-child {font-size:12px;text-align:right}
.map-links {display:flex;gap:12px;flex-wrap:wrap;margin-top:35px}
.map-links a {
 border:1px solid var(--line);padding:13px 18px;
 font-size:9px;letter-spacing:1px;transition:.3s;
}
.map-links a:hover {background:var(--dark);color:white}

/* FOOTER */
footer {
 background:#30291f;color:#e8dfd0;
 padding:70px 8% 25px;
}
.footer-top {
 display:flex;justify-content:space-between;
 align-items:start;gap:35px;padding-bottom:60px;
}
.footer-logo {font-family:var(--serif);font-size:55px;letter-spacing:7px}
.footer-logo small {
 display:block;font-family:var(--sans);
 font-size:9px;letter-spacing:6px;
}
.footer-links {display:flex;gap:25px;flex-wrap:wrap}
.footer-links a {font-size:10px;color:#c5b9a6}
.footer-bottom {
 padding-top:25px;border-top:1px solid rgba(255,255,255,.15);
 display:flex;justify-content:space-between;gap:15px;
 font-size:9px;letter-spacing:1px;color:#aa9e8c;
}
.reveal {opacity:0;transform:translateY(35px);transition:1s}
.reveal.visible {opacity:1;transform:translateY(0)}

@media(max-width:800px) {
 header {padding:20px 6%}
 .logo {font-size:26px}
 nav {
  display:none;position:absolute;top:80px;left:0;width:100%;
  background:var(--cream);color:var(--dark);
  padding:30px;flex-direction:column;gap:25px;
 }
 nav.open {display:flex}
 nav a {color:var(--dark)}
 .nav-book {border-color:var(--gold)}
 .menu-btn {display:block}
 .hero {min-height:720px;background-position:58% center}
 .hero-content {padding:0 8%;margin-top:50px}
 .hero h1 {font-size:clamp(65px,16vw,110px)}
 .hero-bottom {font-size:8px;left:6%;right:6%}
 section {padding:85px 7%}
 .intro,.location-grid {grid-template-columns:1fr;gap:55px}
 .intro-image img {height:420px}
 .intro-copy {padding:0}
 .values-grid {grid-template-columns:1fr}
 .value+.value {border-left:0;border-top:1px solid rgba(87,72,51,.2)}
 .services-head,.gallery-top {align-items:start;flex-direction:column}
 .service {grid-template-columns:35px 1fr auto;gap:12px}
 .service h3 {font-size:24px}
 .service p {font-size:9px}
 .price {font-size:21px}
 .gallery-grid {
  grid-template-columns:1fr 1fr;grid-template-rows:250px 180px 180px;
 }
 .gallery-item:first-child {grid-row:span 2}
 .gallery-item:nth-child(2) {grid-column:span 1}
 .experience {background-attachment:scroll;min-height:420px}
 .location-image img {height:350px}
 .footer-top {flex-direction:column}
 .footer-bottom {flex-direction:column}
}
@media(max-width:390px) {
 .hero h1 {font-size:62px}
 .service h3 {font-size:21px}
 .price {font-size:18px}
}
@media(prefers-reduced-motion:reduce) {
 *,*:before,*:after {scroll-behavior:auto!important;animation:none!important;transition:none!important}
}
</style>
</head>

<body>

<div class="loader" id="loader"><span>OLD MONEY</span></div>

<header>
 <a href="#" class="logo">OLD MONEY<small>BARBER HOUSE</small></a>
 <nav id="nav">
  <a href="#about">О нас</a>
  <a href="#values">Философия</a>
  <a href="#services">Услуги</a>
  <a href="#gallery">Атмосфера</a>
  <a href="#contacts">Контакты</a>
  <a href="https://t.me/Old_Money_barbershop" class="nav-book">Записаться</a>
 </nav>
 <button class="menu-btn" id="menuBtn" aria-label="Открыть меню">☰</button>
</header>

<main>
<section class="hero">
 <div class="hero-content">
  <div class="eyebrow">TASHKENT · EST. OLD MONEY</div>
  <h1>OLD <span>MONEY</span></h1>
  <p>ИСКУССТВО МУЖСКОГО СТИЛЯ.<br>
  ТРАДИЦИИ, КОТОРЫЕ НЕ ТРЕБУЮТ СЛОВ.<br>
  СТИЛЬ, КОТОРЫЙ ГОВОРИТ ЗА ТЕБЯ.</p>
  <div class="hero-actions">
   <a class="btn btn-gold" href="https://t.me/Old_Money_barbershop">Записаться онлайн ↗</a>
   <a class="btn btn-outline" href="#about">Открыть историю</a>
  </div>
 </div>
 <div class="hero-bottom">
  <span>SHARAF RASHIDOV AVENUE · 40</span>
  <span class="scroll">SCROLL TO DISCOVER ↓</span>
  <span>EST. IN TASHKENT</span>
 </div>
</section>

<section class="intro" id="about">
 <div class="intro-image reveal">
  <img src="https://images.unsplash.com/photo-1621605815971-fbc98d665033?auto=format&fit=crop&w=1000&q=85" alt="Искусство мужской стрижки" loading="lazy">
 </div>
 <div class="intro-copy reveal">
  <div class="section-label">THE ART OF GENTLEMAN</div>
  <h2 class="section-title">Больше, чем<br><em>просто стрижка.</em></h2>
  <p class="section-desc">
   OLD MONEY — пространство, где классика встречается с современностью.
   Здесь важна каждая деталь: точность движений, качество сервиса,
   атмосфера и индивидуальный подход.
   <br><br>
   Мы верим, что настоящий стиль не нуждается в демонстрации.
   Он чувствуется в уверенности, простоте и безупречном исполнении.
  </p>
  <div class="signature">Your style. Your legacy.</div>
  <div class="intro-note">OLD MONEY · BARBER HOUSE · TASHKENT</div>
 </div>
</section>

<section class="values" id="values">
 <div class="section-label">OUR PHILOSOPHY</div>
 <h2 class="section-title">Три принципа.<br><em>Один стандарт.</em></h2>
 <p class="section-desc">Эстетика, качество и отношение к деталям — основа всего, что мы делаем.</p>
 <div class="values-grid">
  <div class="value reveal">
   <div class="value-number">I</div>
   <h3>Tradition</h3>
   <p>Уважение к классике и искусству настоящего мужского ухода.</p>
  </div>
  <div class="value reveal">
   <div class="value-number">II</div>
   <h3>Precision</h3>
   <p>Внимание к каждой линии, каждой детали и каждому движению.</p>
  </div>
  <div class="value reveal">
   <div class="value-number">III</div>
   <h3>Character</h3>
   <p>Индивидуальность, уверенность и стиль вне времени.</p>
  </div>
 </div>
</section>

<section id="services">
 <div class="services-head">
  <div>
   <div class="section-label">OUR SERVICES</div>
   <h2 class="section-title">Искусство<br><em>деталей.</em></h2>
  </div>
  <p class="section-desc">Каждая процедура — внимание к вашему образу и комфорту.</p>
 </div>
 <div class="service-list">
  <div class="service reveal">
   <div class="service-num">01</div>
   <div><h3>Men's Haircut</h3><p>Индивидуальная мужская стрижка</p></div>
   <div class="price">По запросу</div>
  </div>
  <div class="service reveal">
   <div class="service-num">02</div>
   <div><h3>Beard Styling</h3><p>Моделирование и оформление бороды</p></div>
   <div class="price">По запросу</div>
  </div>
  <div class="service reveal">
   <div class="service-num">03</div>
   <div><h3>Hair & Beard</h3><p>Комплексный мужской образ</p></div>
   <div class="price">По запросу</div>
  </div>
  <div class="service reveal">
   <div class="service-num">04</div>
   <div><h3>Royal Care</h3><p>Профессиональный уход и дополнительные процедуры</p></div>
   <div class="price">По запросу</div>
  </div>
 </div>
 <p class="section-desc">Для уточнения стоимости и доступного времени свяжитесь с нами.</p>
 <a href="https://t.me/Old_Money_barbershop" class="btn btn-gold" style="margin-top:25px">Узнать цены и записаться ↗</a>
</section>

<section class="gallery" id="gallery">
 <div class="gallery-top">
  <div>
   <div class="section-label">THE ATMOSPHERE</div>
   <h2 class="section-title">Стиль в каждой<br><em>детали.</em></h2>
  </div>
  <p class="section-desc">Пространство, созданное для тех, кто ценит время, эстетику и качество.</p>
 </div>
 <div class="gallery-grid">
  <div class="gallery-item"><img src="https://images.unsplash.com/photo-1599351431202-1e0f0137899a?auto=format&fit=crop&w=900&q=85" alt="Мужской барбершоп" loading="lazy"></div>
  <div class="gallery-item"><img src="https://images.unsplash.com/photo-1503951914875-452162b0f3f1?auto=format&fit=crop&w=900&q=85" alt="Работа барбера" loading="lazy"></div>
  <div class="gallery-item"><img src="https://images.unsplash.com/photo-1621605815971-fbc98d665033?auto=format&fit=crop&w=900&q=85" alt="Мужская стрижка" loading="lazy"></div>
  <div class="gallery-item"><img src="https://images.unsplash.com/photo-1512690459411-b9245aed614b?auto=format&fit=crop&w=900&q=85" alt="Барбер инструменты" loading="lazy"></div>
 </div>
</section>

<section class="experience">
 <div class="reveal">
  <div class="section-label">A DIFFERENT STANDARD</div>
  <h2 class="section-title">Elegance is<br><em>an attitude.</em></h2>
  <p>НЕ СЛЕДУЙ ЗА ТРЕНДАМИ. СОЗДАВАЙ СВОЙ СТИЛЬ.</p>
 </div>
</section>

<section id="contacts">
 <div class="location-grid">
  <div class="location-image reveal">
   <img src="https://images.unsplash.com/photo-1593702295094-aea6393a2d8b?auto=format&fit=crop&w=1000&q=85" alt="Атмосфера барбершопа" loading="lazy">
  </div>
  <div class="reveal">
   <div class="section-label">FIND YOUR PLACE</div>
   <h2 class="section-title">Мы ждём<br><em>вас.</em></h2>
   <p class="section-desc">Ваше место для безупречного стиля находится в самом сердце Ташкента.</p>

   <div class="contact-item">
    <span>Адрес</span>
    <span>просп. Шарафа Рашидова, 40</span>
   </div>
   <div class="contact-item">
    <span>Телефон</span>
    <span><a href="tel:+998335017676">+998 33 501 76 76</a></span>
   </div>
   <div class="contact-item">
    <span>Instagram</span>
    <span><a href="https://www.instagram.com/Barbershop_oldmoney/" target="_blank" rel="noopener">@Barbershop_oldmoney ↗</a></span>
   </div>
   <div class="contact-item">
    <span>Telegram</span>
    <span><a href="https://t.me/Old_Money_barbershop" target="_blank" rel="noopener">@Old_Money_barbershop ↗</a></span>
   </div>

   <div class="map-links">
    <a href="https://yandex.ru/maps/org/oldmoney/42427499446?si=4env4zvakyfjrae0e5cqv3ev04" target="_blank" rel="noopener">YANDEX MAPS ↗</a>
    <a href="https://2gis.ru/tashkent/geo/70000001100856549" target="_blank" rel="noopener">2GIS ↗</a>
    <a href="https://maps.app.goo.gl/UKdA9XxDTUNY3CGU6?g_st=ic" target="_blank" rel="noopener">GOOGLE MAPS ↗</a>
   </div>
   <a href="https://t.me/Old_Money_barbershop" class="btn btn-gold" style="margin-top:30px">Записаться на визит ↗</a>
  </div>
 </div>
</section>
</main>

<footer>
 <div class="footer-top">
  <div class="footer-logo">OLD MONEY<small>BARBER HOUSE · TASHKENT</small></div>
  <div class="footer-links">
   <a href="#about">О нас</a>
   <a href="#services">Услуги</a>
   <a href="#gallery">Атмосфера</a>
   <a href="#contacts">Контакты</a>
   <a href="https://t.me/Old_Money_barbershop">Telegram ↗</a>
  </div>
 </div>
 <div class="footer-bottom">
  <span>© <span id="year"></span> OLD MONEY BARBER HOUSE. ALL RIGHTS RESERVED.</span>
  <span>TIMELESS STYLE. LASTING IMPRESSION.</span>
 </div>
</footer>

<script>
window.addEventListener('load', () => {
 document.getElementById('loader').classList.add('hide');
});

document.getElementById('year').textContent = new Date().getFullYear();

const menuBtn = document.getElementById('menuBtn');
const nav = document.getElementById('nav');

menuBtn.addEventListener('click', () => {
 nav.classList.toggle('open');
 menuBtn.textContent = nav.classList.contains('open') ? '×' : '☰';
});

nav.querySelectorAll('a').forEach(link => {
 link.addEventListener('click', () => {
  nav.classList.remove('open');
  menuBtn.textContent = '☰';
 });
});

const observer = new IntersectionObserver(entries => {
 entries.forEach(entry => {
  if(entry.isIntersecting) {
   entry.target.classList.add('visible');
   observer.unobserve(entry.target);
  }
 });
}, {threshold:0.12});

document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
</script>

</body>
</html>
