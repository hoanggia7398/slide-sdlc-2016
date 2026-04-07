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

  .points {
    list-style: none;
    padding: 0;
  }
  .points li {
    padding-left: 30px;
    margin-bottom: 12px;
    color: #cbd5e1;
    position: relative;
    line-height: 1.35;
  }
  .points li::before {
    content: "→";
    position: absolute;
    left: 0;
    color: #38bdf8;
  }

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
    margin-bottom: 12px;
  }
  .card p {
    color: #cbd5e1;
    font-size: 16px;
    line-height: 1.35;
    margin: 0;
  }

  .flow {
    display: flex;
    align-items: center;
    justify-content: space-around;
    background: #0f172a;
    padding: 20px;
    border-radius: 16px;
    border: 1px solid #1e293b;
    gap: 10px;
  }
  .node-box {
    width: 108px;
    min-height: 56px;
    background: #1e293b;
    border: 1px solid #334155;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    font-size: 14px;
    font-weight: 700;
    padding: 6px;
  }

  .stat-card {
    flex: 1;
    text-align: center;
    padding: 30px 10px;
    background: #0f172a;
    border-radius: 16px;
    border: 1px dashed #38bdf8;
  }
  .stat-num {
    font-size: 56px;
    font-weight: 800;
    color: #38bdf8;
    line-height: 1;
  }
  .stat-label {
    margin-top: 8px;
    color: #94a3b8;
    font-size: 18px;
  }

  .quote-wrapper {
    text-align: center;
    padding-top: 80px;
  }
  .quote-text {
    font-size: 36px;
    font-style: italic;
    color: #f1f5f9;
    line-height: 1.4;
  }
  .quote-author {
    margin-top: 24px;
    color: #38bdf8;
    font-weight: 700;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    font-size: 14px;
  }
---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Engineering Strategy 2026</div>
  <h1>AI in SDLC 2026<br/>From Hype to Operating Model</h1>
</div>
<div style="margin-top: 46px; color: #64748b;">Problem → Use → Trust → System → Scale</div>

---
<!-- LAYOUT-2: 2-Column Focus Text -->

<div class="header">
  <div class="eyebrow">Session Goal</div>
  <h1>What this deck delivers</h1>
</div>
<ul class="points" style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 28px;">
  <li>Developer-first framing</li>
  <li>Practical daily usage</li>
  <li>Trust and control model</li>
  <li>Scalable team system</li>
</ul>

---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Phase 1</div>
  <h1>Problem<br/>Why current delivery strains teams</h1>
</div>

---
<!-- LAYOUT-2: 2-Column Focus Text -->

<div class="header">
  <div class="eyebrow">Current Reality</div>
  <h1>Pressure grows faster than capacity</h1>
</div>
<ul class="points" style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 28px;">
  <li>Backlogs keep expanding</li>
  <li>Release windows shrink</li>
  <li>Codebases become harder to read</li>
  <li>Quality standards keep rising</li>
</ul>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Delivery Friction</div>
  <h1>Where time is lost in a normal task</h1>
</div>
<div style="display: flex; gap: 34px; align-items: center;">
  <ul class="points" style="flex: 1; font-size: 20px;">
    <li><strong>Understand:</strong> Slow context loading across files</li>
    <li><strong>Implement:</strong> Repetitive boilerplate and refactors</li>
    <li><strong>Verify:</strong> Manual testing and review cycles</li>
  </ul>
  <div class="flow" style="flex: 1.35;">
    <div class="node-box">Ticket</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Context</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Code</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Test</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Review</div>
  </div>
</div>

---
<!-- LAYOUT-4: Highlight Comparison -->

<div class="header">
  <div class="eyebrow">Shift</div>
  <h1>From manual-heavy to AI-assisted loops</h1>
</div>
<div class="grid-3" style="display: grid; grid-template-columns: 1fr 1fr;">
  <div class="card">
    <h2 style="color: #94a3b8;">Without AI</h2>
    <ul class="points" style="font-size: 16px; margin: 0;">
      <li>Linear debug and search</li>
      <li>Manual test scaffolding</li>
      <li>Knowledge bottleneck on seniors</li>
    </ul>
  </div>
  <div class="card highlight">
    <h2>With AI assistance</h2>
    <ul class="points" style="font-size: 16px; margin: 0;">
      <li>Faster root-cause discovery</li>
      <li>Draft tests and patches instantly</li>
      <li>Better shared understanding</li>
    </ul>
  </div>
</div>

---
<!-- LAYOUT-7: Big Quote/Statement -->

<div class="quote-wrapper">
  <div class="quote-text">“The bottleneck is no longer typing speed. It is context switching.”</div>
  <div class="quote-author">Problem takeaway</div>
