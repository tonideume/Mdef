<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SONOLICHEN — Barrera Acústica Viva</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,300;9..144,500;9..144,600;9..144,700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0a120f;
    --bg-alt:#0e1913;
    --surface:#122019;
    --surface-2:#182c24;
    --line: rgba(140,214,190,0.16);
    --line-strong: rgba(140,214,190,0.32);
    --text:#e9f2ec;
    --text-dim:#93ac9f;
    --text-faint:#5f776b;
    --accent:#7fe0c4;
    --accent-soft: rgba(127,224,196,0.12);
    --rust:#c98f4e;
    --rust-soft: rgba(201,143,78,0.14);
    --moss:#6b8f7d;
    --radius: 3px;
  }
{ box-sizing:border-box; margin:0; padding:0; }
html{ scroll-behavior:smooth; }
body{
    background:
      radial-gradient(ellipse 900px 500px at 12% -5%, rgba(127,224,196,0.07), transparent 60%),
      radial-gradient(ellipse 700px 500px at 90% 10%, rgba(201,143,78,0.05), transparent 60%),
      var(--bg);
    color:var(--text);
    font-family:'Inter', sans-serif;
    line-height:1.6;
    overflow-x:hidden;
  }
/* organic pore texture overlay */
  body::before{
    content:"";
    position:fixed; inset:0;
    background-image: radial-gradient(circle at 20% 30%, rgba(127,224,196,0.035) 0, transparent 2px),
                       radial-gradient(circle at 70% 65%, rgba(127,224,196,0.03) 0, transparent 2px),
                       radial-gradient(circle at 45% 80%, rgba(201,143,78,0.025) 0, transparent 2px);
    background-size: 140px 140px, 190px 190px, 220px 220px;
    pointer-events:none;
    z-index:0;
  }
 .wrap{ max-width:1180px; margin:0 auto; padding:0 32px; position:relative; z-index:1; }
.eyebrow{
    font-family:'JetBrains Mono', monospace;
    font-size:11.5px;
    letter-spacing:0.16em;
    text-transform:uppercase;
    color:var(--text-faint);
  }
 h1,h2,h3{ font-family:'Fraunces', serif; font-weight:600; letter-spacing:-0.01em; }
a{ color:inherit; }
 /* ============ HEADER ============ */
  header.top{
    padding:26px 0 0;
    display:flex; justify-content:space-between; align-items:center;
    border-bottom:1px solid var(--line);
    padding-bottom:18px;
  }
  header.top .eyebrow{ opacity:0.85; }
/* ============ HERO ============ */
  .hero{
    padding:90px 0 60px;
    display:grid;
    grid-template-columns: 1.15fr 0.85fr;
    gap:56px;
    align-items:center;
    border-bottom:1px solid var(--line);
  }
  .hero h1{
    font-size:clamp(58px, 8vw, 108px);
    line-height:0.92;
    color:var(--text);
  }
  .hero h1 em{
    font-style:italic;
    color:var(--accent);
    font-weight:500;
  }
  .hero .tagline{
    margin-top:22px;
    font-size:18px;
    color:var(--text-dim);
    max-width:480px;
    font-weight:400;
  }
.hypothesis{
    margin-top:34px;
    border-left:2px solid var(--accent);
    padding:6px 0 6px 22px;
    max-width:560px;
  }
  .hypothesis .eyebrow{ color:var(--accent); margin-bottom:8px; display:block; }
  .hypothesis p{ font-size:15.5px; color:var(--text-dim); font-family:'Inter',sans-serif; }
  .hypothesis strong{ color:var(--text); font-weight:600; }
.hero-visual{ position:relative; }
  .hero-visual svg{ width:100%; height:auto; display:block; }
  .hero-caption{
    font-family:'JetBrains Mono', monospace;
    font-size:10.5px;
    letter-spacing:0.1em;
    text-transform:uppercase;
    color:var(--text-faint);
    text-align:center;
    margin-top:14px;
  }
