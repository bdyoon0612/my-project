<svelte:head>
  <title>TennisPro - Premium Court Booking</title>
</svelte:head>

<section class="hero">
  <div class="hero-bg"></div>
  <div class="container hero-content">
    <div class="badge">New Season Open</div>
    <h1>Master Your Game on <br><span class="gradient-text">Premium Courts</span></h1>
    <p>Experience the ultimate tennis reservation system. Real-time booking, pro coaching, and dynamic tournaments at your fingertips.</p>
    <div class="buttons">
      <button class="btn btn-primary">Find a Court</button>
      <button class="btn btn-outline">Explore Lessons</button>
    </div>
    
    <div class="stats">
      <div class="stat-item">
        <span class="stat-num">12</span>
        <span class="stat-label">Pro Courts</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">50+</span>
        <span class="stat-label">Coaches</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">24/7</span>
        <span class="stat-label">Access</span>
      </div>
    </div>
  </div>
</section>

<section class="features">
  <div class="container">
    <h2 class="section-title">Why Choose TennisPro</h2>
    <p class="section-subtitle">Everything you need to elevate your play.</p>
    
    <div class="grid">
      <div class="card">
        <div class="icon">🎾</div>
        <h3>Smart Booking</h3>
        <p>Book your favorite court in seconds with our real-time availability engine.</p>
      </div>
      <div class="card">
        <div class="icon">🏆</div>
        <h3>Tournaments</h3>
        <p>Join local leagues and tournaments. Track your ranking and progress.</p>
      </div>
      <div class="card">
        <div class="icon">⚡</div>
        <h3>Pro Coaching</h3>
        <p>Connect with certified coaches for 1:1 lessons or group clinics.</p>
      </div>
    </div>
  </div>
</section>

<section class="cta">
  <div class="container">
    <div class="cta-card">
      <h2>Ready to Play?</h2>
      <p>Join over 5,000 players who trust TennisPro for their daily game.</p>
      <button class="btn btn-primary">Join Membership</button>
    </div>
  </div>
</section>

<style>
  /* Hero Section */
  .hero {
    position: relative;
    height: 90vh;
    display: flex;
    align-items: center;
    overflow: hidden;
  }

  .hero-bg {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle at 10% 20%, rgba(204, 255, 0, 0.1) 0%, transparent 40%),
                radial-gradient(circle at 90% 80%, rgba(139, 92, 246, 0.15) 0%, transparent 40%);
    z-index: -1;
  }

  .hero-content {
    max-width: 800px;
    position: relative;
    z-index: 1;
  }

  .badge {
    display: inline-block;
    padding: 0.5rem 1rem;
    background: rgba(204, 255, 0, 0.1);
    color: var(--primary);
    border-radius: 20px;
    font-weight: 600;
    margin-bottom: 1.5rem;
    border: 1px solid rgba(204, 255, 0, 0.2);
  }

  h1 {
    font-size: 4.5rem;
    line-height: 1.1;
    margin-bottom: 1.5rem;
    font-weight: 800;
  }

  .gradient-text {
    background: var(--gradient-main);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .hero p {
    font-size: 1.25rem;
    color: var(--text-muted);
    margin-bottom: 2.5rem;
    max-width: 600px;
  }

  .buttons {
    display: flex;
    gap: 1rem;
    margin-bottom: 4rem;
  }

  .stats {
    display: flex;
    gap: 4rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    padding-top: 2rem;
  }

  .stat-item {
    display: flex;
    flex-direction: column;
  }

  .stat-num {
    font-size: 2rem;
    font-weight: 700;
    color: white;
  }

  .stat-label {
    color: var(--text-muted);
    font-size: 0.9rem;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  /* Features Section */
  .features {
    padding: 6rem 0;
    background: var(--dark-bg);
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
  }

  .card {
    background: var(--card-bg);
    padding: 2.5rem;
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.05);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
    border-color: rgba(204, 255, 0, 0.2);
  }

  .icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
  }

  .card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: white;
  }

  .card p {
    color: var(--text-muted);
  }

  /* CTA Section */
  .cta {
    padding: 6rem 0;
  }

  .cta-card {
    background: linear-gradient(135deg, #1e293b, #0f172a);
    padding: 4rem;
    border-radius: 32px;
    text-align: center;
    border: 1px solid rgba(255, 255, 255, 0.1);
    position: relative;
    overflow: hidden;
  }
  
  .cta-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 5px;
    background: var(--gradient-main);
  }

  .cta-card h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .cta-card p {
    color: var(--text-muted);
    font-size: 1.25rem;
    margin-bottom: 2rem;
  }
</style>