</div>

---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Phase 2</div>
  <h1>Use<br/>Where AI helps developers today</h1>
</div>

---
<!-- LAYOUT-5: 3-Column Feature Cards -->

<div class="header">
  <div class="eyebrow">High-Value Work</div>
  <h1>Three daily AI use cases</h1>
</div>
<div class="grid-3">
  <div class="card">
    <h2>Code Understanding</h2>
    <p>Summarize modules, explain flows, and onboard into unfamiliar repositories faster.</p>
  </div>
  <div class="card">
    <h2>Debug & Fix</h2>
    <p>Trace likely failure paths, draft patches, and iterate quickly with targeted verification.</p>
  </div>
  <div class="card highlight">
    <h2>Build & Refactor</h2>
    <p>Generate boilerplate and safe refactors so engineers focus on design decisions.</p>
  </div>
</div>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Use Case</div>
  <h1>AI-assisted debug loop</h1>
</div>
<div style="display: flex; gap: 34px; align-items: center;">
  <ul class="points" style="flex: 1; font-size: 20px;">
    <li><strong>Start:</strong> Feed logs, stack traces, and failing behavior</li>
    <li><strong>Loop:</strong> Ask for hypothesis, patch, and test suggestions</li>
    <li><strong>End:</strong> Keep only verified changes</li>
  </ul>
  <div class="flow" style="flex: 1.35;">
    <div class="node-box">Read</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Trace</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Patch</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Test</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Retry</div>
  </div>
</div>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Use Case</div>
  <h1>AI-assisted feature delivery</h1>
</div>
<div style="display: flex; gap: 34px; align-items: center;">
  <ul class="points" style="flex: 1; font-size: 20px;">
    <li><strong>Planning:</strong> Convert requirement into implementation slices</li>
    <li><strong>Execution:</strong> Generate first draft and edge-case tests</li>
    <li><strong>Review:</strong> Tighten naming, contracts, and failure handling</li>
  </ul>
  <div class="flow" style="flex: 1.35;">
    <div class="node-box">Scope</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Design</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Build</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Verify</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Ship</div>
  </div>
</div>

---
<!-- LAYOUT-5: 3-Column Feature Cards -->

<div class="header">
  <div class="eyebrow">Tool Fit</div>
  <h1>Use the right surface for the job</h1>
</div>
<div class="grid-3">
  <div class="card">
    <h2>Cursor</h2>
    <p>Strong fit for interactive IDE coding, quick edits, and local pair-programming flow.</p>
  </div>
  <div class="card">
    <h2>Cline</h2>
    <p>Useful when you want explicit step-by-step execution and transparent task traces.</p>
  </div>
  <div class="card highlight">
    <h2>Claude Code</h2>
    <p>High leverage for repository-wide reasoning, CLI workflows, and structured edits.</p>
  </div>
</div>

---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Phase 3</div>
  <h1>Trust<br/>How teams keep AI output reliable</h1>
</div>

---
<!-- LAYOUT-4: Highlight Comparison -->

<div class="header">
  <div class="eyebrow">Operating Model</div>
  <h1>Human-in-the-loop is non-negotiable</h1>
</div>
<div class="grid-3" style="display: grid; grid-template-columns: 1fr 1fr;">
  <div class="card">
    <h2 style="color: #94a3b8;">AI responsibilities</h2>
    <ul class="points" style="font-size: 16px; margin: 0;">
      <li>Suggest options and drafts</li>
      <li>Automate repetitive transformations</li>
      <li>Surface possible edge cases</li>
    </ul>
  </div>
  <div class="card highlight">
    <h2>Developer responsibilities</h2>
    <ul class="points" style="font-size: 16px; margin: 0;">
      <li>Approve architecture and constraints</li>
      <li>Validate behavior and security</li>
      <li>Own final merge decision</li>
    </ul>
  </div>
</div>

---
<!-- LAYOUT-2: 2-Column Focus Text -->

<div class="header">
  <div class="eyebrow">Verification</div>
  <h1>Minimal trust checklist per change</h1>
</div>
<ul class="points" style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 28px;">
  <li>Reproduce the issue first</li>
  <li>Diff review before execution</li>
  <li>Run targeted tests</li>
  <li>Confirm rollback path</li>
</ul>

---
<!-- LAYOUT-5: 3-Column Feature Cards -->

<div class="header">
  <div class="eyebrow">Failure Modes</div>
  <h1>Common risks and guardrails</h1>
