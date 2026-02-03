<script>
  import '../app.css';
</script>

<div class="app">
  <header>
    <div class="container nav-container">
      <div class="logo">Tennis<span class="highlight">Pro</span></div>
      <nav>
        <a href="/">Home</a>
        <a href="/courts">Courts</a>
        <a href="/lessons">Lessons</a>
        <a href="/tournaments">Tournaments</a>
      </nav>
      <div class="auth-buttons">
        <button class="btn btn-primary">Book Now</button>
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
        <p>Elevate your game with premium courts and coaching.</p>
      </div>
      <div class="footer-col">
        <h4>Links</h4>
        <a href="/">About Us</a>
        <a href="/">Contact</a>
        <a href="/">Privacy</a>
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
    background: rgba(15, 23, 42, 0.8);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
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
    color: white;
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
    background: var(--card-bg);
    padding: 4rem 0;
    margin-top: 4rem;
  }

  .footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 3rem;
  }

  .footer-col h3 {
    margin-bottom: 1rem;
    color: white;
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
    color: white;
  }
</style>
