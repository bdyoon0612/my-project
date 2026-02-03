<svelte:head>
  <title>TennisPro - 프리미엄 코트 예약</title>
</svelte:head>

<section class="hero">
  <div class="hero-bg"></div>
  <div class="container hero-content">
    <div class="badge">새 시즌 오픈</div>
    <h1>최고의 코트에서<br><span class="gradient-text">완벽한 플레이를</span></h1>
    <p>궁극의 테니스 예약 시스템을 경험해보세요. 실시간 예약, 전문 코칭, 그리고 다이내믹한 토너먼트가 당신을 기다립니다.</p>
    <div class="buttons">
      <button class="btn btn-primary">코트 찾기</button>
      <button class="btn btn-outline">레슨 살펴보기</button>
    </div>
    
    <div class="stats">
      <div class="stat-item">
        <span class="stat-num">12</span>
        <span class="stat-label">프로 코트</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">50+</span>
        <span class="stat-label">코치진</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">24/7</span>
        <span class="stat-label">상시 오픈</span>
      </div>
    </div>
  </div>
</section>

<section class="features">
  <div class="container">
    <h2 class="section-title">TennisPro를 선택해야 하는 이유</h2>
    <p class="section-subtitle">당신의 플레이를 한 단계 더 높여드립니다.</p>
    
    <div class="grid">
      <div class="card">
        <div class="icon">🎾</div>
        <h3>스마트 예약</h3>
        <p>실시간 예약 엔진으로 원하는 코트를 몇 초 만에 예약하세요.</p>
      </div>
      <div class="card">
        <div class="icon">🏆</div>
        <h3>토너먼트</h3>
        <p>지역 리그와 토너먼트에 참여하세요. 랭킹을 올리고 실력을 증명하세요.</p>
      </div>
      <div class="card">
        <div class="icon">⚡</div>
        <h3>전문 코칭</h3>
        <p>공인 코치들과 함께 1:1 레슨이나 그룹 클리닉을 시작하세요.</p>
      </div>
    </div>
  </div>
</section>

<section class="cta">
  <div class="container">
    <div class="cta-card">
      <h2>준비 되셨나요?</h2>
      <p>매일 TennisPro를 이용하는 5,000명 이상의 플레이어와 함께하세요.</p>
      <button class="btn btn-primary">멤버십 가입하기</button>
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
    background: radial-gradient(circle at 10% 20%, rgba(139, 195, 74, 0.1) 0%, transparent 40%),
                radial-gradient(circle at 90% 80%, rgba(6, 182, 212, 0.1) 0%, transparent 40%);
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
    background: rgba(139, 195, 74, 0.1);
    color: var(--primary);
    border-radius: 20px;
    font-weight: 600;
    margin-bottom: 1.5rem;
    border: 1px solid rgba(139, 195, 74, 0.2);
  }

  h1 {
    font-size: 4.5rem;
    line-height: 1.1;
    margin-bottom: 1.5rem;
    font-weight: 800;
    color: var(--text-main);
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
    border-top: 1px solid rgba(0, 0, 0, 0.05);
    padding-top: 2rem;
  }

  .stat-item {
    display: flex;
    flex-direction: column;
  }

  .stat-num {
    font-size: 2rem;
    font-weight: 700;
    color: var(--text-main);
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
    background: var(--bg-secondary);
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
    box-shadow: var(--shadow-sm);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border: 1px solid rgba(0,0,0,0.03);
  }

  .card:hover {
    transform: translateY(-10px);
    box-shadow: var(--shadow-lg);
  }

  .icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
  }

  .card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: var(--text-main);
  }

  .card p {
    color: var(--text-muted);
  }

  /* CTA Section */
  .cta {
    padding: 6rem 0;
  }

  .cta-card {
    background: linear-gradient(135deg, #f8fafc, #eff6ff);
    padding: 4rem;
    border-radius: 32px;
    text-align: center;
    border: 1px solid rgba(0,0,0,0.05);
    position: relative;
    overflow: hidden;
    box-shadow: var(--shadow-md);
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
    color: var(--text-main);
  }

  .cta-card p {
    color: var(--text-muted);
    font-size: 1.25rem;
    margin-bottom: 2rem;
  }
</style>