</div>
<div class="grid-3">
  <div class="card">
    <h2>Hallucinated Logic</h2>
    <p>Mitigate with tighter context windows and concrete acceptance criteria in prompts.</p>
  </div>
  <div class="card">
    <h2>Silent Regressions</h2>
    <p>Mitigate with tests focused on changed behavior, not only broad smoke checks.</p>
  </div>
  <div class="card highlight">
    <h2>Loop Drift</h2>
    <p>Mitigate with step caps, stop conditions, and explicit human checkpoints.</p>
  </div>
</div>

---
<!-- LAYOUT-7: Big Quote/Statement -->

<div class="quote-wrapper">
  <div class="quote-text">“Trust is built by verification, not by model confidence.”</div>
  <div class="quote-author">Trust takeaway</div>
</div>

---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Phase 4</div>
  <h1>System<br/>What runs underneath an AI workflow</h1>
</div>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Architecture</div>
  <h1>Agent is the workflow engine</h1>
</div>
<div style="display: flex; gap: 34px; align-items: center;">
  <ul class="points" style="flex: 1; font-size: 20px;">
    <li><strong>Model:</strong> Generates text and code</li>
    <li><strong>Agent:</strong> Plans steps, calls tools, evaluates results</li>
    <li><strong>Tools:</strong> IDE, CLI, tests, git, and repo search</li>
  </ul>
  <div class="flow" style="flex: 1.35;">
    <div class="node-box">Developer</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Agent</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Models</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Tools</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Result</div>
  </div>
</div>
<div style="margin-top: 14px; color: #94a3b8; font-size: 18px;">Examples of agent surfaces: Cursor, Cline, Claude Code.</div>

---
<!-- LAYOUT-3: Split Flow Diagram -->

<div class="header">
  <div class="eyebrow">Economics</div>
  <h1>Usage Rule Count in practice</h1>
</div>
<div style="display: flex; gap: 34px; align-items: center;">
  <ul class="points" style="flex: 1; font-size: 20px;">
    <li><strong>Rule:</strong> 1 request equals 1 reasoning step</li>
    <li><strong>Reality:</strong> One task triggers many looped requests</li>
    <li><strong>Action:</strong> Monitor loops, retries, and stop conditions</li>
  </ul>
  <div class="flow" style="flex: 1.35;">
    <div class="node-box">Read</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Analyze</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Patch</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Test</div>
    <div style="color: #475569;">→</div>
    <div class="node-box">Retry</div>
  </div>
</div>

---
<!-- LAYOUT-6: Big Metrics/Stat Cards -->

<div class="header">
  <div class="eyebrow">Control Signals</div>
  <h1>Track system behavior, not hype</h1>
</div>
<div class="grid-3">
  <div class="stat-card">
    <div class="stat-num">1</div>
    <div class="stat-label">Task owner</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">3</div>
    <div class="stat-label">Control gates</div>
  </div>
  <div class="stat-card">
    <div class="stat-num">5-10</div>
    <div class="stat-label">Requests/debug loop*</div>
  </div>
</div>
<div style="margin-top: 14px; color: #64748b; font-size: 16px;">*Illustrative loop range, used for planning and monitoring.</div>

---
<!-- LAYOUT-5: 3-Column Feature Cards -->

<div class="header">
  <div class="eyebrow">Team Blueprint</div>
  <h1>Minimal system to adopt AI safely</h1>
</div>
<div class="grid-3">
  <div class="card">
    <h2>Context Pack</h2>
    <p>Shared docs, architecture notes, and coding constraints available to every session.</p>
  </div>
  <div class="card">
    <h2>Policy Layer</h2>
    <p>Rules for approvals, test requirements, and escalation before merge or deployment.</p>
  </div>
  <div class="card highlight">
    <h2>Telemetry</h2>
    <p>Track request count, retries, and outcome quality to improve prompts and workflows.</p>
  </div>
</div>

---
<!-- LAYOUT-1: Title/Cover Slide -->

<div class="header">
  <div class="eyebrow">Phase 5</div>
  <h1>Scale<br/>How to roll this across teams</h1>
</div>

---
<!-- LAYOUT-2: 2-Column Focus Text -->

<div class="header">
  <div class="eyebrow">Scale Plan</div>
  <h1>Start narrow, standardize, then expand</h1>
</div>
<ul class="points" style="display: grid; grid-template-columns: 1fr 1fr; gap: 10px; font-size: 28px;">
  <li>Pilot one workflow per team</li>
  <li>Define shared trust gates</li>
  <li>Instrument usage and outcomes</li>
  <li>Scale proven patterns org-wide</li>
</ul>
<div style="margin-top: 30px; color: #7dd3fc; font-size: 24px; font-weight: 700;">Developers are not replaced by AI. Teams with strong AI systems will outperform teams without them.</div>