/* ============ METRICS ============ */
  .metrics{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    border-bottom:1px solid var(--line);
  }
  .metric{
    padding:38px 30px;
    border-right:1px solid var(--line);
  }
  .metric:last-child{ border-right:none; }
  .metric .num{
    font-family:'Fraunces', serif;
    font-size:44px;
    font-weight:600;
    color:var(--accent);
    line-height:1;
  }
  .metric .label{
    font-family:'JetBrains Mono', monospace;
    font-size:10.5px;
    letter-spacing:0.12em;
    text-transform:uppercase;
    color:var(--text-faint);
    margin:10px 0 6px;
  }
  .metric .desc{ font-size:13.5px; color:var(--text-dim); }
/* ============ SECTION GENERIC ============ */
  section{ padding:80px 0; border-bottom:1px solid var(--line); }
  section:last-of-type{ border-bottom:none; }
.section-head{ margin-bottom:44px; max-width:640px; }
  .section-head h2{ font-size:34px; color:var(--text); margin-top:10px; }
  .section-head .sub{ margin-top:12px; color:var(--text-dim); font-size:15px; }
 /* ============ MECHANISM ============ */
  .mechanism-list{ display:flex; flex-direction:column; gap:0; max-width:760px; }
  .mech-step{
    display:grid;
    grid-template-columns:56px 1fr;
    gap:22px;
    padding:26px 0;
    border-top:1px solid var(--line);
  }
  .mech-step:last-child{ border-bottom:1px solid var(--line); }
  .mech-num{
    font-family:'Fraunces', serif;
    font-size:26px;
    color:var(--accent);
    opacity:0.7;
  }
  .mech-step h3{ font-size:18px; font-weight:600; color:var(--text); margin-bottom:6px; }
  .mech-step p{ color:var(--text-dim); font-size:14.5px; }
/* ============ VISUAL PROJECTION ============ */
  .projection{
    background:var(--surface);
    border:1px solid var(--line);
    border-radius:var(--radius);
    padding:8px;
    margin-top:10px;
  }
  .projection svg{ width:100%; height:auto; display:block; border-radius:2px; }
  .projection-caption{
    font-family:'JetBrains Mono', monospace;
    font-size:10.5px;
    letter-spacing:0.08em;
    text-transform:uppercase;
    color:var(--text-faint);
    padding:14px 10px 6px;
  }
/* ============ GENETIC CONSTRUCT ============ */
  .construct-row{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin-top:28px;
  }
  .gene-box{
    flex:1 1 140px;
    background:var(--surface);
    border:1px solid var(--line-strong);
    border-radius:var(--radius);
    padding:16px 14px;
    position:relative;
  }
  .gene-box.term{ background:var(--rust-soft); border-color:rgba(201,143,78,0.4); }
  .gene-box .tag{
    font-family:'JetBrains Mono', monospace;
    font-size:13px;
    font-weight:600;
    color:var(--accent);
    letter-spacing:0.04em;
  }
  .gene-box.term .tag{ color:var(--rust); }
  .gene-box .desc{ font-size:12px; color:var(--text-dim); margin-top:6px; line-height:1.4; }
  .construct-arrow{
    display:flex; align-items:center; color:var(--text-faint); font-size:16px; padding:0 2px;
  }
/* ============ PIPELINE TIMELINE ============ */
  .pipeline{
    display:grid;
    grid-template-columns:repeat(7,1fr);
    gap:2px;
    margin-top:10px;
  }
  .pipe-step{
    background:var(--surface);
    padding:20px 14px;
    text-align:left;
    border-top:2px solid var(--accent);
  }
  .pipe-step:nth-child(7){ border-top-color:var(--rust); }
  .pipe-step .wk{
    font-family:'JetBrains Mono', monospace;
    font-size:10px;
    color:var(--text-faint);
    letter-spacing:0.06em;
  }
  .pipe-step .title{ font-size:12.5px; color:var(--text); margin-top:8px; font-weight:500; line-height:1.4; }
