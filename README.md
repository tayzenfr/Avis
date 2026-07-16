<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Ton avis — TAYZEN</title>
<meta name="description" content="Laisse ton avis sur ta commande de montage TAYZEN.">
<meta name="robots" content="noindex">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{
  --bg0:#04060f; --bg1:#080b1c;
  --text:#eef2ff; --muted:rgba(238,242,255,.72);
  --accent:#ff1e3c; --accent2:#ff5c7a;
  --ease:cubic-bezier(.22,.9,.24,1);
  --spring:cubic-bezier(.34,1.56,.5,1);
  --font-display:"Space Grotesk", system-ui, sans-serif;
  --font-body:"Inter", system-ui, sans-serif;
}
*{ box-sizing:border-box; margin:0; padding:0; }
body{
  font-family:var(--font-body); color:var(--text);
  background: linear-gradient(180deg, var(--bg0), var(--bg1));
  min-height:100vh; overflow-x:hidden;
}

/* Fond liquide */
.aurora{ position:fixed; inset:-20%; z-index:-2; pointer-events:none; filter:blur(70px) saturate(130%); }
.aurora span{ position:absolute; border-radius:50%; opacity:.55; will-change:transform; }
.aurora .b1{ width:52vw; height:52vw; left:-8%; top:-6%; background:radial-gradient(circle at 35% 35%, rgba(255,30,60,.5), transparent 62%); animation:drift1 26s ease-in-out infinite alternate; }
.aurora .b2{ width:50vw; height:50vw; right:-8%; bottom:-12%; background:radial-gradient(circle at 50% 50%, rgba(91,43,214,.4), transparent 62%); animation:drift2 32s ease-in-out infinite alternate; }
@keyframes drift1{ to{ transform:translate3d(8vw,6vh,0) scale(1.12); } }
@keyframes drift2{ to{ transform:translate3d(-7vw,-8vh,0) scale(.94); } }
body::before{
  content:""; position:fixed; inset:0; z-index:-1; pointer-events:none; opacity:.05;
  background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='240' height='240'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='240' height='240' filter='url(%23n)' opacity='.35'/%3E%3C/svg%3E");
  mix-blend-mode:overlay;
}

.wrap{ width:min(660px, calc(100% - 32px)); margin:0 auto; padding:38px 0 60px; }
.brand{ display:flex; align-items:center; gap:10px; justify-content:center; margin-bottom:24px; }
.brandMark{
  width:34px; height:34px;
  background:linear-gradient(135deg, var(--accent), var(--accent2));
  border:1px solid rgba(255,255,255,.22);
  box-shadow:0 10px 30px rgba(255,30,60,.3), inset 0 1px 0 rgba(255,255,255,.4);
  border-radius:46% 54% 58% 42% / 48% 42% 58% 52%;
  animation:morph 9s ease-in-out infinite;
}
@keyframes morph{
  0%,100%{ border-radius:46% 54% 58% 42% / 48% 42% 58% 52%; }
  33%{ border-radius:58% 42% 44% 56% / 42% 58% 42% 58%; }
  66%{ border-radius:42% 58% 56% 44% / 56% 44% 56% 44%; }
}
.brand strong{ font-family:var(--font-display); letter-spacing:1.5px; }

