[homepage.html](https://github.com/user-attachments/files/30804418/homepage.html)
# https-emailmarketingconsultant.netlify.app-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Email Marketing Consultant — Automation, Flows & Deliverability</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400;1,700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --ink:#0D1B2A;
  --ink-soft:#1D3048;
  --bg:#F9F7F1;
  --accent:#E8A020;
  --accent-dk:#C48A18;
  --accent-lt:#FFF4D6;
  --muted:#6B7A8D;
  --subtle:#9AAAB8;
  --white:#FFFFFF;
  --border:#E4DDD0;
  --red:#D94F3D;
  --red-lt:#FDF0EE;
  --green:#2D9E65;
}
html{scroll-behavior:smooth}
body{font-family:'Inter',sans-serif;background:var(--bg);color:var(--ink);font-size:16px;line-height:1.65;-webkit-font-smoothing:antialiased}
a{text-decoration:none;color:inherit}
img{max-width:100%;display:block}

/* LAYOUT */
.wrap{max-width:1140px;margin:0 auto;padding:0 28px}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.grid-2{display:grid;grid-template-columns:1fr 1fr;gap:56px;align-items:center}

/* BUTTONS */
.btn-amber{display:inline-flex;align-items:center;gap:9px;background:var(--accent);color:var(--ink);font-family:'Inter',sans-serif;font-weight:700;font-size:15px;padding:16px 32px;border-radius:8px;border:none;cursor:pointer;transition:background .2s,transform .15s;letter-spacing:.01em}
.btn-amber:hover{background:var(--accent-dk);transform:translateY(-1px)}
.btn-ghost-w{display:inline-flex;align-items:center;gap:9px;background:transparent;color:#fff;font-family:'Inter',sans-serif;font-weight:500;font-size:15px;padding:15px 26px;border-radius:8px;border:1.5px solid rgba(255,255,255,.3);cursor:pointer;transition:border-color .2s,background .2s}
.btn-ghost-w:hover{border-color:rgba(255,255,255,.65);background:rgba(255,255,255,.06)}

/* TYPE */
.eyebrow{display:inline-block;font-size:11px;font-weight:700;letter-spacing:.16em;text-transform:uppercase;color:var(--accent);margin-bottom:14px}
.h1{font-family:'Playfair Display',serif;font-size:clamp(38px,5.5vw,66px);font-weight:900;line-height:1.08;letter-spacing:-.025em;color:#fff}
.h2{font-family:'Playfair Display',serif;font-size:clamp(28px,3.8vw,46px);font-weight:700;line-height:1.18;letter-spacing:-.015em;color:var(--ink)}
.h3{font-family:'Playfair Display',serif;font-size:21px;font-weight:700;line-height:1.3;color:var(--ink)}
.lead{font-size:17px;line-height:1.78;color:rgba(255,255,255,.65);max-width:540px}
.body-muted{font-size:15px;line-height:1.75;color:var(--muted)}

/* ──────────────── NAV ──────────────── */
.nav{position:sticky;top:0;z-index:100;background:rgba(249,247,241,.92);backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);border-bottom:1px solid var(--border)}
.nav-inner{display:flex;align-items:center;justify-content:space-between;height:70px}
.nav-logo{font-family:'Playfair Display',serif;font-size:17px;font-weight:700;color:var(--ink);letter-spacing:-.01em}
.nav-logo em{color:var(--accent);font-style:normal}
.nav-links{display:flex;align-items:center;gap:34px;list-style:none}
.nav-links a{font-size:14px;font-weight:500;color:var(--muted);transition:color .2s}
.nav-links a:hover{color:var(--ink)}
.nav-cta{background:var(--ink) !important;color:#fff !important;font-weight:600 !important;font-size:13px !important;padding:9px 20px;border-radius:7px}
.nav-cta:hover{background:var(--ink-soft) !important;color:#fff !important}

/* ──────────────── HERO ──────────────── */
.hero{background:linear-gradient(138deg,#071422 0%,#0D1B2A 55%,#152D45 100%);padding:100px 0 88px;position:relative;overflow:hidden}
.hero::after{content:'@';position:absolute;right:-3%;top:-10%;font-size:480px;font-family:'Playfair Display',serif;font-weight:900;color:rgba(232,160,32,.045);line-height:1;pointer-events:none;user-select:none;letter-spacing:-.05em}
.hero-badge{display:inline-flex;align-items:center;gap:9px;background:rgba(232,160,32,.12);border:1px solid rgba(232,160,32,.3);border-radius:100px;padding:7px 16px;font-size:11px;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--accent);margin-bottom:26px}
.pulse{width:7px;height:7px;background:var(--accent);border-radius:50%;animation:pulseAnim 2s infinite}
@keyframes pulseAnim{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.45;transform:scale(.8)}}
.hero-headline em{color:var(--accent);font-style:italic}
.hero-ctas{display:flex;align-items:center;gap:16px;flex-wrap:wrap;margin-top:36px}
.hero-stats{display:flex;gap:0;margin-top:54px;border-top:1px solid rgba(255,255,255,.08);padding-top:32px}
.hstat{flex:1;padding-right:32px}
.hstat:not(:last-child){border-right:1px solid rgba(255,255,255,.08);margin-right:32px}
.hstat-num{font-family:'Playfair Display',serif;font-size:32px;font-weight:900;color:var(--accent);line-height:1;letter-spacing:-.02em}
.hstat-lbl{font-size:12px;color:rgba(255,255,255,.42);margin-top:5px;line-height:1.4}

/* Hero right panel */
.hero-panel{display:flex;flex-direction:column;gap:13px;position:relative;z-index:1}
.panel-label{font-size:10px;font-weight:700;letter-spacing:.14em;text-transform:uppercase;color:rgba(255,255,255,.3);margin-bottom:4px}
.ecard{background:rgba(255,255,255,.035);border:1px solid rgba(255,255,255,.08);border-radius:12px;padding:15px 18px;display:flex;align-items:center;gap:14px;transition:all .25s}
.ecard.live{background:rgba(232,160,32,.09);border-color:rgba(232,160,32,.28)}
.ecard.dead{border-style:dashed;opacity:.45}
.eico{width:36px;height:36px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:15px;flex-shrink:0}
.eico.g{background:rgba(45,158,101,.15)}
.eico.a{background:rgba(232,160,32,.15)}
.eico.r{background:rgba(217,79,61,.12)}
.ecard-body{flex:1}
.ecard-title{font-size:13px;font-weight:600;color:rgba(255,255,255,.9)}
.ecard-sub{font-size:11px;color:rgba(255,255,255,.38);margin-top:3px}
.ecard-rev{font-size:13px;font-weight:700;color:var(--accent)}
.ecard-rev.neg{color:#E07065}

/* ──────────────── TRUST BAR ──────────────── */
.trustbar{background:var(--white);border-bottom:1px solid var(--border);padding:26px 0}
.trustbar-inner{display:flex;align-items:center;justify-content:center;gap:44px;flex-wrap:wrap}
.trust-lbl{font-size:11px;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--subtle)}
.plat{display:flex;align-items:center;gap:9px;opacity:.5;transition:opacity .2s}
.plat:hover{opacity:.9}
.plat-ico{width:28px;height:28px;border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:800;flex-shrink:0}
.plat-name{font-size:14px;font-weight:700;color:var(--ink);letter-spacing:-.01em}

/* ──────────────── PROBLEM ──────────────── */
.problem{padding:96px 0;background:var(--bg)}
.section-hd{text-align:center;margin-bottom:56px}
.section-hd .h2{margin:6px 0 16px}
.section-hd .body-muted{max-width:540px;margin:0 auto;text-align:center}
.pcard{background:var(--white);border-radius:16px;padding:38px 32px;border:1px solid var(--border);position:relative;overflow:hidden;transition:transform .25s,box-shadow .25s}
.pcard::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:var(--red)}
.pcard:hover{transform:translateY(-5px);box-shadow:0 24px 64px rgba(13,27,42,.08)}
.pcard-ico{width:52px;height:52px;background:var(--red-lt);border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:22px;margin-bottom:20px}
.pcard .h3{margin-bottom:12px}
.pain-tag{display:inline-block;margin-top:18px;font-size:11px;font-weight:700;color:var(--red);background:var(--red-lt);padding:4px 10px;border-radius:4px;letter-spacing:.04em}

/* ──────────────── SERVICES ──────────────── */
.services{background:var(--ink);padding:96px 0;position:relative;overflow:hidden}
.services::before{content:'';position:absolute;width:700px;height:700px;background:radial-gradient(circle,rgba(232,160,32,.07) 0%,transparent 68%);top:-250px;right:-150px;pointer-events:none}
.services .eyebrow{color:var(--accent)}
.services .h2{color:#fff;margin:6px 0 16px}
.services .body-muted{color:rgba(255,255,255,.5);max-width:560px}
.svcard{background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.08);border-radius:16px;padding:36px 30px;transition:background .25s,border-color .25s}
.svcard:hover{background:rgba(255,255,255,.07);border-color:rgba(232,160,32,.22)}
.svcard-ico{width:52px;height:52px;background:rgba(232,160,32,.1);border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:22px;margin-bottom:22px}
.svcard .h3{color:#fff;margin-bottom:12px}
.svcard > p{font-size:14px;color:rgba(255,255,255,.48);line-height:1.75;margin-bottom:22px}
.sv-list{list-style:none;display:flex;flex-direction:column;gap:9px}
.sv-list li{font-size:13px;color:rgba(255,255,255,.62);display:flex;align-items:flex-start;gap:9px;line-height:1.55}
.sv-list li::before{content:'→';color:var(--accent);flex-shrink:0;font-size:12px;margin-top:1px}

/* ──────────────── HOW IT WORKS ──────────────── */
.hiw{padding:96px 0;background:var(--bg)}
.hiw-row{display:grid;grid-template-columns:1fr 48px 1fr 48px 1fr;align-items:start;gap:0;margin-top:56px}
.hiw-step{background:var(--white);border-radius:16px;padding:38px 28px;border:1px solid var(--border)}
.step-n{font-family:'Playfair Display',serif;font-size:58px;font-weight:900;line-height:1;color:var(--accent-lt);-webkit-text-stroke:1.5px var(--accent);margin-bottom:18px}
.hiw-step .h3{margin-bottom:11px}
.hiw-arrow{display:flex;align-items:center;justify-content:center;padding-top:68px;color:var(--accent);font-size:22px;font-weight:600}

/* ──────────────── PROOF ──────────────── */
.proof{padding:96px 0;background:var(--white)}
.stats-row{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--border);border:1px solid var(--border);border-radius:16px;overflow:hidden;margin-bottom:64px}
.stat-cell{background:var(--white);padding:38px 26px;text-align:center}
.stat-num{font-family:'Playfair Display',serif;font-size:42px;font-weight:900;color:var(--ink);letter-spacing:-.025em;line-height:1}
.stat-num em{color:var(--accent);font-style:normal}
.stat-lbl{font-size:13px;color:var(--muted);margin-top:7px;line-height:1.55}
.tcard{background:var(--bg);border-radius:16px;padding:32px;border:1px solid var(--border);position:relative}
.tcard-quote{font-family:'Playfair Display',serif;font-size:72px;color:var(--accent);line-height:.75;margin-bottom:14px;opacity:.55;display:block}
.tcard-text{font-size:15px;line-height:1.78;color:var(--ink-soft);font-style:italic;margin-bottom:22px}
.tcard-author{display:flex;align-items:center;gap:12px}
.avatar{width:44px;height:44px;border-radius:50%;background:linear-gradient(135deg,var(--accent),var(--ink));display:flex;align-items:center;justify-content:center;font-weight:700;color:#fff;font-size:13px;flex-shrink:0}
.author-name{font-size:14px;font-weight:700}
.author-role{font-size:12px;color:var(--muted);margin-top:2px}
.result-tag{display:inline-flex;align-items:center;gap:6px;background:rgba(45,158,101,.1);color:var(--green);font-size:11px;font-weight:700;padding:5px 10px;border-radius:5px;margin-top:16px;letter-spacing:.03em}
.proof-note{text-align:center;margin-top:12px;font-size:12px;color:var(--subtle);font-style:italic}

/* ──────────────── FINAL CTA ──────────────── */
.fcta{background:linear-gradient(138deg,#071422 0%,#0D1B2A 60%,#152D45 100%);padding:100px 0;text-align:center;position:relative;overflow:hidden}
.fcta::before{content:'';position:absolute;width:900px;height:900px;background:radial-gradient(circle,rgba(232,160,32,.07) 0%,transparent 65%);top:50%;left:50%;transform:translate(-50%,-50%);pointer-events:none}
.urgency-pill{display:inline-flex;align-items:center;gap:8px;background:rgba(217,79,61,.14);border:1px solid rgba(217,79,61,.3);border-radius:100px;padding:7px 18px;font-size:11px;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:#FF8075;margin-bottom:30px}
.upulse{width:7px;height:7px;background:#FF7066;border-radius:50%;animation:pulseAnim 1.5s infinite}
.fcta .h2{color:#fff;max-width:740px;margin:0 auto 20px}
.fcta .h2 em{color:var(--accent);font-style:italic}
.fcta-sub{font-size:17px;color:rgba(255,255,255,.55);max-width:520px;margin:0 auto 42px;line-height:1.75}
.cta-note{margin-top:20px;font-size:13px;color:rgba(255,255,255,.28)}
.cta-note span{margin:0 10px}

/* ──────────────── FOOTER ──────────────── */
footer{background:#06101A;padding:36px 0;border-top:1px solid rgba(255,255,255,.055)}
.footer-inner{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:20px}
.footer-logo{font-family:'Playfair Display',serif;font-size:16px;font-weight:700;color:rgba(255,255,255,.5)}
.footer-logo em{color:var(--accent);font-style:normal}
.footer-links{display:flex;gap:26px;list-style:none}
.footer-links a{font-size:13px;color:rgba(255,255,255,.3);transition:color .2s}
.footer-links a:hover{color:rgba(255,255,255,.65)}
.footer-copy{font-size:12px;color:rgba(255,255,255,.2)}

/* ──────────────── RESPONSIVE ──────────────── */
@media(max-width:960px){
  .grid-2{grid-template-columns:1fr}
  .hero-panel{display:none}
  .grid-3{grid-template-columns:1fr}
  .hiw-row{grid-template-columns:1fr;gap:24px}
  .hiw-arrow{display:none}
  .stats-row{grid-template-columns:repeat(2,1fr)}
  .nav-links{display:none}
}
@media(max-width:600px){
  .stats-row{grid-template-columns:1fr}
  .trustbar-inner{gap:24px}
  .hero-stats{flex-direction:column;gap:24px}
  .hstat:not(:last-child){border-right:none;margin-right:0;padding-right:0;border-bottom:1px solid rgba(255,255,255,.08);padding-bottom:20px}
  .hero{padding:72px 0 64px}
}
</style>
</head>
<body>

<!-- ═══════════════ NAVIGATION ═══════════════ -->
<nav class="nav">
  <div class="wrap">
    <div class="nav-inner">
      <div class="nav-logo">Email<em>.</em>Marketing</div>
      <ul class="nav-links">
        <li><a href="#problem">The Problem</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#proof">Results</a></li>
        <li><a href="#cta" class="nav-cta">Book a Call</a></li>
      </ul>
    </div>
  </div>
</nav>

<!-- ═══════════════ HERO ═══════════════ -->
<section class="hero" id="hero">
  <div class="wrap">
    <div class="grid-2">

      <!-- Left: Copy -->
      <div>
        <div class="hero-badge">
          <span class="pulse"></span>
          Klaviyo &amp; Mailchimp Certified Expert
        </div>
        <h1 class="h1">Turn Your Email List Into Your Most <em>Profitable</em> Sales Channel</h1>
        <p class="lead" style="margin-top:22px">Advanced automation flows and deliverability strategies that help e-commerce and B2B brands recover lost revenue, increase open rates, and land in inboxes — not spam folders.</p>
        <div class="hero-ctas">
          <button class="btn-amber" onclick="document.getElementById('cta').scrollIntoView({behavior:'smooth'})">
            &#128197; Book a Free Strategy Call
          </button>
          <button class="btn-ghost-w" onclick="document.getElementById('services').scrollIntoView({behavior:'smooth'})">
            See How It Works &rarr;
          </button>
        </div>
        <div class="hero-stats">
          <div class="hstat">
            <div class="hstat-num">200+</div>
            <div class="hstat-lbl">Brands Helped</div>
          </div>
          <div class="hstat">
            <div class="hstat-num">$4.2M</div>
            <div class="hstat-lbl">Revenue Recovered</div>
          </div>
          <div class="hstat">
            <div class="hstat-num">42%</div>
            <div class="hstat-lbl">Avg. Open Rate</div>
          </div>
        </div>
      </div>

      <!-- Right: Visual Panel -->
      <div class="hero-panel">
        <div class="panel-label">Live Automation Flows</div>
        <div class="ecard live">
          <div class="eico a">&#128722;</div>
          <div class="ecard-body">
            <div class="ecard-title">Abandoned Cart — Email 2 of 3</div>
            <div class="ecard-sub">Sent 23 min ago &middot; 48% open rate</div>
          </div>
          <span class="ecard-rev">+$1,240</span>
        </div>
        <div class="ecard">
          <div class="eico g">&#128075;</div>
          <div class="ecard-body">
            <div class="ecard-title">Welcome Series — Day 1</div>
            <div class="ecard-sub">Sending now &middot; 62% open rate</div>
          </div>
          <span class="ecard-rev">+$340</span>
        </div>
        <div class="ecard">
          <div class="eico g">&#128260;</div>
          <div class="ecard-body">
            <div class="ecard-title">Win-Back Campaign — Segment A</div>
            <div class="ecard-sub">Completed &middot; 11% conversion</div>
          </div>
          <span class="ecard-rev">+$6,800</span>
        </div>
        <div class="ecard dead">
          <div class="eico r">&#9888;&#65039;</div>
          <div class="ecard-body">
            <div class="ecard-title">Your current setup (before us)</div>
            <div class="ecard-sub">Manual blasts &middot; 14% open rate</div>
          </div>
          <span class="ecard-rev neg">$0 tracked</span>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ═══════════════ TRUST BAR ═══════════════ -->
<div class="trustbar">
  <div class="wrap">
    <div class="trustbar-inner">
      <span class="trust-lbl">Expert on</span>
      <div class="plat">
        <div class="plat-ico" style="background:#FFB224;color:#1A1A1A">K</div>
        <span class="plat-name">Klaviyo</span>
      </div>
      <div class="plat">
        <div class="plat-ico" style="background:#FFE01B;color:#1A1A1A">MC</div>
        <span class="plat-name">Mailchimp</span>
      </div>
      <div class="plat">
        <div class="plat-ico" style="background:#1CA0F1;color:#fff">AC</div>
        <span class="plat-name">ActiveCampaign</span>
      </div>
      <div class="plat">
        <div class="plat-ico" style="background:#0A5FFF;color:#fff">SF</div>
        <span class="plat-name">Salesforce MC</span>
      </div>
      <div class="plat">
        <div class="plat-ico" style="background:#EA4B35;color:#fff">DR</div>
        <span class="plat-name">Drip</span>
      </div>
    </div>
  </div>
</div>

<!-- ═══════════════ PROBLEM SECTION ═══════════════ -->
<section class="problem" id="problem">
  <div class="wrap">
    <div class="section-hd">
      <span class="eyebrow">The Problem</span>
      <h2 class="h2">Most Email Programs Are Quietly Bleeding Revenue</h2>
      <p class="body-muted">If any of these feel uncomfortably familiar, you're not alone — and none of them are permanent.</p>
    </div>
    <div class="grid-3">

      <div class="pcard">
        <div class="pcard-ico">&#128184;</div>
        <h3 class="h3">You're Leaving Money on the Table</h3>
        <p class="body-muted">Abandoned carts pile up. Browse abandonment goes unnoticed. Post-purchase upsells never land. You're paying for traffic and capturing leads — then watching them leave without a second touchpoint. Without the right automation flows, every visitor who doesn't buy on the first click is revenue you never recover.</p>
        <span class="pain-tag">Lost Revenue</span>
      </div>

      <div class="pcard">
        <div class="pcard-ico">&#128202;</div>
        <h3 class="h3">Your Open Rates Are Embarrassing</h3>
        <p class="body-muted">Generic broadcasts to your entire list. No segmentation. No personalization. Your subscribers have learned to ignore you — and your metrics prove it. When you're not sending the right message to the right person at the right moment, even the best copy becomes invisible. An unread email is a silent cost centre.</p>
        <span class="pain-tag">Low Engagement</span>
      </div>

      <div class="pcard">
        <div class="pcard-ico">&#128683;</div>
        <h3 class="h3">You're Living in the Spam Folder</h3>
        <p class="body-muted">Misconfigured SPF, DKIM, or DMARC records. A damaged sender reputation. Mailing unengaged subscribers. Any one of these quietly buries your emails in spam — meaning your carefully crafted campaign never even gets seen. Deliverability problems are invisible until it's too late, and they compound quickly.</p>
        <span class="pain-tag">Deliverability Issues</span>
      </div>

    </div>
  </div>
</section>

<!-- ═══════════════ SERVICES ═══════════════ -->
<section class="services" id="services">
  <div class="wrap">
    <div style="margin-bottom:52px">
      <span class="eyebrow">What I Do</span>
      <h2 class="h2">End-to-End Email Strategy That Actually Converts</h2>
      <p class="body-muted" style="margin-top:14px">From the technical foundations to the automation flows that earn revenue while you sleep — I build email systems for e-commerce and B2B brands on Klaviyo, Mailchimp, and beyond.</p>
    </div>
    <div class="grid-3">

      <div class="svcard">
        <div class="svcard-ico">&#9889;</div>
        <h3 class="h3">Automation Flow Strategy &amp; Build</h3>
        <p>High-converting email sequences built for your exact customer journey — not copy-pasted templates you've seen a dozen times before.</p>
        <ul class="sv-list">
          <li>Welcome Series — Days 1–7 relationship building</li>
          <li>Abandoned Cart — 3-email recovery sequence</li>
          <li>Browse &amp; Product Abandonment flows</li>
          <li>Post-Purchase &amp; Repeat Buyer sequences</li>
          <li>Win-Back &amp; Sunset flows for cold subscribers</li>
        </ul>
      </div>

      <div class="svcard">
        <div class="svcard-ico">&#127919;</div>
        <h3 class="h3">Advanced Segmentation &amp; Targeting</h3>
        <p>Stop sending everything to everyone. Reach the right subscriber with the right message at exactly the right moment — and watch your metrics reflect it.</p>
        <ul class="sv-list">
          <li>RFM segmentation (Recency, Frequency, Monetary)</li>
          <li>Behavioural segments by browsing &amp; purchase history</li>
          <li>Engagement-based send frequency management</li>
          <li>Dynamic content personalisation by segment</li>
          <li>A/B testing frameworks for continuous improvement</li>
        </ul>
      </div>

      <div class="svcard">
        <div class="svcard-ico">&#9989;</div>
        <h3 class="h3">Deliverability Audit &amp; Optimisation</h3>
        <p>Your emails should reach the inbox every single time. I handle the technical and strategic work that makes that happen and keeps it that way.</p>
        <ul class="sv-list">
          <li>Full DNS audit — SPF, DKIM, DMARC configuration</li>
          <li>Sender reputation diagnosis and repair plan</li>
          <li>IP and domain warm-up strategy</li>
          <li>List hygiene and re-engagement planning</li>
          <li>Spam score reduction &amp; inbox placement testing</li>
        </ul>
      </div>

    </div>
  </div>
</section>

<!-- ═══════════════ HOW IT WORKS ═══════════════ -->
<section class="hiw" id="process">
  <div class="wrap">
    <div class="section-hd">
      <span class="eyebrow">The Process</span>
      <h2 class="h2">From Audit to Revenue in 30 Days</h2>
      <p class="body-muted">No long contracts. No vague deliverables. A clear three-step engagement designed to show measurable results fast.</p>
    </div>
    <div class="hiw-row">

      <div class="hiw-step">
        <div class="step-n">01</div>
        <h3 class="h3">Discovery &amp; Audit</h3>
        <p class="body-muted" style="margin-top:10px">We start with a free 30-minute strategy call to diagnose your current setup. I audit your existing flows, deliverability metrics, platform configuration, and segmentation logic — identifying exactly where revenue is leaking and what to fix first.</p>
      </div>

      <div class="hiw-arrow">&rarr;</div>

      <div class="hiw-step">
        <div class="step-n">02</div>
        <h3 class="h3">Build &amp; Implement</h3>
        <p class="body-muted" style="margin-top:10px">I design, write, and deploy your automation flows, segmentation architecture, and deliverability fixes directly inside your platform. Every element is built for your brand, tested before launch, and fully documented for your team.</p>
      </div>

      <div class="hiw-arrow">&rarr;</div>

      <div class="hiw-step">
        <div class="step-n">03</div>
        <h3 class="h3">Optimise &amp; Scale</h3>
        <p class="body-muted" style="margin-top:10px">After launch, I monitor performance, run A/B tests, and refine based on real data. The goal isn't a one-time win — it's a self-improving email programme that compounds revenue month after month.</p>
      </div>

    </div>
  </div>
</section>

<!-- ═══════════════ SOCIAL PROOF ═══════════════ -->
<section class="proof" id="proof">
  <div class="wrap">

    <!-- Stats Row -->
    <div class="stats-row">
      <div class="stat-cell">
        <div class="stat-num"><em>$</em>4.2M</div>
        <div class="stat-lbl">Revenue recovered via<br>cart abandonment flows</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num">200<em>+</em></div>
        <div class="stat-lbl">E-commerce &amp; B2B<br>brands served</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num">42<em>%</em></div>
        <div class="stat-lbl">Average open rate<br>across client accounts</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num"><em>&uarr;</em>3x</div>
        <div class="stat-lbl">Average email revenue<br>within 60 days</div>
      </div>
    </div>

    <!-- Testimonials -->
    <div class="section-hd">
      <span class="eyebrow">Client Results</span>
      <h2 class="h2">Real Outcomes From Real Brands</h2>
    </div>
    <div class="grid-3">

      <div class="tcard">
        <span class="tcard-quote">&ldquo;</span>
        <p class="tcard-text">Before working together, our abandoned cart emails were going to spam and our open rates sat at 12%. Within 45 days we had a fully built Klaviyo flow system, our open rates hit 38%, and we recovered over $80,000 in carts we never would have captured.</p>
        <div class="tcard-author">
          <div class="avatar">SJ</div>
          <div>
            <div class="author-name">[Sarah J.] — Replace With Client</div>
            <div class="author-role">Founder, DTC Skincare Brand</div>
          </div>
        </div>
        <span class="result-tag">&#8593; $80K in recovered revenue</span>
      </div>

      <div class="tcard">
        <span class="tcard-quote">&ldquo;</span>
        <p class="tcard-text">We'd been on Mailchimp for three years but had no real strategy — just monthly newsletters nobody read. The segmentation rebuild transformed our engagement. We went from 2% click rates to 9% in a single quarter. Email is now our top-performing channel, full stop.</p>
        <div class="tcard-author">
          <div class="avatar">MR</div>
          <div>
            <div class="author-name">[Mark R.] — Replace With Client</div>
            <div class="author-role">VP Marketing, B2B SaaS</div>
          </div>
        </div>
        <span class="result-tag">&#8593; 4.5x click-through rate</span>
      </div>

      <div class="tcard">
        <span class="tcard-quote">&ldquo;</span>
        <p class="tcard-text">The deliverability audit was worth ten times the price. We had no idea our DMARC record was misconfigured and that 30% of our emails weren't reaching inboxes. After the fix and list hygiene, our inbox placement rate went from 67% to 96%. Game-changing.</p>
        <div class="tcard-author">
          <div class="avatar">AC</div>
          <div>
            <div class="author-name">[Alex C.] — Replace With Client</div>
            <div class="author-role">E-commerce Director, Fashion Brand</div>
          </div>
        </div>
        <span class="result-tag">&#8593; 96% inbox placement rate</span>
      </div>

    </div>
    <p class="proof-note">&#9432;&nbsp; Replace placeholder testimonials with real client quotes and results. Keep the result tags — they're conversion gold.</p>

  </div>
</section>

<!-- ═══════════════ FINAL CTA ═══════════════ -->
<section class="fcta" id="cta">
  <div class="wrap" style="position:relative;z-index:1">
    <div class="urgency-pill">
      <span class="upulse"></span>
      Currently Accepting 3 New Clients This Month
    </div>
    <h2 class="h2">Ready to Make Email Your <em>#1 Revenue Channel?</em></h2>
    <p class="fcta-sub">In one free 30-minute call, I'll identify your three biggest email revenue leaks and give you a clear roadmap to fix them — whether we work together or not.</p>
    <button class="btn-amber" style="font-size:16px;padding:18px 38px" onclick="alert('Connect your booking tool here — Calendly, Cal.com, or TidyCal work great.')">
      &#128197; Book Your Free 30-Minute Discovery Call
    </button>
    <p class="cta-note">
      No sales pressure<span>·</span>No commitment required<span>·</span>100% focused on your results
    </p>
  </div>
</section>

<!-- ═══════════════ FOOTER ═══════════════ -->
<footer>
  <div class="wrap">
    <div class="footer-inner">
      <div class="footer-logo">Email<em>.</em>Marketing</div>
      <ul class="footer-links">
        <li><a href="#problem">The Problem</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#proof">Results</a></li>
        <li><a href="#cta">Contact</a></li>
      </ul>
      <p class="footer-copy">&copy; 2025 Email Marketing Consultant. All rights reserved.</p>
    </div>
  </div>
</footer>

</body>
</html>