/* ============ DETAIL CARDS ============ */
  .card-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:2px;
    margin-top:10px;
  }
  .card{
    background:var(--surface);
    padding:32px;
  }
  .card h3{
    font-family:'JetBrains Mono', monospace;
    font-size:11.5px;
    letter-spacing:0.1em;
    text-transform:uppercase;
    color:var(--accent);
    margin-bottom:14px;
    font-weight:600;
  }
  .card p{ font-size:14.5px; color:var(--text-dim); }
  .card p + p{ margin-top:10px; }
  .card strong{ color:var(--text); font-weight:600; }
/* ============ OUTCOMES ============ */
  .outcomes-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:40px;
    margin-top:10px;
  }
  .outcome-block{ padding-left:20px; border-left:1px solid var(--line); }
  .outcome-item{ margin-bottom:22px; }
  .outcome-item .mark{
    font-family:'JetBrains Mono', monospace;
    font-size:11px;
    letter-spacing:0.08em;
    text-transform:uppercase;
    margin-bottom:6px;
    display:inline-block;
  }
  .mark.good{ color:var(--accent); }
  .mark.warn{ color:var(--rust); }
  .outcome-item p{ font-size:14.5px; color:var(--text-dim); }
  .outcome-item strong{ color:var(--text); }
/* ============ IMPACT ============ */
  .impact-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:2px;
    margin-top:10px;
  }
  .impact-card{ background:var(--surface); padding:28px 24px; }
  .impact-card h4{
    font-family:'JetBrains Mono', monospace;
    font-size:11px;
    letter-spacing:0.12em;
    text-transform:uppercase;
    color:var(--rust);
    margin-bottom:12px;
  }
  .impact-card p{ font-size:13.5px; color:var(--text-dim); }
/* ============ CLOSING ============ */
  .closing{
    padding:100px 0 90px;
    text-align:center;
  }
  .closing .eyebrow{ color:var(--accent); }
  .closing h2{
    font-size:clamp(28px, 4vw, 44px);
    max-width:840px;
    margin:20px auto 0;
    font-style:italic;
    font-weight:500;
    line-height:1.35;
    color:var(--text);
  }
  .closing h2 .q{ color:var(--accent); font-style:normal; }
footer{
    padding:30px 0 50px;
    display:flex; justify-content:space-between;
    font-family:'JetBrains Mono', monospace;
    font-size:11px;
    color:var(--text-faint);
    letter-spacing:0.05em;
  }
@media (max-width: 900px){
    .hero{ grid-template-columns:1fr; padding-top:56px; }
    .metrics{ grid-template-columns:1fr 1fr; }
    .metric:nth-child(2){ border-right:none; }
    .metric{ border-bottom:1px solid var(--line); }
    .pipeline{ grid-template-columns:repeat(2,1fr); }
    .card-grid{ grid-template-columns:1fr; }
    .outcomes-grid{ grid-template-columns:1fr; }
    .impact-grid{ grid-template-columns:1fr 1fr; }
    .construct-row{ flex-direction:column; }
    .construct-arrow{ display:none; }
  }
@media (prefers-reduced-motion: reduce){
    * { animation:none !important; transition:none !important; }
  }
.wave-anim { animation: wavepulse 5s ease-in-out infinite; }
  @keyframes wavepulse{
    0%,100%{ opacity:0.9; }
    50%{ opacity:0.55; }
  }
  .spore{ animation: drift 8s ease-in-out infinite; }
  @keyframes drift{
    0%,100%{ transform:translateY(0); }
    50%{ transform:translateY(-6px); }
  }
</style>
</head>
<body>

<div class="wrap">

  <header class="top">
    <span class="eyebrow">MDEF · OTHER SPECIES II</span>
    <span class="eyebrow">SPECULATIVE BIODESIGN</span>
  </header>

  <!-- HERO -->
  <section class="hero" style="border-bottom:1px solid var(--line); padding-top:90px;">
    <div>
      <h1>SONO<em>LICHEN</em></h1>
      <p class="tagline">Una barrera acústica viva para entornos urbanos silenciosos. Un liquen sintético que crece sobre muros, fachadas y barreras de autopista, y absorbe el ruido del tráfico mientras respira el aire contaminado.</p>

