[ahorcado.html](https://github.com/user-attachments/files/27090784/ahorcado.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1"/>
<title>⚡ Ahorcado Pro — Compiladores B</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Exo+2:wght@300;400;600;700&display=swap" rel="stylesheet"/>
<style>
/*
 * ═══════════════════════════════════════════════════════
 *  AHORCADO PRO v4 — Compiladores Sección B — Proyecto 1
 *  • Modo local (mismo dispositivo)
 *  • Modo online con link compartible
 *  • Espectador en vivo (BroadcastChannel API)
 *  • Continue playing / Revancha
 * ═══════════════════════════════════════════════════════
 *
 *  CÓMO FUNCIONA EL ESPECTADOR:
 *  ─────────────────────────────
 *  • P1 comparte el link y queda en pantalla "EN VIVO"
 *  • P2 abre el link y juega normalmente
 *  • Cada letra que adivina P2 se envía a P1 via
 *    BroadcastChannel (API nativa del navegador)
 *  • P1 ve el ahorcado, la palabra y errores actualizarse
 *    en tiempo real (≈ instantáneo)
 *
 *  LIMITACIÓN: BroadcastChannel funciona entre pestañas
 *  del MISMO navegador. Para dispositivos distintos se
 *  requiere hospedaje con backend (ej. Firebase).
 *  Para la demo del proyecto: dos pestañas = perfecto.
 */

:root {
  --bg0:#030312; --bg1:#07071C; --bg2:#0C0C28; --bg3:#111136;
  --edge:rgba(99,102,241,0.2); --edge2:rgba(34,211,238,0.2);
  --v:#818CF8; --vd:#6366F1; --c:#22D3EE; --g:#34D399;
  --r:#F87171; --y:#FBBF24; --pk:#F472B6;
  --w:#F1F5F9; --s:#94A3B8; --d:#475569;
  --fh:'Orbitron',sans-serif; --fb:'Exo 2',sans-serif;
  --rad:14px;
}
*{box-sizing:border-box;margin:0;padding:0}
html,body{min-height:100%;font-family:var(--fb);color:var(--w);background:var(--bg1)}
body{display:flex;flex-direction:column;align-items:center;overflow-x:hidden}
#cv{position:fixed;inset:0;z-index:0;pointer-events:none}
.app{position:relative;z-index:1;width:100%;max-width:560px;padding:0 1rem 4rem;display:flex;flex-direction:column;align-items:center}

/* ── Logo ── */
.logo{text-align:center;padding:1.75rem 0 1rem;position:relative}
.logo-title{font-family:var(--fh);font-size:clamp(24px,6vw,40px);font-weight:900;letter-spacing:5px;
  background:linear-gradient(90deg,var(--v),var(--c),var(--g),var(--pk),var(--v));background-size:300% auto;
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
  animation:gs 5s linear infinite}
@keyframes gs{0%{background-position:0%}100%{background-position:300%}}
.logo-sub{font-size:10px;letter-spacing:3px;text-transform:uppercase;color:var(--d);margin-top:5px;font-weight:600}
.logo::after{content:'';display:block;width:100px;height:1px;margin:.75rem auto 0;
  background:linear-gradient(90deg,transparent,var(--v),var(--c),transparent)}

/* ── Pantallas ── */
.screen{display:none;width:100%;flex-direction:column;align-items:center;gap:1rem}
.screen.active{display:flex;animation:si .4s cubic-bezier(.22,1,.36,1)}
@keyframes si{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}

/* ── Cards ── */
.card{width:100%;background:var(--bg2);border:1px solid var(--edge);border-radius:var(--rad);padding:1.5rem;position:relative;overflow:hidden}
.card::before{content:'';position:absolute;top:0;left:15%;right:15%;height:1px;background:linear-gradient(90deg,transparent,var(--v),transparent);opacity:.5}
.card-glow{box-shadow:0 0 50px rgba(99,102,241,.12),0 8px 32px rgba(0,0,0,.5)}
.card-cyan{border-color:var(--edge2)}
.card-cyan::before{background:linear-gradient(90deg,transparent,var(--c),transparent)}
.card-green{border-color:rgba(52,211,153,.2)}
.card-green::before{background:linear-gradient(90deg,transparent,var(--g),transparent)}
.card-red{border-color:rgba(248,113,113,.2)}
.card-red::before{background:linear-gradient(90deg,transparent,var(--r),transparent)}

/* ── Chips ── */
.chip{display:inline-flex;align-items:center;gap:6px;padding:5px 14px;border-radius:999px;font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;font-family:var(--fh)}
.cp1{background:rgba(129,140,248,.15);border:1px solid rgba(129,140,248,.4);color:var(--v)}
.cp2{background:rgba(52,211,153,.12);border:1px solid rgba(52,211,153,.4);color:var(--g)}
.cpol{background:rgba(34,211,238,.12);border:1px solid rgba(34,211,238,.4);color:var(--c)}
.cplv{background:rgba(248,113,113,.15);border:1px solid rgba(248,113,113,.4);color:var(--r);animation:cpls 1.5s ease-in-out infinite}
@keyframes cpls{0%,100%{opacity:1}50%{opacity:.6}}
.cpw{background:rgba(251,191,36,.12);border:1px solid rgba(251,191,36,.4);color:var(--y)}

/* ── Label & divider ── */
.lbl{font-size:10px;letter-spacing:3px;text-transform:uppercase;color:var(--d);margin-bottom:.75rem;font-family:var(--fh)}
.dvd{display:flex;align-items:center;gap:10px;width:100%;color:var(--d);font-size:10px;letter-spacing:2px;text-transform:uppercase}
.dvd::before,.dvd::after{content:'';flex:1;height:1px;background:linear-gradient(90deg,transparent,var(--edge),transparent)}

/* ── Inputs ── */
input{width:100%;background:rgba(255,255,255,.06);border:1.5px solid rgba(99,102,241,.3);border-radius:10px;
  padding:13px 16px;font-size:15px;font-family:var(--fb);font-weight:600;color:var(--w);
  outline:none;transition:all .2s;letter-spacing:.5px}
input:focus{border-color:var(--v);background:rgba(99,102,241,.1);box-shadow:0 0 0 3px rgba(99,102,241,.2)}
input::placeholder{color:var(--d);font-weight:400}
input[type=password]{letter-spacing:6px;font-size:18px}
input[type=password]::placeholder{letter-spacing:.5px;font-size:14px}

/* ── Botones ── */
.btn{display:flex;align-items:center;justify-content:center;gap:8px;padding:13px 20px;border-radius:10px;border:none;
  font-family:var(--fh);font-size:13px;font-weight:700;letter-spacing:1px;cursor:pointer;width:100%;
  transition:all .18s cubic-bezier(.34,1.56,.64,1);text-transform:uppercase;color:#fff;position:relative;overflow:hidden}
.btn::after{content:'';position:absolute;inset:0;background:linear-gradient(rgba(255,255,255,.1),transparent);pointer-events:none}
.btn:active{transform:scale(.95)!important}
.btn-v{background:linear-gradient(135deg,#6366F1,#8B5CF6);box-shadow:0 4px 24px rgba(99,102,241,.4)}
.btn-v:hover{transform:translateY(-2px);box-shadow:0 8px 32px rgba(99,102,241,.6)}
.btn-c{background:linear-gradient(135deg,#0891B2,#22D3EE);color:#000;font-weight:900;box-shadow:0 4px 20px rgba(6,182,212,.3)}
.btn-c:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(6,182,212,.5)}
.btn-g{background:linear-gradient(135deg,#059669,#34D399);box-shadow:0 4px 20px rgba(16,185,129,.3)}
.btn-g:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(16,185,129,.5)}
.btn-pk{background:linear-gradient(135deg,#BE185D,#F472B6);box-shadow:0 4px 20px rgba(244,114,182,.3)}
.btn-pk:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(244,114,182,.5)}
.btn-ol{background:transparent;border:1.5px solid rgba(255,255,255,.15);color:var(--s);font-size:12px;padding:10px 16px;width:auto;letter-spacing:.5px}
.btn-ol:hover{border-color:var(--v);color:var(--v)}
.btn-sm{padding:9px 16px;font-size:11px;width:auto}
.btn-row{display:flex;gap:.75rem;width:100%;flex-wrap:wrap}
.btn-row .btn{flex:1;min-width:140px}

/* ── Alertas ── */
.al{padding:12px 16px;border-radius:10px;font-size:13px;font-family:var(--fb);font-weight:600;width:100%;animation:si .3s ease;line-height:1.5}
.al-w{background:rgba(251,191,36,.1);border:1px solid rgba(251,191,36,.35);color:#FDE68A}
.al-e{background:rgba(248,113,113,.1);border:1px solid rgba(248,113,113,.35);color:#FCA5A5}
.al-ok{background:rgba(52,211,153,.1);border:1px solid rgba(52,211,153,.35);color:#6EE7B7}
.al-i{background:rgba(34,211,238,.1);border:1px solid rgba(34,211,238,.35);color:#67E8F9}

/* ══ HISTORIAL ══ */
.hrow{display:flex;align-items:center;justify-content:space-between;padding:10px 0;border-bottom:1px solid rgba(255,255,255,.05);font-size:13px}
.hrow:last-child{border-bottom:none}
.hw{text-transform:uppercase;font-weight:700;letter-spacing:2px;color:var(--w);font-family:var(--fh);font-size:11px}
.htg{padding:3px 10px;border-radius:999px;font-size:9px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;font-family:var(--fh)}
.htg-y{background:rgba(52,211,153,.15);color:#6EE7B7;border:1px solid rgba(52,211,153,.3)}
.htg-n{background:rgba(248,113,113,.1);color:#FCA5A5;border:1px solid rgba(248,113,113,.25)}

/* ══ AHORCADO SVG ══ */
.hpart{stroke-dasharray:300;stroke-dashoffset:300;transition:stroke-dashoffset .7s cubic-bezier(.22,1,.36,1)}
.hpart.on{stroke-dashoffset:0}
#spec-eyes{transition:opacity .4s .3s}

/* ══ TRIES BAR ══ */
.tbar{display:flex;gap:5px;justify-content:center;margin:.4rem 0}
.tp{height:7px;border-radius:4px;background:rgba(255,255,255,.08);transition:all .3s}
.tp.ok{background:var(--g);box-shadow:0 0 8px rgba(52,211,153,.6)}
.tp.no{background:var(--r);box-shadow:0 0 8px rgba(248,113,113,.6)}
.tlbl{font-family:var(--fh);font-size:10px;letter-spacing:2px;color:var(--d);text-transform:uppercase;text-align:center}

/* ══ PALABRA ══ */
.wrow{display:flex;gap:6px;justify-content:center;flex-wrap:wrap;margin:.6rem 0}
.lb{position:relative;min-width:36px;height:52px;display:flex;align-items:center;justify-content:center}
.lb::after{content:'';position:absolute;bottom:0;left:0;right:0;height:2px;border-radius:2px;
  background:linear-gradient(90deg,var(--vd),var(--c));box-shadow:0 0 8px rgba(99,102,241,.5)}
.lb.emp::after{background:rgba(99,102,241,.3);box-shadow:none}
.ll{font-family:var(--fh);font-size:22px;font-weight:900;text-transform:uppercase;
  color:#fff;text-shadow:0 0 12px rgba(34,211,238,.8),0 0 28px rgba(34,211,238,.4);
  opacity:0;transform:scaleY(0);transition:opacity .3s,transform .35s cubic-bezier(.34,1.56,.64,1);display:block}
.ll.on{opacity:1;transform:scaleY(1)}

/* ══ TECLADO ══ */
.kgrid{display:flex;flex-wrap:wrap;gap:4px;justify-content:center}
.key{min-width:31px;height:36px;padding:0 5px;
  background:rgba(255,255,255,.09);border:1.5px solid rgba(255,255,255,.2);
  border-radius:7px;font-family:var(--fh);font-size:11px;font-weight:700;
  color:#FFFFFF;text-transform:uppercase;cursor:pointer;
  display:flex;align-items:center;justify-content:center;
  transition:all .15s cubic-bezier(.34,1.56,.64,1)}
.key:hover:not(:disabled){background:rgba(99,102,241,.35);border-color:var(--v);color:#E0E7FF;transform:translateY(-3px);box-shadow:0 5px 14px rgba(99,102,241,.5)}
.key:active:not(:disabled){transform:translateY(1px)}
.key:disabled{cursor:default;opacity:.25}
.key.kok{background:rgba(52,211,153,.22)!important;border-color:var(--g)!important;color:#A7F3D0!important;text-shadow:0 0 8px rgba(52,211,153,.7);box-shadow:0 0 12px rgba(52,211,153,.2);opacity:1!important}
.key.kno{background:rgba(248,113,113,.12)!important;border-color:rgba(248,113,113,.4)!important;color:#FCA5A5!important;opacity:.45!important}
@keyframes ksh{0%,100%{transform:translateX(0)}25%{transform:translateX(-5px)}75%{transform:translateX(5px)}}
.key.sh{animation:ksh .3s ease}
.guess-row{display:flex;gap:8px;width:100%}
.guess-row input{flex:1;min-width:0;font-size:14px}

/* ══ TIMER ══ */
.tmr{display:flex;align-items:center;gap:6px;font-family:var(--fh);font-size:12px;letter-spacing:2px;color:var(--d)}
.tv{color:var(--c);font-size:15px}
.tv.warn{color:var(--r);animation:tp2 .5s ease-in-out infinite}
@keyframes tp2{0%,100%{opacity:1}50%{opacity:.3}}

/* ══ ESPECTADOR ══ */
.live-badge{display:flex;align-items:center;gap:8px;padding:6px 14px;border-radius:999px;
  background:rgba(248,113,113,.15);border:1px solid rgba(248,113,113,.4);
  font-family:var(--fh);font-size:10px;letter-spacing:2px;color:var(--r);font-weight:700;text-transform:uppercase}
.live-dot{width:8px;height:8px;border-radius:50%;background:var(--r);
  box-shadow:0 0 8px var(--r);animation:ld 1.2s ease-in-out infinite}
@keyframes ld{0%,100%{transform:scale(1);opacity:1}50%{transform:scale(.4);opacity:.3}}
.spec-wrong{display:flex;flex-wrap:wrap;gap:6px;min-height:32px}
.sw-chip{padding:5px 10px;border-radius:7px;font-family:var(--fh);font-size:12px;font-weight:700;
  background:rgba(248,113,113,.15);border:1px solid rgba(248,113,113,.4);color:#FCA5A5;
  text-transform:uppercase;letter-spacing:1px}
.wait-msg{display:flex;align-items:center;gap:10px;font-size:13px;color:var(--s);padding:.5rem 0}
.pdot{width:8px;height:8px;border-radius:50%;background:var(--g);box-shadow:0 0 8px rgba(52,211,153,.6);flex-shrink:0;animation:ld 1.4s ease-in-out infinite}

/* ══ LINK SHARE ══ */
.link-box{background:rgba(0,0,0,.5);border:1.5px dashed rgba(34,211,238,.4);border-radius:10px;padding:1rem;
  font-family:var(--fb);font-size:12px;color:var(--c);word-break:break-all;line-height:1.7;text-align:center;user-select:all}
.step-list{display:flex;flex-direction:column;gap:.6rem}
.step{display:flex;align-items:flex-start;gap:.75rem;font-size:13px;color:var(--s);line-height:1.5}
.sn{flex-shrink:0;width:22px;height:22px;border-radius:50%;background:rgba(99,102,241,.2);
  border:1px solid rgba(99,102,241,.4);font-family:var(--fh);font-size:10px;color:var(--v);
  display:flex;align-items:center;justify-content:center}

/* ══ INVITADO ══ */
.inv-icon{font-size:64px;display:block;text-align:center;margin-bottom:.75rem;
  animation:bounce .7s cubic-bezier(.34,1.56,.64,1)}
@keyframes bounce{from{transform:scale(0) rotate(-15deg);opacity:0}to{transform:scale(1) rotate(0);opacity:1}}
.inv-title{font-family:var(--fh);font-size:18px;font-weight:900;color:var(--c);letter-spacing:2px;text-align:center;margin-bottom:.5rem}
.inv-sub{font-size:13px;color:var(--s);line-height:1.6;text-align:center}
.wlrow{display:flex;gap:5px;justify-content:center;flex-wrap:wrap;margin:1rem 0 .25rem}
.wlb{width:30px;height:36px;border-radius:6px;border:2px solid rgba(34,211,238,.4);background:rgba(34,211,238,.06);
  display:flex;align-items:center;justify-content:center;font-size:14px;color:var(--c);font-family:var(--fh)}

/* ══ RESULTADO ══ */
.res-emoji{font-size:72px;text-align:center}
.res-title{font-family:var(--fh);font-size:clamp(20px,5vw,28px);font-weight:900;text-align:center;letter-spacing:2px}
.res-word{font-family:var(--fh);font-size:18px;letter-spacing:5px;text-align:center;
  color:var(--c);text-transform:uppercase;text-shadow:0 0 20px rgba(34,211,238,.5)}
.stat-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:.75rem;width:100%}
.sbox{background:rgba(255,255,255,.04);border:1px solid var(--edge);border-radius:10px;padding:.75rem;text-align:center}
.sv{font-family:var(--fh);font-size:20px;color:var(--c)}
.slbl{font-size:9px;color:var(--d);letter-spacing:1px;margin-top:2px;text-transform:uppercase}

/* ══ CONFETTI ══ */
.cw{position:fixed;inset:0;pointer-events:none;z-index:200;overflow:hidden}
.cp2{position:absolute;top:-20px;animation:cpf linear forwards}
@keyframes cpf{to{transform:translateY(110vh) rotate(800deg);opacity:0}}

/* ══ RESPONSIVE ══ */
@media(max-width:400px){.key{min-width:27px;height:32px;font-size:10px}.ll{font-size:18px}.lb{min-width:28px;height:44px}.btn-row .btn{min-width:120px}}
</style>
</head>
<body>
<canvas id="cv"></canvas>
<div class="app">

  <div class="logo">
    <div class="logo-title">⚡ AHORCADO</div>
    <div class="logo-sub">Compiladores · Sección B · Proyecto 1 · v4</div>
  </div>

  <!-- ══════════ HOME ══════════ -->
  <div id="s-home" class="screen">
    <div class="card card-glow" style="display:flex;flex-direction:column;gap:.85rem">
      <div class="lbl">Modo de juego</div>
      <button class="btn btn-v" onclick="goCreate('local')">🎮&nbsp;&nbsp;Jugar en este dispositivo</button>
      <div class="dvd">online con link</div>
      <button class="btn btn-c" onclick="goCreate('online')">🔗&nbsp;&nbsp;Crear partida + ver en vivo</button>
    </div>
    <div class="card" id="home-hist" style="display:none">
      <div class="lbl">Historial</div>
      <div id="hist-list"></div>
    </div>
  </div>

  <!-- ══════════ CREATE ══════════ -->
  <div id="s-create" class="screen">
    <div class="chip cp1">👤 Jugador 1</div>
    <div class="card card-glow" style="display:flex;flex-direction:column;gap:1rem">
      <div class="lbl">Ingresa la palabra secreta</div>
      <input type="password" id="wi" placeholder="Escribe sin que te vean..." autocomplete="off"
             onkeydown="if(event.key==='Enter')confirm_word()"/>
      <div id="cm"></div>
      <button class="btn btn-v" onclick="confirm_word()">Confirmar →</button>
      <button class="btn btn-ol" onclick="goHome()">← Volver</button>
    </div>
  </div>

  <!-- ══════════ SHARE + ESPERA ══════════ -->
  <div id="s-share" class="screen">
    <div class="chip cpol">🔗 Partida Online</div>

    <div class="card card-cyan" style="display:flex;flex-direction:column;gap:1rem">
      <div class="lbl">Envía este link al Jugador 2</div>
      <div class="link-box" id="share-link">—</div>
      <div style="display:flex;gap:.75rem">
        <button class="btn btn-c" onclick="copyLink()" style="flex:1">📋 Copiar link</button>
        <button class="btn btn-g" onclick="goSpectate()" style="flex:1">👁 Ver en vivo</button>
      </div>
      <div id="copy-st"></div>
    </div>

    <div class="card" style="display:flex;flex-direction:column;gap:.75rem">
      <div class="lbl">Instrucciones</div>
      <div class="step-list">
     
    <button class="btn btn-ol" onclick="goHome()">← Cancelar</button>
  </div>

  <!-- ══════════ SPECTATE (P1 ve en vivo) ══════════ -->
  <div id="s-spectate" class="screen">
    <div style="display:flex;align-items:center;justify-content:space-between;width:100%">
      <div class="chip cp1">👁 Espectador</div>
      <div class="live-badge"><div class="live-dot"></div>EN VIVO</div>
    </div>

    <div class="card card-glow" style="display:flex;flex-direction:column;align-items:center;gap:.5rem;padding:1.25rem">
      <!-- Ahorcado espectador -->
      <svg width="180" height="155" viewBox="0 0 180 155">
        <line x1="18" y1="148" x2="162" y2="148" stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="48" y1="148" x2="48" y2="12"   stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="48" y1="12"  x2="112" y2="12"  stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="112" y1="12" x2="112" y2="32"  stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="112" y1="32" x2="112" y2="42"  stroke="rgba(248,113,113,.4)" stroke-width="1.5" stroke-linecap="round"/>
        <circle id="sh-head" cx="112" cy="53" r="12" stroke="#F87171" stroke-width="2.5" fill="rgba(248,113,113,.05)" class="hpart" stroke-dasharray="75" stroke-dashoffset="75"/>
        <g id="spec-eyes" opacity="0"><circle cx="108" cy="51" r="1.8" fill="#F87171"/><circle cx="116" cy="51" r="1.8" fill="#F87171"/><path d="M107 59 Q112 55 117 59" stroke="#F87171" stroke-width="1.5" fill="none" stroke-linecap="round"/></g>
        <line id="sh-body" x1="112" y1="65" x2="112" y2="104" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="sh-la"   x1="112" y1="75" x2="93"  y2="94"  stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="sh-ra"   x1="112" y1="75" x2="131" y2="94"  stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="sh-ll"   x1="112" y1="104" x2="95" y2="128" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="sh-rl"   x1="112" y1="104" x2="129" y2="128" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
      </svg>
      <div class="tbar" id="spec-tbar"></div>
      <div class="tlbl" id="spec-tlbl">ESPERANDO AL JUGADOR 2...</div>
      <div class="wrow" id="spec-wrow"></div>
    </div>

    <div class="card" style="display:flex;flex-direction:column;gap:.75rem">
      <div class="lbl">Letras incorrectas</div>
      <div class="spec-wrong" id="spec-wrong">
        <span style="font-size:13px;color:var(--d)">Ninguna aún</span>
      </div>
    </div>

    <div class="card" style="padding:1rem">
      <div class="wait-msg" id="spec-wait">
        <div class="pdot"></div>
        <span>Esperando que el Jugador 2 abra el link...</span>
      </div>
      <div id="spec-msg"></div>
    </div>

    <!-- Timer espectador -->
    <div style="display:flex;align-items:center;gap:.5rem">
      <span style="font-size:10px;color:var(--d)">⏱ Tiempo de partida:</span>
      <span class="tv" id="spec-timer">0:00</span>
    </div>

    <button class="btn btn-ol btn-sm" onclick="goHome()">← Abandonar partida</button>
  </div>

  <!-- ══════════ INVITED (P2 abre el link) ══════════ -->
  <div id="s-invited" class="screen">
    <div class="chip cpw">🎯 Desafío</div>
    <div class="card card-glow">
      <span class="inv-icon">🎮</span>
      <div class="inv-title">¡Te han desafiado!</div>
      <p class="inv-sub">El Jugador 1 te envió una palabra secreta.<br>¿Puedes adivinarla?</p>
      <div style="text-align:center;margin:1.25rem 0">
        <div class="lbl" style="margin-bottom:.5rem">La palabra tiene</div>
        <div class="wlrow" id="inv-len"></div>
        <div style="font-size:12px;color:var(--d);margin-top:.5rem;letter-spacing:1px" id="inv-cnt"></div>
      </div>
      <button class="btn btn-g" onclick="startFromInvite()" style="font-size:14px;padding:15px">🚀&nbsp;&nbsp;¡Acepto el desafío!</button>
    </div>
  </div>

  <!-- ══════════ GAME (P2 juega) ══════════ -->
  <div id="s-game" class="screen">
    <div style="display:flex;align-items:center;justify-content:space-between;width:100%">
      <div class="chip cp2">👤 Jugador 2</div>
      <div class="tmr"><span style="font-size:10px">⏱</span><span class="tv" id="gtimer">0:00</span></div>
    </div>

    <div class="card card-glow" style="display:flex;flex-direction:column;align-items:center;gap:.5rem;padding:1.25rem">
      <svg id="game-svg" width="180" height="155" viewBox="0 0 180 155">
        <line x1="18" y1="148" x2="162" y2="148" stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="48" y1="148" x2="48" y2="12"   stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="48" y1="12"  x2="112" y2="12"  stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="112" y1="12" x2="112" y2="32"  stroke="rgba(99,102,241,.25)" stroke-width="3" stroke-linecap="round"/>
        <line x1="112" y1="32" x2="112" y2="42"  stroke="rgba(248,113,113,.4)" stroke-width="1.5" stroke-linecap="round"/>
        <circle id="gh-head" cx="112" cy="53" r="12" stroke="#F87171" stroke-width="2.5" fill="rgba(248,113,113,.05)" class="hpart" stroke-dasharray="75" stroke-dashoffset="75"/>
        <g id="game-eyes" opacity="0" style="transition:opacity .4s .3s"><circle cx="108" cy="51" r="1.8" fill="#F87171"/><circle cx="116" cy="51" r="1.8" fill="#F87171"/><path d="M107 59 Q112 55 117 59" stroke="#F87171" stroke-width="1.5" fill="none" stroke-linecap="round"/></g>
        <line id="gh-body" x1="112" y1="65" x2="112" y2="104" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="gh-la"   x1="112" y1="75" x2="93"  y2="94"  stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="gh-ra"   x1="112" y1="75" x2="131" y2="94"  stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="gh-ll"   x1="112" y1="104" x2="95" y2="128" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
        <line id="gh-rl"   x1="112" y1="104" x2="129" y2="128" stroke="#F87171" stroke-width="2.5" stroke-linecap="round" class="hpart"/>
      </svg>
      <div class="tbar" id="game-tbar"></div>
      <div class="tlbl" id="game-tlbl">INTENTOS: 6 / 6</div>
      <div class="wrow" id="game-wrow"></div>
    </div>

    <div class="card" style="padding:1.25rem">
      <div class="lbl" style="margin-bottom:.75rem">Selecciona una letra</div>
      <div class="kgrid" id="keyboard"></div>
    </div>

    <div class="card" style="padding:1rem">
      <div class="lbl" style="margin-bottom:.5rem">O adivina la palabra completa</div>
      <div class="guess-row">
        <input type="text" id="gi" placeholder="Escribe la palabra..." autocomplete="off"
               onkeydown="if(event.key==='Enter')guessWord()"/>
        <button class="btn btn-v btn-sm" onclick="guessWord()">→</button>
      </div>
      <div id="gm" style="margin-top:8px"></div>
    </div>
  </div>

  <!-- ══════════ RESULT ══════════ -->
  <div id="s-result" class="screen">
    <div class="card card-glow" style="display:flex;flex-direction:column;align-items:center;gap:1.25rem;padding:2rem">
      <div class="res-emoji" id="re"></div>
      <div>
        <div class="res-title" id="rt"></div>
        <div style="font-size:13px;color:var(--s);text-align:center;margin-top:.25rem" id="rs"></div>
      </div>
      <div class="res-word" id="rw"></div>
      <div class="stat-grid" id="rstat"></div>
      <div id="rst" style="width:100%"></div>

      <!-- ★ BOTONES DE CONTINUAR ★ -->
      <div class="btn-row">
        <button class="btn btn-v" onclick="playAgain()">🔄 Nueva partida</button>
        <button class="btn btn-pk" onclick="rematch()">⚡ Revancha</button>
      </div>
      <button class="btn btn-ol" onclick="goHome()">🏠 Menú principal</button>
    </div>

    <div class="card" id="r-hist" style="display:none;width:100%">
      <div class="lbl">Historial</div>
      <div id="r-hist-list"></div>
    </div>
  </div>

</div>
<div class="cw" id="cw"></div>

<script>
/* ============================================================
   AHORCADO PRO v4 — Lógica completa
   ============================================================
   VARIABLES GLOBALES
   CANVAS DE PARTÍCULAS
   AUDIO (Web Audio API)
   HISTORIAL (localStorage)
   NAVEGACIÓN
   BROADCAST CHANNEL (comunicación en tiempo real)
   CODIFICACIÓN DE URL
   DETECCIÓN DE HASH
   CREAR PARTIDA
   COMPARTIR LINK
   ESPECTADOR (P1 ve en vivo)
   INVITADO (P2 abre link)
   INICIO DEL JUEGO
   LÓGICA DEL JUEGO
   TIMER
   FIN DEL JUEGO
   CONTINUAR / REVANCHA
   CONFETTI
   INICIALIZACIÓN
   ============================================================ */

// ── Variables globales ──────────────────────────────────────
const MAX   = 6;
const PARTS_G = ['gh-head','gh-body','gh-la','gh-ra','gh-ll','gh-rl'];
const PARTS_S = ['sh-head','sh-body','sh-la','sh-ra','sh-ll','sh-rl'];
const ALPHA   = 'abcdefghijklmnñopqrstuvwxyz'.split('');

let G = {
  modo:      'local',  // 'local' | 'online'
  palabra:   '',
  reveladas: [],
  errores:   [],
  historial: [],
  timerSec:  0,
  timerID:   null,
  gameId:    '',       // ID único de la partida (para BroadcastChannel)
  bc:        null,     // BroadcastChannel activo
  invitada:  '',       // palabra recibida por link
  specTimer: null,     // timer del espectador
  specSec:   0,
};

// ── Canvas de partículas ─────────────────────────────────────
(function(){
  const cv = document.getElementById('cv');
  const ctx = cv.getContext('2d');
  let stars = [];
  function resize(){
    cv.width = window.innerWidth; cv.height = window.innerHeight;
    stars = Array.from({length:120},()=>({
      x:Math.random()*cv.width, y:Math.random()*cv.height,
      r:Math.random()*1.5+.3, sp:Math.random()*.35+.08,
      op:Math.random()*.6+.2,
    }));
  }
  function draw(){
    ctx.clearRect(0,0,cv.width,cv.height);
    const g=ctx.createRadialGradient(cv.width/2,cv.height/2,0,cv.width/2,cv.height/2,cv.width*.8);
    g.addColorStop(0,'#0C0C28'); g.addColorStop(1,'#030312');
    ctx.fillStyle=g; ctx.fillRect(0,0,cv.width,cv.height);
    stars.forEach(s=>{
      s.y-=s.sp; if(s.y<-2){s.y=cv.height+2;s.x=Math.random()*cv.width;}
      ctx.save(); ctx.globalAlpha=s.op*(Math.sin(Date.now()*.001+s.x)*.3+.7);
      ctx.beginPath(); ctx.arc(s.x,s.y,s.r,0,Math.PI*2);
      ctx.fillStyle=['#818CF8','#22D3EE','#F472B6'][Math.random()>.85?~~(Math.random()*3):0]||'#818CF8';
      ctx.fill(); ctx.restore();
    });
    requestAnimationFrame(draw);
  }
  window.addEventListener('resize',resize); resize(); draw();
})();

// ── Audio ─────────────────────────────────────────────────────
let _ac=null;
function ac(){if(!_ac)_ac=new(window.AudioContext||window.webkitAudioContext)();return _ac;}
function tone(f,t,d,g=.12){
  try{const c=ac(),o=c.createOscillator(),gn=c.createGain();
  o.connect(gn);gn.connect(c.destination);o.type=t;
  o.frequency.setValueAtTime(f,c.currentTime);
  gn.gain.setValueAtTime(g,c.currentTime);
  gn.gain.exponentialRampToValueAtTime(.001,c.currentTime+d);
  o.start(c.currentTime);o.stop(c.currentTime+d);}catch(e){}
}
const SFX={
  correct:()=>{tone(523,'sine',.15,.1);setTimeout(()=>tone(659,'sine',.2,.08),100);},
  wrong:  ()=>tone(200,'sawtooth',.25,.1),
  win:    ()=>[523,659,784,1047].forEach((f,i)=>setTimeout(()=>tone(f,'sine',.3,.12),i*130)),
  lose:   ()=>{tone(180,'sawtooth',.6,.12);setTimeout(()=>tone(120,'sawtooth',.8,.08),200);},
  key:    ()=>tone(800,'sine',.05,.025),
};

// ── Historial ─────────────────────────────────────────────────
function loadH(){
  try{const d=localStorage.getItem('ahorcado-v4');if(d)G.historial=JSON.parse(d);}catch(e){}
}
function saveH(){
  try{localStorage.setItem('ahorcado-v4',JSON.stringify(G.historial));}catch(e){}
}
function renderH(){
  const hc=document.getElementById('home-hist'), rc=document.getElementById('r-hist');
  const tiene=G.historial.length>0;
  if(hc)hc.style.display=tiene?'block':'none';
  if(rc)rc.style.display=tiene?'block':'none';
  const html=tiene?[...G.historial].reverse().slice(0,10).map(h=>
    `<div class="hrow"><span class="hw">${h.palabra}</span>
     <span class="htg ${h.estado==='Adivinada'?'htg-y':'htg-n'}">${h.estado}</span></div>`
  ).join(''):'';
  ['hist-list','r-hist-list'].forEach(id=>{const el=document.getElementById(id);if(el)el.innerHTML=html;});
}

// ── Navegación ────────────────────────────────────────────────
function show(id){
  document.querySelectorAll('.screen').forEach(s=>s.classList.remove('active'));
  const el=document.getElementById('s-'+id);
  if(!el)return;
  el.style.animation='none';void el.offsetWidth;el.style.animation='';
  el.classList.add('active');
  window.scrollTo({top:0,behavior:'smooth'});
}
function goHome(){
  stopTimer(); stopSpecTimer(); closeBc();
  renderH(); show('home');
}
function goCreate(m){
  G.modo=m;
  document.getElementById('cm').innerHTML='';
  document.getElementById('wi').value='';
  show('create');
  setTimeout(()=>document.getElementById('wi').focus(),400);
}

// ── BroadcastChannel ──────────────────────────────────────────
/*
 * El BroadcastChannel permite comunicación en tiempo real
 * entre pestañas del mismo navegador.
 * Canal: "ahorcado_GAMEID"
 *
 * Tipos de mensajes:
 *   'start'  → P2 comenzó a jugar
 *   'update' → estado del juego actualizado { reveladas, errores, timerSec }
 *   'end'    → partida terminada { won, palabra, timerSec, errores }
 */
function openBc(gameId, handler){
  closeBc();
  try {
    G.bc = new BroadcastChannel('ahorcado_' + gameId);
    G.bc.onmessage = (e) => handler(e.data);
  } catch(e) {
    console.warn('BroadcastChannel no disponible:', e);
  }
}
function closeBc(){
  if(G.bc){ try{G.bc.close();}catch(e){} G.bc=null; }
}
function bcSend(msg){
  if(G.bc){ try{G.bc.postMessage(msg);}catch(e){} }
}

// ── ID de partida ─────────────────────────────────────────────
function genId(){
  return Math.random().toString(36).substring(2,8).toUpperCase();
}

// ── Codificación URL ──────────────────────────────────────────
function enc(w){try{return btoa(unescape(encodeURIComponent(w)));}catch(e){return btoa(w);}}
function dec(b){try{return decodeURIComponent(escape(atob(b)));}catch(e){try{return atob(b);}catch(e2){return null;}}}

// Link format: file.html#g=GAMEID&w=WORD_B64
function makeLink(gameId, palabra){
  const base=window.location.href.split('#')[0];
  return `${base}#g=${gameId}&w=${enc(palabra)}`;
}

// ── Detección de hash ─────────────────────────────────────────
function checkHash(){
  const hash=window.location.hash.slice(1);
  if(!hash)return false;
  const p=new URLSearchParams(hash);
  const gameId=p.get('g'), wordB64=p.get('w');
  if(!gameId||!wordB64)return false;
  const palabra=dec(wordB64);
  if(!palabra)return false;
  // Limpiar hash de la URL
  window.history.replaceState(null,'',window.location.pathname+window.location.search);
  G.gameId=gameId; G.invitada=palabra;
  showInvited(palabra);
  return true;
}

function showInvited(p){
  const ct=document.getElementById('inv-len');ct.innerHTML='';
  document.getElementById('inv-cnt').textContent=`${p.length} ${p.length===1?'letra':'letras'}`;
  const n=Math.min(p.length,14);
  for(let i=0;i<n;i++){const b=document.createElement('div');b.className='wlb';b.textContent='?';ct.appendChild(b);}
  if(p.length>14){const b=document.createElement('div');b.className='wlb';b.textContent='…';ct.appendChild(b);}
  show('invited');
}

function startFromInvite(){
  G.palabra=G.invitada; G.invitada='';
  // Abrir BroadcastChannel como emisor (P2)
  openBc(G.gameId, ()=>{/* P2 no necesita recibir */});
  // Notificar a P1 que P2 empezó
  bcSend({type:'start'});
  initGame();
}

// ── Crear partida ─────────────────────────────────────────────
function confirm_word(){
  const val=document.getElementById('wi').value.trim().toLowerCase();
  const msg=document.getElementById('cm');msg.innerHTML='';
  if(!val){msg.innerHTML='<div class="al al-w">⚠ Ingresa una palabra.</div>';return;}
  if(!/^[a-záéíóúüñ]+$/i.test(val)){msg.innerHTML='<div class="al al-w">⚠ Solo letras, sin espacios ni números.</div>';return;}
  const prev=G.historial.find(h=>h.palabra===val);
  if(prev){msg.innerHTML=`<div class="al al-w">⚠ Esta palabra ya fue jugada como <strong>${prev.estado}</strong>. Elige otra.</div>`;return;}
  G.palabra=val; document.getElementById('wi').value='';
  if(G.modo==='online'){
    G.gameId=genId();
    const link=makeLink(G.gameId,G.palabra);
    document.getElementById('share-link').textContent=link;
    document.getElementById('copy-st').innerHTML='';
    show('share');
  } else {
    initGame();
  }
}

// ── Compartir link ────────────────────────────────────────────
function copyLink(){
  const link=document.getElementById('share-link').textContent;
  const st=document.getElementById('copy-st');
  navigator.clipboard.writeText(link).then(()=>{
    st.innerHTML='<div class="al al-ok">✓ ¡Link copiado! Envíaselo al Jugador 2.</div>';
  }).catch(()=>{
    const el=document.getElementById('share-link');
    const r=document.createRange();r.selectNode(el);
    window.getSelection().removeAllRanges();window.getSelection().addRange(r);
    st.innerHTML='<div class="al al-i">Selecciona el texto del link y cópialo.</div>';
  });
}

// ── Pantalla espectador ───────────────────────────────────────
function goSpectate(){
  // Inicializar pantalla espectador con la palabra (todo oculto)
  initSpecView(G.palabra, [], []);
  // Abrir BroadcastChannel como receptor (P1)
  openBc(G.gameId, handleSpecMessage);
  // Iniciar timer espectador
  startSpecTimer();
  show('spectate');
}

function initSpecView(palabra, reveladas, errores){
  // Palabra (casillas)
  const wr=document.getElementById('spec-wrow');
  wr.innerHTML=palabra.split('').map((l,i)=>
    `<div class="lb ${reveladas[i]?'':'emp'}"><span class="ll ${reveladas[i]?'on':''}">${reveladas[i]?l:''}</span></div>`
  ).join('');
  // Tries bar
  const tb=document.getElementById('spec-tbar');
  tb.innerHTML=Array.from({length:MAX},(_,i)=>
    `<div class="tp ${i<errores.length?'no':'ok'}" style="width:30px"></div>`
  ).join('');
  document.getElementById('spec-tlbl').textContent=
    `INTENTOS RESTANTES: ${MAX-errores.length} / ${MAX}`;
  // Letras incorrectas
  const sw=document.getElementById('spec-wrong');
  const soloLetras=errores.filter(e=>!e.startsWith('['));
  if(soloLetras.length){
    sw.innerHTML=soloLetras.map(l=>`<div class="sw-chip">${l}</div>`).join('');
  } else {
    sw.innerHTML='<span style="font-size:13px;color:var(--d)">Ninguna aún</span>';
  }
  // Ahorcado
  PARTS_S.forEach((id,i)=>{
    const el=document.getElementById(id);if(el)el.classList.toggle('on',i<errores.length);
  });
  document.getElementById('spec-eyes').style.opacity=errores.length>=1?'1':'0';
}

function handleSpecMessage(data){
  const {type}=data;
  const msg=document.getElementById('spec-msg');
  const wait=document.getElementById('spec-wait');

  if(type==='start'){
    if(wait)wait.innerHTML='<div class="wait-msg"><div class="pdot"></div><span>El Jugador 2 está jugando...</span></div>';
    msg.innerHTML='<div class="al al-ok">✓ ¡El Jugador 2 comenzó a jugar!</div>';
    setTimeout(()=>{if(msg.textContent)msg.innerHTML='';},3000);
  }
  else if(type==='update'){
    const {reveladas,errores,timerSec}=data;
    initSpecView(G.palabra,reveladas,errores);
    if(timerSec!==undefined){
      const m=Math.floor(timerSec/60),s=timerSec%60;
      document.getElementById('spec-timer').textContent=`${m}:${s.toString().padStart(2,'0')}`;
    }
  }
  else if(type==='end'){
    const {won,timerSec,erroresCnt}=data;
    stopSpecTimer();
    if(wait)wait.innerHTML='';
    msg.innerHTML=`<div class="al ${won?'al-ok':'al-e'}">
      ${won?'🎉 ¡El Jugador 2 adivinó la palabra!':'💀 El Jugador 2 no adivinó la palabra.'}
    </div>`;
    // Mostrar resultado en pantalla espectador después de 2 segundos
    setTimeout(()=>{
      showResultScreen(won, G.palabra, timerSec||0, erroresCnt||0);
    }, 2000);
  }
}

// ── Timer espectador ──────────────────────────────────────────
function startSpecTimer(){
  stopSpecTimer(); G.specSec=0;
  G.specTimer=setInterval(()=>{
    G.specSec++;
    const m=Math.floor(G.specSec/60),s=G.specSec%60;
    const el=document.getElementById('spec-timer');
    if(el)el.textContent=`${m}:${s.toString().padStart(2,'0')}`;
  },1000);
}
function stopSpecTimer(){
  if(G.specTimer){clearInterval(G.specTimer);G.specTimer=null;}
}

// ── Iniciar juego ─────────────────────────────────────────────
function initGame(){
  G.reveladas=Array(G.palabra.length).fill(false);
  G.errores=[];G.timerSec=0;
  document.getElementById('gm').innerHTML='';
  document.getElementById('gi').value='';
  buildKB();renderGame();resetHangmanGame();
  document.getElementById('game-eyes').style.opacity='0';
  startTimer();show('game');
}

function buildKB(){
  const kb=document.getElementById('keyboard');kb.innerHTML='';
  ALPHA.forEach(l=>{
    const b=document.createElement('button');b.className='key';b.textContent=l;b.id='key-'+l;
    b.onclick=()=>{SFX.key();guessLetter(l);};
    kb.appendChild(b);
  });
}

function renderGame(){
  // Palabra
  document.getElementById('game-wrow').innerHTML=
    G.palabra.split('').map((l,i)=>
      `<div class="lb ${G.reveladas[i]?'':'emp'}"><span class="ll ${G.reveladas[i]?'on':''}">${G.reveladas[i]?l:''}</span></div>`
    ).join('');
  // Tries bar
  document.getElementById('game-tbar').innerHTML=
    Array.from({length:MAX},(_,i)=>
      `<div class="tp ${i<G.errores.length?'no':'ok'}" style="width:30px"></div>`
    ).join('');
  document.getElementById('game-tlbl').textContent=
    `INTENTOS: ${MAX-G.errores.length} / ${MAX}`;
}

function resetHangmanGame(){
  PARTS_G.forEach(id=>document.getElementById(id)?.classList.remove('on'));
}

// ── Lógica del juego ──────────────────────────────────────────
function guessLetter(l){
  const btn=document.getElementById('key-'+l);if(!btn||btn.disabled)return;
  btn.disabled=true;
  if(G.palabra.includes(l)){
    G.palabra.split('').forEach((c,i)=>{if(c===l)G.reveladas[i]=true;});
    btn.classList.add('kok');SFX.correct();renderGame();
    bcSend({type:'update',reveladas:[...G.reveladas],errores:[...G.errores],timerSec:G.timerSec});
    if(G.reveladas.every(Boolean))endGame(true);
  } else {
    G.errores.push(l);
    btn.classList.add('kno','sh');setTimeout(()=>btn.classList.remove('sh'),350);
    SFX.wrong();
    const idx=G.errores.length-1;
    if(idx<PARTS_G.length)document.getElementById(PARTS_G[idx])?.classList.add('on');
    if(idx===0)setTimeout(()=>document.getElementById('game-eyes').style.opacity='1',700);
    renderGame();
    bcSend({type:'update',reveladas:[...G.reveladas],errores:[...G.errores],timerSec:G.timerSec});
    if(G.errores.length>=MAX)endGame(false);
  }
}

function guessWord(){
  const inp=document.getElementById('gi'),att=inp.value.trim().toLowerCase();
  const msg=document.getElementById('gm');inp.value='';
  if(!att)return;
  if(att===G.palabra){
    G.reveladas=G.reveladas.map(()=>true);renderGame();
    bcSend({type:'update',reveladas:[...G.reveladas],errores:[...G.errores],timerSec:G.timerSec});
    endGame(true);
  } else {
    G.errores.push('['+att+']');
    const idx=G.errores.length-1;
    if(idx<PARTS_G.length)document.getElementById(PARTS_G[idx])?.classList.add('on');
    SFX.wrong();renderGame();
    bcSend({type:'update',reveladas:[...G.reveladas],errores:[...G.errores],timerSec:G.timerSec});
    msg.innerHTML=`<div class="al al-e">✗ "<strong>${att}</strong>" no es correcta. Quedan <strong>${MAX-G.errores.length}</strong> intento(s).</div>`;
    if(G.errores.length>=MAX)endGame(false);
  }
}

// ── Timer del juego ───────────────────────────────────────────
function startTimer(){
  stopTimer();G.timerSec=0;updTimer();
  G.timerID=setInterval(()=>{G.timerSec++;updTimer();},1000);
}
function stopTimer(){if(G.timerID){clearInterval(G.timerID);G.timerID=null;}}
function updTimer(){
  const el=document.getElementById('gtimer');if(!el)return;
  const m=Math.floor(G.timerSec/60),s=G.timerSec%60;
  el.textContent=`${m}:${s.toString().padStart(2,'0')}`;
  el.className='tv'+(G.timerSec>120?' warn':'');
}

// ── Fin del juego ─────────────────────────────────────────────
function endGame(won){
  stopTimer();
  const estado=won?'Adivinada':'No adivinada';
  // Guardar historial
  G.historial.push({palabra:G.palabra,estado,tiempo:G.timerSec,errores:G.errores.length,fecha:new Date().toLocaleDateString('es')});
  saveH();
  // Notificar al espectador (P1)
  bcSend({type:'end',won,timerSec:G.timerSec,erroresCnt:G.errores.length});
  closeBc();
  if(won)SFX.win(); else SFX.lose();
  if(won)confetti();
  setTimeout(()=>showResultScreen(won,G.palabra,G.timerSec,G.errores.length), won?800:400);
}

// ── Pantalla de resultado ─────────────────────────────────────
function showResultScreen(won, palabra, timerSec, erroresCnt){
  document.getElementById('re').textContent=won?'🎉':'💀';
  document.getElementById('rt').textContent=won?'¡ADIVINADA!':'NO ADIVINADA';
  document.getElementById('rt').style.color=won?'var(--g)':'var(--r)';
  document.getElementById('rs').textContent=won?'El Jugador 2 ganó esta ronda.':'El Jugador 1 ganó esta ronda.';
  document.getElementById('rw').textContent=palabra.toUpperCase();
  const m=Math.floor(timerSec/60),s=timerSec%60;
  document.getElementById('rstat').innerHTML=`
    <div class="sbox"><div class="sv">${m}:${s.toString().padStart(2,'0')}</div><div class="slbl">Tiempo</div></div>
    <div class="sbox"><div class="sv" style="color:${won?'var(--g)':'var(--r)'}">${erroresCnt}</div><div class="slbl">Errores</div></div>
    <div class="sbox"><div class="sv">${MAX-erroresCnt}</div><div class="slbl">Vidas</div></div>
  `;
  document.getElementById('rst').innerHTML=`<div class="al ${won?'al-ok':'al-e'}" style="text-align:center">Guardada como: <strong>${won?'Adivinada':'No adivinada'}</strong></div>`;
  renderH();
  show('result');
}

// ── Continuar / Revancha ──────────────────────────────────────
/*
 * playAgain: reinicia el flujo completo (nueva palabra, nuevo modo)
 * rematch:   mantiene el mismo modo (local u online) y pide nueva palabra
 */
function playAgain(){
  // Volver al inicio para elegir modo
  goHome();
}

function rematch(){
  // Mantener el mismo modo, ir a crear nueva palabra
  goCreate(G.modo);
}

// ── Confetti ──────────────────────────────────────────────────
function confetti(){
  const w=document.getElementById('cw');w.innerHTML='';
  const cols=['#818CF8','#FF0080','#22D3EE','#34D399','#FBBF24','#F87171','#F472B6'];
  for(let i=0;i<100;i++){
    const el=document.createElement('div');el.className='cp2';
    const c=cols[~~(Math.random()*cols.length)],t=Math.random()*12+6,ci=Math.random()>.6;
    el.style.cssText=`left:${Math.random()*100}%;width:${t}px;height:${ci?t:t*.4}px;background:${c};border-radius:${ci?'50%':'3px'};animation-duration:${Math.random()*2+2}s;animation-delay:${Math.random()*.6}s`;
    w.appendChild(el);
  }
  setTimeout(()=>w.innerHTML='',5500);
}

// ── Inicialización ────────────────────────────────────────────
document.addEventListener('DOMContentLoaded',()=>{
  loadH();
  // Si hay hash en la URL (P2 abre el link), mostrar pantalla de invitado
  if(!checkHash()){
    renderH(); show('home');
  }
});
</script>
</body>
</html>
