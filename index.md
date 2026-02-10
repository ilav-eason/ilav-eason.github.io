---
layout: home
title: Home
---

<style type="text/css" media="screen">
  .home-container {
    margin: 0 auto;
    max-width: 1100px;
    padding: 60px 40px;
    min-height: calc(100vh - 200px);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  }

  .header-section {
    text-align: center;
    padding: 80px 0;
    background: #ffffff;
    border-bottom: 3px solid #1a365d;
    margin-bottom: 50px;
  }

  .main-title {
    font-size: 3em;
    font-weight: 700;
    color: #1a365d !important;
    margin: 0;
    letter-spacing: 2px;
    text-transform: uppercase;
  }

  .subtitle {
    font-size: 1.2em;
    color: #4a5568 !important;
    margin: 15px 0 0 0;
    font-weight: 400;
    letter-spacing: 1px;
  }

  .divider {
    width: 80px;
    height: 3px;
    background: #c53030;
    margin: 30px auto;
  }

  .profile-section {
    background: #f7fafc;
    padding: 40px;
    border-left: 4px solid #1a365d;
    margin-bottom: 50px;
    border-radius: 4px;
  }

  .profile-section h2 {
    font-size: 1.8em;
    color: #1a365d !important;
    margin: 0 0 20px 0;
    font-weight: 600;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .profile-section .section-icon {
    color: #1a365d !important;
  }

  .profile-content {
    color: #2d3748 !important;
    line-height: 1.8;
    font-size: 1.05em;
    text-align: justify;
  }

  .sections-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 30px;
    margin-top: 30px;
  }

  .section-card {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    padding: 35px 30px;
    transition: all 0.3s ease;
    position: relative;
    border-radius: 2px;
  }

  .section-card:hover {
    border-color: #1a365d;
    box-shadow: 0 4px 12px rgba(26, 54, 93, 0.1);
  }

  .section-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 4px;
    background: #1a365d;
  }

  .section-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 25px;
    padding-bottom: 15px;
    border-bottom: 1px solid #e2e8f0;
  }

  .section-icon {
    font-size: 1.8em;
    color: #1a365d !important;
  }

  .section-title {
    font-size: 1.4em;
    margin: 0;
    color: #1a365d !important;
    font-weight: 600;
    letter-spacing: 0.5px;
  }

  .section-content {
    color: #4a5568 !important;
    line-height: 1.8;
    font-size: 1em;
  }

  .section-content ul {
    margin: 15px 0;
    padding-left: 25px;
  }

  .section-content li {
    margin: 10px 0;
    color: #4a5568 !important;
  }

  .section-content strong {
    color: #2d3748 !important;
    font-weight: 600;
  }

  .highlight {
    background: #edf2f7;
    padding: 15px 20px;
    border-left: 3px solid #c53030;
    margin: 15px 0;
    font-style: italic;
    color: #4a5568 !important;
  }

  .status-badge {
    display: inline-block;
    padding: 4px 12px;
    background: #1a365d;
    color: #ffffff !important;
    font-size: 0.85em;
    border-radius: 2px;
    margin-left: 10px;
  }

  .contact-section {
    background: #1a365d;
    color: #ffffff;
    padding: 40px;
    margin-top: 50px;
    text-align: center;
    border-radius: 2px;
  }

  .contact-section h2 {
    color: #ffffff !important;
    margin: 0 0 15px 0;
    font-weight: 600;
  }

  .contact-section p {
    color: #cbd5e0 !important;
    margin: 10px 0;
    font-size: 1.1em;
  }

  .contact-section a {
    color: #ffffff !important;
    text-decoration: underline;
  }

  @media (max-width: 768px) {
    .home-container {
      padding: 40px 20px;
    }

    .main-title {
      font-size: 2.2em;
    }

    .subtitle {
      font-size: 1em;
    }

    .sections-grid {
      grid-template-columns: 1fr;
      gap: 25px;
    }

    .section-card {
      padding: 25px 20px;
    }

    .profile-section {
      padding: 30px 25px;
    }
  }