<div class="hypothesis">
        <span class="eyebrow">Hypothesis</span>
        <p>If a synthetic lichen composed of genetically modified fungal and moss symbionts is designed to produce porous cellular structures and resonance-dampening formations capable of absorbing urban traffic frequencies (200–4000 Hz), while simultaneously capturing airborne particulate matter (PM2.5 and PM10), then urban surfaces colonized by Sonolichen could reduce perceived environmental noise by 20–40% and improve local air quality, without the need for conventional acoustic infrastructure.</p>
      </div>
    </div>
<div class="hero-visual">
      <svg viewBox="0 0 480 420" xmlns="http://www.w3.org/2000/svg">
        <defs>
          <radialGradient id="lichenGlow" cx="50%" cy="50%" r="60%">
            <stop offset="0%" stop-color="#7fe0c4" stop-opacity="0.28"/>
            <stop offset="100%" stop-color="#7fe0c4" stop-opacity="0"/>
          </radialGradient>
        </defs>
        <rect x="0" y="0" width="480" height="420" fill="#0e1913" rx="3"/>
        <circle cx="330" cy="150" r="150" fill="url(#lichenGlow)"/>
<!-- sound waves entering from left, decaying -->
        <g stroke="#c98f4e" stroke-width="2" fill="none" opacity="0.75" class="wave-anim">
          <path d="M20,180 Q50,140 80,180 T140,180"/>
          <path d="M20,210 Q50,150 80,210 T140,210" opacity="0.7"/>
          <path d="M20,240 Q50,200 80,240 T140,240" opacity="0.55"/>
        </g>
        <!-- decaying waves mid zone -->
        <g stroke="#c98f4e" stroke-width="1.6" fill="none" opacity="0.4">
          <path d="M150,190 Q168,175 186,190 T222,190"/>
          <path d="M150,215 Q168,203 186,215 T222,215" opacity="0.3"/>
        </g>
        <!-- flat line = silence -->
        <line x1="240" y1="205" x2="460" y2="205" stroke="#7fe0c4" stroke-width="1.5" opacity="0.5" stroke-dasharray="2 5"/>
<!-- lichen mass, organic blobs -->
        <g>
          <ellipse cx="300" cy="150" rx="70" ry="60" fill="#183a30" stroke="#7fe0c4" stroke-width="1" opacity="0.9"/>
          <ellipse cx="350" cy="120" rx="55" ry="48" fill="#1c4438" stroke="#7fe0c4" stroke-width="1" opacity="0.9"/>
          <ellipse cx="270" cy="110" rx="46" ry="40" fill="#204c3f" stroke="#7fe0c4" stroke-width="1" opacity="0.9"/>
          <ellipse cx="330" cy="185" rx="60" ry="45" fill="#173427" stroke="#7fe0c4" stroke-width="1" opacity="0.9"/>
          <ellipse cx="380" cy="165" rx="42" ry="36" fill="#1b3e32" stroke="#7fe0c4" stroke-width="1" opacity="0.9"/>
<!-- pores / spores -->
          <g fill="#7fe0c4">
            <circle class="spore" cx="290" cy="140" r="3" opacity="0.8"/>
            <circle class="spore" cx="320" cy="115" r="2.4" opacity="0.7"/>
            <circle class="spore" cx="355" cy="150" r="2.8" opacity="0.75"/>
            <circle class="spore" cx="300" cy="185" r="2.2" opacity="0.6"/>
            <circle class="spore" cx="365" cy="120" r="2" opacity="0.65"/>
            <circle class="spore" cx="250" cy="115" r="2.2" opacity="0.6"/>
          </g>
          <!-- rust apothecia dots (real lichen fruiting bodies) -->
          <g fill="#c98f4e">
            <circle cx="310" cy="160" r="4" opacity="0.85"/>
            <circle cx="345" cy="135" r="3.2" opacity="0.75"/>
            <circle cx="280" cy="130" r="3" opacity="0.7"/>
          </g>
        </g>
