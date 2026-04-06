---
marp: true
html: true
size: 16:9
paginate: true
style: |
  section {
    background-color: #030712;
    background-image: radial-gradient(circle at 0% 0%, #111827 0%, #030712 100%);
    color: #f1f5f9;
    padding: 60px 80px;
    font-family: sans-serif;
  }

  /* Header định dạng chuẩn */
  .header {
    border-left: 4px solid #38bdf8;
    padding-left: 24px;
    margin-bottom: 30px;
  }
  .eyebrow {
    font-size: 14px;
    font-weight: 800;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: #38bdf8;
    opacity: 0.8;
  }
  h1 {
    font-size: 52px;
    font-weight: 800;
    color: #ffffff;
    margin: 10px 0 0 0;
  }

  /* List points */
  .points {
    list-style: none;
    padding: 0;
  }
  .points li {
    padding-left: 30px;
    margin-bottom: 12px;
    color: #cbd5e1;
    position: relative;
  }
  .points li::before {
    content: "→";
    position: absolute;
    left: 0;
    color: #38bdf8;
  }

  /* Cấu trúc Card đơn giản, an toàn */
  .grid-3 {
    display: flex;
    gap: 24px;
  }
  .card {
    flex: 1;
    padding: 24px;
    border-radius: 16px;
    background: #111827;
    border: 1px solid #1e293b;
  }
  .card.highlight {
    border: 2px solid #38bdf8;
    background: #1e293b;
  }
  .card h2 {
    color: #7dd3fc;
    font-size: 22px;
    margin-top: 0;
  }

  /* Flow Diagram */
  .flow {
    display: flex;
    align-items: center;
    justify-content: space-around;
    background: #0f172a;
    padding: 20px;
    border-radius: 16px;
    border: 1px solid #1e293b;
  }
  .node-box {
    width: 100px;
    height: 50px;
    background: #1e293b;
    border: 1px solid #334155;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    font-weight: bold;
  }

  /* Stats */
  .stat-card {
    flex: 1;
    text-align: center;
    padding: 30px 10px;
    background: #0f172a;
    border-radius: 16px;
    border: 1px dashed #38bdf8;
  }
  .stat-num {
    font-size: 60px;
    font-weight: 800;
    color: #38bdf8;
  }

  /* Quote */
  .quote-wrapper {
    text-align: center;
    padding-top: 50px;
  }
  .quote-text {
    font-size: 36px;
    font-style: italic;
    color: #f1f5f9;
    line-height: 1.4;
  }
---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Vision 2026</div>
  <h1>Modern AI <br/>Architecture Patterns</h1>
</div>
<div style="margin-top: 50px; color: #64748b;">Press → to explore</div>

---
<!-- LAYOUT-2: 2-Column Focus Text -->

<div class="header">
  <div class="eyebrow">Perspective</div>
  <h1>AI changes how we <br/>build software</h1>
</div>
<ul class="points" style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 28px;">
  <li>Execution is automated</li>
  <li>Thinking becomes leverage</li>
  <li>Context is advantage</li>
  <li>Speed is expectation</li>
</ul>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Infrastructure</div>
  <h1>Request Pipeline</h1>
</div>
<div style="display: flex; gap: 40px; align-items: center;">
  <ul class="points" style="flex: 1;">
    <li><strong>Input:</strong> User intent capture</li>
    <li><strong>Process:</strong> Context orchestration</li>
    <li><strong>Output:</strong> LLM generation</li>
  </ul>
  <div class="flow" style="flex: 1.5;">
    <div class="node-box">Input</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Process</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Output</div>
  </div>
</div>

---
<!-- LAYOUT-4: Highlight Comparison -->

<div class="header">
  <div class="eyebrow">Efficiency</div>
  <h1>Transformation Paradigm</h1>
</div>
<div class="grid-3">
  <div class="card">
    <h2 style="color: #94a3b8;">Traditional</h2>
    <ul class="points" style="font-size: 16px;">
      <li>Manual analysis & tagging</li>
      <li>Slow, linear iterations</li>
    </ul>
  </div>
  <div class="card highlight">
    <h2 style="color: #38bdf8;">AI-Augmented</h2>
    <ul class="points" style="font-size: 16px;">
      <li>Agentic reasoning flows</li>
      <li>Rapid parallel iteration</li>
    </ul>
  </div>
</div>

---
<!-- LAYOUT-5: 3-Column Feature Cards -->

<div class="header">
  <div class="eyebrow">Core Pillars</div>
  <h1>Architecture Principles</h1>
</div>
<div class="grid-3">
  <div class="card"><h2>1. Scalability</h2><p style="font-size: 14px;">Horizontal scaling for traffic spikes.</p></div>
  <div class="card"><h2>2. Resilience</h2><p style="font-size: 14px;">Zero-downtime failover mechanisms.</p></div>
  <div class="card"><h2>3. Security</h2><p style="font-size: 14px;">End-to-end Zero Trust topology.</p></div>
</div>

---
<!-- LAYOUT-6: Big Metrics/Stat Cards -->

<div class="header">
  <div class="eyebrow">Impact</div>
  <h1>Performance Gains</h1>
</div>
<div class="grid-3">
  <div class="stat-card"><div class="stat-num">10x</div><div style="color: #94a3b8;">Speed</div></div>
  <div class="stat-card"><div class="stat-num">99.9%</div><div style="color: #94a3b8;">Uptime</div></div>
  <div class="stat-card"><div class="stat-num">-40%</div><div style="color: #94a3b8;">Cost</div></div>
</div>

---
<!-- LAYOUT-7: Big Quote/Statement -->

<div class="quote-wrapper">
  <div class="quote-text">
    "The future of software engineering isn't writing code. It's guiding intelligent systems to solve complex problems."
  </div>
  <div style="margin-top: 30px; color: #38bdf8; font-weight: bold;">— Tech Vision 2026</div>
</div>
