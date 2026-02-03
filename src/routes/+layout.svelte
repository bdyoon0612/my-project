<script>
  import '../app.css';
</script>

<div class="app">
  <header>
    <div class="container nav-container">
      <div class="logo">Tennis<span class="highlight">Pro</span></div>
      <nav>
        <a href="/">홈</a>
        <a href="/courts">코트 예약</a>
        <a href="/lessons">레슨</a>
        <a href="/tournaments">대회</a>
      </nav>
      <div class="auth-buttons">
        <button class="btn btn-primary">지금 예약하기</button>
      </div>
    </div>
  </header>

  <main>
    <slot />
  </main>

  <footer>
    <div class="container footer-content">
      <div class="footer-col">
        <h3>TennisPro</h3>
        <p>최고의 코트와 코칭으로 당신의 게임을 업그레이드하세요.</p>
      </div>
      <div class="footer-col">
        <h4>링크</h4>
        <a href="/">회사 소개</a>
        <a href="/">문의하기</a>
        <a href="/">개인정보 처리방침</a>
      </div>
      <div class="footer-col">
        <p>&copy; 2024 TennisPro Systems. All rights reserved.</p>
      </div>
    </div>
  </footer>
</div>

<style>
  header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 100;
    background: rgba(255, 255, 255, 0.9);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(0, 0, 0, 0.05);
    box-shadow: 0 2px 10px rgba(0,0,0,0.02);
  }

  .nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;
  }

  .logo {
    font-size: 1.5rem;
    font-weight: 800;
    color: var(--text-main);
  }

  .highlight {
    color: var(--primary);
  }

  nav {
    display: flex;
    gap: 2rem;
  }

  nav a {
    font-weight: 500;
    color: var(--text-muted);
    transition: color 0.3s;
  }

  nav a:hover {
    color: var(--primary);
  }

  main {
    padding-top: 80px;
    min-height: 100vh;
  }

  footer {
    background: var(--bg-secondary);
    padding: 4rem 0;
    margin-top: 4rem;
    border-top: 1px solid rgba(0,0,0,0.05);
  }

  .footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 3rem;
  }

  .footer-col h3 {
    margin-bottom: 1rem;
    color: var(--text-main);
  }
  
  .footer-col h4 {
    margin-bottom: 1rem;
    color: var(--primary);
  }

  .footer-col a {
    display: block;
    margin-bottom: 0.5rem;
    color: var(--text-muted);
  }
  
  .footer-col a:hover {
    color: var(--primary);
  }
</style>