</style>

<div class="home-container">
  <div class="header-section">
    <h1 class="main-title">Ilav</h1>
    <div class="divider"></div>
    <p class="subtitle">网络空间安全 · 学术研究 · 技术分享</p>
  </div>

  <div class="profile-section">
    <h2><i class="fa fa-user section-icon"></i>个人简介</h2>
    <div class="profile-content">
      <p>
        北京邮电大学网络空间安全学院2022届本科生，专注于<strong>网络安全</strong>与<strong>人工智能安全</strong>领域的研究与实践。
        在学术研究中，重点关注网络攻防技术、漏洞分析与安全防护体系建设。
      </p>
      <p>
        作为CTF竞赛参与者，主要参与<strong>MISC（杂项）</strong>方向的技术挑战，涵盖隐写术、流量分析、逆向工程等多个技术领域。
        同时具备<strong>团队协作</strong>与<strong>问题解决</strong>能力，在实践中不断深化对网络安全的理解。
      </p>
      <p>
        致力于将理论知识与实际应用相结合，通过技术博客分享学习心得与实践经验，与同行交流探讨前沿安全话题。
      </p>
    </div>
  </div>

  <div class="sections-grid">
    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-trophy section-icon"></i>
        <h2 class="section-title">竞赛经历</h2>
      </div>
      <div class="section-content">
        <ul>
          <li><strong>2023届 NCTF</strong> - 参与网络安全竞赛，提升实战能力</li>
          <li><strong>赛迪·创安杯</strong> - 网络安全专项竞赛</li>
          <li><strong>第18届信息安全作品赛</strong> - 信息安全创新作品竞赛</li>
          <li><strong>第一届AI安全作品赛</strong> - 人工智能安全领域竞赛</li>
        </ul>
        <div class="highlight">
          通过各类竞赛活动，持续强化技术实践能力与团队协作经验。
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-flask section-icon"></i>
        <h2 class="section-title">科研经历</h2>
      </div>
      <div class="section-content">
        <p>
          积极参与网络安全相关科研项目，研究方向涵盖：
        </p>
        <ul>
          <li><strong>网络安全攻防技术</strong> - 深入研究各类攻击手段与防护策略</li>
          <li><strong>漏洞分析与挖掘</strong> - 系统性学习漏洞发现与利用方法</li>
          <li><strong>安全检测技术</strong> - 探索自动化安全检测方案</li>
        </ul>
        <div class="highlight">
          具体项目成果待数据脱敏处理后发布。
        </div>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-book section-icon"></i>
        <h2 class="section-title">研究方向</h2>
      </div>
      <div class="section-content">
        <ul>
          <li><strong>CTF技术</strong> - 二进制安全、Web安全、密码学</li>
          <li><strong>漏洞挖掘</strong> - 静态分析、动态分析、模糊测试</li>
          <li><strong>AI安全</strong> - 对抗样本、模型鲁棒性、隐私保护</li>
          <li><strong>安全工程</strong> - 安全开发、渗透测试、安全运维</li>
        </ul>
      </div>
    </div>

    <div class="section-card">
      <div class="section-header">
        <i class="fa fa-briefcase section-icon"></i>
        <h2 class="section-title">实习经历</h2>
        <span class="status-badge">寻求机会</span>
      </div>
      <div class="section-content">
        <p>
          正在积极寻求网络安全领域的实习机会，期望在以下方向获得实践经验：
        </p>
        <ul>
          <li>安全研究岗位</li>
          <li>渗透测试工程师</li>
          <li>安全开发工程师</li>
          <li>安全运营分析</li>
        </ul>
        <div class="highlight">
          如有相关机会，欢迎联系交流。
        </div>
      </div>
    </div>
  </div>

  <div class="contact-section">
    <h2>联系方式</h2>
    <p>Email: <a href="mailto:easonilav@gmail.com">easonilav@gmail.com</a></p>
    <p>GitHub: <a href="https://github.com/ilav-eason" target="_blank">ilav-eason</a></p>
  </div>
</div>
