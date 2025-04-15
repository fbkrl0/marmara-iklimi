<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Marmara İklimi</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f4f4f4; }
    header { background: #2d3436; padding: 20px; text-align: center; color: white; }
    nav { background: #636e72; display: flex; justify-content: center; }
    nav a { color: white; padding: 15px 20px; text-decoration: none; }
    nav a:hover { background: #00cec9; }
    section { padding: 20px; display: none; }
    section.active { display: block; background: white; margin: 20px; border-radius: 10px; }
    img { width: 300px; margin: 10px; border-radius: 8px; }
  </style>
</head>
<body>

<header>
  <h1>Marmara İklimi</h1>
</header>

<nav>
  <a href="#" onclick="showSection('iklim')">İklim Özellikleri</a>
  <a href="#" onclick="showSection('bitki')">Bitki Türleri</a>
  <a href="#" onclick="showSection('hayvan')">Hayvan Türleri</a>
  <a href="#" onclick="showSection('foto')">Fotoğraflar</a>
</nav>

<section id="iklim" class="active">
  <h2>Marmara İklimi Özellikleri</h2>
  <p>Marmara iklimi, Akdeniz ve Karadeniz iklimlerinin geçiş özelliklerini taşır. Yazlar sıcak ve kurak, kışlar ise ılık ve yağışlı geçer. Yağış rejimi düzenlidir, ancak kıyıdan iç kesimlere gidildikçe karasallık artar. Sıcaklık farkları yıl içinde belirgindir. İstanbul gibi büyük şehirlerde kentsel ısı adası etkisi gözlemlenir.</p>
  <img src="marmara1.jpg" alt="Marmara İklimi 1">
  <img src="marmara2.jpg" alt="Marmara İklimi 2">
</section>

<section id="bitki">
  <h2>Marmara İkliminde Bitki Türleri</h2>
  <p>Marmara Bölgesi’nde orman, maki ve step bitki örtüsü iç içe geçmiş şekilde bulunur. Meşe, kestane, kayın, ıhlamur gibi geniş yapraklı ağaç türleri yaygındır. Ayrıca tarım açısından verimli topraklara sahiptir ve ayçiçeği, üzüm, buğday, zeytin gibi ürünler yetiştirilir.</p>
  <img src="marmara_bitki1.jpg" alt="Marmara Bitki 1">
  <img src="marmara_bitki2.jpg" alt="Marmara Bitki 2">
</section>

<section id="hayvan">
  <h2>Marmara İkliminde Hayvan Türleri</h2>
  <p>Marmara’da farklı iklimlerin etkisiyle geniş bir hayvan çeşitliliği vardır. Yaban domuzu, tilki, sansar gibi memeliler, çeşitli su kuşları ve göçmen kuşlar bölgeye özgüdür. Ayrıca kıyı ve sulak alanlarda ördek, balıkçıl, leylek gibi türler gözlemlenir. Boğaz çevresi, yunuslar ve martılar gibi deniz canlılarına da ev sahipliği yapar.</p>
  <img src="marmara_hayvan1.jpg" alt="Marmara Hayvan 1">
  <img src="marmara_hayvan2.jpg" alt="Marmara Hayvan 2">
</section>

<section id="foto">
  <h2>Tüm Fotoğraflar</h2>
  <img src="marmara1.jpg" alt="İklim 1">
  <img src="marmara2.jpg" alt="İklim 2">
  <img src="marmara_bitki1.jpg" alt="Bitki 1">
  <img src="marmara_bitki2.jpg" alt="Bitki 2">
  <img src="marmara_hayvan1.jpg" alt="Hayvan 1">
  <img src="marmara_hayvan2.jpg" alt="Hayvan 2">
</section>

<script>
  function showSection(id) {
    document.querySelectorAll('section').forEach(section => {
      section.classList.remove('active');
    });
    document.getElementById(id).classList.add('active');
  }
</script>

</body>
</html>
