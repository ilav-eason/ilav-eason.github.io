---
layout: home
title: Home
---

<style type="text/css" media="screen">
  .home-container {
    margin: 0 auto;
    max-width: 900px;
    padding: 40px 20px;
    min-height: calc(100vh - 200px);
  }

  .hero-section {
    text-align: center;
    padding: 60px 0;
    background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
    border-radius: 12px;
    margin-bottom: 40px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.1);
  }

  .hero-title {
    font-size: 3.5em;
    font-weight: 800;
    color: #42b983 !important;
    margin: 0;
    line-height: 1.2;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
  }

  .hero-subtitle {
    font-size: 1.3em;
    color: #666 !important;
    margin: 20px 0 0 0;
    font-weight: 400;
  }

  .sections-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-top: 40px;
  }

  .section-card {
    background: white;
    border-radius: 12px;
    padding: 30px;
    box-shadow: 0 4px 16px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
    border: 1px solid #e9ecef;
    position: relative;
    overflow: hidden;
  }

  .section-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 24px rgba(66, 185, 131, 0.2);
  }

  .section-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 4px;
    background: #42b983;
    border-radius: 12px 12px 0 0;
  }

  .section-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 20px;
  }

  .section-icon {
    font-size: 2em;
    color: #42b983 !important;
  }

  .section-title {
    font-size: 1.5em;
    margin: 0;
    color: #333 !important;
    font-weight: 600;
  }

  .section-content {
    color: #666 !important;
    line-height: 1.6;
    font-size: 1.1em;
  }

  .section-placeholder {
    font-style: italic;
    color: #999 !important;
    background: #f8f9fa;
    padding: 20px;
    border-radius: 8px;
    border-left: 4px solid #42b983;
    margin-top: 15px;
  }

  .intro-section {
    grid-column: 1 / -1;
    text-align: center;
    background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%);
  }

  .intro-section .section-content {
    font-size: 1.2em;
    max-width: 600px;
    margin: 0 auto;
  }

  @media (max-width: 768px) {
    .hero-title {
      font-size: 2.5em;
    }
    
    .hero-subtitle {
      font-size: 1.1em;
    }
    
    .sections-grid {
      grid-template-columns: 1fr;
      gap: 20px;
    }
    
    .section-card {
      padding: 20px;
    }
  }
</style>

<div class="home-container">
  <div class="hero-section">
    <h1 class="hero-title">ilav</h1>
    <p class="hero-subtitle">探索技术，记录成长，分享经验</p>
  </div>

  <div class="sections-grid">
    <div class="section-card intro-section">
      <div class="section-header">
        <i class="fa fa-user section-icon"></i>
        <h2 class="section-title">自我介绍</h2>
      </div>
      <div class="section-content">
        <div class="section-placeholder">
          2022届北邮网络空间安全学院本科生，CTF比赛MISC选手（我看是路边），CS2步枪手（尼永孝）。
          尼尼孩孩major冠军!
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-trophy section-icon"></i>
        <h2 class="section-title">竞赛经历</h2>
      </div>
      <div class="section-content">
        <div class="section-placeholder">
          参与的竞赛活动，包括：
          <br>• 2023届NCTF
          <br>• “赛迪·创安杯”
          <br>• 2025年18届信息安全作品赛
          <br>• 2025年第一届AI安全作品赛
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-flask section-icon"></i>
        <h2 class="section-title">科研经历</h2>
      </div>
      <div class="section-content">
        <div class="section-placeholder">
          科研项目参与经历：
          <br>•数据未脱敏，后续发布 
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-briefcase section-icon"></i>
        <h2 class="section-title">实习经历</h2>
      </div>
      <div class="section-content">
        <div class="section-placeholder">
          这里将分享实习工作经验：
          <br>• 目前正在找第一段实习。。。
        </div>
      </div>
    </div>
  </div>
</div>