<!-- concrete wall base -->
        <rect x="0" y="360" width="480" height="60" fill="#0a1512"/>
        <g stroke="#1c2e27" stroke-width="1">
          <line x1="0" y1="380" x2="480" y2="380"/>
          <line x1="120" y1="360" x2="120" y2="420"/>
          <line x1="240" y1="360" x2="240" y2="420"/>
          <line x1="360" y1="360" x2="360" y2="420"/>
        </g>
        <rect x="250" y="230" width="120" height="130" fill="#122019" opacity="0.4"/>
      </svg>
      <div class="hero-caption">SONOLICHEN · ACOUSTIC WALL · NOISE → SILENCE</div>
    </div>
  </section>
  
![](images/IMG_2899.jpeg)
![](images/IMG_2899.jpeg)

  <!-- METRICS -->
  <div class="metrics">
    <div class="metric">
      <div class="num">3</div>
      <div class="label">Designed Traits</div>
      <div class="desc">Acoustic absorption, contaminant capture, self-regeneration</div>
    </div>
    <div class="metric">
      <div class="num">200–4000<span style="font-size:20px;">Hz</span></div>
      <div class="label">Target Frequency Range</div>
      <div class="desc">Typical traffic, engines, braking, and urban noise</div>
    </div>
    <div class="metric">
      <div class="num">~35%</div>
      <div class="label">Projected Noise Reduction</div>
      <div class="desc">In enclosed urban environments</div>
    </div>
    <div class="metric">
      <div class="num">0<span style="font-size:20px;">kWh</span></div>
      <div class="label">External Energy Required</div>
      <div class="desc">Complete self-sufficiency via photosynthesis</div>
    </div>
  </div>

  <!-- MECHANISM -->
  <section>
    <div class="section-head">
      <span class="eyebrow">BIOLOGICAL MECHANISM</span>
      <h2>How the Lichen Absorbs Sound</h2>
      <p class="sub">Five chained processes transform the cellular structure of the lichen into a living acoustic trap, capable of metabolizing the pollution it captures.</p>
    </div>
    <div class="mechanism-list">
      <div class="mech-step">
        <div class="mech-num">01</div>
        <div><h3>Formation of Porous Acoustic Tissue</h3><p>Modified fungal hyphae generate interconnected micro-cavities that act as biological sound traps.</p></div>
      </div>
      <div class="mech-step">
        <div class="mech-num">02</div>
        <div><h3>Resonance Absorption Layer</h3><p>Specialized cellular chambers absorb and dissipate the vibration energy of traffic-associated frequencies.</p></div>
      </div>
      <div class="mech-step">
        <div class="mech-num">03</div>
        <div><h3>Particulate Matter Capture</h3><p>Mucilaginous secretions on the surface trap suspended particles PM2.5 and PM10.</p></div>
      </div>
      <div class="mech-step">
        <div class="mech-num">04</div>
        <div><h3>Biofiltration Metabolism</h3><p>Associated bacteria metabolize the captured pollutants and convert them into harmless compounds.</p></div>
      </div>
      <div class="mech-step">
        <div class="mech-num">05</div>
        <div><h3>Continuous Autorregeneration</h3><p> Damaged tissue is naturally replaced through vegetative growth, eliminating the need for maintenance.</p></div>
      </div>
    </div>
  </section>

  <!-- GENETIC CONSTRUCT -->
  <section>
    <div class="section-head">
      <span class="eyebrow">GENETIC DESIGN</span>
      <h2>Genetic Construct</h2>
      <p class="sub">Six genetically engineered components arranged within a single expression cassette, inserted via Agrobacterium-mediated transformation.</p>
    </div>
    <div class="construct-row">
      <div class="gene-box"><div class="tag">ACO-1</div><div class="desc">Acoustic cavity development regulator</div></div>
      <div class="construct-arrow">→</div>
      <div class="gene-box"><div class="tag">POR-2</div><div class="desc">Enhanced porous acoustic tissue formation</div></div>
      <div class="construct-arrow">→</div>
      <div class="gene-box"><div class="tag">PMT-3</div><div class="desc">Secretion pathway for particle capture</div></div>
      <div class="construct-arrow">→</div>
      <div class="gene-box"><div class="tag">BIO-4</div><div class="desc">Symbiotic degradation of pollutants</div></div>
      <div class="construct-arrow">→</div>
      <div class="gene-box"><div class="tag">REG-5</div><div class="desc">Autoregulation and accelerated growth regulator</div></div>
      <div class="construct-arrow">→</div>
      <div class="gene-box term"><div class="tag">TERM</div><div class="desc">Environmental containment sequence</div></div>
    </div>
  </section>

  <!-- VISUAL PROJECTION -->
  <section>
    <div class="section-head">
      <span class="eyebrow">VISUAL PROJECTION</span>
      <h2>City as a Landscape of Silence</h2>
      <p class="sub">Urban walls, highway barriers and facades are covered with green-blue acoustic biofilms. Near the busiest roads, the organism develops denser growth patterns, creating "zones of silence" that are alive.</p>
    </div>
    <div class="projection">
      <svg viewBox="0 0 1080 460" xmlns="http://www.w3.org/2000/svg">
        <rect width="1080" height="460" fill="#0e1913"/>
        <!-- sky gradient -->
        <defs>
          <linearGradient id="sky" x1="0" y1="0" x2="0" y2="1">
            <stop offset="0%" stop-color="#0a1512"/>
            <stop offset="100%" stop-color="#122019"/>
          </linearGradient>
        </defs>
        <rect width="1080" height="300" fill="url(#sky)"/>
