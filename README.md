<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
    <meta name="color-scheme" content="dark" />
    <link rel="icon" href="data:," />
    <title>Siddartha Jamandla GitHub Profile</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:ital,wght@0,400;0,500;0,700;0,800;1,400&family=Inter:wght@400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <style>
      :root {
        --bg: #06060d;
        --bg-2: #0a0a15;
        --panel: #0d0d1a;
        --panel-2: #11112200;
        --line: #23233c;
        --line-soft: #1a1a2e;
        --ink: #f3f2fb;
        --mut: #a8a6c6;
        --dim: #6f6d8f;
        --vio: #8b5cf6;
        --vio-2: #c084fc;
        --pink: #f472b6;
        --cyan: #3ee6ff;
        --green: #3fb950;
        --amber: #e3b341;
        --mono: "JetBrains Mono", ui-monospace, SFMono-Regular, Menlo, monospace;
        --sans: "Inter", system-ui, -apple-system, "Segoe UI", sans-serif;
      }
      * { box-sizing: border-box; }
      html { scroll-behavior: smooth; }
      body {
        margin: 0;
        background:
          radial-gradient(1100px 500px at 85% -10%, rgba(139, 92, 246, 0.14), transparent 60%),
          radial-gradient(900px 480px at -10% 30%, rgba(62, 230, 255, 0.05), transparent 55%),
          var(--bg);
        color: var(--ink);
        font-family: var(--sans);
        -webkit-font-smoothing: antialiased;
      }
      a { color: var(--cyan); text-decoration: none; }
      a:hover { text-decoration: underline; }
      .wrap { max-width: 1160px; margin: 0 auto; padding: 0 20px 72px; }

      /* ---------- hero ---------- */
      .hero {
        display: grid;
        grid-template-columns: minmax(0, 0.92fr) minmax(0, 1.25fr);
        gap: 34px;
        align-items: center;
        padding: 44px 0 30px;
      }
      .status-pill {
        display: inline-flex; align-items: center; gap: 8px;
        font-family: var(--mono); font-size: 12px; color: #b9f5c2;
        border: 1px solid #1f4630; background: rgba(63, 185, 80, 0.08);
        padding: 6px 12px; border-radius: 999px;
      }
      .status-pill .dot {
        width: 8px; height: 8px; border-radius: 50%; background: var(--green);
        box-shadow: 0 0 10px var(--green);
        animation: pulse 2s infinite;
      }
      @keyframes pulse { 0%,100% { opacity: 1; } 50% { opacity: 0.35; } }
      h1 {
        font-family: var(--mono); font-weight: 800;
        font-size: clamp(34px, 4.6vw, 54px);
        line-height: 1.04; letter-spacing: -0.01em;
        margin: 18px 0 10px;
      }
      h1 .grad {
        background: linear-gradient(92deg, var(--vio-2), var(--pink) 55%, var(--cyan));
        -webkit-background-clip: text; background-clip: text; color: transparent;
      }
      .role {
        font-family: var(--mono); font-size: clamp(14px, 1.6vw, 17px);
        color: var(--mut); margin: 0 0 6px; min-height: 1.5em;
      }
      .role .cursor {
        display: inline-block; width: 9px; height: 1.05em; vertical-align: text-bottom;
        background: var(--vio-2); margin-left: 3px; animation: blink 1s steps(1) infinite;
      }
      @keyframes blink { 50% { opacity: 0; } }
      .lede { color: var(--mut); font-size: 16px; line-height: 1.65; margin: 12px 0 0; max-width: 46ch; }
      .lede strong { color: var(--ink); font-weight: 600; }

      .term {
        margin-top: 24px; border: 1px solid var(--line); border-radius: 10px;
        background: #08080f; overflow: hidden;
        font-family: var(--mono); font-size: 13px; line-height: 1.75;
      }
      .term-bar {
        display: flex; align-items: center; gap: 7px;
        padding: 9px 12px; border-bottom: 1px solid var(--line-soft);
        background: var(--panel); color: var(--dim); font-size: 11.5px;
      }
      .tdot { width: 11px; height: 11px; border-radius: 50%; }
      .term-body { padding: 13px 16px 15px; overflow-x: auto; }
      .term-body p { margin: 0; white-space: nowrap; }
      .tp { color: var(--vio-2); }
      .tc { color: #e8e6ff; }
      .to { color: var(--mut); }
      .to b { color: var(--cyan); font-weight: 500; }
      .to .ok { color: #7ee787; }

      .cta-row { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px; }
      .btn {
        display: inline-flex; align-items: center; gap: 8px;
        font-family: var(--mono); font-size: 13px; font-weight: 500;
        padding: 10px 16px; border-radius: 8px; border: 1px solid var(--line);
        background: var(--panel); color: var(--ink);
        transition: border-color 0.15s, transform 0.15s, background 0.15s;
      }
      .btn:hover { text-decoration: none; border-color: var(--vio); transform: translateY(-1px); }
      .btn.primary { background: var(--vio); border-color: var(--vio); color: #fff; }
      .btn.primary:hover { background: #7c4def; }
      .btn svg { width: 16px; height: 16px; flex: none; }

      /* ---------- visual map ---------- */
      .vmap {
        border: 1px solid var(--line); border-radius: 14px;
        background: linear-gradient(180deg, #0c0c1a, #07070f);
        overflow: hidden;
        box-shadow: 0 24px 70px rgba(0, 0, 0, 0.5), 0 0 0 1px rgba(139, 92, 246, 0.06), 0 0 90px rgba(139, 92, 246, 0.07);
      }
      .vmap-bar {
        display: flex; align-items: center; gap: 10px;
        padding: 11px 14px; border-bottom: 1px solid var(--line-soft);
        font-family: var(--mono);
      }
      .vmap-bar .name { font-size: 13px; font-weight: 700; letter-spacing: 0.14em; color: var(--ink); }
      .vmap-bar .name span { color: var(--vio-2); }
      .vmap-bar .sub { font-size: 11px; color: var(--dim); }
      .live-tag {
        margin-left: auto; display: inline-flex; align-items: center; gap: 6px;
        font-size: 10.5px; letter-spacing: 0.12em; color: #ffb3cd;
        border: 1px solid rgba(244, 114, 182, 0.35); border-radius: 999px; padding: 3px 9px;
      }
      .live-tag i { width: 6px; height: 6px; border-radius: 50%; background: var(--pink); box-shadow: 0 0 8px var(--pink); animation: pulse 1.6s infinite; }
      .vmap-stage { position: relative; }
      canvas#stage { display: block; width: 100%; height: auto; touch-action: pan-y; }
      .vmap-foot {
        display: flex; flex-wrap: wrap; align-items: center; gap: 8px;
        padding: 12px 14px; border-top: 1px solid var(--line-soft);
      }
      .shape-btn {
        font-family: var(--mono); font-size: 12px; color: var(--mut);
        background: #0a0a16; border: 1px solid var(--line); border-radius: 999px;
        padding: 7px 13px; cursor: pointer;
        transition: color 0.15s, border-color 0.15s, background 0.15s;
      }
      .shape-btn:hover { color: var(--ink); border-color: var(--vio); }
      .shape-btn[aria-pressed="true"] {
        color: #fff; background: var(--vio); border-color: var(--vio);
      }
      .shape-btn:focus-visible, .btn:focus-visible, a:focus-visible { outline: 2px solid var(--cyan); outline-offset: 2px; }
      .vmap-hint { margin-left: auto; font-family: var(--mono); font-size: 11px; color: var(--dim); }
      .vmap-fallback {
        display: none; width: 100%; height: auto;
      }

      /* ---------- stats strip ---------- */
      .stats {
        display: grid; grid-template-columns: repeat(5, 1fr); gap: 12px; margin: 6px 0 8px;
      }
      .stat {
        border: 1px solid var(--line-soft); background: var(--panel); border-radius: 10px;
        padding: 16px 14px; text-align: left;
      }
      .stat .num { font-family: var(--mono); font-size: 26px; font-weight: 800; color: var(--ink); }
      .stat .num em { font-style: normal; color: var(--vio-2); }
      .stat .lbl { font-size: 12px; color: var(--mut); margin-top: 3px; line-height: 1.4; }

      /* ---------- sections ---------- */
      section { margin-top: 52px; }
      .sec-head { display: flex; align-items: baseline; gap: 14px; margin-bottom: 18px; }
      .sec-head h2 {
        font-family: var(--mono); font-size: 19px; font-weight: 700; margin: 0; color: var(--ink);
      }
      .sec-head h2 .path { color: var(--vio-2); }
      .sec-head .rule { flex: 1; height: 1px; background: var(--line-soft); }
      .sec-head .note { font-family: var(--mono); font-size: 11.5px; color: var(--dim); }

      .grid-4 { display: grid; grid-template-columns: repeat(4, 1fr); gap: 12px; }
      .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 12px; }
      .grid-2 { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; }

      .card {
        border: 1px solid var(--line-soft); background: var(--panel); border-radius: 12px;
        padding: 18px;
      }
      .card h3 { margin: 0 0 7px; font-size: 15.5px; font-weight: 600; color: var(--ink); }
      .card p { margin: 0; font-size: 13.5px; line-height: 1.6; color: var(--mut); }
      .gauge { width: 46px; height: 46px; margin-bottom: 13px; }
      .gauge .track { stroke: #1d1d33; }
      .gauge .val { stroke-linecap: round; transform: rotate(-90deg); transform-origin: center; }

      .skill-group { margin-bottom: 14px; }
      .skill-group:last-child { margin-bottom: 0; }
      .skill-group .gname {
        font-family: var(--mono); font-size: 11.5px; color: var(--dim);
        letter-spacing: 0.08em; margin-bottom: 8px;
      }
      .chips { display: flex; flex-wrap: wrap; gap: 8px; }
      .chip {
        font-family: var(--mono); font-size: 12.5px; color: #ddd9ff;
        border: 1px solid var(--line); background: #0a0a16; border-radius: 7px; padding: 6px 11px;
      }
      .chip b { color: var(--vio-2); font-weight: 500; }

      .proj { display: flex; flex-direction: column; gap: 8px; }
      .proj .top { display: flex; align-items: center; gap: 9px; }
      .proj .top h3 { margin: 0; font-family: var(--mono); font-size: 15px; }
      .proj .top h3 a { color: var(--ink); }
      .proj .top h3 a:hover { color: var(--cyan); }
      .lang { display: inline-flex; align-items: center; gap: 6px; font-size: 12px; color: var(--mut); font-family: var(--mono); }
      .lang i { width: 10px; height: 10px; border-radius: 50%; display: inline-block; }
      .live-chip {
        margin-left: auto; font-family: var(--mono); font-size: 10.5px; letter-spacing: 0.08em;
        color: #b9f5c2; border: 1px solid #1f4630; border-radius: 999px; padding: 3px 9px;
        display: inline-flex; align-items: center; gap: 6px; flex: none;
      }
      .live-chip i { width: 6px; height: 6px; border-radius: 50%; background: var(--green); box-shadow: 0 0 7px var(--green); }
      .live-chip:hover { text-decoration: none; border-color: var(--green); }
      .soon-chip {
        margin-left: auto; font-family: var(--mono); font-size: 10.5px; letter-spacing: 0.06em;
        color: var(--amber); border: 1px solid rgba(227, 179, 65, 0.35); border-radius: 999px; padding: 3px 9px; flex: none;
      }

      .edu-item { display: flex; gap: 14px; padding: 15px 0; border-bottom: 1px solid var(--line-soft); }
      .edu-item:last-child { border-bottom: 0; padding-bottom: 2px; }
      .edu-item:first-child { padding-top: 2px; }
      .edu-mark {
        flex: none; width: 38px; height: 38px; border-radius: 9px;
        border: 1px solid var(--line); background: #0a0a16;
        display: grid; place-items: center; font-family: var(--mono); font-size: 13px; color: var(--vio-2);
      }
      .edu-item h3 { margin: 0 0 3px; font-size: 15px; }
      .edu-item p { margin: 0; font-size: 13.5px; color: var(--mut); line-height: 1.55; }
      .edu-item .when { font-family: var(--mono); font-size: 11.5px; color: var(--dim); margin-left: auto; flex: none; padding-top: 3px; }

      .focus-list { list-style: none; margin: 12px 0 0; padding: 12px 0 0; border-top: 1px solid var(--line-soft); display: grid; gap: 6px; }
      .focus-list li { font-size: 13px; line-height: 1.5; color: var(--mut); display: flex; gap: 8px; }
      .focus-list li::before { content: "▸"; color: var(--vio-2); flex: none; }
      .proj .live-url { font-family: var(--mono); font-size: 11.5px; color: var(--dim); word-break: break-all; }
      .proj .live-url a { color: var(--cyan); }
      .status-line { font-family: var(--mono); font-size: 11.5px; color: var(--amber); margin-top: auto; padding-top: 4px; }
      .hl-list { list-style: none; margin: 0; padding: 0; display: grid; gap: 12px; }
      .hl-list li { display: flex; gap: 12px; font-size: 14px; line-height: 1.6; color: var(--mut); }
      .hl-list li strong { color: var(--ink); font-weight: 600; }
      .hl-ico { flex: none; width: 32px; height: 32px; border-radius: 8px; border: 1px solid var(--line); background: #0a0a16; display: grid; place-items: center; font-family: var(--mono); font-size: 12px; color: var(--vio-2); }
      .hud-chip { font-family: var(--mono); font-size: 12px; padding: 6px 11px; border-radius: 7px; border: 1px solid var(--line); background: #0a0a16; color: var(--mut); }
      .hud-chip b { color: var(--ink); font-weight: 700; }
      .contrib-stats { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 12px; }
      .contrib-graph { display: block; width: 100%; height: auto; }
      .contrib-graph .cg-m, .contrib-graph .cg-d { font-family: var(--mono); font-size: 9px; fill: var(--dim); }
      .contrib-graph .cc { stroke: rgba(255, 255, 255, 0.05); stroke-width: 1; }
      .contrib-graph .l0 { fill: #1d1d33; }
      .contrib-graph .l1 { fill: #0e4429; }
      .contrib-graph .l2 { fill: #006d32; }
      .contrib-graph .l3 { fill: #26a641; }
      .contrib-graph .l4 { fill: #39d353; }
      .achieve { display: flex; flex-wrap: wrap; gap: 10px; align-items: center; }
      .badge-pill { font-family: var(--mono); font-size: 13px; padding: 9px 14px; border-radius: 999px; border: 1px solid var(--line); background: #0a0a16; color: var(--ink); }
      .badge-pill.ok { border-color: #1f4630; color: #b9f5c2; }
      .badge-pill.wait { border-color: rgba(227,179,65,.35); color: #f0d48a; }
      .focus-now { list-style: none; margin: 0; padding: 0; display: grid; gap: 0; }
      .focus-now li { display: flex; gap: 12px; padding: 13px 0; border-bottom: 1px solid var(--line-soft); font-size: 14px; line-height: 1.6; color: var(--mut); }
      .focus-now li:last-child { border-bottom: 0; padding-bottom: 2px; }
      .focus-now li:first-child { padding-top: 2px; }
      .focus-now strong { color: var(--ink); font-weight: 600; }
      .journey-flow { display: flex; flex-wrap: wrap; align-items: center; gap: 8px; margin-bottom: 16px; }
      .jstep { font-family: var(--mono); font-size: 12.5px; padding: 8px 13px; border-radius: 8px; border: 1px solid var(--line); background: #0a0a16; color: var(--ink); }
      .jarrow { color: var(--vio-2); font-family: var(--mono); }
      .open-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; }
      .open-item { display: flex; gap: 12px; align-items: flex-start; }
      .open-item h3 { font-size: 14.5px; margin: 0 0 3px; }
      .open-item p { font-size: 13px; }
      .connect-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; }
      .connect-item { display: flex; gap: 12px; align-items: center; padding: 14px 16px; }
      .connect-item:hover { border-color: var(--vio); text-decoration: none; }
      .connect-item .cl { font-family: var(--mono); font-size: 11px; letter-spacing: .08em; color: var(--dim); }
      .connect-item .cv { font-size: 13.5px; color: var(--ink); word-break: break-all; line-height: 1.45; }
      .quote-block { text-align: center; padding: 34px 22px; }
      .quote-block blockquote { margin: 0 auto; max-width: 640px; font-family: var(--mono); font-size: clamp(17px, 2.4vw, 22px); line-height: 1.55; font-weight: 700; color: var(--ink); }
      .quote-block p { margin: 12px 0 0; color: var(--mut); font-size: 14.5px; }

      footer {
        margin-top: 60px; border-top: 1px solid var(--line-soft); padding-top: 22px;
        display: flex; flex-wrap: wrap; gap: 10px; align-items: center;
        font-family: var(--mono); font-size: 12px; color: var(--dim);
      }
      footer .who { color: var(--mut); }
      footer nav { margin-left: auto; display: flex; gap: 18px; flex-wrap: wrap; }
      footer a { color: var(--mut); }
      footer a:hover { color: var(--cyan); }

      /* ---------- responsive ---------- */
      @media (max-width: 960px) {
        .hero { grid-template-columns: 1fr; padding-top: 30px; gap: 26px; }
        .grid-4 { grid-template-columns: repeat(2, 1fr); }
        .grid-3 { grid-template-columns: 1fr; }
        .stats { grid-template-columns: repeat(3, 1fr); }
        .stat:nth-child(4), .stat:nth-child(5) { grid-column: span 1; }
      }
      @media (max-width: 560px) {
        .wrap { padding: 0 14px 56px; }
        .grid-4, .grid-2, .open-grid, .connect-grid { grid-template-columns: 1fr; }
        .journey-flow { gap: 6px; }
        .stats { grid-template-columns: repeat(2, 1fr); }
        .vmap-hint { display: none; }
        .term-body p { white-space: normal; }
        .edu-item .when { display: none; }
        h1 { font-size: 33px; }
      }
      @media (prefers-reduced-motion: reduce) {
        html { scroll-behavior: auto; }
        .status-pill .dot, .live-tag i, .role .cursor { animation: none; }
        .btn:hover { transform: none; }
      }
    </style>
  </head>
  <body>
    <div class="wrap">
      <!-- ================= HERO ================= -->
      <div class="hero">
        <div>
          <span class="status-pill"><span class="dot"></span> Open to paid remote internships</span>
          <h1>Siddartha<br /><span class="grad">Jamandla</span></h1>
          <p class="role"><span id="typer">B.Tech AI &amp; ML Student</span><span class="cursor"></span></p>
          <p class="lede">
            Second-year <strong>B.Tech Artificial Intelligence &amp; Machine Learning</strong> student and
            <strong>Python developer</strong> from Warangal, Telangana. I build AI tools and full-stack web
            apps — and I ship them live, not just to a repo.
          </p>

          <div class="term" aria-label="Terminal summary">
            <div class="term-bar"><span class="tdot" style="background:#ff5f57"></span><span class="tdot" style="background:#febc2e"></span><span class="tdot" style="background:#28c840"></span>&nbsp;siddartha@github: ~/profile</div>
            <div class="term-body">
              <p><span class="tp">$</span> <span class="tc">whoami</span></p>
              <p class="to">siddartha_jamandla — AI/ML · Python · Web Dev</p>
              <p><span class="tp">$</span> <span class="tc">cat focus.txt</span></p>
              <p class="to">CareerPlus+ · AI agents · full-stack apps</p>
              <p><span class="tp">$</span> <span class="tc">./status --open-to-work</span></p>
              <p class="to"><span class="ok">●</span> paid remote internships — AI/ML, Python, web</p>
            </div>
          </div>

          <div class="cta-row">
            <a class="btn primary" href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener">
              <svg viewBox="0 0 16 16" fill="currentColor" aria-hidden="true"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8Z"/></svg>
              GitHub
            </a>
            <a class="btn" href="https://www.linkedin.com/in/siddartha-jamandla-97350b384" target="_blank" rel="noopener">
              <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M20.45 20.45h-3.55v-5.57c0-1.33-.03-3.04-1.85-3.04-1.86 0-2.14 1.45-2.14 2.94v5.67H9.35V9h3.41v1.56h.05c.47-.9 1.63-1.85 3.36-1.85 3.6 0 4.27 2.37 4.27 5.46v6.28ZM5.34 7.43a2.06 2.06 0 1 1 0-4.12 2.06 2.06 0 0 1 0 4.12ZM7.12 20.45H3.55V9h3.57v11.45Z"/></svg>
              LinkedIn
            </a>
            <a class="btn" href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener">Portfolio ↗</a>
            <a class="btn" href="mailto:siddarthajamandla@gmail.com">Email ↗</a>
          </div>
        </div>

        <!-- VISUAL.MAP -->
        <div class="vmap">
          <div class="vmap-bar">
            <span class="name">VISUAL<span>.</span>MAP</span>
            <span class="sub">particle portrait — live</span>
            <span class="live-tag"><i></i>LIVE</span>
          </div>
          <div class="vmap-stage">
            <canvas id="stage" width="880" height="640" role="img"
              aria-label="Animated particle portrait of Siddartha Jamandla: thousands of dots fly together to form his face, then morph into his name and code symbols"></canvas>
            <img class="vmap-fallback" id="vmapFallback" src="data:image/jpeg;base64,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"
              alt="Portrait of Siddartha Jamandla" />
          </div>
          <div class="vmap-foot" role="group" aria-label="Portrait shapes">
            <button class="shape-btn" data-shape="portrait" aria-pressed="true">◉ Portrait</button>
            <button class="shape-btn" data-shape="name" aria-pressed="false">SIDDARTHA</button>
            <button class="shape-btn" data-shape="code" aria-pressed="false">&lt;/&gt;</button>
            <button class="shape-btn" data-shape="aiml" aria-pressed="false">AI·ML</button>
            <button class="shape-btn" id="replayBtn" type="button">↻ Replay</button>
            <span class="vmap-hint">move your pointer through the dots</span>
          </div>
        </div>
      </div>

      <!-- ================= STATS ================= -->
      <div class="stats">
        <div class="stat"><div class="num">6</div><div class="lbl">Featured projects — live on GitHub</div></div>
        <div class="stat"><div class="num">4</div><div class="lbl">Live sites — ShopEase, LearnHub, Portfolio, Blow Crackers</div></div>
        <div class="stat"><div class="num">8</div><div class="lbl">Public repos · 3 stars · on GitHub since Oct 2025</div></div>
        <div class="stat"><div class="num">8.0<em>/10</em></div><div class="lbl">B.Tech CGPA — AI &amp; ML</div></div>
        <div class="stat"><div class="num">80<em>%</em></div><div class="lbl">Diploma in Computer Engineering</div></div>
      </div>

      <!-- ================= FOCUS ================= -->
      <section aria-labelledby="focus-h">
        <div class="sec-head">
          <h2 id="focus-h"><span class="path">~/</span>what_i_focus_on</h2>
          <span class="rule"></span>
          <span class="note">as an AI &amp; ML student</span>
        </div>
        <div class="grid-4">
          <div class="card">
            <svg class="gauge" viewBox="0 0 46 46" aria-hidden="true"><circle class="track" cx="23" cy="23" r="19" fill="none" stroke-width="5"/><circle class="val" cx="23" cy="23" r="19" fill="none" stroke="#8b5cf6" stroke-width="5" stroke-dasharray="119.4" stroke-dashoffset="24"/></svg>
            <h3>🤖 AI &amp; ML</h3>
            <p>Machine-learning projects in Python — including CareerPlus+, an AI resume analyzer that scores resumes and tells you exactly what to fix.</p>
            <ul class="focus-list"><li>Artificial Intelligence</li><li>Machine Learning</li><li>AI-powered tools</li></ul>
          </div>
          <div class="card">
            <svg class="gauge" viewBox="0 0 46 46" aria-hidden="true"><circle class="track" cx="23" cy="23" r="19" fill="none" stroke-width="5"/><circle class="val" cx="23" cy="23" r="19" fill="none" stroke="#f472b6" stroke-width="5" stroke-dasharray="119.4" stroke-dashoffset="36"/></svg>
            <h3>⚡ AI Agents &amp; Automation</h3>
            <p>Agents that plan, execute and verify — a website testing agent and a job-hunting agent that scores roles against my own resume.</p>
            <ul class="focus-list"><li>Agent workflows</li><li>Task automation</li><li>Real-world checks</li></ul>
          </div>
          <div class="card">
            <svg class="gauge" viewBox="0 0 46 46" aria-hidden="true"><circle class="track" cx="23" cy="23" r="19" fill="none" stroke-width="5"/><circle class="val" cx="23" cy="23" r="19" fill="none" stroke="#3ee6ff" stroke-width="5" stroke-dasharray="119.4" stroke-dashoffset="30"/></svg>
            <h3>🌐 Full-Stack Web</h3>
            <p>Real backends, not just pages — ShopEase and LearnHub run on Python + SQLite with auth, APIs and live deployments.</p>
            <ul class="focus-list"><li>Responsive web apps</li><li>Python + SQLite backends</li><li>Clean, usable UI</li></ul>
          </div>
          <div class="card">
            <svg class="gauge" viewBox="0 0 46 46" aria-hidden="true"><circle class="track" cx="23" cy="23" r="19" fill="none" stroke-width="5"/><circle class="val" cx="23" cy="23" r="19" fill="none" stroke="#3fb950" stroke-width="5" stroke-dasharray="119.4" stroke-dashoffset="42"/></svg>
            <h3>🧩 Core CS</h3>
            <p>Data structures &amp; algorithms, OOP and databases — the fundamentals underneath everything above, practised daily in C and Java.</p>
            <ul class="focus-list"><li>Data Structures</li><li>Algorithms · OOP</li><li>Problem solving</li></ul>
          </div>
        </div>
      </section>

      <!-- ================= SKILLS ================= -->
      <section aria-labelledby="skills-h">
        <div class="sec-head">
          <h2 id="skills-h"><span class="path">~/</span>tech_stack</h2>
          <span class="rule"></span>
          <span class="note">skills from my resume</span>
        </div>
        <div class="card">
          <div class="skill-group">
            <div class="gname">LANGUAGES &amp; WEB</div>
            <div class="chips">
              <span class="chip"><b>◆</b> Python</span><span class="chip"><b>◆</b> C</span><span class="chip"><b>◆</b> C++</span>
              <span class="chip"><b>◆</b> Java</span><span class="chip"><b>◆</b> JavaScript</span><span class="chip"><b>◆</b> SQL</span>
              <span class="chip"><b>◆</b> HTML5</span><span class="chip"><b>◆</b> CSS3</span>
            </div>
          </div>
          <div class="skill-group">
            <div class="gname">TOOLS</div>
            <div class="chips">
              <span class="chip"><b>◆</b> Git</span><span class="chip"><b>◆</b> GitHub</span><span class="chip"><b>◆</b> VS Code</span>
            </div>
          </div>
          <div class="skill-group">
            <div class="gname">CORE &amp; DESIGN</div>
            <div class="chips">
              <span class="chip"><b>◆</b> DSA</span><span class="chip"><b>◆</b> OOP</span>
              <span class="chip"><b>◆</b> Responsive Design</span><span class="chip"><b>◆</b> UI/UX Structure</span>
              <span class="chip"><b>◆</b> Wireframing</span>
            </div>
          </div>
          <div class="skill-group">
            <div class="gname">PROFESSIONAL &amp; SPOKEN</div>
            <div class="chips">
              <span class="chip">Communication</span><span class="chip">Teamwork</span>
              <span class="chip">English</span><span class="chip">Telugu — native</span><span class="chip">Hindi</span>
            </div>
          </div>
        </div>
      </section>

      <!-- ================= PROJECTS ================= -->
      <section aria-labelledby="projects-h">
        <div class="sec-head">
          <h2 id="projects-h"><span class="path">~/</span>featured_projects</h2>
          <span class="rule"></span>
          <span class="note">live on GitHub</span>
        </div>
        <div class="grid-3">
          <div class="card proj">
            <div class="top">
              <h3><a href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener">🤖 CareerPlus+ — AI Resume Analyzer</a></h3>
            </div>
            <p>CareerPlus+ uses AI to scan, score, and optimise a CV against industry standards and ATS algorithms — surfacing missing skills, keyword mismatches and structural improvements.</p>
            <span class="lang"><i style="background:#3178c6"></i>TypeScript</span>
          </div>
          <div class="card proj">
            <div class="top">
              <h3><a href="https://siddarthashopease.pythonanywhere.com/" target="_blank" rel="noopener">🛒 ShopEase — E-Commerce</a></h3>
              <a class="live-chip" href="https://siddarthashopease.pythonanywhere.com/" target="_blank" rel="noopener"><i></i>LIVE</a>
            </div>
            <p>Modern e-commerce experience — curated products, smart filtering, easy navigation and a seamless checkout. Now full-stack with Python + SQLite.</p>
            <p class="live-url">Live: <a href="https://siddarthashopease.pythonanywhere.com/" target="_blank" rel="noopener">siddarthashopease.pythonanywhere.com</a></p>
            <span class="lang"><i style="background:#e34c26"></i>HTML</span>
          </div>
          <div class="card proj">
            <div class="top">
              <h3><a href="https://learnhubapp.pythonanywhere.com/" target="_blank" rel="noopener">📚 LearnHub — LMS Website</a></h3>
              <a class="live-chip" href="https://learnhubapp.pythonanywhere.com/" target="_blank" rel="noopener"><i></i>LIVE</a>
            </div>
            <p>Online learning platform with expert-led courses in web development, programming, design, marketing, AI, and business — wishlist and cart, secure checkout and personalised, career-focused learning. Now full-stack with Python + SQLite.</p>
            <p class="live-url">Live: <a href="https://learnhubapp.pythonanywhere.com/" target="_blank" rel="noopener">learnhubapp.pythonanywhere.com</a></p>
            <span class="lang"><i style="background:#e34c26"></i>HTML</span>
          </div>
          <div class="card proj">
            <div class="top">
              <h3><a href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener">🌐 MY-Portfolio</a></h3>
              <a class="live-chip" href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener"><i></i>LIVE</a>
            </div>
            <p>My personal portfolio — AI &amp; ML projects, skills and journey, built as a clean, developer-focused site.</p>
            <p class="live-url">Live: <a href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener">siddartha-jamandla.github.io/MY-Portfolio</a></p>
            <span class="lang"><i style="background:#3178c6"></i>TypeScript</span>
          </div>
          <div class="card proj">
            <div class="top">
              <h3><a href="https://siddartha-jamandla.github.io/Blow-Crackers/" target="_blank" rel="noopener">🪔 Blow Crackers</a></h3>
              <a class="live-chip" href="https://siddartha-jamandla.github.io/Blow-Crackers/" target="_blank" rel="noopener"><i></i>LIVE</a>
            </div>
            <p>Blow 100 Diwali crackers yourself in the browser — interactive fireworks with realistic sounds, 5 themes, Sky Writing, smooth on 2GB phones.</p>
            <p class="live-url">Live: <a href="https://siddartha-jamandla.github.io/Blow-Crackers/" target="_blank" rel="noopener">siddartha-jamandla.github.io/Blow-Crackers</a></p>
            <span class="lang"><i style="background:#e34c26"></i>HTML</span>
          </div>
          <div class="card proj">
            <div class="top">
              <h3><a href="https://github.com/Siddartha-Jamandla/LearnHub-LMS" target="_blank" rel="noopener">📚 LearnHub-LMS — clean rebuild</a></h3>
            </div>
            <p>Clean LearnHub rebuild — C + DSA flagships, no C++ course. Brand: LearnHub, one word.</p>
            <span class="lang"><i style="background:#e34c26"></i>HTML</span>
          </div>
        </div>
      </section>

      <!-- ================= CURRENTLY BUILDING ================= -->
      <section aria-labelledby="building-h">
        <div class="sec-head">
          <h2 id="building-h"><span class="path">~/</span>currently_building</h2>
          <span class="rule"></span>
          <span class="note">built, repo coming soon</span>
        </div>
        <div class="grid-2">
          <div class="card proj">
            <div class="top"><h3>🤖 Testing Agent</h3><span class="soon-chip">BUILT · REPO SOON</span></div>
            <p>Agentic AI that tests websites — Planner → Executor → Verifier, with real link, image, form and security-header checks. Python + SQLite. Demo run: 67.7% pass rate.</p>
            <span class="status-line">Status: Built — repo coming soon</span>
            <span class="lang"><i style="background:#3572A5"></i>Python · SQLite</span>
          </div>
          <div class="card proj">
            <div class="top"><h3>💼 Job Automation Agent</h3><span class="soon-chip">BUILT · REPO SOON</span></div>
            <p>Agentic AI for job hunting — live job fetching, skill-match scoring on my resume, cover-letter generator, and a Saved → Applied → Interview → Offer pipeline with analytics. Python + SQLite.</p>
            <span class="status-line">Status: Built — repo coming soon</span>
            <span class="lang"><i style="background:#3572A5"></i>Python · SQLite</span>
          </div>
          <div class="card proj">
            <div class="top"><h3>📶 OffGrid Chat</h3><span class="soon-chip">BUILT · REPO SOON</span></div>
            <p>Offline-only Android chat, phone-to-phone with no internet or SIM — Bluetooth + Wi-Fi Direct, AES-256 encryption, offline queue and mesh relay. Kotlin + Jetpack Compose.</p>
            <span class="status-line">Status: Built — repo coming soon</span>
            <span class="lang"><i style="background:#A97BFF"></i>Kotlin · Jetpack Compose</span>
          </div>
          <div class="card proj">
            <div class="top"><h3>🎙️ Jarvis — Python Voice Assistant</h3><span class="soon-chip">BUILT · REPO SOON</span></div>
            <p>Voice assistant with wake-word mode, YouTube voice control, weather / news / Wikipedia, notes and reminders, and Gmail / WhatsApp drafts. Python.</p>
            <span class="status-line">Status: Built — repo coming soon</span>
            <span class="lang"><i style="background:#3572A5"></i>Python</span>
          </div>
        </div>
      </section>

      <!-- ================= GITHUB ANALYTICS ================= -->
      <section aria-labelledby="analytics-h">
        <div class="sec-head">
          <h2 id="analytics-h"><span class="path">~/</span>github_analytics</h2>
          <span class="rule"></span>
          <span class="note">real data · github.com</span>
        </div>
        <div class="grid-2">
          <div class="card">
            <h3 style="margin-bottom:14px">🏆 Highlights</h3>
            <ul class="hl-list">
              <li><span class="hl-ico">🌐</span><span><strong>4 live sites</strong> — ShopEase, LearnHub, MY-Portfolio, Blow Crackers</span></li>
              <li><span class="hl-ico">🤖</span><span><strong>4 AI projects built</strong> — CareerPlus+, Testing Agent, Job Automation Agent, Jarvis</span></li>
              <li><span class="hl-ico">📚</span><span><strong>8 public repos</strong> — 3 stars, on GitHub since Oct 2025</span></li>
              <li><span class="hl-ico">🎓</span><span><strong>Diploma in Computer Engineering — 80%</strong>, B.Tech AI &amp; ML in progress</span></li>
              <li><span class="hl-ico">🚀</span><span><strong>ShopEase &amp; LearnHub</strong> being upgraded daily to full-stack Python + SQLite</span></li>
            </ul>
          </div>
          <div class="card">
            <h3 style="margin-bottom:6px">📊 GitHub Contributions</h3>
            <p style="margin-bottom:14px">My real contribution graph, exactly as it appears on my GitHub profile — every day of the last year.</p>
<svg class="contrib-graph" viewBox="0 0 718 132" width="100%" role="img" aria-label="GitHub contribution graph for Siddartha Jamandla: 181 contributions in the last year">
<text class="cg-m" x="30" y="11">Nov</text>
<text class="cg-m" x="82" y="11">Dec</text>
<text class="cg-m" x="134" y="11">Jan</text>
<text class="cg-m" x="186" y="11">Feb</text>
<text class="cg-m" x="238" y="11">Mar</text>
<text class="cg-m" x="303" y="11">Apr</text>
<text class="cg-m" x="355" y="11">May</text>
<text class="cg-m" x="420" y="11">Jun</text>
<text class="cg-m" x="472" y="11">Jul</text>
<text class="cg-m" x="524" y="11">Aug</text>
<text class="cg-m" x="589" y="11">Sep</text>
<text class="cg-m" x="641" y="11">Oct</text>
<text class="cg-m" x="693" y="11">Nov</text>
<text class="cg-d" x="0" y="40">Mon</text>
<text class="cg-d" x="0" y="66">Wed</text>
<text class="cg-d" x="0" y="92">Fri</text>
<rect class="cc l0" x="30" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Nov 9, 2025</title></rect>
<rect class="cc l0" x="30" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Nov 10, 2025</title></rect>
<rect class="cc l0" x="30" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Nov 11, 2025</title></rect>
<rect class="cc l0" x="30" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Nov 12, 2025</title></rect>
<rect class="cc l0" x="30" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Nov 13, 2025</title></rect>
<rect class="cc l0" x="30" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Nov 14, 2025</title></rect>
<rect class="cc l0" x="30" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Nov 15, 2025</title></rect>
<rect class="cc l0" x="43" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Nov 16, 2025</title></rect>
<rect class="cc l0" x="43" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Nov 17, 2025</title></rect>
<rect class="cc l0" x="43" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Nov 18, 2025</title></rect>
<rect class="cc l0" x="43" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Nov 19, 2025</title></rect>
<rect class="cc l0" x="43" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Nov 20, 2025</title></rect>
<rect class="cc l0" x="43" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Nov 21, 2025</title></rect>
<rect class="cc l0" x="43" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Nov 22, 2025</title></rect>
<rect class="cc l0" x="56" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Nov 23, 2025</title></rect>
<rect class="cc l0" x="56" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Nov 24, 2025</title></rect>
<rect class="cc l0" x="56" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Nov 25, 2025</title></rect>
<rect class="cc l0" x="56" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Nov 26, 2025</title></rect>
<rect class="cc l0" x="56" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Nov 27, 2025</title></rect>
<rect class="cc l0" x="56" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Nov 28, 2025</title></rect>
<rect class="cc l0" x="56" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Nov 29, 2025</title></rect>
<rect class="cc l0" x="69" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Nov 30, 2025</title></rect>
<rect class="cc l0" x="69" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Dec 1, 2025</title></rect>
<rect class="cc l0" x="69" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Dec 2, 2025</title></rect>
<rect class="cc l0" x="69" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Dec 3, 2025</title></rect>
<rect class="cc l0" x="69" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Dec 4, 2025</title></rect>
<rect class="cc l0" x="69" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Dec 5, 2025</title></rect>
<rect class="cc l0" x="69" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Dec 6, 2025</title></rect>
<rect class="cc l0" x="82" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Dec 7, 2025</title></rect>
<rect class="cc l0" x="82" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Dec 8, 2025</title></rect>
<rect class="cc l0" x="82" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Dec 9, 2025</title></rect>
<rect class="cc l0" x="82" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Dec 10, 2025</title></rect>
<rect class="cc l0" x="82" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Dec 11, 2025</title></rect>
<rect class="cc l0" x="82" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Dec 12, 2025</title></rect>
<rect class="cc l0" x="82" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Dec 13, 2025</title></rect>
<rect class="cc l0" x="95" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Dec 14, 2025</title></rect>
<rect class="cc l0" x="95" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Dec 15, 2025</title></rect>
<rect class="cc l0" x="95" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Dec 16, 2025</title></rect>
<rect class="cc l0" x="95" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Dec 17, 2025</title></rect>
<rect class="cc l0" x="95" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Dec 18, 2025</title></rect>
<rect class="cc l0" x="95" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Dec 19, 2025</title></rect>
<rect class="cc l0" x="95" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Dec 20, 2025</title></rect>
<rect class="cc l0" x="108" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Dec 21, 2025</title></rect>
<rect class="cc l0" x="108" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Dec 22, 2025</title></rect>
<rect class="cc l0" x="108" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Dec 23, 2025</title></rect>
<rect class="cc l0" x="108" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Dec 24, 2025</title></rect>
<rect class="cc l0" x="108" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Dec 25, 2025</title></rect>
<rect class="cc l0" x="108" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Dec 26, 2025</title></rect>
<rect class="cc l0" x="108" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Dec 27, 2025</title></rect>
<rect class="cc l0" x="121" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Dec 28, 2025</title></rect>
<rect class="cc l0" x="121" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Dec 29, 2025</title></rect>
<rect class="cc l0" x="121" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Dec 30, 2025</title></rect>
<rect class="cc l0" x="121" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Dec 31, 2025</title></rect>
<rect class="cc l0" x="121" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jan 1, 2026</title></rect>
<rect class="cc l0" x="121" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jan 2, 2026</title></rect>
<rect class="cc l0" x="121" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jan 3, 2026</title></rect>
<rect class="cc l0" x="134" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jan 4, 2026</title></rect>
<rect class="cc l0" x="134" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jan 5, 2026</title></rect>
<rect class="cc l0" x="134" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jan 6, 2026</title></rect>
<rect class="cc l0" x="134" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jan 7, 2026</title></rect>
<rect class="cc l0" x="134" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jan 8, 2026</title></rect>
<rect class="cc l0" x="134" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jan 9, 2026</title></rect>
<rect class="cc l0" x="134" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jan 10, 2026</title></rect>
<rect class="cc l0" x="147" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jan 11, 2026</title></rect>
<rect class="cc l0" x="147" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jan 12, 2026</title></rect>
<rect class="cc l0" x="147" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jan 13, 2026</title></rect>
<rect class="cc l0" x="147" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jan 14, 2026</title></rect>
<rect class="cc l0" x="147" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jan 15, 2026</title></rect>
<rect class="cc l0" x="147" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jan 16, 2026</title></rect>
<rect class="cc l0" x="147" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jan 17, 2026</title></rect>
<rect class="cc l0" x="160" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jan 18, 2026</title></rect>
<rect class="cc l0" x="160" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jan 19, 2026</title></rect>
<rect class="cc l0" x="160" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jan 20, 2026</title></rect>
<rect class="cc l0" x="160" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jan 21, 2026</title></rect>
<rect class="cc l0" x="160" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jan 22, 2026</title></rect>
<rect class="cc l0" x="160" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jan 23, 2026</title></rect>
<rect class="cc l0" x="160" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jan 24, 2026</title></rect>
<rect class="cc l0" x="173" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jan 25, 2026</title></rect>
<rect class="cc l0" x="173" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jan 26, 2026</title></rect>
<rect class="cc l0" x="173" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jan 27, 2026</title></rect>
<rect class="cc l0" x="173" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jan 28, 2026</title></rect>
<rect class="cc l0" x="173" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jan 29, 2026</title></rect>
<rect class="cc l0" x="173" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jan 30, 2026</title></rect>
<rect class="cc l0" x="173" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jan 31, 2026</title></rect>
<rect class="cc l0" x="186" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Feb 1, 2026</title></rect>
<rect class="cc l0" x="186" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Feb 2, 2026</title></rect>
<rect class="cc l0" x="186" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Feb 3, 2026</title></rect>
<rect class="cc l0" x="186" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Feb 4, 2026</title></rect>
<rect class="cc l0" x="186" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Feb 5, 2026</title></rect>
<rect class="cc l0" x="186" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Feb 6, 2026</title></rect>
<rect class="cc l0" x="186" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Feb 7, 2026</title></rect>
<rect class="cc l0" x="199" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Feb 8, 2026</title></rect>
<rect class="cc l0" x="199" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Feb 9, 2026</title></rect>
<rect class="cc l0" x="199" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Feb 10, 2026</title></rect>
<rect class="cc l0" x="199" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Feb 11, 2026</title></rect>
<rect class="cc l0" x="199" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Feb 12, 2026</title></rect>
<rect class="cc l0" x="199" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Feb 13, 2026</title></rect>
<rect class="cc l0" x="199" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Feb 14, 2026</title></rect>
<rect class="cc l0" x="212" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Feb 15, 2026</title></rect>
<rect class="cc l0" x="212" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Feb 16, 2026</title></rect>
<rect class="cc l0" x="212" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Feb 17, 2026</title></rect>
<rect class="cc l0" x="212" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Feb 18, 2026</title></rect>
<rect class="cc l0" x="212" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Feb 19, 2026</title></rect>
<rect class="cc l0" x="212" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Feb 20, 2026</title></rect>
<rect class="cc l0" x="212" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Feb 21, 2026</title></rect>
<rect class="cc l0" x="225" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Feb 22, 2026</title></rect>
<rect class="cc l0" x="225" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Feb 23, 2026</title></rect>
<rect class="cc l0" x="225" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Feb 24, 2026</title></rect>
<rect class="cc l0" x="225" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Feb 25, 2026</title></rect>
<rect class="cc l0" x="225" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Feb 26, 2026</title></rect>
<rect class="cc l0" x="225" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Feb 27, 2026</title></rect>
<rect class="cc l0" x="225" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Feb 28, 2026</title></rect>
<rect class="cc l0" x="238" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Mar 1, 2026</title></rect>
<rect class="cc l0" x="238" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Mar 2, 2026</title></rect>
<rect class="cc l0" x="238" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Mar 3, 2026</title></rect>
<rect class="cc l0" x="238" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Mar 4, 2026</title></rect>
<rect class="cc l0" x="238" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Mar 5, 2026</title></rect>
<rect class="cc l0" x="238" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Mar 6, 2026</title></rect>
<rect class="cc l0" x="238" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Mar 7, 2026</title></rect>
<rect class="cc l0" x="251" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Mar 8, 2026</title></rect>
<rect class="cc l0" x="251" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Mar 9, 2026</title></rect>
<rect class="cc l0" x="251" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Mar 10, 2026</title></rect>
<rect class="cc l0" x="251" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Mar 11, 2026</title></rect>
<rect class="cc l0" x="251" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Mar 12, 2026</title></rect>
<rect class="cc l0" x="251" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Mar 13, 2026</title></rect>
<rect class="cc l0" x="251" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Mar 14, 2026</title></rect>
<rect class="cc l0" x="264" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Mar 15, 2026</title></rect>
<rect class="cc l0" x="264" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Mar 16, 2026</title></rect>
<rect class="cc l0" x="264" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Mar 17, 2026</title></rect>
<rect class="cc l0" x="264" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Mar 18, 2026</title></rect>
<rect class="cc l0" x="264" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Mar 19, 2026</title></rect>
<rect class="cc l0" x="264" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Mar 20, 2026</title></rect>
<rect class="cc l0" x="264" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Mar 21, 2026</title></rect>
<rect class="cc l0" x="277" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Mar 22, 2026</title></rect>
<rect class="cc l0" x="277" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Mar 23, 2026</title></rect>
<rect class="cc l0" x="277" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Mar 24, 2026</title></rect>
<rect class="cc l0" x="277" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Mar 25, 2026</title></rect>
<rect class="cc l0" x="277" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Mar 26, 2026</title></rect>
<rect class="cc l0" x="277" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Mar 27, 2026</title></rect>
<rect class="cc l0" x="277" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Mar 28, 2026</title></rect>
<rect class="cc l0" x="290" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Mar 29, 2026</title></rect>
<rect class="cc l0" x="290" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Mar 30, 2026</title></rect>
<rect class="cc l0" x="290" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Mar 31, 2026</title></rect>
<rect class="cc l0" x="290" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Apr 1, 2026</title></rect>
<rect class="cc l0" x="290" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Apr 2, 2026</title></rect>
<rect class="cc l0" x="290" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Apr 3, 2026</title></rect>
<rect class="cc l0" x="290" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Apr 4, 2026</title></rect>
<rect class="cc l0" x="303" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Apr 5, 2026</title></rect>
<rect class="cc l0" x="303" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Apr 6, 2026</title></rect>
<rect class="cc l0" x="303" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Apr 7, 2026</title></rect>
<rect class="cc l0" x="303" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Apr 8, 2026</title></rect>
<rect class="cc l0" x="303" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Apr 9, 2026</title></rect>
<rect class="cc l0" x="303" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Apr 10, 2026</title></rect>
<rect class="cc l0" x="303" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Apr 11, 2026</title></rect>
<rect class="cc l0" x="316" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Apr 12, 2026</title></rect>
<rect class="cc l0" x="316" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Apr 13, 2026</title></rect>
<rect class="cc l0" x="316" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Apr 14, 2026</title></rect>
<rect class="cc l0" x="316" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Apr 15, 2026</title></rect>
<rect class="cc l0" x="316" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Apr 16, 2026</title></rect>
<rect class="cc l0" x="316" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Apr 17, 2026</title></rect>
<rect class="cc l0" x="316" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Apr 18, 2026</title></rect>
<rect class="cc l0" x="329" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Apr 19, 2026</title></rect>
<rect class="cc l0" x="329" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Apr 20, 2026</title></rect>
<rect class="cc l0" x="329" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Apr 21, 2026</title></rect>
<rect class="cc l0" x="329" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Apr 22, 2026</title></rect>
<rect class="cc l0" x="329" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Apr 23, 2026</title></rect>
<rect class="cc l0" x="329" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Apr 24, 2026</title></rect>
<rect class="cc l0" x="329" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Apr 25, 2026</title></rect>
<rect class="cc l0" x="342" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Apr 26, 2026</title></rect>
<rect class="cc l0" x="342" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Apr 27, 2026</title></rect>
<rect class="cc l0" x="342" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Apr 28, 2026</title></rect>
<rect class="cc l0" x="342" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Apr 29, 2026</title></rect>
<rect class="cc l0" x="342" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Apr 30, 2026</title></rect>
<rect class="cc l0" x="342" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, May 1, 2026</title></rect>
<rect class="cc l0" x="342" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, May 2, 2026</title></rect>
<rect class="cc l0" x="355" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, May 3, 2026</title></rect>
<rect class="cc l0" x="355" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, May 4, 2026</title></rect>
<rect class="cc l0" x="355" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, May 5, 2026</title></rect>
<rect class="cc l0" x="355" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, May 6, 2026</title></rect>
<rect class="cc l0" x="355" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, May 7, 2026</title></rect>
<rect class="cc l0" x="355" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, May 8, 2026</title></rect>
<rect class="cc l0" x="355" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, May 9, 2026</title></rect>
<rect class="cc l0" x="368" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, May 10, 2026</title></rect>
<rect class="cc l0" x="368" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, May 11, 2026</title></rect>
<rect class="cc l0" x="368" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, May 12, 2026</title></rect>
<rect class="cc l0" x="368" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, May 13, 2026</title></rect>
<rect class="cc l0" x="368" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, May 14, 2026</title></rect>
<rect class="cc l0" x="368" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, May 15, 2026</title></rect>
<rect class="cc l0" x="368" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, May 16, 2026</title></rect>
<rect class="cc l0" x="381" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, May 17, 2026</title></rect>
<rect class="cc l0" x="381" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, May 18, 2026</title></rect>
<rect class="cc l0" x="381" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, May 19, 2026</title></rect>
<rect class="cc l0" x="381" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, May 20, 2026</title></rect>
<rect class="cc l0" x="381" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, May 21, 2026</title></rect>
<rect class="cc l0" x="381" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, May 22, 2026</title></rect>
<rect class="cc l0" x="381" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, May 23, 2026</title></rect>
<rect class="cc l0" x="394" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, May 24, 2026</title></rect>
<rect class="cc l0" x="394" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, May 25, 2026</title></rect>
<rect class="cc l0" x="394" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, May 26, 2026</title></rect>
<rect class="cc l0" x="394" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, May 27, 2026</title></rect>
<rect class="cc l0" x="394" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, May 28, 2026</title></rect>
<rect class="cc l0" x="394" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, May 29, 2026</title></rect>
<rect class="cc l0" x="394" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, May 30, 2026</title></rect>
<rect class="cc l0" x="407" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, May 31, 2026</title></rect>
<rect class="cc l0" x="407" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jun 1, 2026</title></rect>
<rect class="cc l0" x="407" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jun 2, 2026</title></rect>
<rect class="cc l0" x="407" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jun 3, 2026</title></rect>
<rect class="cc l0" x="407" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jun 4, 2026</title></rect>
<rect class="cc l0" x="407" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jun 5, 2026</title></rect>
<rect class="cc l0" x="407" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jun 6, 2026</title></rect>
<rect class="cc l0" x="420" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jun 7, 2026</title></rect>
<rect class="cc l0" x="420" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jun 8, 2026</title></rect>
<rect class="cc l0" x="420" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jun 9, 2026</title></rect>
<rect class="cc l0" x="420" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jun 10, 2026</title></rect>
<rect class="cc l0" x="420" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jun 11, 2026</title></rect>
<rect class="cc l0" x="420" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jun 12, 2026</title></rect>
<rect class="cc l0" x="420" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jun 13, 2026</title></rect>
<rect class="cc l0" x="433" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jun 14, 2026</title></rect>
<rect class="cc l0" x="433" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jun 15, 2026</title></rect>
<rect class="cc l0" x="433" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jun 16, 2026</title></rect>
<rect class="cc l0" x="433" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jun 17, 2026</title></rect>
<rect class="cc l0" x="433" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jun 18, 2026</title></rect>
<rect class="cc l0" x="433" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jun 19, 2026</title></rect>
<rect class="cc l0" x="433" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jun 20, 2026</title></rect>
<rect class="cc l0" x="446" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jun 21, 2026</title></rect>
<rect class="cc l0" x="446" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jun 22, 2026</title></rect>
<rect class="cc l0" x="446" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jun 23, 2026</title></rect>
<rect class="cc l0" x="446" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jun 24, 2026</title></rect>
<rect class="cc l0" x="446" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jun 25, 2026</title></rect>
<rect class="cc l0" x="446" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jun 26, 2026</title></rect>
<rect class="cc l0" x="446" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jun 27, 2026</title></rect>
<rect class="cc l0" x="459" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jun 28, 2026</title></rect>
<rect class="cc l0" x="459" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jun 29, 2026</title></rect>
<rect class="cc l0" x="459" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jun 30, 2026</title></rect>
<rect class="cc l0" x="459" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jul 1, 2026</title></rect>
<rect class="cc l0" x="459" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jul 2, 2026</title></rect>
<rect class="cc l0" x="459" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jul 3, 2026</title></rect>
<rect class="cc l0" x="459" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jul 4, 2026</title></rect>
<rect class="cc l0" x="472" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jul 5, 2026</title></rect>
<rect class="cc l0" x="472" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jul 6, 2026</title></rect>
<rect class="cc l0" x="472" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jul 7, 2026</title></rect>
<rect class="cc l0" x="472" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jul 8, 2026</title></rect>
<rect class="cc l0" x="472" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jul 9, 2026</title></rect>
<rect class="cc l0" x="472" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jul 10, 2026</title></rect>
<rect class="cc l0" x="472" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jul 11, 2026</title></rect>
<rect class="cc l0" x="485" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jul 12, 2026</title></rect>
<rect class="cc l0" x="485" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jul 13, 2026</title></rect>
<rect class="cc l0" x="485" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jul 14, 2026</title></rect>
<rect class="cc l0" x="485" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jul 15, 2026</title></rect>
<rect class="cc l0" x="485" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jul 16, 2026</title></rect>
<rect class="cc l0" x="485" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jul 17, 2026</title></rect>
<rect class="cc l0" x="485" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jul 18, 2026</title></rect>
<rect class="cc l0" x="498" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jul 19, 2026</title></rect>
<rect class="cc l0" x="498" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jul 20, 2026</title></rect>
<rect class="cc l0" x="498" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jul 21, 2026</title></rect>
<rect class="cc l0" x="498" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jul 22, 2026</title></rect>
<rect class="cc l0" x="498" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jul 23, 2026</title></rect>
<rect class="cc l0" x="498" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jul 24, 2026</title></rect>
<rect class="cc l0" x="498" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Jul 25, 2026</title></rect>
<rect class="cc l0" x="511" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Jul 26, 2026</title></rect>
<rect class="cc l0" x="511" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Jul 27, 2026</title></rect>
<rect class="cc l0" x="511" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Jul 28, 2026</title></rect>
<rect class="cc l0" x="511" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Jul 29, 2026</title></rect>
<rect class="cc l0" x="511" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Jul 30, 2026</title></rect>
<rect class="cc l0" x="511" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Jul 31, 2026</title></rect>
<rect class="cc l0" x="511" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Aug 1, 2026</title></rect>
<rect class="cc l2" x="524" y="18" width="10" height="10" rx="2"><title>6 contributions on Sun, Aug 2, 2026</title></rect>
<rect class="cc l0" x="524" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Aug 3, 2026</title></rect>
<rect class="cc l0" x="524" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Aug 4, 2026</title></rect>
<rect class="cc l0" x="524" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Aug 5, 2026</title></rect>
<rect class="cc l3" x="524" y="70" width="10" height="10" rx="2"><title>11 contributions on Thu, Aug 6, 2026</title></rect>
<rect class="cc l3" x="524" y="83" width="10" height="10" rx="2"><title>8 contributions on Fri, Aug 7, 2026</title></rect>
<rect class="cc l0" x="524" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Aug 8, 2026</title></rect>
<rect class="cc l0" x="537" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Aug 9, 2026</title></rect>
<rect class="cc l0" x="537" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Aug 10, 2026</title></rect>
<rect class="cc l0" x="537" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Aug 11, 2026</title></rect>
<rect class="cc l0" x="537" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Aug 12, 2026</title></rect>
<rect class="cc l0" x="537" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Aug 13, 2026</title></rect>
<rect class="cc l0" x="537" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Aug 14, 2026</title></rect>
<rect class="cc l0" x="537" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Aug 15, 2026</title></rect>
<rect class="cc l0" x="550" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Aug 16, 2026</title></rect>
<rect class="cc l0" x="550" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Aug 17, 2026</title></rect>
<rect class="cc l0" x="550" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Aug 18, 2026</title></rect>
<rect class="cc l0" x="550" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Aug 19, 2026</title></rect>
<rect class="cc l0" x="550" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Aug 20, 2026</title></rect>
<rect class="cc l0" x="550" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Aug 21, 2026</title></rect>
<rect class="cc l0" x="550" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Aug 22, 2026</title></rect>
<rect class="cc l0" x="563" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Aug 23, 2026</title></rect>
<rect class="cc l1" x="563" y="31" width="10" height="10" rx="2"><title>2 contributions on Mon, Aug 24, 2026</title></rect>
<rect class="cc l0" x="563" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Aug 25, 2026</title></rect>
<rect class="cc l0" x="563" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Aug 26, 2026</title></rect>
<rect class="cc l0" x="563" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Aug 27, 2026</title></rect>
<rect class="cc l0" x="563" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Aug 28, 2026</title></rect>
<rect class="cc l0" x="563" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Aug 29, 2026</title></rect>
<rect class="cc l1" x="576" y="18" width="10" height="10" rx="2"><title>2 contributions on Sun, Aug 30, 2026</title></rect>
<rect class="cc l0" x="576" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Aug 31, 2026</title></rect>
<rect class="cc l0" x="576" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Sep 1, 2026</title></rect>
<rect class="cc l0" x="576" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Sep 2, 2026</title></rect>
<rect class="cc l0" x="576" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Sep 3, 2026</title></rect>
<rect class="cc l0" x="576" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Sep 4, 2026</title></rect>
<rect class="cc l0" x="576" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Sep 5, 2026</title></rect>
<rect class="cc l0" x="589" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Sep 6, 2026</title></rect>
<rect class="cc l1" x="589" y="31" width="10" height="10" rx="2"><title>1 contribution on Mon, Sep 7, 2026</title></rect>
<rect class="cc l0" x="589" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Sep 8, 2026</title></rect>
<rect class="cc l0" x="589" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Sep 9, 2026</title></rect>
<rect class="cc l0" x="589" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Sep 10, 2026</title></rect>
<rect class="cc l3" x="589" y="83" width="10" height="10" rx="2"><title>8 contributions on Fri, Sep 11, 2026</title></rect>
<rect class="cc l0" x="589" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Sep 12, 2026</title></rect>
<rect class="cc l0" x="602" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Sep 13, 2026</title></rect>
<rect class="cc l0" x="602" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Sep 14, 2026</title></rect>
<rect class="cc l0" x="602" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Sep 15, 2026</title></rect>
<rect class="cc l0" x="602" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Sep 16, 2026</title></rect>
<rect class="cc l0" x="602" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Sep 17, 2026</title></rect>
<rect class="cc l0" x="602" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Sep 18, 2026</title></rect>
<rect class="cc l0" x="602" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Sep 19, 2026</title></rect>
<rect class="cc l0" x="615" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Sep 20, 2026</title></rect>
<rect class="cc l0" x="615" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Sep 21, 2026</title></rect>
<rect class="cc l0" x="615" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Sep 22, 2026</title></rect>
<rect class="cc l0" x="615" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Sep 23, 2026</title></rect>
<rect class="cc l0" x="615" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Sep 24, 2026</title></rect>
<rect class="cc l0" x="615" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Sep 25, 2026</title></rect>
<rect class="cc l0" x="615" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Sep 26, 2026</title></rect>
<rect class="cc l0" x="628" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Sep 27, 2026</title></rect>
<rect class="cc l0" x="628" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Sep 28, 2026</title></rect>
<rect class="cc l0" x="628" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Sep 29, 2026</title></rect>
<rect class="cc l0" x="628" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Sep 30, 2026</title></rect>
<rect class="cc l0" x="628" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Oct 1, 2026</title></rect>
<rect class="cc l0" x="628" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Oct 2, 2026</title></rect>
<rect class="cc l0" x="628" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Oct 3, 2026</title></rect>
<rect class="cc l0" x="641" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Oct 4, 2026</title></rect>
<rect class="cc l0" x="641" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Oct 5, 2026</title></rect>
<rect class="cc l0" x="641" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Oct 6, 2026</title></rect>
<rect class="cc l0" x="641" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Oct 7, 2026</title></rect>
<rect class="cc l0" x="641" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Oct 8, 2026</title></rect>
<rect class="cc l0" x="641" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Oct 9, 2026</title></rect>
<rect class="cc l0" x="641" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Oct 10, 2026</title></rect>
<rect class="cc l0" x="654" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Oct 11, 2026</title></rect>
<rect class="cc l0" x="654" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Oct 12, 2026</title></rect>
<rect class="cc l0" x="654" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Oct 13, 2026</title></rect>
<rect class="cc l0" x="654" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Oct 14, 2026</title></rect>
<rect class="cc l0" x="654" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Oct 15, 2026</title></rect>
<rect class="cc l0" x="654" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Oct 16, 2026</title></rect>
<rect class="cc l0" x="654" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Oct 17, 2026</title></rect>
<rect class="cc l0" x="667" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Oct 18, 2026</title></rect>
<rect class="cc l0" x="667" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Oct 19, 2026</title></rect>
<rect class="cc l0" x="667" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Oct 20, 2026</title></rect>
<rect class="cc l0" x="667" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Oct 21, 2026</title></rect>
<rect class="cc l0" x="667" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Oct 22, 2026</title></rect>
<rect class="cc l0" x="667" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Oct 23, 2026</title></rect>
<rect class="cc l0" x="667" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Oct 24, 2026</title></rect>
<rect class="cc l0" x="680" y="18" width="10" height="10" rx="2"><title>No contributions on Sun, Oct 25, 2026</title></rect>
<rect class="cc l0" x="680" y="31" width="10" height="10" rx="2"><title>No contributions on Mon, Oct 26, 2026</title></rect>
<rect class="cc l0" x="680" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Oct 27, 2026</title></rect>
<rect class="cc l0" x="680" y="57" width="10" height="10" rx="2"><title>No contributions on Wed, Oct 28, 2026</title></rect>
<rect class="cc l0" x="680" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Oct 29, 2026</title></rect>
<rect class="cc l0" x="680" y="83" width="10" height="10" rx="2"><title>No contributions on Fri, Oct 30, 2026</title></rect>
<rect class="cc l4" x="680" y="96" width="10" height="10" rx="2"><title>12 contributions on Sat, Oct 31, 2026</title></rect>
<rect class="cc l3" x="693" y="18" width="10" height="10" rx="2"><title>8 contributions on Sun, Nov 1, 2026</title></rect>
<rect class="cc l1" x="693" y="31" width="10" height="10" rx="2"><title>3 contributions on Mon, Nov 2, 2026</title></rect>
<rect class="cc l0" x="693" y="44" width="10" height="10" rx="2"><title>No contributions on Tue, Nov 3, 2026</title></rect>
<rect class="cc l4" x="693" y="57" width="10" height="10" rx="2"><title>15 contributions on Wed, Nov 4, 2026</title></rect>
<rect class="cc l0" x="693" y="70" width="10" height="10" rx="2"><title>No contributions on Thu, Nov 5, 2026</title></rect>
<rect class="cc l1" x="693" y="83" width="10" height="10" rx="2"><title>2 contributions on Fri, Nov 6, 2026</title></rect>
<rect class="cc l0" x="693" y="96" width="10" height="10" rx="2"><title>No contributions on Sat, Nov 7, 2026</title></rect>
<rect class="cc l4" x="706" y="18" width="10" height="10" rx="2"><title>34 contributions on Sun, Nov 8, 2026</title></rect>
<rect class="cc l4" x="706" y="31" width="10" height="10" rx="2"><title>69 contributions on Mon, Nov 9, 2026</title></rect>
<text class="cg-m" x="570" y="133">Less</text>
<rect class="cc l0" x="600" y="124" width="10" height="10" rx="2"></rect>
<rect class="cc l1" x="613" y="124" width="10" height="10" rx="2"></rect>
<rect class="cc l2" x="626" y="124" width="10" height="10" rx="2"></rect>
<rect class="cc l3" x="639" y="124" width="10" height="10" rx="2"></rect>
<rect class="cc l4" x="652" y="124" width="10" height="10" rx="2"></rect>
<text class="cg-m" x="667" y="133">More</text>
</svg>
            <div class="contrib-stats">
              <span class="hud-chip">TOTAL <b>181</b> contributions</span>
              <span class="hud-chip">ACTIVE DAYS <b>14</b></span>
              <span class="hud-chip">BUSIEST DAY <b>69</b> · Nov 9, 2026</span>
            </div>
            <p style="margin-top:12px">Snapshot from <a href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener">github.com/Siddartha-Jamandla</a> · Nov 10, 2026 · <a href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener">View live stats, streak &amp; languages on GitHub →</a></p>
          </div>
        </div>
      </section>

      <!-- ================= ACHIEVEMENTS ================= -->
      <section aria-labelledby="achieve-h">
        <div class="sec-head">
          <h2 id="achieve-h"><span class="path">~/</span>github_achievements</h2>
          <span class="rule"></span>
        </div>
        <div class="card">
          <div class="achieve">
            <span class="badge-pill ok">Quickdraw ✅</span>
            <span class="badge-pill ok">YOLO ✅</span>
            <span class="badge-pill wait">Pull Shark ⏳</span>
            <span style="font-size:13.5px;color:var(--mut)">16 merged PRs done — the badge appears once GitHub processes it</span>
          </div>
        </div>
      </section>

      <!-- ================= CURRENTLY FOCUSED ================= -->
      <section aria-labelledby="focused-h">
        <div class="sec-head">
          <h2 id="focused-h"><span class="path">~/</span>currently_focused_on</h2>
          <span class="rule"></span>
        </div>
        <div class="card">
          <ul class="focus-now">
            <li><span class="hl-ico">🤖</span><span><strong>Artificial Intelligence &amp; Machine Learning</strong></span></li>
            <li><span class="hl-ico">⚡</span><span><strong>AI agents &amp; automation</strong> — Testing Agent, Job Automation Agent</span></li>
            <li><span class="hl-ico">🌐</span><span><strong>Responsive web development</strong> — ShopEase &amp; LearnHub, full-stack with Python + SQLite</span></li>
            <li><span class="hl-ico">🧩</span><span><strong>Data Structures &amp; Algorithms, OOP</strong> — daily practice</span></li>
            <li><span class="hl-ico">🚀</span><span><strong>Building real-world projects</strong> — and landing a paid, remote internship</span></li>
          </ul>
        </div>
      </section>

      <!-- ================= JOURNEY ================= -->
      <section aria-labelledby="journey-h">
        <div class="sec-head">
          <h2 id="journey-h"><span class="path">~/</span>my_journey</h2>
          <span class="rule"></span>
          <span class="note">Learn → Build → Improve → Repeat</span>
        </div>
        <div class="card">
          <div class="journey-flow" aria-label="Journey steps">
            <span class="jstep">💡 Idea</span><span class="jarrow">→</span>
            <span class="jstep">📚 Research</span><span class="jarrow">→</span>
            <span class="jstep">📝 Plan</span><span class="jarrow">→</span>
            <span class="jstep">💻 Build</span><span class="jarrow">→</span>
            <span class="jstep">🧪 Test</span><span class="jarrow">→</span>
            <span class="jstep">🚀 Deploy live</span><span class="jarrow">→</span>
            <span class="jstep">📈 Improve daily</span>
          </div>
          <p style="font-size:14.5px;line-height:1.7;color:var(--mut);margin:0"><strong style="color:var(--ink)">Where I am now:</strong> B.Tech AI &amp; ML, 2nd year — building AI tools, AI agents and full-stack web apps every day, and growing this profile with real shipped work.</p>
        </div>
      </section>

      <!-- ================= EDUCATION ================= -->
      <section aria-labelledby="edu-h">
        <div class="sec-head">
          <h2 id="edu-h"><span class="path">~/</span>education_&amp;_certs</h2>
          <span class="rule"></span>
        </div>
        <div class="card">
          <div class="edu-item">
            <div class="edu-mark">B.T</div>
            <div>
              <h3>B.Tech, AI &amp; ML — 2nd Year</h3>
              <p>Balaji Institute of Technology and Science, Narsampet, Warangal, Telangana · Lateral entry into 2nd year · CGPA 8.0/10</p>
            </div>
            <span class="when">2026 — 2029</span>
          </div>
          <div class="edu-item">
            <div class="edu-mark">DIP</div>
            <div>
              <h3>Diploma in Computer Engineering — 80%</h3>
              <p>Warangal Institute of Technology and Science · Completed before joining B.Tech through lateral entry.</p>
            </div>
            <span class="when">2023 — 2026</span>
          </div>
          <div class="edu-item">
            <div class="edu-mark">SSC</div>
            <div>
              <h3>SSC — 78%</h3>
              <p>ZPHS Itikalapally, Narsampet</p>
            </div>
            <span class="when">2023</span>
          </div>
          <div class="edu-item">
            <div class="edu-mark">CRT</div>
            <div>
              <h3>Certification: Web Designing and Development</h3>
              <p>CADD Centre, Hanumakonda</p>
            </div>
            <span class="when">CERTIFIED</span>
          </div>
        </div>
      </section>

      <!-- ================= OPEN TO ================= -->
      <section aria-labelledby="open-h">
        <div class="sec-head">
          <h2 id="open-h"><span class="path">~/</span>open_to</h2>
          <span class="rule"></span>
        </div>
        <div class="open-grid">
          <div class="card open-item"><span class="hl-ico">💼</span><div><h3>Paid remote internships</h3><p>AI / ML, Python, Web Development</p></div></div>
          <div class="card open-item"><span class="hl-ico">🤖</span><div><h3>AI / Machine Learning projects</h3><p>AI-powered tools and ML work</p></div></div>
          <div class="card open-item"><span class="hl-ico">🌐</span><div><h3>Full-stack web development</h3><p>Responsive apps with real backends</p></div></div>
          <div class="card open-item"><span class="hl-ico">🚀</span><div><h3>Open source contributions</h3><p>Projects where I can ship real code</p></div></div>
          <div class="card open-item"><span class="hl-ico">💡</span><div><h3>Startup collaborations</h3><p>Building products with small teams</p></div></div>
        </div>
      </section>

      <!-- ================= CONNECT ================= -->
      <section aria-labelledby="connect-h">
        <div class="sec-head">
          <h2 id="connect-h"><span class="path">~/</span>connect_with_me</h2>
          <span class="rule"></span>
        </div>
        <div class="connect-grid">
          <a class="card connect-item" href="mailto:siddarthajamandla@gmail.com"><span class="hl-ico">📧</span><span><span class="cl">EMAIL</span><br /><span class="cv">siddarthajamandla@gmail.com</span></span></a>
          <a class="card connect-item" href="https://www.linkedin.com/in/siddartha-jamandla-97350b384" target="_blank" rel="noopener"><span class="hl-ico">💼</span><span><span class="cl">LINKEDIN</span><br /><span class="cv">linkedin.com/in/siddartha-jamandla-97350b384</span></span></a>
          <a class="card connect-item" href="https://www.instagram.com/siddu_edits_hub" target="_blank" rel="noopener"><span class="hl-ico">📸</span><span><span class="cl">INSTAGRAM</span><br /><span class="cv">instagram.com/siddu_edits_hub</span></span></a>
          <a class="card connect-item" href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener"><span class="hl-ico">🌐</span><span><span class="cl">PORTFOLIO</span><br /><span class="cv">siddartha-jamandla.github.io/MY-Portfolio</span></span></a>
          <a class="card connect-item" href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener"><span class="hl-ico">🐙</span><span><span class="cl">GITHUB</span><br /><span class="cv">github.com/Siddartha-Jamandla</span></span></a>
        </div>
      </section>

      <!-- ================= QUOTE ================= -->
      <section aria-label="Closing quote">
        <div class="card quote-block">
          <blockquote>“Discipline builds skill. Skill creates opportunities. Opportunities shape the future.”</blockquote>
          <p>The future belongs to those who build it.</p>
        </div>
      </section>

      <footer>
        <span class="who">© Siddartha Jamandla · Warangal, Telangana, India</span>
        <nav>
          <a href="https://github.com/Siddartha-Jamandla" target="_blank" rel="noopener">GitHub</a>
          <a href="https://www.linkedin.com/in/siddartha-jamandla-97350b384" target="_blank" rel="noopener">LinkedIn</a>
          <a href="https://www.instagram.com/siddu_edits_hub" target="_blank" rel="noopener">Instagram</a>
          <a href="https://siddartha-jamandla.github.io/MY-Portfolio/" target="_blank" rel="noopener">Portfolio</a>
          <a href="mailto:siddarthajamandla@gmail.com">siddarthajamandla@gmail.com</a>
        </nav>
      </footer>
    </div>

    <script>
      (function () {
        "use strict";

        /* ============ typing role line ============ */
        var roles = [
          "B.Tech AI & ML Student",
          "Python Developer",
          "Builder of CareerPlus+",
          "Full-Stack Web Developer",
          "AI Agents · Automation"
        ];
        var typer = document.getElementById("typer");
        var reduceMotion = window.matchMedia("(prefers-reduced-motion: reduce)").matches;
        if (typer && !reduceMotion) {
          var ri = 0, ci = roles[0].length, deleting = false;
          (function tick() {
            var word = roles[ri];
            if (!deleting) {
              ci++;
              typer.textContent = word.slice(0, ci);
              if (ci === word.length) { deleting = true; return setTimeout(tick, 1900); }
              return setTimeout(tick, 55);
            }
            ci--;
            typer.textContent = word.slice(0, ci);
            if (ci === 0) { deleting = false; ri = (ri + 1) % roles.length; return setTimeout(tick, 350); }
            setTimeout(tick, 28);
          })();
        }

        /* ============ VISUAL.MAP particle engine ============ */
        var canvas = document.getElementById("stage");
        var ctx = canvas.getContext("2d");
        var CW = 880, CH = 640; // logical stage size (portrait panel, landscape)
        var dpr = Math.min(window.devicePixelRatio || 1, 2);
        canvas.width = CW * dpr; canvas.height = CH * dpr;
        ctx.setTransform(dpr, 0, 0, dpr, 0, 0);

        // The portrait panel: centred and filling the stage, aspect locked to
        // the sampler (288x360 = 0.8) so the face is never stretched
        var PANEL = { x: 224, y: 50, w: 432, h: 540 };
        var CENTER = { x: CW / 2, y: CH / 2 };
        // Tight source crop on head + shoulders from the 460x460 photo
        var CROP = { x: 86, y: 2, w: 288, h: 360 };

        var PALETTE = ["#c084fc", "#a855f7", "#8b5cf6", "#f472b6", "#e879f9", "#3ee6ff", "#7dd3fc"];

        /* ---------- samplers: everything returns [{x,y,r,g,b}] in stage coords ---------- */
        function makeSampler(w, h) {
          var c = document.createElement("canvas"); c.width = w; c.height = h;
          return { c: c, x: c.getContext("2d", { willReadFrequently: true }) };
        }
        function collect(s, step, keepFn) {
          var d = s.x.getImageData(0, 0, s.c.width, s.c.height).data;
          var pts = [];
          for (var y = 0; y < s.c.height; y += step) {
            for (var x = 0; x < s.c.width; x += step) {
              var i = (y * s.c.width + x) * 4;
              var keep = keepFn(d[i], d[i + 1], d[i + 2], d[i + 3], x, y);
              if (keep) pts.push({ sx: x, sy: y, r: d[i], g: d[i + 1], b: d[i + 2] });
            }
          }
          return pts;
        }
        // map sampler points into a stage rect
        function fit(pts, sw, sh, rect) {
          return pts.map(function (p) {
            return {
              x: rect.x + (p.sx / sw) * rect.w,
              y: rect.y + (p.sy / sh) * rect.h,
              r: p.r, g: p.g, b: p.b
            };
          });
        }

        /* portrait: tight face crop, DENSE uniform grid — every grid point
           inside the subject silhouette is kept (no random dropout, which is
           what dissolved the face into noise), the office background is
           masked out entirely, and colours get a contrast/saturation lift so
           hair, eyes, brows and mouth read clearly at dot size */
        function samplePortrait(img) {
          var SW = 288, SH = 360;
          var s = makeSampler(SW, SH);
          s.x.drawImage(img, CROP.x, CROP.y, CROP.w, CROP.h, 0, 0, SW, SH);
          var pts = collect(s, 4, function (r, g, b, a, x, y) {
            var nx = x / SW, ny = y / SH;
            // subject silhouette: head ellipse (hair, face, ears) …
            var ex = (nx - 0.5) / 0.45, ey = (ny - 0.42) / 0.45;
            var inHead = ex * ex + ey * ey <= 1;
            // … union a neck-and-shoulders trapezoid below the chin
            var inShoulders = ny > 0.78 && Math.abs(nx - 0.5) < 0.30 + (ny - 0.78) * 1.05;
            return inHead || inShoulders;
          });
          // clarity lift: gentle contrast + saturation, shadows raised a touch
          for (var i = 0; i < pts.length; i++) {
            var p = pts[i];
            var lum = 0.2126 * p.r + 0.7152 * p.g + 0.0722 * p.b;
            p.r = Math.max(0, Math.min(255, lum + (p.r - lum) * 1.22));
            p.g = Math.max(0, Math.min(255, lum + (p.g - lum) * 1.22));
            p.b = Math.max(0, Math.min(255, lum + (p.b - lum) * 1.22));
            p.r = Math.max(0, Math.min(255, ((p.r / 255 - 0.5) * 1.14 + 0.53) * 255));
            p.g = Math.max(0, Math.min(255, ((p.g / 255 - 0.5) * 1.14 + 0.53) * 255));
            p.b = Math.max(0, Math.min(255, ((p.b / 255 - 0.5) * 1.14 + 0.53) * 255));
          }
          return fit(pts, SW, SH, PANEL);
        }

        /* text: rendered bold, sampled, painted in the reel's violet/pink/cyan palette */
        function sampleText(text, fontPx, rect, sub) {
          var SW = 880, SH = 300;
          var s = makeSampler(SW, SH);
          s.x.clearRect(0, 0, SW, SH);
          s.x.fillStyle = "#fff";
          s.x.textAlign = "center"; s.x.textBaseline = "middle";
          s.x.font = "800 " + fontPx + "px 'JetBrains Mono', monospace";
          s.x.fillText(text, SW / 2, SH / 2 - (sub ? 22 : 0));
          if (sub) {
            s.x.font = "500 " + Math.round(fontPx * 0.30) + "px 'JetBrains Mono', monospace";
            s.x.fillText(sub, SW / 2, SH / 2 + fontPx * 0.62);
          }
          var pts = collect(s, 4, function (r, g, b, a) { return a > 120; });
          return pts.map(function (p, idx) {
            var t = p.sx / SW;
            var hex = PALETTE[Math.floor(t * PALETTE.length) % PALETTE.length];
            var n = parseInt(hex.slice(1), 16);
            return {
              x: rect.x + (p.sx / SW) * rect.w,
              y: rect.y + (p.sy / SH) * rect.h,
              r: (n >> 16) & 255, g: (n >> 8) & 255, b: n & 255
            };
          });
        }

        /* ring: a glowing orbit ring + core, the reel's morph-away shape */
        function sampleRing() {
          var pts = [];
          var cx = CENTER.x, cy = CENTER.y, R = 218;
          var n = 620;
          for (var i = 0; i < n; i++) {
            var a = (i / n) * Math.PI * 2;
            var rr = R + (Math.random() - 0.5) * 7;
            var hex = PALETTE[i % PALETTE.length];
            var v = parseInt(hex.slice(1), 16);
            pts.push({ x: cx + Math.cos(a) * rr, y: cy + Math.sin(a) * rr, r: (v >> 16) & 255, g: (v >> 8) & 255, b: v & 255 });
          }
          for (var j = 0; j < 260; j++) { // inner dashed ring
            var a2 = Math.random() * Math.PI * 2, rr2 = 150 + (Math.random() - 0.5) * 5;
            pts.push({ x: cx + Math.cos(a2) * rr2, y: cy + Math.sin(a2) * rr2, r: 139, g: 92, b: 246 });
          }
          return pts;
        }

        /* ---------- particle pool ---------- */
        var shapes = {};      // name -> target list
        var order = ["portrait", "name", "code", "ring", "aiml"];
        var particles = [];
        var MAXP = 6800;
        var current = "portrait";
        var started = false;
        var portraitImg = null;   // kept for the faint clarity underlay
        var underlay = 0;         // 0..1, eases toward 1 while portrait shows

        function buildParticles() {
          var counts = order.map(function (k) { return shapes[k] ? shapes[k].length : 0; });
          var n = Math.min(MAXP, Math.max.apply(null, counts));
          // phones keep nearly the full pool — thinning it is what made the
          // face unreadable on small screens
          if (window.innerWidth < 620) n = Math.min(n, 6000);
          particles = [];
          for (var i = 0; i < n; i++) {
            particles.push({
              x: Math.random() * CW, y: Math.random() * CH,
              vx: 0, vy: 0,
              tx: CENTER.x, ty: CENTER.y,
              r: 200, g: 200, b: 255, tr: 200, tg: 200, tb: 255,
              // dots sized to overlap the portrait grid spacing (~6px), so
              // the face renders as a continuous image, not scattered specks
              size: 2.4 + Math.random() * 1.0,
              delay: Math.random() * 55,
              seed: Math.random() * Math.PI * 2
            });
          }
        }

        function setShape(name, scatter) {
          current = name;
          var targets = shapes[name] || [];
          var i, p, t;
          // shuffle assignment so the morph swirls instead of sliding in rows
          var idx = targets.map(function (_, k) { return k; });
          for (i = idx.length - 1; i > 0; i--) { var j = Math.floor(Math.random() * (i + 1)); var tmp = idx[i]; idx[i] = idx[j]; idx[j] = tmp; }
          for (i = 0; i < particles.length; i++) {
            p = particles[i];
            if (i < targets.length) {
              t = targets[idx[i]];
              p.tx = t.x; p.ty = t.y; p.tr = t.r; p.tg = t.g; p.tb = t.b; p.dead = false;
            } else {
              // spare particles drift off into a faint halo ring
              var a = Math.random() * Math.PI * 2, rr = 300 + Math.random() * 190;
              p.tx = CENTER.x + Math.cos(a) * rr; p.ty = CENTER.y + Math.sin(a) * rr * 0.72;
              p.tr = 99; p.tg = 80; p.tb = 180; p.dead = true;
            }
            if (scatter) {
              p.x = Math.random() * CW; p.y = Math.random() * CH;
              p.vx = 0; p.vy = 0; p.delay = Math.random() * 55;
            }
          }
          var btns = document.querySelectorAll(".shape-btn[data-shape]");
          btns.forEach(function (b) { b.setAttribute("aria-pressed", b.getAttribute("data-shape") === name ? "true" : "false"); });
        }

        /* ---------- ambient sparks (the reel's starfield) ---------- */
        var sparks = [];
        for (var si = 0; si < 70; si++) {
          sparks.push({
            x: Math.random() * CW, y: Math.random() * CH,
            r: Math.random() * 1.4 + 0.3,
            s: 0.12 + Math.random() * 0.4,
            ph: Math.random() * Math.PI * 2,
            col: PALETTE[si % PALETTE.length]
          });
        }

        /* ---------- pointer interaction ---------- */
        var mouse = { x: -9999, y: -9999, active: false };
        function toStage(e) {
          var rect = canvas.getBoundingClientRect();
          var cx = (e.touches ? e.touches[0].clientX : e.clientX);
          var cy = (e.touches ? e.touches[0].clientY : e.clientY);
          mouse.x = (cx - rect.left) / rect.width * CW;
          mouse.y = (cy - rect.top) / rect.height * CH;
          mouse.active = true;
        }
        canvas.addEventListener("pointermove", toStage);
        canvas.addEventListener("pointerdown", function (e) {
          toStage(e);
          // tap burst: push nearby particles outward
          for (var i = 0; i < particles.length; i++) {
            var p = particles[i], dx = p.x - mouse.x, dy = p.y - mouse.y;
            var d2 = dx * dx + dy * dy;
            if (d2 < 210 * 210) {
              var d = Math.sqrt(d2) || 1, f = (1 - d / 210) * 15;
              p.vx += (dx / d) * f; p.vy += (dy / d) * f;
            }
          }
        });
        canvas.addEventListener("pointerleave", function () { mouse.active = false; mouse.x = -9999; });

        /* ---------- render loop ---------- */
        var frame = 0, raf = null, running = false;
        // faint real-photo underlay beneath the dots while the portrait is
        // showing — grounds the facial features so the portrait reads as a
        // real photo made of particles, and fades away for the other shapes
        function drawUnderlay(alpha) {
          if (!portraitImg || alpha <= 0.01) return;
          ctx.save();
          ctx.globalAlpha = alpha * 0.22;
          ctx.drawImage(portraitImg, CROP.x, CROP.y, CROP.w, CROP.h, PANEL.x, PANEL.y, PANEL.w, PANEL.h);
          ctx.restore();
        }
        function drawStatic() {
          ctx.clearRect(0, 0, CW, CH);
          drawUnderlay(current === "portrait" ? 1 : 0);
          for (var i = 0; i < particles.length; i++) {
            var p = particles[i];
            ctx.fillStyle = "rgba(" + p.tr + "," + p.tg + "," + p.tb + "," + (p.dead ? 0.08 : 1) + ")";
            ctx.beginPath();
            ctx.arc(p.tx, p.ty, p.size, 0, Math.PI * 2);
            ctx.fill();
          }
        }
        function loop() {
          frame++;
          ctx.clearRect(0, 0, CW, CH);
          underlay += (((current === "portrait") ? 1 : 0) - underlay) * 0.04;
          drawUnderlay(underlay);
          // sparks
          for (var s = 0; s < sparks.length; s++) {
            var sp = sparks[s];
            sp.y -= sp.s; if (sp.y < -4) { sp.y = CH + 4; sp.x = Math.random() * CW; }
            var tw = 0.25 + 0.55 * Math.abs(Math.sin(frame * 0.02 + sp.ph));
            ctx.globalAlpha = tw * 0.6;
            ctx.fillStyle = sp.col;
            ctx.beginPath(); ctx.arc(sp.x, sp.y, sp.r, 0, Math.PI * 2); ctx.fill();
          }
          ctx.globalAlpha = 1;
          // particles
          for (var i = 0; i < particles.length; i++) {
            var p = particles[i];
            if (frame > p.delay) {
              var ax = (p.tx - p.x) * 0.028, ay = (p.ty - p.y) * 0.028;
              p.vx = (p.vx + ax) * 0.86;
              p.vy = (p.vy + ay) * 0.86;
              if (mouse.active) {
                var dx = p.x - mouse.x, dy = p.y - mouse.y;
                var d2 = dx * dx + dy * dy;
                if (d2 < 110 * 110 && d2 > 0.01) {
                  var d = Math.sqrt(d2), f = (1 - d / 110) * 2.6;
                  p.vx += (dx / d) * f; p.vy += (dy / d) * f;
                }
              }
              // idle breathing
              p.vx += Math.cos(frame * 0.02 + p.seed) * 0.012;
              p.vy += Math.sin(frame * 0.017 + p.seed) * 0.012;
              p.x += p.vx; p.y += p.vy;
            }
            p.r += (p.tr - p.r) * 0.06; p.g += (p.tg - p.g) * 0.06; p.b += (p.tb - p.b) * 0.06;
            ctx.fillStyle = "rgba(" + (p.r | 0) + "," + (p.g | 0) + "," + (p.b | 0) + "," + (p.dead ? 0.07 : 1) + ")";
            ctx.beginPath();
            ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2);
            ctx.fill();
          }
          raf = requestAnimationFrame(loop);
        }
        function startLoop() { if (!running && !reduceMotion) { running = true; raf = requestAnimationFrame(loop); } }
        function stopLoop() { running = false; if (raf) cancelAnimationFrame(raf); }

        /* ---------- shape cycling (like the reel: portrait → name → symbols) ---------- */
        var cycleTimer = null, userHoldUntil = 0;
        function cycle() {
          if (Date.now() < userHoldUntil) return;
          var next = order[(order.indexOf(current) + 1) % order.length];
          setShape(next, false);
        }
        function startCycle() {
          if (reduceMotion) return;
          stopCycle();
          cycleTimer = setInterval(cycle, 6000);
        }
        function stopCycle() { if (cycleTimer) clearInterval(cycleTimer); cycleTimer = null; }

        /* ---------- controls ---------- */
        document.querySelectorAll(".shape-btn[data-shape]").forEach(function (b) {
          b.addEventListener("click", function () {
            userHoldUntil = Date.now() + 16000;
            setShape(b.getAttribute("data-shape"), false);
            if (reduceMotion) drawStatic();
          });
        });
        document.getElementById("replayBtn").addEventListener("click", function () {
          userHoldUntil = Date.now() + 16000;
          setShape(current, true);
          if (reduceMotion) drawStatic(); else startLoop();
        });

        /* pause when off-screen or tab hidden — saves battery on the phone */
        if ("IntersectionObserver" in window && !reduceMotion) {
          new IntersectionObserver(function (entries) {
            entries.forEach(function (en) {
              if (en.isIntersecting) { startLoop(); startCycle(); }
              else { stopLoop(); stopCycle(); }
            });
          }, { threshold: 0.08 }).observe(canvas);
        }
        document.addEventListener("visibilitychange", function () {
          if (document.hidden) { stopLoop(); stopCycle(); }
          else if (started) { startLoop(); startCycle(); }
        });

        /* ---------- boot: load the real photo, sample it, build the show ---------- */
        var textRect = { x: 40, y: 190, w: 800, h: 260 };
        function buildShapes(img) {
          portraitImg = img;
          shapes.portrait = samplePortrait(img);
          shapes.name = sampleText("SIDDARTHA", 118, textRect, "JAMANDLA");
          shapes.code = sampleText("</>", 190, { x: 190, y: 170, w: 500, h: 300 });
          shapes.aiml = sampleText("AI · ML", 150, textRect, "PYTHON · AGENTS · WEB");
          shapes.ring = sampleRing();
          buildParticles();
          // hold the portrait first — it is the point of the panel — before
          // the auto-cycle starts morphing it into the other shapes
          userHoldUntil = Date.now() + 11000;
          setShape("portrait", true);
          started = true;
          if (reduceMotion) { drawStatic(); }
          else { startLoop(); startCycle(); }
        }
        var img = new Image();
        img.onload = function () {
          if (document.fonts && document.fonts.ready) {
            document.fonts.ready.then(function () { buildShapes(img); });
          } else buildShapes(img);
        };
        img.onerror = function () {
          // honest fallback: show the photo itself inside the panel
          canvas.style.display = "none";
          document.getElementById("vmapFallback").style.display = "block";
        };
        img.src = "data:image/jpeg;base64,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";
      })();
    </script>
  </body>
</html>
