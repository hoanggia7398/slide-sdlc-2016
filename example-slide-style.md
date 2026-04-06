---
marp: true
html: true
size: 16:9
paginate: true
style: |
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap');

  section {
    font-family: 'Inter', sans-serif;
    background: radial-gradient(circle at 0% 0%, #111827 0%, #030712 100%);
    color: #f1f5f9;
    padding: 60px 80px;
    font-size: 24px;
  }

  /* Header Styles */
  .header {
    margin-bottom: 40px;
    border-left: 4px solid #38bdf8;
    padding-left: 24px;
  }

  .eyebrow {
    font-size: 14px;
    font-weight: 800;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: #38bdf8;
    margin-bottom: 8px;
    opacity: 0.8;
  }

  h1 {
    font-size: 56px;
    font-weight: 800;
    line-height: 1.1;
    background: linear-gradient(to right, #f8fafc, #94a3b8);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 0;
  }

  h2 {
    color: #7dd3fc;
    font-size: 28px;
    margin-top: 0;
  }

  /* Content Structures */
  .content {
    display: grid;
    grid-template-columns: 1fr 1.2fr;
    gap: 48px;
    align-items: center;
  }

  .points {
    list-style: none;
    padding: 0;
  }

  .points li {
    position: relative;
    padding-left: 32px;
    margin-bottom: 16px;
    color: #cbd5e1;
  }

  .points li::before {
    content: "→";
    position: absolute;
    left: 0;
    color: #38bdf8;
    font-weight: bold;
  }

  /* Flow Diagram Styles */
  .flow {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: rgba(255, 255, 255, 0.03);
    padding: 30px;
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.05);
  }

  .node {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 8px;
  }

  .node-box {
    width: 100px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #1e293b;
    border: 1px solid #334155;
    border-radius: 12px;
    font-size: 14px;
    font-weight: 600;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    transition: all 0.3s ease;
  }

  .node:hover .node-box {
    border-color: #38bdf8;
    transform: translateY(-2px);
    box-shadow: 0 0 20px rgba(56, 189, 248, 0.2);
  }

  .step-num {
    font-size: 12px;
    color: #38bdf8;
    font-family: monospace;
  }

  .arrow-icon {
    color: #475569;
    font-size: 20px;
  }

  /* Cards & Comparisons */
  .compare {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 32px;
  }

  .card {
    padding: 32px;
    border-radius: 20px;
    background: linear-gradient(145deg, rgba(30, 41, 59, 0.7), rgba(15, 23, 42, 0.8));
    border: 1px solid rgba(56, 189, 248, 0.1);
    backdrop-filter: blur(10px);
  }

  .card.highlight {
    border: 1px solid rgba(56, 189, 248, 0.4);
    background: linear-gradient(145deg, rgba(30, 41, 59, 0.9), rgba(15, 23, 42, 1));
  }

  footer {
    font-size: 12px;
    color: #475569;
  }
  /* Grid 3 Columns */
  .grid-3 {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 32px;
  }

  /* Stat Cards for Metrics */
  .stat-card {
    text-align: center;
    padding: 40px 24px;
    background: linear-gradient(180deg, rgba(30, 41, 59, 0.6) 0%, rgba(15, 23, 42, 0.2) 100%);
    border-radius: 20px;
    border: 1px dashed rgba(56, 189, 248, 0.3);
    transition: transform 0.3s;
  }

  .stat-num {
    font-size: 72px;
    font-weight: 800;
    background: linear-gradient(to right, #38bdf8, #818cf8);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    line-height: 1;
    margin-bottom: 16px;
  }

  .stat-label {
    font-size: 18px;
    color: #94a3b8;
    font-weight: 600;
  }

  /* Quote / Statement Layout */
  .quote-wrapper {
    text-align: center;
    max-width: 850px;
    margin: 60px auto 0;
  }

  .quote-text {
    font-size: 42px;
    font-weight: 600;
    line-height: 1.4;
    color: #f1f5f9;
  }

  .quote-text::before, .quote-text::after {
    content: '"';
    color: #38bdf8;
    opacity: 0.5;
  }

  .quote-author {
    margin-top: 32px;
    color: #7dd3fc;
    font-size: 16px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
  }
---

<div class="header">
  <div class="eyebrow">Vision 2026</div>
  <h1>Modern AI <br/>Architecture Patterns</h1>
</div>

<div style="margin-top: 60px; color: #64748b;">
  Press → to explore layout examples
</div>

---

<div class="header">
  <div class="eyebrow">Perspective</div>
  <h1>AI changes how we <br/>build software</h1>
</div>

<div class="content" style="grid-template-columns: 1fr;">
  <ul class="points" style="font-size: 32px; display: grid; grid-template-columns: 1fr 1fr; gap: 20px;">
    <li>Execution is automated</li>
    <li>Thinking becomes leverage</li>
    <li>Context is advantage</li>
    <li>Speed is expectation</li>
  </ul>
</div>

---

<div class="header">
  <div class="eyebrow">Infrastructure</div>
  <h1>Request Pipeline</h1>
</div>

<div class="content">
  <div>
    <h2 style="font-size: 24px; color: #94a3b8;">Streamlined Processing</h2>
    <ul class="points" style="font-size: 18px;">
      <li><strong>Input:</strong> User intent capture</li>
      <li><strong>Process:</strong> Context orchestration</li>
      <li><strong>Output:</strong> LLM generation</li>
      <li><strong>Review:</strong> Human-in-the-loop</li>
    </ul>
  </div>

  <div class="flow">
    <div class="node"><span class="step-num">01</span><div class="node-box">Input</div></div>
    <div class="arrow-icon">→</div>
    <div class="node"><span class="step-num">02</span><div class="node-box">Process</div></div>
    <div class="arrow-icon">→</div>
    <div class="node"><span class="step-num">03</span><div class="node-box">Output</div></div>
  </div>
</div>

---

<div class="header">
  <div class="eyebrow">Efficiency</div>
  <h1>Transformation Paradigm</h1>
</div>

<div class="compare">
  <div class="card">
    <h2 style="color: #94a3b8;">Traditional</h2>
    <ul class="points" style="font-size: 18px;">
      <li>Manual analysis & tagging</li>
      <li>Slow, linear iterations</li>
      <li>Human scale limitations</li>
    </ul>
  </div>

  <div class="card highlight">
    <h2 style="color: #38bdf8;">AI-Augmented</h2>
    <ul class="points" style="font-size: 18px;">
      <li>Agentic reasoning flows</li>
      <li>Rapid parallel iteration</li>
      <li>Exponential output growth</li>
    </ul>
  </div>
</div>

---

<div class="header">
  <div class="eyebrow">Core Pillars</div>
  <h1>Architecture Principles</h1>
</div>

<div class="grid-3">
  <div class="card">
    <h2 style="font-size: 20px; color: #f8fafc;">1. Scalability</h2>
    <p style="color: #94a3b8; font-size: 16px; line-height: 1.6;">
      Hệ thống được thiết kế để mở rộng ngang linh hoạt, tự động cấp phát tài nguyên khi traffic tăng đột biến.
    </p>
  </div>

  <div class="card">
    <h2 style="font-size: 20px; color: #f8fafc;">2. Resilience</h2>
    <p style="color: #94a3b8; font-size: 16px; line-height: 1.6;">
      Cơ chế failover tự động đảm bảo zero-downtime ngay cả khi một node trong cluster gặp sự cố.
    </p>
  </div>

  <div class="card">
    <h2 style="font-size: 20px; color: #f8fafc;">3. Security</h2>
    <p style="color: #94a3b8; font-size: 16px; line-height: 1.6;">
      Mã hóa end-to-end kết hợp với Zero Trust network topology để bảo vệ dữ liệu ở mọi layer.
    </p>
  </div>
</div>

---

<div class="header">
  <div class="eyebrow">Impact & Results</div>
  <h1>Performance Gains</h1>
</div>

<div class="grid-3" style="margin-top: 40px;">
  <div class="stat-card">
    <div class="stat-num">10x</div>
    <div class="stat-label">Faster Deployment</div>
  </div>
  
  <div class="stat-card">
    <div class="stat-num">99.9%</div>
    <div class="stat-label">System Uptime</div>
  </div>
  
  <div class="stat-card">
    <div class="stat-num">-40%</div>
    <div class="stat-label">Infrastructure Cost</div>
  </div>
</div>

---

<div class="quote-wrapper">
  <div class="quote-text">
    The future of software engineering isn't writing code. It's guiding intelligent systems to solve complex problems.
  </div>
  <div class="quote-author">
    — Tech Vision 2026
  </div>
</div>