<!-- road -->
        <rect x="0" y="360" width="1080" height="100" fill="#0a1210"/>
        <g stroke="#2a3f36" stroke-width="3" stroke-dasharray="26 20">
          <line x1="0" y1="410" x2="1080" y2="410"/>
        </g>
<!-- acoustic barrier wall with lichen -->
        <rect x="60" y="230" width="960" height="130" fill="#152c24" stroke="#1c3a30" stroke-width="2"/>
        <g fill="#1a3a2f">
          <rect x="60" y="230" width="960" height="130"/>
        </g>
        <!-- lichen patches denser near center (busiest zone) -->
        <g opacity="0.95">
          <ellipse cx="180" cy="270" rx="34" ry="24" fill="#1e4a3c"/>
          <ellipse cx="230" cy="290" rx="26" ry="18" fill="#225644"/>
          <ellipse cx="420" cy="260" rx="46" ry="30" fill="#1e4a3c"/>
          <ellipse cx="480" cy="290" rx="52" ry="34" fill="#256050"/>
          <ellipse cx="540" cy="255" rx="44" ry="28" fill="#1e4a3c"/>
          <ellipse cx="600" cy="295" rx="50" ry="32" fill="#256050"/>
          <ellipse cx="660" cy="260" rx="40" ry="26" fill="#1e4a3c"/>
          <ellipse cx="800" cy="280" rx="30" ry="20" fill="#1e4a3c"/>
          <ellipse cx="880" cy="265" rx="24" ry="16" fill="#225644"/>
        </g>
        <!-- rust apothecia flecks -->
        <g fill="#c98f4e" opacity="0.8">
          <circle cx="440" cy="270" r="2.5"/>
          <circle cx="500" cy="285" r="2"/>
          <circle cx="560" cy="250" r="2.2"/>
          <circle cx="610" cy="300" r="2"/>
          <circle cx="230" cy="285" r="1.8"/>
        </g>
<!-- silence zone concentric rings above the densest section -->
        <g stroke="#7fe0c4" fill="none" opacity="0.35">
          <circle cx="520" cy="180" r="60"/>
          <circle cx="520" cy="180" r="100"/>
          <circle cx="520" cy="180" r="140"/>
        </g>
        <text x="520" y="180" text-anchor="middle" fill="#7fe0c4" font-family="JetBrains Mono, monospace" font-size="11" opacity="0.85">SILENCE ZONE</text>
