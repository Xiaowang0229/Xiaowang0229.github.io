<style>
  :root {
    --primary: #00a1d6;
    --primary-dark: #008ab8;
    --text: #18191c;
    --text-light: #505050;
    --bg: #f6f7f9;
    --card: white;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --primary: #00d1ff;
      --primary-dark: #00b0d9;
      --text: #e5e6eb;
      --text-light: #9ca3af;
      --bg: #0e1117;
      --card: #161b22;
    }
  }

  body {
    margin: 0;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
  }

  .container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
  }

  header {
    background: linear-gradient(135deg, #00a1d6 0%, #0077aa 100%);
    color: white;
    padding: 1.2rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 10px rgba(0,0,0,0.15);
  }

  .header-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    font-size: 1.9rem;
    font-weight: bold;
  }

  nav a {
    color: white;
    text-decoration: none;
    margin-left: 2.2rem;
    font-weight: 500;
  }

  nav a:hover {
    color: #e6faff;
  }

  .profile {
    text-align: center;
    padding: 7rem 0 5rem;
  }

  .avatar {
    width: 170px;
    height: 170px;
    border-radius: 50%;
    border: 5px solid var(--card);
    box-shadow: 0 10px 35px rgba(0,0,0,0.2);
    object-fit: cover;
    margin-bottom: 1.8rem;
  }

  h1 {
    font-size: 3.4rem;
    margin: 0.3rem 0;
    background: linear-gradient(90deg, #00a1d6, #ff85a2);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .subtitle {
    font-size: 1.35rem;
    color: var(--text-light);
    margin: 0.6rem 0 1.5rem;
  }

  .info {
    max-width: 720px;
    margin: 0 auto 2.5rem;
    font-size: 1.1rem;
    color: var(--text-light);
  }

  .works {
    padding: 3rem 0 5rem;
  }

  h2 {
    text-align: center;
    font-size: 2.6rem;
    margin-bottom: 3rem;
    position: relative;
  }

  h2:after {
    content: '';
    position: absolute;
    width: 90px;
    height: 4px;
    background: var(--primary);
    bottom: -12px;
    left: 50%;
    transform: translateX(-50%);
    border-radius: 2px;
  }

  .works-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
    gap: 2rem;
  }

  .work-card {
    background: var(--card);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 15px rgba(0,0,0,0.08);
    transition: all 0.3s ease;
  }

  .work-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.12);
  }

  .work-img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }

  .work-content {
    padding: 1.4rem;
  }

  .work-title {
    margin: 0 0 0.7rem;
    font-size: 1.32rem;
  }

  .work-desc {
    color: var(--text-light);
    font-size: 0.97rem;
    margin: 0;
  }

  footer {
    background: #0f1117;
    color: #8a8f98;
    text-align: center;
    padding: 3rem 0 2rem;
    margin-top: 4rem;
  }

  .social a {
    color: #8a8f98;
    margin: 0 1.2rem;
    font-size: 1.6rem;
    text-decoration: none;
  }

  .social a:hover {
    color: white;
  }

  @media (max-width: 768px) {
    .profile { padding: 5rem 0 3rem; }
    h1 { font-size: 2.6rem; }
    .avatar { width: 140px; height: 140px; }
    .works-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="container">

<header>
  <div class="header-inner">
    <div class="logo">珈蓝yaa</div>
    <nav>
      <a href="#home">首页</a>
      <a href="#works">创作</a>
      <a href="https://space.bilibili.com/3546926523877748" target="_blank">B站</a>
    </nav>
  </div>
</header>

<main>

<section class="profile" id="home">

  <img 
    src="https://github.com/Xiaowang0229/Xiaowang0229.github.io/blob/main/bbcb5f8e36f816dd6f08d5a8768955488c29910d.jpg@128w_128h_1c_1s.webp?raw=true" 
    alt="珈蓝yaa" 
    class="avatar">

  <h1>珈蓝yaa</h1>
  <div class="subtitle">又菜又爱玩的B站小Up | 目前掌握：Py,C#,C++,Forms,WPF,WinUI3</div>

  <div class="info">
    
  </div>

</section>

<section class="works" id="works">

  <h2>个人项目</h2>

  <div class="works-grid">

    <div class="work-card">
      <img src="" alt="1" class="work-img">
      <div class="work-content">
        <h3 class="work-title">了！</h3>
        <p class="work-desc">ax</p>
      </div>
    </div>

    

  </div>

</section>

</main>

<footer>
  <div class="social">
    <a href="https://space.bilibili.com/3546926523877748" target="_blank">Bilibili</a> •
    <a href="https://github.com/Xiaowang0229" target="_blank">Github</a>
  </div>
  <p style="margin-top:1.8rem;">© 2026 珈蓝yaa · 今天也要开心摸鱼哦</p>
</footer>

</div>
