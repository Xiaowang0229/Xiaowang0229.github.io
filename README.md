# 我的个人主页

<style>
  :root {
    --primary: #6366f1;
    --text: #1f2937;
    --text-light: #4b5563;
    --bg: #f8fafc;
    --card: white;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --primary: #818cf8;
      --text: #f1f5f9;
      --text-light: #94a3b8;
      --bg: #0f172a;
      --card: #1e293b;
    }
  }

  body {
    margin: 0;
    padding: 0;
    font-family: system-ui, -apple-system, BlinkMacOSystemFont, 'Segoe UI', Roboto, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
  }

  /* Header */
  header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 1.5rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);
  }

  header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    font-size: 1.6rem;
    font-weight: bold;
  }

  nav a {
    color: white;
    text-decoration: none;
    margin-left: 2rem;
    font-weight: 500;
    transition: all 0.2s;
  }

  nav a:hover {
    color: #e0e7ff;
    transform: translateY(-2px);
  }

  /* Main Content */
  .profile {
    text-align: center;
    padding: 6rem 0 4rem;
  }

  .avatar {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    object-fit: cover;
    border: 6px solid white;
    box-shadow: 0 10px 30px rgba(0,0,0,0.15);
    margin-bottom: 1.8rem;
  }

  h1 {
    font-size: 3.2rem;
    margin: 0.4rem 0;
    background: linear-gradient(90deg, #667eea, #9f7aea);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .subtitle {
    font-size: 1.3rem;
    color: var(--text-light);
    margin: 0.8rem 0 2rem;
  }

  .info {
    max-width: 680px;
    margin: 0 auto 4rem;
    font-size: 1.15rem;
  }

  /* Works Section */
  .works {
    padding: 3rem 0 5rem;
  }

  h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    position: relative;
  }

  h2:after {
    content: '';
    position: absolute;
    width: 80px;
    height: 4px;
    background: var(--primary);
    bottom: -12px;
    left: 50%;
    transform: translateX(-50%);
    border-radius: 2px;
  }

  .works-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 2rem;
  }

  .work-card {
    background: var(--card);
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1), 0 2px 4px -1px rgba(0,0,0,0.06);
    transition: all 0.3s ease;
  }

  .work-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 25px -5px rgba(0,0,0,0.1), 0 10px 10px -5px rgba(0,0,0,0.04);
  }

  .work-img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }

  .work-content {
    padding: 1.5rem;
  }

  .work-title {
    margin: 0 0 0.6rem;
    font-size: 1.35rem;
  }

  .work-desc {
    color: var(--text-light);
    font-size: 0.98rem;
    margin: 0;
  }

  /* Footer */
  footer {
    background: #111827;
    color: #9ca3af;
    text-align: center;
    padding: 3rem 0 2rem;
    margin-top: 4rem;
  }

  .social-links a {
    color: #9ca3af;
    margin: 0 1rem;
    font-size: 1.6rem;
    transition: color 0.2s;
  }

  .social-links a:hover {
    color: white;
  }
</style>

<div class="container">

<header>
  <div class="container">
    <div class="logo">关于我</div>
    <nav>
      <a href="#home">首页</a>
      <a href="#works">作品</a>
      <a href="#contact">联系</a>
    </nav>
  </div>
</header>

<main>

  <section class="profile" id="home">
    <img 
      src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=400&h=400&fit=crop" 
      alt="我的头像" 
      class="avatar"
    >
    
    <h1>珈蓝yaa_</h1>
    <div class="subtitle">又菜又爱玩的B站小Up | 目前掌握：Py,C#,C++,Forms,WPF,WinUI3</div>
    
    <div class="info">
      <p>目前主要在开发C#相关的程序</p>
    </div>
  </section>

  <section class="works" id="works">
    <h2>已发布作品</h2>
    
    <div class="works-grid">
      <div class="work-card">
        <img src="9" alt="项目1" class="work-img">
        <div class="work-content">
          <h3 class="work-title">测试</h3>
          <p class="work-desc">测试</p>
        </div>
      </div>

     
    </div>
  </section>

</main>

<footer>
  <div class="social-links">
    <a href="https://github.com" target="_blank">GitHub</a> •
    <a href="https://bilibili.com" target="_blank">B站</a>
  </div>
  <p style="margin-top:1.5rem;">© 2026 珈蓝yaa_ · 版权所有，请勿盗用样式</p>
</footer>

</div>