/* Carte glass */
.card{
  position:relative; overflow:hidden;
  background:
    linear-gradient(115deg, rgba(255,255,255,.12), transparent 32%),
    linear-gradient(150deg, rgba(255,255,255,.09), rgba(255,255,255,.05) 55%);
  border-radius:26px;
  box-shadow:0 24px 80px rgba(0,0,0,.55), inset 0 1.5px 0 rgba(255,255,255,.35), inset 0 -28px 56px -32px rgba(255,30,60,.2);
  backdrop-filter:blur(28px) saturate(180%);
  -webkit-backdrop-filter:blur(28px) saturate(180%);
  padding:30px 28px;
}
.card::before{
  content:""; position:absolute; inset:0; border-radius:inherit; padding:1px;
  background:linear-gradient(150deg, rgba(255,255,255,.6), rgba(255,255,255,.08) 40%, rgba(255,30,60,.35) 80%, rgba(255,92,122,.5));
  -webkit-mask:linear-gradient(#000 0 0) content-box, linear-gradient(#000 0 0);
  -webkit-mask-composite:xor; mask-composite:exclude;
  pointer-events:none;
}

h1{ font-family:var(--font-display); font-size:25px; letter-spacing:-.5px; margin-bottom:6px; }
.sub{ color:var(--muted); font-size:13.5px; margin-bottom:22px; line-height:1.5; }
.sub b{ color:#7CFFB2; }

form{ display:grid; gap:16px; }
label{ font-size:13px; color:rgba(238,242,255,.78); display:block; margin-bottom:6px; }
input, textarea{
  width:100%; padding:13px 14px; border-radius:13px;
  border:1px solid rgba(255,255,255,.10);
  background:rgba(255,255,255,.04);
  box-shadow:inset 0 1px 0 rgba(255,255,255,.05);
  color:var(--text); font-size:15px; outline:none; font-family:var(--font-body);
  transition:border-color .2s var(--ease), box-shadow .2s var(--ease);
}
textarea{ min-height:80px; resize:vertical; }
input:focus, textarea:focus{
  border-color:rgba(255,30,60,.55);
  box-shadow:0 0 0 4px rgba(255,30,60,.12), inset 0 1px 0 rgba(255,255,255,.08);
}
.groupTitle{
  font-size:11.5px; font-weight:700; letter-spacing:.14em; text-transform:uppercase;
  color:rgba(238,242,255,.5);
  padding-bottom:8px; margin-top:6px;
  border-bottom:1px solid rgba(255,255,255,.08);
}
.twoCols{ display:grid; grid-template-columns:1fr 1fr; gap:12px; }
@media (max-width:560px){ .twoCols{ grid-template-columns:1fr; } }

/* Chips type de vidéo (DA du site, fini le select blanc) */
.chips{ display:flex; flex-wrap:wrap; gap:8px; }
.chips button{
  padding:10px 15px; border-radius:999px;
  border:1px solid rgba(255,255,255,.14);
  background:rgba(255,255,255,.05);
  color:var(--muted); font-size:13.5px; font-weight:600;
  font-family:var(--font-body); cursor:pointer;
  transition:transform .2s var(--spring), background .2s var(--ease), border-color .2s var(--ease), color .2s var(--ease);
}
.chips button:hover{ transform:translateY(-2px); background:rgba(255,255,255,.09); color:#fff; }
.chips button.on{
  color:#fff;
  background:linear-gradient(135deg, var(--accent), var(--accent2));
  border-color:rgba(255,255,255,.3);
  box-shadow:0 10px 26px rgba(255,30,60,.3), inset 0 1px 0 rgba(255,255,255,.35);
}

/* Étoiles */
.starRow{ display:flex; align-items:center; justify-content:space-between; gap:12px; flex-wrap:wrap; }
.starRow label{ margin:0; }
.stars{ display:flex; gap:3px; }
.stars button{
  background:none; border:none; cursor:pointer;
  font-size:25px; line-height:1;
  color:rgba(255,255,255,.18);
  transition:transform .2s var(--spring), color .12s var(--ease), text-shadow .2s var(--ease);
  padding:2px;
}
.stars button.on{ color:#FFD166; text-shadow:0 0 14px rgba(255,209,102,.55); }
.stars button:hover{ transform:scale(1.3) rotate(8deg); }
.stars button.bump{ animation:starBump .35s var(--spring); }
@keyframes starBump{ 50%{ transform:scale(1.45) rotate(-8deg); } }

/* Consentement */
.check{
  display:flex; gap:12px; align-items:flex-start;
  padding:13px 14px; border-radius:13px;
  border:1px solid rgba(255,255,255,.10);
  background:rgba(255,255,255,.04);
  cursor:pointer; font-size:13px; color:var(--muted); line-height:1.5;
  transition:border-color .2s var(--ease);
}
.check:hover{ border-color:rgba(255,255,255,.2); }
.check input{ width:17px; height:17px; margin-top:1px; accent-color:var(--accent); flex:0 0 17px; }

button.primary{
  position:relative; overflow:hidden;
  padding:15px; border-radius:14px;
  border:1px solid rgba(255,255,255,.28);
  background:linear-gradient(135deg, var(--accent), var(--accent2));
  background-size:160% 160%;
  animation:gradShift 5s ease infinite;
  color:#fff; font-weight:800; font-size:15px; cursor:pointer;
  font-family:var(--font-body);
  box-shadow:0 18px 50px rgba(255,30,60,.22), inset 0 1px 0 rgba(255,255,255,.45);
  transition:transform .22s var(--spring), box-shadow .25s var(--ease);
}
@keyframes gradShift{ 0%,100%{ background-position:0% 50%; } 50%{ background-position:100% 50%; } }
button.primary:hover{ transform:translateY(-2px); box-shadow:0 24px 70px rgba(255,30,60,.34), inset 0 1px 0 rgba(255,255,255,.5); }
button.primary:active{ transform:scale(.98); }

/* Révélations à l'arrivée */
.rv{ opacity:0; transform:translateY(18px); animation:rvIn .6s var(--ease) forwards; }
.rv:nth-child(1){ animation-delay:.05s; } .rv:nth-child(2){ animation-delay:.1s; }
.rv:nth-child(3){ animation-delay:.15s; } .rv:nth-child(4){ animation-delay:.2s; }
.rv:nth-child(5){ animation-delay:.25s; } .rv:nth-child(6){ animation-delay:.3s; }
.rv:nth-child(7){ animation-delay:.35s; } .rv:nth-child(8){ animation-delay:.4s; }
.rv:nth-child(9){ animation-delay:.45s; } .rv:nth-child(10){ animation-delay:.5s; }
.rv:nth-child(11){ animation-delay:.55s; } .rv:nth-child(12){ animation-delay:.6s; }
.rv:nth-child(13){ animation-delay:.65s; } .rv:nth-child(14){ animation-delay:.7s; }
.rv:nth-child(15){ animation-delay:.75s; } .rv:nth-child(16){ animation-delay:.8s; }
@keyframes rvIn{ to{ opacity:1; transform:translateY(0); } }

/* ---------- Écran de merci (motion design) ---------- */
.thanks{ display:none; text-align:center; padding:22px 6px; position:relative; overflow:visible; }
.confettiLayer{ position:absolute; inset:-30px; pointer-events:none; }
.confettiBit{ position:absolute; top:30%; left:50%; width:9px; height:9px; border-radius:2px; opacity:0; }
.planeFly{
  position:absolute; left:-50px; bottom:22%;
  font-size:32px; pointer-events:none; opacity:0;
  filter:drop-shadow(0 6px 14px rgba(0,0,0,.4));
  animation:planeFly 1.5s cubic-bezier(.3,.6,.4,1) .25s both;
}
@keyframes planeFly{
  0%{ opacity:0; transform:translate(0,30px) rotate(18deg) scale(.7); }
  12%{ opacity:1; }
  45%{ transform:translate(40vw,-60px) rotate(-6deg) scale(1); }
  80%{ opacity:1; }
  100%{ opacity:0; transform:translate(min(80vw,640px),-140px) rotate(-14deg) scale(.85); }
}
.checkWrap{ position:relative; width:104px; height:104px; margin:0 auto 18px; animation:popIn .55s var(--spring) both; }
.checkWrap::before, .checkWrap::after{
  content:""; position:absolute; inset:0; border-radius:50%;
  border:2px solid rgba(57,224,127,.5); opacity:0;
  animation:ringPulse 1.5s ease-out .55s 2;
}
.checkWrap::after{ animation-delay:.95s; }
@keyframes ringPulse{ 0%{ opacity:.85; transform:scale(.72); } 100%{ opacity:0; transform:scale(1.65); } }
@keyframes popIn{ 0%{ opacity:0; transform:scale(.3) rotate(-12deg); } 70%{ transform:scale(1.08) rotate(2deg); } 100%{ opacity:1; transform:scale(1) rotate(0); } }
.checkmark{
  width:100%; height:100%; display:block; border-radius:50%;
  stroke-width:3; stroke:#fff; stroke-miterlimit:10;
  filter:drop-shadow(0 0 18px rgba(57,224,127,.45));
  animation:checkFill .4s ease-in-out .4s forwards, checkScale .3s ease-in-out .9s both;
}
.checkmark-circle{
  stroke-dasharray:166; stroke-dashoffset:166; stroke:url(#checkGrad); fill:none;
  animation:checkStroke .6s cubic-bezier(.65,0,.45,1) forwards;
}
.checkmark-check{
  stroke-dasharray:48; stroke-dashoffset:48;
  animation:checkStroke .3s cubic-bezier(.65,0,.45,1) .7s forwards;
}
@keyframes checkStroke{ 100%{ stroke-dashoffset:0; } }
@keyframes checkScale{ 0%,100%{ transform:none; } 50%{ transform:scale3d(1.12,1.12,1); } }
@keyframes checkFill{ 100%{ box-shadow:inset 0 0 0 60px rgba(57,224,127,.10); } }
.thanks h2{
  font-family:var(--font-display); font-size:24px; margin-bottom:8px;
  background:linear-gradient(120deg, #7CFFB2, #39e07f 45%, #eef2ff);
  -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent;
  animation:riseIn .55s var(--spring) .75s both;
}
.thanks p{ color:var(--muted); font-size:14px; animation:riseIn .5s var(--ease) .95s both; }
.backLink{
  display:inline-block; margin-top:18px;
  padding:12px 20px; border-radius:14px;
  border:1px solid rgba(255,255,255,.28);
  background:linear-gradient(135deg, var(--accent), var(--accent2));
  color:#fff; font-weight:700; text-decoration:none; font-size:14px;
  box-shadow:0 14px 40px rgba(255,30,60,.25), inset 0 1px 0 rgba(255,255,255,.4);
  animation:riseIn .5s var(--spring) 1.15s both;
  transition:transform .22s var(--spring);
}
.backLink:hover{ transform:translateY(-2px); }
@keyframes riseIn{ from{ opacity:0; transform:translateY(22px) scale(.97); } to{ opacity:1; transform:translateY(0) scale(1); } }

footer{ text-align:center; margin-top:24px; font-size:12.5px; color:rgba(238,242,255,.45); }
footer a{ color:inherit; }
</style>
</head>
<body>

<div class="aurora" aria-hidden="true"><span class="b1"></span><span class="b2"></span></div>

<div class="wrap">
  <div class="brand"><div class="brandMark"></div><strong>TAYZEN</strong></div>

  <div class="card">
    <div id="formZone">
      <h1 class="rv" style="animation-delay:0s;">Ton avis compte ✨</h1>
      <p class="sub rv" style="animation-delay:.06s;">2 minutes — <b>ton avis sera affiché sur le site avec un lien vers ta chaîne</b> (si tu es d'accord).</p>

      <form id="avisForm" action="https://formspree.io/f/mojgjgrl" method="POST" novalidate>
        <input type="hidden" name="_subject" value="⭐ Nouvel avis client — TAYZEN">
        <input type="hidden" name="source" value="Page avis TAYZEN">
        <input type="hidden" name="type_video" id="typeVideoField" value="">

        <div class="groupTitle rv">Toi</div>

        <div class="twoCols rv">
          <div>
            <label for="pseudo">Pseudo *</label>
            <input id="pseudo" name="pseudo" type="text" placeholder="Affiché avec l'avis" required>
          </div>
          <div>
            <label for="email">Email *</label>
            <input id="email" name="email" type="email" placeholder="Pour te reconnaître" required>
          </div>
        </div>
        <div class="rv">
          <label for="chaine">Ta chaîne YouTube</label>
          <input id="chaine" name="chaine_youtube" type="url" placeholder="Lien affiché avec ton avis (optionnel)">
        </div>
        <div class="rv">
          <label>La vidéo que je t'ai montée</label>
          <div class="chips" id="typeChips">
            <button type="button">🎮 Gaming</button>
            <button type="button">📖 Storytelling</button>
            <button type="button">🎙️ Commentary</button>
            <button type="button">📹 Vlog</button>
            <button type="button">✍️ Autre</button>
          </div>
        </div>

        <div class="groupTitle rv">Tes notes</div>

        <div class="starRow rv"><label>Note globale *</label><div class="stars" data-name="note_globale"></div></div>
        <div class="starRow rv"><label>Rythme</label><div class="stars" data-name="note_rythme"></div></div>
        <div class="starRow rv"><label>Sound design</label><div class="stars" data-name="note_sound_design"></div></div>
        <div class="starRow rv"><label>Communication</label><div class="stars" data-name="note_communication"></div></div>
        <div class="starRow rv"><label>Délais</label><div class="stars" data-name="note_delais"></div></div>

        <div class="groupTitle rv">Ton retour</div>

        <div class="rv">
          <label for="avisCourt">Ton avis en une phrase * <span style="color:rgba(238,242,255,.45);">(affiché sur le site)</span></label>
          <input id="avisCourt" name="avis_affiche" type="text" maxlength="200" placeholder="Ex : Montage nickel, ma rétention a grimpé !" required>
        </div>
        <div class="twoCols rv">
          <div>
            <label for="plu">Ce qui t'a plu</label>
            <textarea id="plu" name="ce_qui_a_plu" placeholder="Rythme, sound design…"></textarea>
          </div>
          <div>
            <label for="ameliorer">À améliorer</label>
            <textarea id="ameliorer" name="a_ameliorer" placeholder="Sois cash 💪"></textarea>
          </div>
        </div>
        <div class="rv">
          <label>Tu me recommanderais ?</label>
          <div class="chips" id="recoChips">
            <button type="button" class="on">Oui, carrément</button>
            <button type="button">Peut-être</button>
            <button type="button">Non</button>
          </div>
          <input type="hidden" name="recommande" id="recoField" value="Oui, carrément">
        </div>

        <label class="check rv">
          <input type="checkbox" id="consent" required>
          <span>J'autorise l'affichage de mon pseudo, ma note, ma phrase et ma chaîne sur le site. *</span>
        </label>
        <input type="hidden" name="autorisation_affichage" id="consentField" value="Non">

        <div class="rv">
          <button class="primary" type="submit" style="width:100%;">Envoyer mon avis ⭐</button>
        </div>
      </form>
    </div>

    <div class="thanks" id="thanks">
      <div class="confettiLayer" aria-hidden="true"></div>
      <div class="planeFly" aria-hidden="true">✈️</div>
      <div class="checkWrap">
        <svg class="checkmark" viewBox="0 0 52 52" aria-hidden="true">
          <defs>
            <linearGradient id="checkGrad" x1="0%" y1="0%" x2="100%" y2="100%">
              <stop offset="0%" stop-color="#7CFFB2"/>
              <stop offset="100%" stop-color="#39e07f"/>
            </linearGradient>
          </defs>
          <circle class="checkmark-circle" cx="26" cy="26" r="25" fill="none"/>
          <path class="checkmark-check" fill="none" d="M14.1 27.2l7.1 7.2 16.7-16.8"/>
        </svg>
      </div>
      <h2>Merci énormément ! 🙏</h2>
      <p>Ton avis est envoyé — il apparaîtra bientôt sur le site avec ta chaîne.</p>
      <a class="backLink" href="index.html">← Retour au site</a>
    </div>
  </div>

  <footer>© TAYZEN — <a href="index.html">tayzen</a></footer>
</div>

<script>
(() => {
  "use strict";

  // ---------- Sons (même moteur que le site) ----------
  let soundOn = true;
  try { soundOn = localStorage.getItem("tayzen_sound") !== "off"; } catch (e) {}
  let audioCtx = null;
  function getCtx() {
    if (!audioCtx) {
      const AC = window.AudioContext || window.webkitAudioContext;
      if (!AC) return null;
      audioCtx = new AC();
    }
    if (audioCtx.state === "suspended") audioCtx.resume();
    return audioCtx;
  }
  function pop(fStart, fEnd, dur, vol, delay, type) {
    const ctx = getCtx();
    if (!ctx) return;
    const jitter = 1 + (Math.random() * 0.06 - 0.03);
    const t0 = ctx.currentTime + (delay || 0);
    const osc = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.type = type || "sine";
    osc.frequency.setValueAtTime(fStart * jitter, t0);
    osc.frequency.exponentialRampToValueAtTime(fEnd * jitter, t0 + dur * 0.85);
    gain.gain.setValueAtTime(0.0001, t0);
    gain.gain.exponentialRampToValueAtTime(vol, t0 + 0.008);
    gain.gain.exponentialRampToValueAtTime(0.0001, t0 + dur);
    osc.connect(gain).connect(ctx.destination);
    osc.start(t0);
    osc.stop(t0 + dur + 0.05);
  }
  const sfx = {
    click()  { if (soundOn) pop(1100, 1450, 0.05, 0.03, 0, "sine"); },
    select() { if (soundOn) { pop(1000, 1300, 0.05, 0.028, 0, "sine"); pop(1400, 1850, 0.06, 0.026, 0.06, "sine"); } },
    hover()  { if (soundOn) pop(1500, 1800, 0.035, 0.014, 0, "sine"); },
    star(i)  { if (soundOn) pop(700 + i * 140, 900 + i * 180, 0.07, 0.035, 0, "sine"); },
    success() {
      if (!soundOn) return;
      pop(523, 545, 0.16, 0.06, 0, "sine");
      pop(659, 685, 0.16, 0.06, 0.11, "sine");
      pop(784, 815, 0.22, 0.065, 0.22, "sine");
      pop(1047, 1090, 0.34, 0.055, 0.33, "sine");
      pop(1568, 2350, 0.28, 0.025, 0.42, "sine");
    }
  };
  const isTouch = window.matchMedia("(hover: none), (pointer: coarse)").matches;
  if (!isTouch) {
    let lastHovered = null;
    document.addEventListener("pointerover", (e) => {
      const el = e.target.closest("button, .check, a.backLink");
      if (el && el !== lastHovered) { lastHovered = el; sfx.hover(); }
      else if (!el) lastHovered = null;
    });
  }

  // ---------- Chips (type de vidéo + recommandation) ----------
  function bindChips(boxId, fieldId) {
    const box = document.getElementById(boxId);
    const field = document.getElementById(fieldId);
    box.querySelectorAll("button").forEach((b) => {
      b.addEventListener("click", () => {
        box.querySelectorAll("button").forEach((x) => x.classList.remove("on"));
        b.classList.add("on");
        field.value = b.textContent.replace(/^[^\w«]*\s*/u, "").trim() || b.textContent.trim();
        sfx.select();
      });
    });
  }
  bindChips("typeChips", "typeVideoField");
  bindChips("recoChips", "recoField");

  // ---------- Étoiles ----------
  document.querySelectorAll(".stars").forEach((box) => {
    const hidden = document.createElement("input");
    hidden.type = "hidden";
    hidden.name = box.dataset.name;
    hidden.value = "";
    box.appendChild(hidden);
    const btns = [];
    for (let i = 1; i <= 5; i++) {
      const b = document.createElement("button");
      b.type = "button";
      b.textContent = "★";
      b.setAttribute("aria-label", i + " étoile" + (i > 1 ? "s" : ""));
      b.addEventListener("click", () => {
        hidden.value = i + "/5";
        btns.forEach((x, j) => {
          x.classList.toggle("on", j < i);
          x.classList.remove("bump");
          if (j < i) { void x.offsetWidth; x.classList.add("bump"); }
        });
        sfx.star(i);
      });
      btns.push(b);
      box.appendChild(b);
    }
  });

  // ---------- Consentement ----------
  const consent = document.getElementById("consent");
  const consentField = document.getElementById("consentField");
  consent.addEventListener("change", () => {
    consentField.value = consent.checked ? "Oui" : "Non";
    sfx.select();
  });

  // ---------- Confettis ----------
  function launchConfetti(layer) {
    if (!layer) return;
    const colors = ["#ff1e3c", "#ff5c7a", "#7CFFB2", "#39e07f", "#5b2bd6", "#ffd166", "#7cc4ff"];
    for (let i = 0; i < 42; i++) {
      const bit = document.createElement("span");
      bit.className = "confettiBit";
      bit.style.background = colors[i % colors.length];
      layer.appendChild(bit);
      const angle = Math.random() * Math.PI * 2;
      const dist = 80 + Math.random() * 170;
      const x = Math.cos(angle) * dist;
      const y = Math.sin(angle) * dist * 0.7 - 50;
      bit.animate([
        { transform: "translate(-50%,-50%) rotate(0deg) scale(1)", opacity: 1 },
        { transform: `translate(calc(-50% + ${x}px), calc(-50% + ${y + 150}px)) rotate(${Math.random() * 720 - 360}deg) scale(.5)`, opacity: 0 }
      ], { duration: 1300 + Math.random() * 900, delay: Math.random() * 180, easing: "cubic-bezier(.2,.7,.3,1)", fill: "forwards" });
      setTimeout(() => bit.remove(), 2800);
    }
  }

  // ---------- Envoi ----------
  const form = document.getElementById("avisForm");
  const formZone = document.getElementById("formZone");
  const thanks = document.getElementById("thanks");

  form.addEventListener("submit", async (e) => {
    e.preventDefault();
    for (const f of form.querySelectorAll("input[required]")) {
      if (!f.checkValidity()) { f.reportValidity(); f.focus(); return; }
    }
    if (!form.querySelector('input[name="note_globale"]').value) {
      alert("Donne au moins ta note globale ⭐");
      return;
    }

    const btn = form.querySelector("button.primary");
    btn.textContent = "Envoi…";
    btn.disabled = true;

    try {
      const res = await fetch(form.action, {
        method: "POST",
        body: new FormData(form),
        headers: { "Accept": "application/json" }
      });
      if (res.ok) {
        formZone.style.display = "none";
        thanks.style.display = "block";
        launchConfetti(thanks.querySelector(".confettiLayer"));
        sfx.success();
        window.scrollTo({ top: 0, behavior: "smooth" });
      } else {
        // Affiche la vraie raison renvoyée par Formspree (quota dépassé, champ invalide, etc.)
        const detail = await res.json().catch(() => null);
        const msg = detail && detail.errors
          ? detail.errors.map((x) => x.message).join(" • ")
          : "code " + res.status;
        alert("Erreur Formspree : " + msg + "\nRéessaie ou écris-moi par email.");
      }
    } catch (err) {
      alert("Erreur réseau. Réessaie plus tard.");
    } finally {
      btn.textContent = "Envoyer mon avis ⭐";
      btn.disabled = false;
    }
  });
})();
</script>

</body>
</html>
