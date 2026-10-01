<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GK GS MASTI | Chapter-1: प्रागैतिहासिक काल</title>
<style>
/* ================= BASE ================= */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', 'Noto Sans Devanagari', Arial, sans-serif;
  -webkit-tap-highlight-color: transparent;
}

:root {
  --gold: #fbbf24;
  --gold2: #f59e0b;
  --green: #10b981;
  --red: #ef4444;
  --ink: #0f1b3d;
  --purple: #7c3aed;
  --cyan: #06b6d4;
  --pink: #ec4899;
}

html, body {
  min-height: 100%;
  overflow-x: hidden;
}

body {
  background: radial-gradient(circle at 20% 0%, #1e1b4b 0%, #0f0c29 40%, #05030f 100%);
  padding: 14px 10px 40px;
  perspective: 1400px;
  color: #fff;
}

/* floating glow blobs */
body::before, body::after {
  content: "";
  position: fixed;
  border-radius: 50%;
  filter: blur(100px);
  opacity: .4;
  z-index: 0;
  pointer-events: none;
}
body::before {
  width: 360px; height: 360px;
  background: #06b6d4;
  top: -140px; left: -140px;
  animation: float 10s ease-in-out infinite;
}
body::after {
  width: 400px; height: 400px;
  background: #7c3aed;
  bottom: -180px; right: -160px;
  animation: float 13s ease-in-out infinite reverse;
}
@keyframes float {
  0%,100% { transform: translateY(0) translateX(0); }
  50% { transform: translateY(45px) translateX(30px); }
}

/* ================= HEADER ================= */
.header {
  position: sticky;
  top: 10px;
  z-index: 50;
  max-width: 820px;
  margin: 0 auto 22px;
  padding: 16px 18px 18px;
  border-radius: 22px;
  background: linear-gradient(145deg, #ffffff 0%, #f1f5ff 55%, #e3e9ff 100%);
  transform-style: preserve-3d;
  transform: rotateX(5deg);
  box-shadow:
    0 2px 0 #ffffff inset,
    0 -7px 0 #c5cfef inset,
    0 24px 44px -18px rgba(0,0,0,.95),
    0 0 0 2px rgba(255,255,255,.12);
  animation: headerIn .8s cubic-bezier(.2,.9,.3,1.2) both;
}
@keyframes headerIn {
  from { opacity: 0; transform: rotateX(30deg) translateY(-40px) scale(.9); }
  to   { opacity: 1; transform: rotateX(5deg) translateY(0) scale(1); }
}

.header-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  flex-wrap: wrap;
}

.brand {
  font-size: clamp(18px, 4.5vw, 30px);
  font-weight: 900;
  letter-spacing: 1.5px;
  padding: 6px 16px;
  border-radius: 12px;
  color: #fff;
  background: linear-gradient(135deg, #06b6d4, #7c3aed 60%, #ec4899);
  text-shadow: 0 2px 6px rgba(0,0,0,.45);
  box-shadow:
    0 6px 0 #4c1d95,
    0 14px 24px -10px rgba(0,0,0,.9),
    0 0 26px rgba(124,58,237,.65);
  animation: brandPulse 3s ease-in-out infinite;
  white-space: nowrap;
}
@keyframes brandPulse {
  0%,100% { filter: brightness(1); }
  50% { filter: brightness(1.15); }
}

.timer {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: clamp(15px, 3.4vw, 20px);
  font-weight: 900;
  letter-spacing: 1.5px;
  padding: 8px 16px;
  border-radius: 14px;
  color: #fff;
  background: linear-gradient(145deg, #1e1b4b, #0b0821);
  border: 2px solid rgba(6,182,212,.45);
  box-shadow: 0 6px 0 #05030f, 0 12px 22px -10px #000, 0 0 18px rgba(6,182,212,.35);
  transition: all .3s ease;
  font-variant-numeric: tabular-nums;
}
.timer .icon { font-size: 1.1em; }
.timer.warning {
  background: linear-gradient(145deg, #7f1d1d, #450a0a);
  border-color: rgba(239,68,68,.7);
  animation: timerBlink 1s ease-in-out infinite;
}
@keyframes timerBlink {
  0%,100% { box-shadow: 0 6px 0 #05030f, 0 0 20px rgba(239,68,68,.7); }
  50% { box-shadow: 0 6px 0 #05030f, 0 0 34px rgba(239,68,68,1); }
}

.chapter-line {
  margin-top: 14px;
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  justify-content: center;
}
.chapter-line span {
  font-size: clamp(11px, 2.6vw, 14px);
  font-weight: 800;
  letter-spacing: 1.2px;
  padding: 7px 18px;
  border-radius: 999px;
  color: #fff;
  background: linear-gradient(135deg, #7c3aed, #06b6d4);
  box-shadow: 0 5px 0 #312e81, 0 10px 18px -8px rgba(0,0,0,.85);
}
.chapter-line span.gold {
  background: linear-gradient(135deg, #f59e0b, #fbbf24);
  color: #3b1f00;
  box-shadow: 0 5px 0 #92400e, 0 10px 18px -8px rgba(0,0,0,.85);
}

/* ================= MAIN ================= */
.main {
  max-width: 820px;
  margin: 0 auto;
  position: relative;
  z-index: 5;
  transform-style: preserve-3d;
}

/* progress */
.progress-wrap {
  margin-bottom: 16px;
  height: 12px;
  border-radius: 999px;
  background: #1a1440;
  border: 2px solid rgba(255,255,255,.1);
  box-shadow: inset 0 3px 8px rgba(0,0,0,.75);
  overflow: hidden;
  position: relative;
}
.progress-bar {
  height: 100%;
  width: 0%;
  border-radius: 999px;
  background: linear-gradient(90deg, #06b6d4, #7c3aed 50%, #ec4899);
  box-shadow: 0 0 16px rgba(124,58,237,.9);
  transition: width .5s cubic-bezier(.2,.9,.3,1);
}

/* ================= QUESTION CARD ================= */
.q-card {
  border-radius: 24px;
  padding: 22px 20px 22px;
  background: linear-gradient(150deg, #ffffff 0%, #f6f8ff 100%);
  transform-style: preserve-3d;
  transform: rotateX(4deg);
  box-shadow:
    0 2px 0 #ffffff inset,
    0 -9px 0 #c9d2f0 inset,
    0 28px 44px -20px rgba(0,0,0,.95),
    0 0 0 1px rgba(255,255,255,.1);
  animation: cardIn .55s cubic-bezier(.2,.9,.3,1.2) both;
}
@keyframes cardIn {
  from { opacity: 0; transform: rotateX(24deg) translateY(45px) scale(.96); }
  to   { opacity: 1; transform: rotateX(4deg) translateY(0) scale(1); }
}

.q-meta {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  margin-bottom: 14px;
  flex-wrap: wrap;
}

.q-tag {
  display: inline-block;
  font-size: 11px;
  font-weight: 800;
  letter-spacing: .6px;
  text-transform: uppercase;
  padding: 5px 13px;
  border-radius: 999px;
  color: #fff;
  background: linear-gradient(135deg, #7c3aed, #06b6d4);
  box-shadow: 0 4px 0 #312e81;
}

.q-counter {
  font-size: 13px;
  font-weight: 900;
  color: #4b5680;
  padding: 6px 14px;
  border-radius: 999px;
  background: #eef1ff;
  border: 2px solid #d5dcfb;
}

.q-head {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  margin-bottom: 6px;
}

.q-num {
  flex: 0 0 auto;
  width: 46px; height: 46px;
  display: grid;
  place-items: center;
  font-size: 19px;
  font-weight: 900;
  color: #fff;
  border-radius: 14px;
  background: linear-gradient(145deg, #06b6d4, #0e7490);
  box-shadow: 0 6px 0 #083344, 0 12px 18px -8px rgba(0,0,0,.85);
  transform: translateZ(30px);
}

.q-text {
  font-size: clamp(15px, 3.3vw, 18.5px);
  font-weight: 800;
  line-height: 1.7;
  color: var(--ink);
  transform: translateZ(20px);
}

/* options */
.options {
  display: flex;
  flex-direction: column;
  gap: 11px;
  margin-top: 18px;
  transform-style: preserve-3d;
}

.opt {
  position: relative;
  display: flex;
  align-items: center;
  gap: 12px;
  width: 100%;
  text-align: left;
  cursor: pointer;
  font-size: clamp(13.5px, 3vw, 16px);
  font-weight: 700;
  line-height: 1.55;
  color: #1a2352;
  padding: 13px 15px;
  border: 2px solid #d5dcfb;
  border-radius: 15px;
  background: linear-gradient(150deg, #ffffff, #eef1ff);
  box-shadow: 0 7px 0 #bec8eb, 0 14px 20px -14px rgba(0,0,0,.9);
  transform-style: preserve-3d;
  transition: transform .18s ease, box-shadow .18s ease, background .25s ease, border-color .25s ease;
  font-family: inherit;
}
.opt .key {
  flex: 0 0 auto;
  width: 34px; height: 34px;
  display: grid;
  place-items: center;
  font-weight: 900;
  font-size: 15px;
  color: #fff;
  border-radius: 10px;
  background: linear-gradient(145deg, #7c3aed, #5b21b6);
  box-shadow: 0 4px 0 #3b0764;
  transition: transform .25s ease;
}

.opt:hover:not(.locked) {
  transform: translateY(-3px) translateZ(14px);
  border-color: #a78bfa;
  box-shadow: 0 11px 0 #aeb9e6, 0 22px 30px -16px rgba(0,0,0,.95);
}
.opt:hover:not(.locked) .key { transform: scale(1.1) rotate(-6deg); }

.opt:active:not(.locked) {
  transform: translateY(2px) translateZ(0);
  box-shadow: 0 4px 0 #bec8eb;
}

.opt.locked { cursor: default; }

.opt.correct {
  color: #03330f;
  border-color: #10b981;
  background: linear-gradient(150deg, #d1fae5, #a7f3d0);
  box-shadow: 0 7px 0 #047857, 0 16px 26px -12px rgba(0,0,0,.85), 0 0 28px rgba(16,185,129,.6);
  animation: pop .45s cubic-bezier(.2,.9,.3,1.6) both;
}
.opt.correct .key { background: linear-gradient(145deg, #10b981, #047857); box-shadow: 0 4px 0 #064e3b; }

.opt.wrong {
  color: #4a0505;
  border-color: #ef4444;
  background: linear-gradient(150deg, #fee2e2, #fecaca);
  box-shadow: 0 7px 0 #b91c1c, 0 16px 26px -12px rgba(0,0,0,.85), 0 0 28px rgba(239,68,68,.55);
  animation: shake .45s ease both;
}
.opt.wrong .key { background: linear-gradient(145deg, #ef4444, #991b1b); box-shadow: 0 4px 0 #7f1d1d; }

@keyframes pop {
  0% { transform: scale(.94); }
  60% { transform: scale(1.03); }
  100% { transform: scale(1); }
}
@keyframes shake {
  0%,100% { transform: translateX(0); }
  20% { transform: translateX(-8px); }
  40% { transform: translateX(7px); }
  60% { transform: translateX(-5px); }
  80% { transform: translateX(3px); }
}

.opt .mark {
  margin-left: auto;
  font-size: 20px;
  font-weight: 900;
  opacity: 0;
  transform: scale(.4) rotate(-40deg);
  transition: all .35s cubic-bezier(.2,.9,.3,1.6);
  flex: 0 0 auto;
}
.opt.correct .mark, .opt.wrong .mark {
  opacity: 1;
  transform: scale(1) rotate(0deg);
}

/* explanation */
.explain {
  margin-top: 16px;
  border-radius: 16px;
  padding: 0 18px;
  max-height: 0;
  opacity: 0;
  overflow: hidden;
  font-size: clamp(12.5px, 2.9vw, 15px);
  line-height: 1.8;
  color: #10214a;
  font-weight: 600;
  background: linear-gradient(150deg, #fefce8, #fef3c7);
  border-left: 7px solid var(--gold2);
  box-shadow: 0 8px 0 #eab308 inset, 0 14px 24px -16px rgba(0,0,0,.9);
  transition: max-height .55s cubic-bezier(.2,.9,.3,1), opacity .45s ease, padding .45s ease;
}
.explain.show {
  max-height: 900px;
  opacity: 1;
  padding: 16px 18px;
}
.explain .ans-line {
  display: block;
  margin-bottom: 8px;
  font-weight: 900;
  color: #047857;
  font-size: 1.02em;
}
.explain .lbl {
  display: inline-block;
  font-weight: 900;
  color: #92400e;
  margin-right: 6px;
}

/* next button */
.next-wrap {
  margin-top: 20px;
  display: flex;
  justify-content: flex-end;
}
.next-btn {
  cursor: pointer;
  font-family: inherit;
  font-size: clamp(14px, 3vw, 16px);
  font-weight: 900;
  letter-spacing: .8px;
  color: #fff;
  padding: 14px 32px;
  border: none;
  border-radius: 15px;
  background: linear-gradient(145deg, #7c3aed, #06b6d4);
  box-shadow: 0 8px 0 #312e81, 0 18px 28px -14px #000;
  transition: transform .18s ease, box-shadow .18s ease, opacity .3s ease;
  display: none;
  align-items: center;
  gap: 8px;
}
.next-btn.show { display: inline-flex; animation: pop .4s ease both; }
.next-btn:hover { transform: translateY(-4px); box-shadow: 0 12px 0 #312e81, 0 24px 34px -16px #000; }
.next-btn:active { transform: translateY(4px); box-shadow: 0 4px 0 #312e81; }
.next-btn.gold {
  background: linear-gradient(145deg, #f59e0b, #fbbf24);
  color: #3b1f00;
  box-shadow: 0 8px 0 #92400e, 0 18px 28px -14px #000;
}
.next-btn.gold:hover { box-shadow: 0 12px 0 #92400e, 0 24px 34px -16px #000; }
.next-btn.gold:active { box-shadow: 0 4px 0 #92400e; }

/* ================= RESULT DASHBOARD ================= */
.result-section {
  display: none;
  animation: cardIn .6s cubic-bezier(.2,.9,.3,1.2) both;
}
.result-section.show { display: block; }

.dashboard {
  border-radius: 26px;
  padding: 30px 22px 28px;
  background: linear-gradient(150deg, #ffffff 0%, #f6f8ff 100%);
  transform-style: preserve-3d;
  transform: rotateX(3deg);
  box-shadow:
    0 2px 0 #ffffff inset,
    0 -10px 0 #c9d2f0 inset,
    0 32px 48px -22px rgba(0,0,0,.95),
    0 0 0 1px rgba(255,255,255,.12);
  text-align: center;
}

.dash-title {
  font-size: clamp(22px, 5vw, 32px);
  font-weight: 900;
  color: var(--ink);
  margin-bottom: 6px;
  letter-spacing: .5px;
}
.dash-sub {
  font-size: clamp(12px, 2.9vw, 15px);
  font-weight: 700;
  color: #6b76a3;
  margin-bottom: 26px;
}

/* circular percent */
.circle-wrap {
  position: relative;
  width: 190px;
  height: 190px;
  margin: 0 auto 26px;
  filter: drop-shadow(0 18px 26px rgba(0,0,0,.4));
}
.circle-wrap svg {
  width: 100%; height: 100%;
  transform: rotate(-90deg);
}
.circle-bg { fill: none; stroke: #e2e7fb; stroke-width: 14; }
.circle-fg {
  fill: none;
  stroke: url(#gradCircle);
  stroke-width: 14;
  stroke-linecap: round;
  stroke-dasharray: 440;
  stroke-dashoffset: 440;
  transition: stroke-dashoffset 1.2s cubic-bezier(.2,.9,.3,1);
}
.circle-inner {
  position: absolute;
  inset: 0;
  display: grid;
  place-items: center;
}
.circle-pct {
  font-size: 46px;
  font-weight: 900;
  color: var(--ink);
  line-height: 1;
  transform: translateY(-6px);
}
.circle-lbl {
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 1.5px;
  color: #6b76a3;
  text-transform: uppercase;
  transform: translateY(8px);
}

/* stats grid */
.stats {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin-bottom: 26px;
}
.stat {
  border-radius: 18px;
  padding: 18px 8px 16px;
  background: linear-gradient(150deg, #ffffff, #eef1ff);
  border: 2px solid #d5dcfb;
  box-shadow: 0 7px 0 #bec8eb, 0 14px 20px -14px rgba(0,0,0,.9);
  transform-style: preserve-3d;
  transition: transform .25s ease;
}
.stat:hover { transform: translateY(-4px) translateZ(14px); }
.stat .num {
  font-size: clamp(24px, 6vw, 34px);
  font-weight: 900;
  line-height: 1;
  margin-bottom: 6px;
  color: var(--ink);
}
.stat .lbl {
  font-size: clamp(10px, 2.4vw, 12px);
  font-weight: 800;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #6b76a3;
}
.stat.ok .num { color: #059669; }
.stat.bad .num { color: #dc2626; }
.stat.total .num { color: #7c3aed; }

.dash-msg {
  font-size: clamp(15px, 3.4vw, 19px);
  font-weight: 800;
  padding: 14px 18px;
  border-radius: 16px;
  margin-bottom: 26px;
  color: #4b2a00;
  background: linear-gradient(150deg, #fefce8, #fde68a);
  border: 2px solid #fbbf24;
  box-shadow: 0 6px 0 #d97706;
}

.dash-actions {
  display: flex;
  gap: 12px;
  justify-content: center;
  flex-wrap: wrap;
}
.btn {
  cursor: pointer;
  font-family: inherit;
  font-size: clamp(14px, 3vw, 16px);
  font-weight: 900;
  letter-spacing: .8px;
  color: #fff;
  padding: 14px 30px;
  border: none;
  border-radius: 15px;
  transition: transform .18s ease, box-shadow .18s ease;
}
.btn-primary {
  background: linear-gradient(145deg, #7c3aed, #06b6d4);
  box-shadow: 0 8px 0 #312e81, 0 18px 28px -14px #000;
}
.btn-primary:hover { transform: translateY(-4px); box-shadow: 0 12px 0 #312e81, 0 24px 34px -16px #000; }
.btn-primary:active { transform: translateY(4px); box-shadow: 0 4px 0 #312e81; }

.btn-gold {
  background: linear-gradient(145deg, #f59e0b, #fbbf24);
  color: #3b1f00;
  box-shadow: 0 8px 0 #92400e, 0 18px 28px -14px #000;
}
.btn-gold:hover { transform: translateY(-4px); box-shadow: 0 12px 0 #92400e, 0 24px 34px -16px #000; }
.btn-gold:active { transform: translateY(4px); box-shadow: 0 4px 0 #92400e; }

/* ================= BALLOON ANIMATION ================= */
.balloon {
  position: fixed;
  bottom: -80px;
  font-size: 42px;
  pointer-events: none;
  z-index: 999;
  animation: balloonRise 3.2s cubic-bezier(.2,.7,.3,1) forwards;
  filter: drop-shadow(0 6px 10px rgba(0,0,0,.4));
  will-change: transform, opacity;
}
@keyframes balloonRise {
  0% {
    transform: translateY(0) scale(.4) rotate(0deg);
    opacity: 1;
  }
  15% {
    transform: translateY(-60px) scale(1.1) rotate(-8deg);
    opacity: 1;
  }
  100% {
    transform: translateY(-110vh) scale(1) rotate(12deg);
    opacity: 0;
  }
}

/* confetti burst */
.confetti {
  position: fixed;
  width: 10px;
  height: 14px;
  z-index: 999;
  pointer-events: none;
  animation: confettiFall 3s ease-out forwards;
}
@keyframes confettiFall {
  0% { transform: translateY(0) rotate(0deg); opacity: 1; }
  100% { transform: translateY(105vh) rotate(720deg); opacity: 0; }
}

/* ================= FOOTER ================= */
footer {
  text-align: center;
  margin-top: 34px;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 1px;
  color: #8b93c0;
  position: relative;
  z-index: 5;
}

/* ================= RESPONSIVE ================= */
@media (max-width: 480px) {
  body { padding: 10px 8px 30px; }
  .header { padding: 13px 14px 15px; border-radius: 18px; top: 6px; }
  .q-card { padding: 18px 14px 18px; border-radius: 20px; }
  .q-num { width: 38px; height: 38px; font-size: 16px; border-radius: 11px; }
  .opt { padding: 12px 12px; gap: 10px; border-radius: 13px; }
  .opt .key { width: 28px; height: 28px; font-size: 13px; border-radius: 8px; }
  .dashboard { padding: 22px 14px 22px; border-radius: 20px; }
  .circle-wrap { width: 155px; height: 155px; }
  .circle-pct { font-size: 36px; }
  .stats { gap: 8px; }
  .stat { padding: 14px 4px 12px; border-radius: 14px; }
  .next-btn { width: 100%; justify-content: center; }
  .next-wrap { justify-content: stretch; }
  .dash-actions .btn { flex: 1 1 100%; }
}

@media (min-width: 900px) {
  .q-card { padding: 28px 26px 26px; }
  .q-text { font-size: 19px; }
}
</style>
</head>
<body>

<!-- ================= HEADER ================= -->
<header class="header">
  <div class="header-top">
    <div class="brand">GK GS MASTI</div>
    <div class="timer" id="timerBox">
      <span class="icon">⏱️</span>
      <span id="timerText">20:00</span>
    </div>
  </div>
  <div class="chapter-line">
    <span>CHAPTER-1</span>
    <span class="gold">प्रागैतिहासिक काल</span>
  </div>
</header>

<!-- ================= MAIN ================= -->
<main class="main">

  <div class="progress-wrap">
    <div class="progress-bar" id="progressBar"></div>
  </div>

  <section class="q-card" id="quizCard">
    <div class="q-meta">
      <span class="q-tag" id="qTag">Direct Fact Based</span>
      <span class="q-counter" id="qCounter">प्रश्न 1 / 20</span>
    </div>

    <div class="q-head">
      <div class="q-num" id="qNum">1</div>
      <div class="q-text" id="qText"></div>
    </div>

    <div class="options" id="optionsBox"></div>

    <div class="explain" id="explainBox"></div>

    <div class="next-wrap">
      <button class="next-btn" id="nextBtn">अगला प्रश्न →</button>
    </div>
  </section>

  <section class="result-section" id="resultSection">
    <div class="dashboard">
      <div class="dash-title">🎯 परिणाम डैशबोर्ड</div>
      <div class="dash-sub">आपका प्रदर्शन — GK GS MASTI</div>

      <div class="circle-wrap">
        <svg viewBox="0 0 160 160">
          <defs>
            <linearGradient id="gradCircle" x1="0%" y1="0%" x2="100%" y2="100%">
              <stop offset="0%" stop-color="#06b6d4"/>
              <stop offset="50%" stop-color="#7c3aed"/>
              <stop offset="100%" stop-color="#ec4899"/>
            </linearGradient>
          </defs>
          <circle class="circle-bg" cx="80" cy="80" r="70"/>
          <circle class="circle-fg" id="circleFg" cx="80" cy="80" r="70"/>
        </svg>
        <div class="circle-inner">
          <div class="circle-pct" id="pctText">0%</div>
          <div class="circle-lbl">SCORE</div>
        </div>
      </div>

      <div class="stats">
        <div class="stat total">
          <div class="num" id="statTotal">20</div>
          <div class="lbl">कुल प्रश्न</div>
        </div>
        <div class="stat ok">
          <div class="num" id="statOk">0</div>
          <div class="lbl">सही</div>
        </div>
        <div class="stat bad">
          <div class="num" id="statBad">0</div>
          <div class="lbl">गलत</div>
        </div>
      </div>

      <div class="dash-msg" id="dashMsg">शानदार प्रयास!</div>

      <div class="dash-actions">
        <button class="btn btn-gold" onclick="restartQuiz()">🔄 फिर से खेलें</button>
      </div>
    </div>
  </section>

</main>

<footer>© GK GS MASTI — Practice Quiz • All the Best!</footer>

<script>
/* ================= QUESTION DATA ================= */
const QUESTIONS = [
  {
    tag: "Direct Fact Based",
    q: "भारतीय पुरातत्व सर्वेक्षण (Archaeological Survey of India) की स्थापना किस वर्ष की गई थी और इसके जनक किसे माना जाता है?",
    options: ["1857; जेम्स प्रिंसेप", "1861; सर अलेक्जेंडर कनिंघम", "1904; लॉर्ड कर्जन", "1921; जॉन मार्शल"],
    correct: 1,
    explain: "भारतीय पुरातत्व सर्वेक्षण की स्थापना 1861 ई. में की गई थी और सर अलेक्जेंडर कनिंघम को भारतीय पुरातत्व का जनक कहा जाता है।"
  },
  {
    tag: "Concept Based",
    q: "इतिहास के काल-विभाजन के अंतर्गत 'आद्य-ऐतिहासिक काल' (Protohistoric Age) की सबसे प्रमुख विशेषता निम्नलिखित में से कौन-सी है?",
    options: [
      "इस काल के केवल पुरातात्विक साक्ष्य उपलब्ध हैं, लिखित साक्ष्य बिल्कुल नहीं हैं।",
      "इस काल के लिखित साक्ष्य उपलब्ध हैं परंतु उन्हें अभी तक पढ़ा नहीं जा सका है।",
      "इस काल के लिखित साक्ष्य उपलब्ध हैं और उन्हें पढ़ भी लिया गया है।",
      "इस काल में केवल लोहे का प्रयोग होता था।"
    ],
    correct: 1,
    explain: "आद्य-ऐतिहासिक काल (जैसे सिंधु घाटी सभ्यता) में लिखित साक्ष्य और पुरातात्विक साक्ष्य दोनों उपलब्ध हैं, परंतु उसकी लिपि को अभी तक पढ़ा नहीं जा सका है।"
  },
  {
    tag: "Statement & Assumption",
    q: "<b>कथन:</b> पाषाण काल के अंतर्गत 'नवपाषाण काल' (Neolithic Age) को मानव समाज के इतिहास में एक क्रांतिकारी युग माना जाता है, जिसमें स्थायी जीवन और समाज का निर्माण हुआ।<br><br><b>मान्यता:</b> नवपाषाण काल में ही मानव ने खेती करना, पशुपालन और आग का नियमित प्रयोग सीख लिया था जिससे उसका घुमक्कड़ जीवन समाप्त हो गया।",
    options: [
      "केवल मान्यता सही है और वह कथन की सही व्याख्या करती है।",
      "मान्यता गलत है लेकिन कथन सही है।",
      "कथन और मान्यता दोनों गलत हैं।",
      "कथन सही है लेकिन मान्यता उसका खंडन करती है।"
    ],
    correct: 0,
    explain: "नवपाषाण काल में मानव ने खेती करना और पशुपालन शुरू किया था, जिससे स्थायी जीवन की शुरुआत हुई और समाज का निर्माण हुआ।"
  },
  {
    tag: "Statement & Conclusion",
    q: "<b>कथन:</b> जीवाश्म (सजीव वस्तु) की आयु की जांच करने के लिए कार्बन डेटिंग (C-14) विधि का प्रयोग किया जाता है, जबकि चट्टान और पृथ्वी जैसी निर्जीव वस्तुओं की आयु U-238 (यूरेनियम डेटिंग) विधि से पता की जाती है।<br><br><b>निष्कर्ष I:</b> C-14 विधि का प्रयोग पुरातात्विक अवशेषों और पाषाणिक मानव के काल-निर्धारण में मुख्य रूप से होता है।<br><b>निष्कर्ष II:</b> U-238 विधि का प्रयोग केवल सजीव पेड़-पौधों की उम्र जानने के लिए किया जाता है।",
    options: [
      "केवल निष्कर्ष I सही है।",
      "केवल निष्कर्ष II सही है।",
      "निष्कर्ष I और II दोनों सही हैं।",
      "न तो I और न ही II सही है।"
    ],
    correct: 0,
    explain: "निष्कर्ष I सही है क्योंकि C-14 सजीव/जीवाश्म की आयु के लिए है। निष्कर्ष II गलत है क्योंकि U-238 निर्जीव (चट्टान, पृथ्वी) वस्तुओं के लिए है।"
  },
  {
    tag: "Assertion & Reason",
    q: "<b>अभिकथन (A):</b> भारत में पुरापाषाणकालीन औजारों की खोज सर्वप्रथम 1863 ई. में रॉबर्ट ब्रूस फूट द्वारा पल्लवरम (तमिलनाडु) में की गई थी।<br><br><b>कारण (R):</b> रॉबर्ट ब्रूस फूट भारतीय भूगर्भ सर्वेक्षण (Geological Survey of India) के एक प्रसिद्ध पुरातत्वविद और भूगर्भ शास्त्री थे।",
    options: [
      "(A) और (R) दोनों सही हैं तथा (R), (A) की सही व्याख्या है।",
      "(A) और (R) दोनों सही हैं लेकिन (R), (A) की सही व्याख्या नहीं है।",
      "(A) सही है लेकिन (R) गलत है।",
      "(A) गलत है लेकिन (R) सही है।"
    ],
    correct: 0,
    explain: "1863 में रॉबर्ट ब्रूस फूट ने तमिलनाडु के पल्लवरम से पुरापाषाणकालीन औजार खोजे थे और वे इस क्षेत्र के मुख्य शास्त्री थे।"
  },
  {
    tag: "Match the Following",
    q: "सूची-I (पाषाण काल के स्थल) को सूची-II (राज्य/क्षेत्र) के साथ सुमेलित कीजिए:<br>1. भीमबेटका<br>2. चिरंद<br>3. बुर्जहोम<br>4. मेहरगढ़<br><br>a. कश्मीर &nbsp;|&nbsp; b. मध्य प्रदेश &nbsp;|&nbsp; c. बिहार (सारण) &nbsp;|&nbsp; d. बलूचिस्तान (पाकिस्तान)",
    options: [
      "1-b, 2-c, 3-a, 4-d",
      "1-a, 2-b, 3-c, 4-d",
      "1-d, 2-c, 3-b, 4-a",
      "1-b, 2-a, 3-d, 4-c"
    ],
    correct: 0,
    explain: "भीमबेटका मध्य प्रदेश में है; चिरंद सारण (बिहार) में है; बुर्जहोम कश्मीर में है; और मेहरगढ़ बलूचिस्तान (पाकिस्तान) में स्थित नवपाषाणिक स्थल है।"
  },
  {
    tag: "Passage Based",
    q: "<i>\"यह स्थल मध्य प्रदेश की नर्मदा नदी घाटी में स्थित है, जहां से प्राचीन शैल-आश्रय (Rock Shelters) प्राप्त हुए हैं। इसकी खोज 1957-58 में डॉ. विष्णु श्रीधर वाकणकर द्वारा की गई थी और इसके महत्व को देखते हुए UNESCO ने 2003 में इसे विश्व धरोहर स्थल घोषित किया।\"</i><br><br>उपरोक्त गद्यांश किस ऐतिहासिक स्थल को इंगित करता है?",
    options: ["मेहरगढ़", "भीमबेटका", "इनामगांव", "कोलदहवा"],
    correct: 1,
    explain: "भीमबेटका (मध्य प्रदेश) की खोज विष्णु श्रीधर वाकणकर ने की थी और इसे 2003 में UNESCO विश्व धरोहर स्थल बनाया गया।"
  },
  {
    tag: "Exam Level Tricky",
    q: "निम्नलिखित में से किस स्थल से 'चावल का प्राचीनतम साक्ष्य' और किस स्थल से 'मानव के साथ कुत्ते को दफनाने के साक्ष्य' प्राप्त हुए हैं?",
    options: [
      "कोलदहवा और बुर्जहोम",
      "चिरंद और मेहरगढ़",
      "इनामगांव और भीमबेटका",
      "बागोर और आमगढ़"
    ],
    correct: 0,
    explain: "उत्तर प्रदेश के कोलदहवा से चावल का प्राचीनतम साक्ष्य और कश्मीर के बुर्जहोम से मानव के साथ कुत्ते को दफनाने के साक्ष्य मिलते हैं।"
  },
  {
    tag: "Correct / Incorrect Statement",
    q: "पाषाण काल और उसके तत्वों के संदर्भ में निम्नलिखित कथनों पर विचार कीजिए:<br><br>1. पुरापाषाण काल में मानव बड़े पत्थर के औजारों (Macrolithic) का प्रयोग करता था और खानाबदोश जीवन व्यतीत करता था।<br>2. मध्यपाषाण काल में छोटे पत्थर के औजारों (Microlithic) का प्रयोग होने लगा और आग का उपयोग करना सीखा गया।<br>3. ताम्र-पाषाण काल की सबसे बड़ी बस्ती इनामगांव (महाराष्ट्र) थी।<br>4. मानव द्वारा खोजी गई पहली धातु 'लोहा' थी।<br><br>उपर्युक्त में से कौन-सा/से कथन असत्य (Incorrect) है/हैं?",
    options: ["केवल 4", "1 और 2", "3 और 4", "कोई भी असत्य नहीं है"],
    correct: 0,
    explain: "कथन 4 असत्य है क्योंकि मानव द्वारा खोजी गई पहली धातु 'तांबा' थी, लोहा नहीं। बाकी तीनों कथन बिल्कुल सत्य हैं।"
  },
  {
    tag: "Application Based",
    q: "यदि आप एक पुरातत्वविद् हैं और आपको किसी उत्खनन में तांबा और पत्थर के औजार एक साथ मिलते हैं, साथ ही पहिये की खोज के प्रमाण और सबसे बड़ी बस्ती 'इनामगांव' के अवशेष मिलते हैं, तो आप इसे किस काल के अंतर्गत रखेंगे?",
    options: ["पुरापाषाण काल", "मध्यपाषाण काल", "नवपाषाण काल", "ताम्र-पाषाण काल (Chalcolithic Age)"],
    correct: 3,
    explain: "तांबा और पत्थर का संयुक्त प्रयोग, पहिये की खोज और इनामगांव (महाराष्ट्र) ताम्र-पाषाण काल की मुख्य विशेषताएं हैं।"
  },
  {
    tag: "Direct Fact Based",
    q: "वायसराय लॉर्ड कर्जन के प्रयासों से 'पुरातात्विक विभाग' की स्थापना किस वर्ष की गई थी?",
    options: ["1861", "1904", "1921", "1935"],
    correct: 1,
    explain: "पुरातात्विक विभाग की स्थापना 1904 में वायसराय लॉर्ड कर्जन के प्रयास से की गई थी।"
  },
  {
    tag: "Concept Based",
    q: "मानव उत्पत्ति और ज्ञात मानव के संदर्भ में सबसे पहले मानव की उत्पत्ति किस महाद्वीप में मानी गई है?",
    options: ["एशिया", "अफ्रीका", "यूरोप", "ऑस्ट्रेलिया"],
    correct: 1,
    explain: "मानव की उत्पत्ति सर्वप्रथम अफ्रीका महाद्वीप में हुई थी।"
  },
  {
    tag: "Statement & Assumption",
    q: "<b>कथन:</b> प्राचीन इतिहास के अध्ययन के लिए हेरोडोटस को 'इतिहास का जनक' (Father of History) कहा जाता है और इनकी प्रसिद्ध पुस्तक का नाम 'हिस्ट्रीज़' है।<br><br><b>मान्यता:</b> हेरोडोटस की पुस्तक में पहली बार ऐतिहासिक घटनाओं का क्रमबद्ध विवरण मिलता है जिसने इतिहास लेखन की नींव रखी।",
    options: [
      "कथन और मान्यता दोनों सही हैं तथा मान्यता कथन की सही व्याख्या है।",
      "कथन सही है लेकिन मान्यता गलत है।",
      "दोनों गलत हैं।",
      "मान्यता गलत है लेकिन कथन सही है।"
    ],
    correct: 0,
    explain: "हेरोडोटस को इतिहास का जनक कहा जाता है और उनकी पुस्तक का नाम 'हिस्ट्रीज़' है।"
  },
  {
    tag: "Statement & Conclusion",
    q: "<b>कथन:</b> मानव द्वारा पालतू बनाया गया पहला जानवर कुत्ता था और उसे सबसे पहले प्रयोग में लाया गया औजार 'कुल्हाड़ी' था।<br><br><b>निष्कर्ष I:</b> शिकार करने और वनों को साफ करने के लिए कुल्हाड़ी मानव का सबसे पहला महत्वपूर्ण हथियार बनी।<br><b>निष्कर्ष II:</b> कुत्ता मानव का पहला पालतू जानवर होने के कारण शिकार में सहायक बना।",
    options: [
      "केवल निष्कर्ष I सही है।",
      "केवल निष्कर्ष II सही है।",
      "निष्कर्ष I और II दोनों सही हैं।",
      "न तो I और न ही II सही है।"
    ],
    correct: 2,
    explain: "पहला पालतू जानवर कुत्ता और पहला औजार कुल्हाड़ी था, जिससे दोनों निष्कर्ष तथ्यात्मक रूप से सही हैं।"
  },
  {
    tag: "Assertion & Reason",
    q: "<b>अभिकथन (A):</b> प्राचीन संग्रहालयों में 'भारतीय पुरातात्विक संग्रहालय कोलकाता' को भारत का सबसे पुराना संग्रहालय माना जाता है।<br><br><b>कारण (R):</b> इसके अतिरिक्त राष्ट्रीय संग्रहालय दिल्ली में भी पुरातात्विक महत्व की वस्तुएं सुरक्षित रखी गई हैं।",
    options: [
      "(A) और (R) दोनों सही हैं तथा (R), (A) की सही व्याख्या नहीं है।",
      "(A) और (R) दोनों सही हैं तथा (R), (A) की सही व्याख्या है।",
      "(A) सही है लेकिन (R) गलत है।",
      "(A) गलत है लेकिन (R) सही है।"
    ],
    correct: 0,
    explain: "दोनों कथन सत्य हैं कि कोलकाता संग्रहालय सबसे पुराना है और दिल्ली में राष्ट्रीय संग्रहालय है, परंतु कारण (R) अभिकथन (A) की सीधी व्याख्या नहीं करता।"
  },
  {
    tag: "Match the Following",
    q: "सूची-I (पाषाण काल के स्थल) को सूची-II (संबंधित राज्य) के साथ सुमेलित कीजिए:<br>1. आमगढ़<br>2. बागोर<br>3. मेहरगढ़<br>4. कोलदहवा<br><br>a. मध्य प्रदेश &nbsp;|&nbsp; b. राजस्थान &nbsp;|&nbsp; c. बलूचिस्तान &nbsp;|&nbsp; d. उत्तर प्रदेश",
    options: [
      "1-a, 2-b, 3-c, 4-d",
      "1-b, 2-a, 3-d, 4-c",
      "1-c, 2-d, 3-a, 4-b",
      "1-d, 2-c, 3-b, 4-a"
    ],
    correct: 0,
    explain: "आमगढ़ (म.प्र.), बागोर (राजस्थान), मेहरगढ़ (बलूचिस्तान) और कोलदहवा (उ.प्र.) का सटीक मिलान यही है।"
  },
  {
    tag: "Passage Based",
    q: "<i>\"इस काल में मानव ने छोटे, चमकदार और नुकीले पत्थर के औजारों की खोज की थी। इस दौरान खेती करना और पशुपालन (जैसे कुत्ता) शुरू हुआ, जिससे घुमक्कड़ जीवन छोड़कर स्थायी रूप से रहना और समाज का निर्माण करना प्रारंभ हो गया था।\"</i><br><br>यह गद्यांश किस काल को दर्शाता है?",
    options: ["पुरापाषाण काल", "मध्यपाषाण काल", "नवपाषाण काल", "ताम्र-पाषाण काल"],
    correct: 2,
    explain: "छोटे-नुकीले चमकदार औजार, खेती और स्थायी जीवन की शुरुआत नवपाषाण काल की मुख्य पहचान है।"
  },
  {
    tag: "Exam Level Tricky",
    q: "ज्ञात मानव (Homo sapiens) का उदय कब माना जाता है?",
    options: ["5 हजार BC", "10 हजार BC", "25 हजार BC", "50 हजार BC"],
    correct: 2,
    explain: "ज्ञात मानव (Homo sapiens) का काल 25 हजार BC माना गया है।"
  },
  {
    tag: "Correct / Incorrect Statement",
    q: "इतिहास के स्रोत और काल-विभाजन के संदर्भ में निम्नलिखित कथनों पर विचार कीजिए:<br><br>1. प्रागैतिहासिक काल में लिखित साक्ष्य उपलब्ध नहीं थे, केवल पुरातात्विक साक्ष्य उपलब्ध थे।<br>2. आद्य-ऐतिहासिक काल में लिखित साक्ष्य उपलब्ध थे पर उन्हें पढ़ा नहीं गया।<br>3. ऐतिहासिक काल में लिखित और पुरातात्विक दोनों साक्ष्य उपलब्ध हैं और उन्हें पढ़ा भी गया है।<br><br>उपर्युक्त में से कौन-सा/से कथन सत्य है/हैं?",
    options: ["केवल 1 और 2", "केवल 2 और 3", "केवल 1 और 3", "1, 2 और 3 सभी"],
    correct: 3,
    explain: "तीनों कथन इतिहास के काल-विभाजन के नियम के अनुसार बिल्कुल सत्य हैं।"
  },
  {
    tag: "Application Based",
    q: "यदि आपको एग्जाम में प्रश्न मिले कि मानव द्वारा सबसे पहले उगाई गई फसलें कौन-सी थीं, तो आपका उत्तर क्या होगा?",
    options: ["गेहूं, जौ और चावल", "मक्का और चना", "बाजरा और ज्वार", "गन्ना और कपास"],
    correct: 0,
    explain: "मानव द्वारा प्रयोग की गई पहली फसलें गेहूं, जौ और चावल थीं।"
  }
];

const KEYS = ["A", "B", "C", "D"];
const TOTAL_TIME = 20 * 60; // 20 minutes

/* ================= STATE ================= */
let currentIndex = 0;
let score = 0;
let wrongCount = 0;
let answeredCurrent = false;
let timeLeft = TOTAL_TIME;
let timerInterval = null;
let quizFinished = false;

/* ================= ELEMENTS ================= */
const el = (id) => document.getElementById(id);
const timerBox = el("timerBox");
const timerText = el("timerText");
const progressBar = el("progressBar");
const quizCard = el("quizCard");
const qTag = el("qTag");
const qCounter = el("qCounter");
const qNum = el("qNum");
const qText = el("qText");
const optionsBox = el("optionsBox");
const explainBox = el("explainBox");
const nextBtn = el("nextBtn");
const resultSection = el("resultSection");

/* ================= TIMER ================= */
function startTimer() {
  clearInterval(timerInterval);
  updateTimerDisplay();
  timerInterval = setInterval(() => {
    timeLeft--;
    updateTimerDisplay();
    if (timeLeft <= 0) {
      clearInterval(timerInterval);
      finishQuiz(true);
    }
  }, 1000);
}

function updateTimerDisplay() {
  const m = Math.floor(Math.max(timeLeft, 0) / 60);
  const s = Math.max(timeLeft, 0) % 60;
  timerText.textContent = `${String(m).padStart(2, "0")}:${String(s).padStart(2, "0")}`;
  if (timeLeft <= 120) {
    timerBox.classList.add("warning");
  } else {
    timerBox.classList.remove("warning");
  }
}

/* ================= RENDER ================= */
function renderQuestion() {
  if (currentIndex >= QUESTIONS.length) {
    finishQuiz(false);
    return;
  }

  answeredCurrent = false;
  const item = QUESTIONS[currentIndex];

  qTag.textContent = item.tag;
  qCounter.textContent = `प्रश्न ${currentIndex + 1} / ${QUESTIONS.length}`;
  qNum.textContent = currentIndex + 1;
  qText.innerHTML = item.q;

  optionsBox.innerHTML = "";
  item.options.forEach((optText, oi) => {
    const btn = document.createElement("button");
    btn.className = "opt";
    btn.type = "button";

    const key = document.createElement("span");
    key.className = "key";
    key.textContent = KEYS[oi];

    const span = document.createElement("span");
    span.className = "opt-text";
    span.innerHTML = optText;

    const mark = document.createElement("span");
    mark.className = "mark";

    btn.appendChild(key);
    btn.appendChild(span);
    btn.appendChild(mark);

    btn.addEventListener("click", () => selectAnswer(oi));
    optionsBox.appendChild(btn);
  });

  explainBox.classList.remove("show");
  explainBox.innerHTML = "";
  nextBtn.classList.remove("show", "gold");
  nextBtn.textContent = "अगला प्रश्न →";

  const pct = (currentIndex / QUESTIONS.length) * 100;
  progressBar.style.width = pct + "%";

  quizCard.style.animation = "none";
  void quizCard.offsetWidth;
  quizCard.style.animation = "cardIn .55s cubic-bezier(.2,.9,.3,1.2) both";
}

/* ================= SELECT ================= */
function selectAnswer(choiceIndex) {
  if (answeredCurrent) return;
  answeredCurrent = true;

  const item = QUESTIONS[currentIndex];
  const allOpts = optionsBox.querySelectorAll(".opt");

  allOpts.forEach((o, i) => {
    o.classList.add("locked");
    if (i === item.correct) {
      o.classList.add("correct");
      o.querySelector(".mark").textContent = "✔";
    }
  });

  if (choiceIndex === item.correct) {
    score++;
    spawnHearts();
  } else {
    allOpts[choiceIndex].classList.add("wrong");
    allOpts[choiceIndex].querySelector(".mark").textContent = "✘";
    wrongCount++;
  }

  explainBox.innerHTML = `
    <span class="ans-line">✅ सही उत्तर: (${KEYS[item.correct]}) ${item.options[item.correct]}</span>
    <span class="lbl">विवरण:</span>${item.explain}
  `;
  setTimeout(() => explainBox.classList.add("show"), 250);

  setTimeout(() => {
    nextBtn.classList.add("show");
    if (currentIndex === QUESTIONS.length - 1) {
      nextBtn.textContent = "🎯 परिणाम देखें";
      nextBtn.classList.add("gold");
    }
    const pct = ((currentIndex + 1) / QUESTIONS.length) * 100;
    progressBar.style.width = pct + "%";
  }, 400);
}

/* ================= NEXT ================= */
nextBtn.addEventListener("click", () => {
  if (currentIndex === QUESTIONS.length - 1) {
    finishQuiz(false);
  } else {
    currentIndex++;
    renderQuestion();
    window.scrollTo({ top: 0, behavior: "smooth" });
  }
});

/* ================= HEART BALLOONS ================= */
function spawnHearts() {
  const hearts = ["❤️", "💖", "💕", "💗", "💓", "🩷", "💝"];
  for (let i = 0; i < 12; i++) {
    setTimeout(() => {
      const b = document.createElement("div");
      b.className = "balloon";
      b.textContent = hearts[Math.floor(Math.random() * hearts.length)];
      b.style.left = (5 + Math.random() * 90) + "vw";
      b.style.fontSize = (28 + Math.random() * 26) + "px";
      b.style.animationDuration = (2.8 + Math.random() * 1.6) + "s";
      document.body.appendChild(b);
      setTimeout(() => b.remove(), 5000);
    }, i * 90);
  }
}

/* ================= CONFETTI ================= */
function spawnConfetti() {
  const colors = ["#06b6d4", "#7c3aed", "#ec4899", "#10b981", "#fbbf24", "#ef4444"];
  for (let i = 0; i < 70; i++) {
    const c = document.createElement("div");
    c.className = "confetti";
    c.style.left = Math.random() * 100 + "vw";
    c.style.top = "-20px";
    c.style.background = colors[Math.floor(Math.random() * colors.length)];
    c.style.animationDuration = (2.5 + Math.random() * 2) + "s";
    c.style.animationDelay = (Math.random() * 0.6) + "s";
    c.style.borderRadius = Math.random() > 0.5 ? "50%" : "2px";
    document.body.appendChild(c);
    setTimeout(() => c.remove(), 5200);
  }
}

/* ================= FINISH ================= */
function finishQuiz(timeUp) {
  if (quizFinished) return;
  quizFinished = true;
  clearInterval(timerInterval);

  quizCard.style.display = "none";
  progressBar.parentElement.style.display = "none";

  const total = QUESTIONS.length;
  const correct = score;
  const wrong = wrongCount;
  const unanswered = total - correct - wrong;
  const finalWrong = wrong + unanswered;
  const percentage = Math.round((correct / total) * 100);

  el("statTotal").textContent = total;
  el("statOk").textContent = correct;
  el("statBad").textContent = finalWrong;
  el("pctText").textContent = percentage + "%";

  const circle = el("circleFg");
  const radius = 70;
  const circumference = 2 * Math.PI * radius;
  const offset = circumference - (percentage / 100) * circumference;
  circle.style.strokeDasharray = circumference;
  circle.style.strokeDashoffset = circumference;
  setTimeout(() => {
    circle.style.strokeDashoffset = offset;
  }, 300);

  const msg = el("dashMsg");
  msg.textContent = timeUp ? "⏰ समय समाप्त! " + getMessage(percentage) : getMessage(percentage);

  resultSection.classList.add("show");
  window.scrollTo({ top: 0, behavior: "smooth" });

  if (percentage >= 60) {
    setTimeout(spawnConfetti, 500);
    setTimeout(spawnConfetti, 1500);
  }
  if (percentage >= 80) {
    setTimeout(spawnHearts, 800);
    setTimeout(spawnHearts, 1800);
  }
}

function getMessage(pct) {
  if (pct >= 90) return "🏆 शानदार! आप तो टॉपर हैं!";
  if (pct >= 75) return "🌟 बहुत बढ़िया! शानदार प्रदर्शन!";
  if (pct >= 60) return "👍 अच्छा प्रयास! थोड़ी और मेहनत करें।";
  if (pct >= 40) return "📚 ठीक है, लेकिन अभ्यास की जरूरत है।";
  if (pct >= 20) return "💪 चिंता न करें, रिवीजन करें और फिर प्रयास करें।";
  return "🙂 कोई बात नहीं! अभ्यास से सब होगा। फिर कोशिश करें।";
}

/* ================= RESTART ================= */
function restartQuiz() {
  currentIndex = 0;
  score = 0;
  wrongCount = 0;
  answeredCurrent = false;
  quizFinished = false;
  timeLeft = TOTAL_TIME;

  resultSection.classList.remove("show");
  quizCard.style.display = "";
  progressBar.parentElement.style.display = "";
  progressBar.style.width = "0%";
  timerBox.classList.remove("warning");
  el("circleFg").style.strokeDashoffset = 440;

  renderQuestion();
  startTimer();
  window.scrollTo({ top: 0, behavior: "smooth" });
}

/* ================= INIT ================= */
function init() {
  renderQuestion();
  startTimer();
}
init();
</script>
</body>
</html>
