photography-portfolio/
│
├─ index.html        首页
├─ portfolio.html    作品集
├─ about.html        关于我
├─ contact.html      联系方式
│
├─ css/
│   └─ style.css
│
├─ images/
│   ├─ hero.jpg          首页背景（占位）
│   ├─ avatar.jpg        头像（占位）
│   ├─ city/
│   ├─ wild/
│   ├─ light/
│   └─ life/
│
└─ js/
    └─ main.js
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>波波 · 摄影作品集</title>
  <link rel="stylesheet" href="css/style.css">
  <link href="https://fonts.googleapis.com/css2?family=Baloo+2:wght@600&family=Poppins&display=swap" rel="stylesheet">
</head>
<body class="home">
  <section class="hero">
    <div class="hero-text">
      <h1>波波</h1>
      <p>摄影作品集</p>
    </div>
  </section>
</body>
</html>
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>作品集 · 波波</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <h2 class="page-title">作品集</h2>

  <section class="grid">
    <div class="project large city">
      <h3>城市建筑</h3>
      <p>记录钢筋水泥中隐藏的秩序与节奏。</p>
    </div>

    <div class="project wild">
      <h3>旷野遐想</h3>
      <p>远离城市，回归自然的呼吸。</p>
    </div>

    <div class="project light">
      <h3>建筑光影</h3>
      <p>光线塑造空间的瞬间。</p>
    </div>

    <div class="project life">
      <h3>生活碎片</h3>
      <p>平凡日常里的温度与故事。</p>
    </div>
  </section>
</body>
</html>
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>关于我 · 波波</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <section class="about">
    <img src="images/avatar.jpg" class="avatar">
    <div class="bio">
      <h2>关于我</h2>
      <p>
        我叫波波，是一名专注于视觉叙事的摄影师。
        我的创作横跨城市建筑、自然风景与日常生活。
        摄影于我而言，不只是记录，而是理解世界的一种方式。
        多年来，我不断在快节奏的都市与静谧的旷野之间切换视角，
        用镜头捕捉那些容易被忽略的瞬间。
        我相信画面可以安静地讲故事，
        也可以在一瞬间击中人心。
      </p>
    </div>
  </section>
</body>
</html>
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>联系我 · 波波</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <section class="contact">
    <form class="contact-form">
      <input type="text" placeholder="姓名">
      <input type="email" placeholder="邮箱">
      <textarea placeholder="留言"></textarea>
      <button>发送</button>
    </form>

    <div class="social">
      <a href="#">QQ</a>
      <a href="#">WeChat</a>
      <a href="#">Behance</a>
    </div>
  </section>
</body>
</html>
body {
  margin: 0;
  font-family: 'Poppins', sans-serif;
  background: #fff;
  color: #111;
}

.hero {
  height: 100vh;
  background: url("../images/hero.jpg") center/cover;
  display: flex;
  justify-content: center;
  align-items: center;
}

.hero-text h1 {
  font-family: 'Baloo 2';
  font-size: 5rem;
  color: #fff;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 40px;
}

.project {
  padding: 30px;
  background: #f4f4f4;
}