<!-- icons row above barrier: park, school, hospital, residential, pedestrian -->
        <g font-family="JetBrains Mono, monospace" font-size="10.5" fill="#93ac9f">
          <text x="140" y="140" text-anchor="middle">PARK</text>
          <text x="330" y="120" text-anchor="middle">SCHOOL</text>
          <text x="520" y="100" text-anchor="middle" fill="#7fe0c4">HOSPITAL</text>
          <text x="710" y="120" text-anchor="middle">RESIDENTIAL</text>
          <text x="900" y="140" text-anchor="middle">PEDESTRIAN STREET</text>
        </g>
        <g stroke="#3a5a4d" stroke-width="1" stroke-dasharray="2 4" opacity="0.6">
          <line x1="140" y1="150" x2="180" y2="230"/>
          <line x1="330" y1="130" x2="420" y2="230"/>
          <line x1="520" y1="110" x2="520" y2="230"/>
          <line x1="710" y1="130" x2="660" y2="230"/>
          <line x1="900" y1="150" x2="880" y2="230"/>
        </g>
<!-- cars passing -->
        <g fill="#22352d">
          <rect x="120" y="392" width="46" height="16" rx="3"/>
          <rect x="380" y="392" width="46" height="16" rx="3"/>
          <rect x="700" y="392" width="46" height="16" rx="3"/>
          <rect x="920" y="392" width="46" height="16" rx="3"/>
        </g>
      </svg>
      <div class="projection-caption">SONOLICHEN · HIGHWAY BARRIER · DIFFERENTIAL GROWTH ACCORDING TO TRAFFIC INTENSITY</div>
    </div>
  </section>

