<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Marmara İklimi</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Roboto:wght@400;500&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0; padding: 0;
      font-family: 'Roboto', sans-serif;
      background: #f8f9fa;
      color: #333;
    }
    header {
      background: #2c3e50;
      color: #ecf0f1;
      text-align: center;
      padding: 40px 20px;
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    nav {
      display: flex; justify-content: center;
      background: #34495e;
      box-shadow: inset 0 -2px 4px rgba(0,0,0,0.2);
    }
    nav button {
      background: none;
      border: none;
      color: #bdc3c7;
      padding: 15px 25px;
      font-size: 1rem;
      cursor: pointer;
      transition: color .3s, background .3s;
      font-weight: 500;
    }
    nav button:hover,
    nav button.active {
      background: #ecf0f1;
      color: #2c3e50;
      border-top-left-radius: 8px;
      border-top-right-radius: 8px;
      box-shadow: 0 -4px 8px rgba(0,0,0,0.1);
    }
    .container {
      max-width: 1100px;
      margin: 30px auto;
      padding: 0 20px;
    }
    section {
      display: none;
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    section.active {
      display: block;
    }
    h2 {
      font-family: 'Playfair Display', serif;
      color: #2c3e50;
      margin-bottom: 15px;
      font-size: 1.8rem;
      border-bottom: 2px solid #ecf0f1;
      padding-bottom: 5px;
    }
    h3 {
      color: #34495e;
      margin-top: 25px;
      font-size: 1.3rem;
    }
    p {
      line-height: 1.6;
      margin: 10px 0;
    }
    .stats {
      display: flex;
      justify-content: space-around;
      margin: 20px 0;
    }
    .stat {
      text-align: center;
    }
    .stat h4 {
      font-size: 2rem;
      margin: 0;
      color: #e67e22;
      font-weight: 700;
    }
    .stat span {
      display: block;
      margin-top: 5px;
      color: #7f8c8d;
    }
    .image-container {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      margin-top: 20px;
      justify-content: center;
    }
    .image-container img {
      width: calc(33% - 10px);
      border-radius: 6px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform .3s;
    }
    .image-container img:hover {
      transform: scale(1.03);
    }
  </style>
</head>
<body>

<header>Marmara İklimi</header>

<nav>
  <button class="active" onclick="show('iklim')">İklim Özellikleri</button>
  <button onclick="show('bitki')">Bitki Türleri</button>
  <button onclick="show('hayvan')">Hayvan Türleri</button>
  <button onclick="show('foto')">Fotoğraflar</button>
</nav>

<div class="container">

  <section id="iklim" class="active">
    <h2>Genel Bakış</h2>
    <p>Marmara iklimi, Akdeniz ve Karadeniz iklimlerinin geçiş özelliklerini taşır. Yazları sıcak ve kurak, kışları ılık ve yağışlıdır. Kıyıdan iç kesimlere gidildikçe kara etki artar. İstanbul'da kentsel ısı adası etkisi gözlemlenir.</p>
    <div class="stats">
      <div class="stat">
        <h4>20-28°C</h4>
        <span>Yaz Sıcaklığı</span>
      </div>
      <div class="stat">
        <h4>5-12°C</h4>
        <span>Kış Sıcaklığı</span>
      </div>
      <div class="stat">
        <h4>600-900 mm</h4>
        <span>Yıllık Yağış</span>
      </div>
    </div>
    <h3>Mevsimsel Dağılım</h3>
    <p>Yağışlar yıl boyunca dengeli dağılmıştır. Kış aylarında nispeten daha yoğundur; yazın kısa kurak dönemler görülebilir.</p>
  </section>

  <section id="bitki">
    <h2>Bitki Türleri</h2>
    <h3>Ormanlar ve Makiler</h3>
    <p>Marmara’da meşe, kestane, kayın, ıhlamur gibi geniş yapraklı ormanlar ile maki (bodur çalı formasyonu) iç içe geçer.</p>
    <h3>Tarım Ürünleri</h3>
    <p>Verimli topraklarda ayçiçeği, üzüm, buğday ve zeytin yetişir. Trakya ve Marmara kıyıları, ülkemizin önemli tarım alanlarıdır.</p>
    <div class="image-container">
      <img src="marmara_bitki1.jpg" alt="Marmara Üzüm Bağları">
      <img src="marmara_bitki2.jpg" alt="Marmara Zeytinlikleri">
    </div>
  </section>

  <section id="hayvan">
    <h2>Hayvan Türleri</h2>
    <h3>Orman ve Karasal Fauna</h3>
    <p>Yaban domuzu, tilki, sansar, porsuk gibi memeliler yaygındır. Orman altı faunasına sincap ve çeşitli küçük kemirgenler dahildir.</p>
    <h3>Kıyı ve Sulak Alanlar</h3>
    <p>Boğaz’da yunuslar, martılar; deltalar ve göletlerde su kuşları (ördek, balıkçıl, leylek) görülür.</p>
    <div class="image-container">
      <img src="marmara_hayvan1.jpg" alt="Marmara Yaban Domuzu">
      <img src="marmara_hayvan2.jpg" alt="Marmara Martıları">
    </div>
  </section>

  <section id="foto">
    <h2>Fotoğraflar</h2>
    <div class="image-container">
      <img src="marmara1.jpg" alt="Marmara Kıyısı">
      <img src="marmara2.jpg" alt="Marmara Kışı">
      <img src="marmara_bitki1.jpg" alt="Marmara Ayçiçeği">
      <img src="marmara_hayvan1.jpg" alt="Marmara Yaban Hayatı">
    </div>
  </section>

</div>

<script>
  function show(id) {
    document.querySelectorAll('nav button').forEach(btn => btn.classList.remove('active'));
    document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
    document.querySelector(`nav button[onclick="show('${id}')"]`).classList.add('active');
    document.getElementById(id).classList.add('active');
  }
</script>

</body>
</html>