![](images/IMG_2899.jpeg)
![](images/IMG_2899.jpeg)

  <!-- TESTING PIPELINE -->
  <section>
    <div class="section-head">
      <span class="eyebrow">EXPERIMENTAL PIPELINE</span>
      <h2>From Genetic Synthesis to Urban Deployment</h2>
    </div>
    <div class="pipeline">
      <div class="pipe-step"><div class="wk">SEM. 1–3</div><div class="title">Genetic Synthesis and Assembly</div></div>
      <div class="pipe-step"><div class="wk">SEM. 4–8</div><div class="title">Fungal Transformation in the Laboratory</div></div>
      <div class="pipe-step"><div class="wk">SEM. 9–12</div><div class="title">Symbiotic integration with moss cultivation</div></div>
      <div class="pipe-step"><div class="wk">SEM. 13–18</div><div class="title">Acoustic Camera Tests</div></div>
      <div class="pipe-step"><div class="wk">SEM. 19–22</div><div class="title">Evaluation of Contaminant Filtration</div></div>
      <div class="pipe-step"><div class="wk">SEM. 23–30</div><div class="title">Tests in External Microenvironment</div></div>
      <div class="pipe-step"><div class="wk">YEAR 2</div><div class="title">Pilot Urban Deployment</div></div>
    </div>
  </section>

  <!-- EXPERIMENTAL DESIGN DETAILS -->
  <section>
    <div class="section-head">
      <span class="eyebrow">EXPERIMENTAL DESIGN DETAILS</span>
      <h2>Organism Selection, Methodology, and Controls</h2>
    </div>
    <div class="card-grid">
      <div class="card">
        <h3>Organism Selection</h3>
        <p><strong>Primary Organism:</strong> Cladonia rangiferina (lichen)</p>
        <p><strong>Secondary Organism:</strong> Mnium hornum (moss adapted to urban environments)</p>
        <p><strong>Supporting Microbiome:</strong> modified bacteria capable of degrading pollutants</p>
      </div>
      <div class="card">
        <h3>Transformation Method</h3>
        <p>Transformation mediated by Agrobacterium and genetic insertion using CRISPR-Cas9.</p>
        <p><strong>Promoters:</strong> constitutive growth promoter for laboratory tests; pollution-sensitive promoter for urban deployment.</p>
      </div>
      <div class="card">
        <h3>Control Groups</h3>
        <p><strong>Positive Control:</strong> commercial acoustic foam panels.</p>
        <p><strong>Negative Control:</strong> unmodified communities of lichen and moss.</p>
        <p><strong>Comparative Control:</strong> green walls without acoustic modification.</p>
      </div>
      <div class="card">
        <h3>Measurement Protocol</h3>
        <p><strong>Acoustic Performance:</strong> calibrated microphones before and after the treated surface, at 200, 500, 1000, 2000 and 4000&nbsp;Hz.</p>
        <p><strong>Air Quality:</strong> monitoring of PM2.5, PM10, nitrogen oxides and carbon deposition.</p>
      </div>
    </div>
  </section>

  <!-- OUTCOMES -->
  <section>
    <div class="section-head">
      <span class="eyebrow">Possible Outcomes and Biosecurity</span>
      <h2>What Could Happen, and How It's Contained</h2>
    </div>
    <div class="outcomes-grid">
      <div class="outcome-block">
        <div class="outcome-item">
          <span class="mark good">Primary Outcome</span>
          <p>Creation of self-sustaining acoustic surfaces capable of reducing urban traffic noise without external energy input.</p>
        </div>
        <div class="outcome-item">
          <span class="mark good">Secondary Outcome</span>
          <p>Simultaneous reduction of particulate pollution in areas with high traffic density.</p>
        </div>
        <div class="outcome-item">
          <span class="mark good">Additional Outcome</span>
          <p>Development of living infrastructure that requires significantly less maintenance than conventional sound barriers.</p>
        </div>
        <div class="outcome-item">
          <span class="mark warn">Possible Challenge</span>
          <p>Excessive moisture requirements in arid climates may limit deployment, necessitating drought-adapted variants.</p>
        </div>
      </div>
      <div class="outcome-block">
        <div class="outcome-item">
          <span class="mark good">Containment</span>
          <p>Initial testing in controlled greenhouse facilities under biosecurity protocols.</p>
        </div>
        <div class="outcome-item">
          <span class="mark good">Ecological Interaction</span>
          <p>Restricted growth on urban mineral substrates through designed nutritional dependencies.</p>
        </div>
        <div class="outcome-item">
          <span class="mark good">Genetic Flow</span>
          <p>Minimal risk due to low reproductive capacity and sterile deployment strains.</p>
        </div>
        <div class="outcome-item">
          <span class="mark good">Regulatory Compliance</span>
          <p>Compliance with European OGM regulations and urban environmental approval frameworks.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- IMPACT -->
  <section>
    <div class="section-head">
      <span class="eyebrow">Projected Social and Environmental Impact</span>
      <h2>An Ecological Layer Over the City</h2>
    </div>
    <div class="impact-grid">
      <div class="impact-card">
        <h4>Noise</h4>
        <p>Urban noise reduction around critical public spaces. Possible reduction of chronic stress and sleep disturbances.</p>
      </div>
      <div class="impact-card">
        <h4>Air Quality</h4>
        <p>Passive and continuous elimination of contaminating particles. Improvement of respiratory health outcomes in dense urban areas.</p>
      </div>
      <div class="impact-card">
        <h4>Infrastructure</h4>
        <p>Replacement of concrete acoustic barriers with living and regenerative systems. Reduction of construction materials and maintenance costs.</p>
      </div>
      <div class="impact-card">
        <h4>Urban Experience</h4>
        <p>Transformation of parks into authentic acoustic refuges. Creation of "silent corridors" where to escape the sensory overload of the city.</p>
      </div>
    </div>
  </section>

  <!-- CLOSING -->
  <section class="closing" style="border-bottom:none;">
    <span class="eyebrow">Design Question</span>
    <h2>What would happen if silence were considered a <span class="q">public ecological resource</span>, rather than the mere absence of sound?</h2>
  </section>

  <footer>
    <span>SONOLICHEN · SPECULATIVE BIODESIGN PROYECT</span>
    <span>ANTONIO GARCÍA· MDEF</span>
  </footer>

</div>

</body>
</html>
