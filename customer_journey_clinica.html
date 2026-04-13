<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Customer Journey — Consulta Médica</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;400;500;600&family=DM+Serif+Display&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #F7F6F2;
    --surface: #FFFFFF;
    --border: rgba(0,0,0,0.08);
    --text-primary: #1A1916;
    --text-secondary: #6B6A65;
    --text-tertiary: #A09F9A;
    --accent: #2B5CE6;
    --accent-light: #EEF2FD;
    --pain: #C0392B;
    --pain-bg: #FDF0EE;
    --gain: #1A7A4A;
    --gain-bg: #EDF7F2;
    --touch: #7C5BBF;
    --touch-bg: #F4F1FB;
    --stage-1: #2B5CE6;
    --stage-2: #7C5BBF;
    --stage-3: #D97706;
    --stage-4: #1A7A4A;
    --stage-5: #C0392B;
    --radius: 12px;
    --radius-sm: 8px;
  }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--bg);
    color: var(--text-primary);
    min-height: 100vh;
    padding: 24px;
  }

  .header {
    margin-bottom: 24px;
  }

  .header-eyebrow {
    font-size: 11px;
    font-weight: 500;
    letter-spacing: .1em;
    text-transform: uppercase;
    color: var(--text-tertiary);
    margin-bottom: 6px;
  }

  .header-title {
    font-family: 'DM Serif Display', serif;
    font-size: 26px;
    color: var(--text-primary);
    line-height: 1.2;
  }

  .header-title span {
    color: var(--accent);
  }

  /* Stage tabs */
  .stages-row {
    display: grid;
    grid-template-columns: repeat(5, minmax(0, 1fr));
    gap: 8px;
    margin-bottom: 16px;
  }

  .stage-tab {
    background: var(--surface);
    border: 1.5px solid var(--border);
    border-radius: var(--radius-sm);
    padding: 12px 10px;
    cursor: pointer;
    transition: all .2s ease;
    text-align: center;
    position: relative;
    overflow: hidden;
  }

  .stage-tab::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: var(--c);
    opacity: 0;
    transition: opacity .2s;
  }

  .stage-tab:hover { border-color: var(--c); }
  .stage-tab:hover::before { opacity: 1; }
  .stage-tab.active { border-color: var(--c); background: var(--surface); }
  .stage-tab.active::before { opacity: 1; }

  .tab-num {
    font-size: 10px;
    font-weight: 600;
    letter-spacing: .06em;
    color: var(--text-tertiary);
    margin-bottom: 4px;
  }

  .tab-icon { font-size: 20px; margin-bottom: 4px; line-height: 1; }

  .tab-name {
    font-size: 12px;
    font-weight: 500;
    color: var(--text-primary);
  }

  /* Detail panel */
  .detail-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-bottom: 16px;
  }

  .detail-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 16px;
  }

  .detail-card.full { grid-column: 1 / -1; }

  .detail-card-header {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 14px;
  }

  .detail-icon {
    width: 32px; height: 32px;
    border-radius: 8px;
    display: flex; align-items: center; justify-content: center;
    font-size: 16px;
    flex-shrink: 0;
  }

  .detail-card-title {
    font-size: 12px;
    font-weight: 600;
    letter-spacing: .05em;
    text-transform: uppercase;
    color: var(--text-tertiary);
  }

  .detail-stage-name {
    font-family: 'DM Serif Display', serif;
    font-size: 22px;
    color: var(--text-primary);
    margin-bottom: 6px;
  }

  .detail-meta {
    font-size: 13px;
    color: var(--text-secondary);
    line-height: 1.6;
  }

  .pill {
    display: inline-flex;
    align-items: center;
    font-size: 12px;
    font-weight: 400;
    padding: 5px 11px;
    border-radius: 20px;
    margin: 3px 3px 3px 0;
    line-height: 1.2;
  }

  .pill-pain { background: var(--pain-bg); color: var(--pain); }
  .pill-gain { background: var(--gain-bg); color: var(--gain); }
  .pill-touch { background: var(--touch-bg); color: var(--touch); }

  .pills-wrap { display: flex; flex-wrap: wrap; gap: 2px; }

  /* Emotion bar */
  .emotion-wrap {
    margin-top: 10px;
  }

  .emotion-label {
    display: flex;
    justify-content: space-between;
    font-size: 11px;
    color: var(--text-tertiary);
    margin-bottom: 6px;
  }

  .emotion-track {
    height: 8px;
    background: var(--bg);
    border-radius: 4px;
    overflow: hidden;
  }

  .emotion-fill {
    height: 100%;
    border-radius: 4px;
    transition: width .5s cubic-bezier(.4,0,.2,1);
  }

  /* Emotion chart */
  .chart-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 16px;
    margin-bottom: 16px;
  }

  .chart-label {
    font-size: 11px;
    font-weight: 600;
    letter-spacing: .06em;
    text-transform: uppercase;
    color: var(--text-tertiary);
    margin-bottom: 12px;
  }

  .chart-wrap svg { display: block; width: 100%; }

  /* Legend */
  .legend {
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
    margin-top: 12px;
  }

  .legend-item {
    display: flex;
    align-items: center;
    gap: 6px;
    font-size: 12px;
    color: var(--text-secondary);
  }

  .legend-dot {
    width: 10px; height: 10px;
    border-radius: 50%;
    flex-shrink: 0;
  }

  /* Animated entrance */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(8px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .detail-grid { animation: fadeUp .25s ease forwards; }
</style>
</head>
<body>

<div class="header">
  <p class="header-eyebrow">Mapa de experiencia</p>
  <h1 class="header-title">Customer Journey — <span>Consulta Médica</span></h1>
</div>

<div class="stages-row" id="stages-row"></div>

<div class="detail-grid" id="detail-grid"></div>

<div class="chart-card">
  <p class="chart-label">Curva emocional del paciente</p>
  <div class="chart-wrap">
    <svg viewBox="0 0 600 120" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id="lineGrad" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#2B5CE6" stop-opacity="0.15"/>
          <stop offset="100%" stop-color="#2B5CE6" stop-opacity="0"/>
        </linearGradient>
      </defs>
      <!-- Grid lines -->
      <line x1="0" y1="30" x2="600" y2="30" stroke="#E5E4DF" stroke-width="1" stroke-dasharray="4 4"/>
      <line x1="0" y1="60" x2="600" y2="60" stroke="#E5E4DF" stroke-width="1" stroke-dasharray="4 4"/>
      <line x1="0" y1="90" x2="600" y2="90" stroke="#E5E4DF" stroke-width="1" stroke-dasharray="4 4"/>
      <!-- Area fill -->
      <path d="M60 66 C130 66, 150 78, 180 78 C230 78, 250 24, 300 30 C350 30, 380 18, 420 18 C470 18, 490 12, 540 6 L540 120 L60 120 Z"
            fill="url(#lineGrad)"/>
      <!-- Line -->
      <path d="M60 66 C130 66, 150 78, 180 78 C230 78, 250 24, 300 30 C350 30, 380 18, 420 18 C470 18, 490 12, 540 6"
            fill="none" stroke="#2B5CE6" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
      <!-- Points -->
      <circle cx="60"  cy="66" r="5" fill="#2B5CE6"/>
      <circle cx="180" cy="78" r="5" fill="#C0392B"/>
      <circle cx="300" cy="30" r="5" fill="#D97706"/>
      <circle cx="420" cy="18" r="5" fill="#1A7A4A"/>
      <circle cx="540" cy="6"  r="5" fill="#1A7A4A"/>
      <!-- X Labels -->
      <text x="60"  y="115" text-anchor="middle" font-size="10" fill="#A09F9A" font-family="DM Sans, sans-serif">Descubrir</text>
      <text x="180" y="115" text-anchor="middle" font-size="10" fill="#A09F9A" font-family="DM Sans, sans-serif">Considerar</text>
      <text x="300" y="115" text-anchor="middle" font-size="10" fill="#A09F9A" font-family="DM Sans, sans-serif">Reservar</text>
      <text x="420" y="115" text-anchor="middle" font-size="10" fill="#A09F9A" font-family="DM Sans, sans-serif">Visita</text>
      <text x="540" y="115" text-anchor="middle" font-size="10" fill="#A09F9A" font-family="DM Sans, sans-serif">Post-visita</text>
    </svg>
  </div>
</div>

<div class="legend">
  <div class="legend-item"><div class="legend-dot" style="background:var(--pain-bg);border:1.5px solid var(--pain)"></div>Punto de dolor</div>
  <div class="legend-item"><div class="legend-dot" style="background:var(--gain-bg);border:1.5px solid var(--gain)"></div>Momento de alegría</div>
  <div class="legend-item"><div class="legend-dot" style="background:var(--touch-bg);border:1.5px solid var(--touch)"></div>Touchpoint</div>
</div>

<script>
const stages = [
  {
    num:"01", name:"Descubrir", icon:"🔍", color:"var(--stage-1)",
    persona:"Paciente con síntomas nuevos",
    goal:"Encontrar un médico de confianza",
    emotion:55,
    touchpoints:["Google","Recomendación familiar","Redes sociales"],
    pains:["Demasiadas opciones","Reseñas poco claras"],
    gains:["Perfil del médico online","Ver disponibilidad"]
  },
  {
    num:"02", name:"Considerar", icon:"🤔", color:"var(--stage-2)",
    persona:"Paciente evaluando opciones",
    goal:"Elegir al médico adecuado",
    emotion:35,
    touchpoints:["Sitio web clínica","Plataformas de citas","WhatsApp"],
    pains:["Tarifas poco visibles","Horarios confusos"],
    gains:["Fotos del consultorio","Especialidades claras"]
  },
  {
    num:"03", name:"Reservar", icon:"📅", color:"var(--stage-3)",
    persona:"Paciente tomando acción",
    goal:"Agendar cita fácilmente",
    emotion:60,
    touchpoints:["App / web","Llamada telefónica","Correo de confirmación"],
    pains:["Sistema lento","Sin confirmación inmediata"],
    gains:["Recordatorio automático","Instrucciones claras"]
  },
  {
    num:"04", name:"Visita", icon:"🏥", color:"var(--stage-4)",
    persona:"Paciente en consulta",
    goal:"Ser atendido con calidez y eficiencia",
    emotion:80,
    touchpoints:["Recepción","Sala de espera","Consulta médica"],
    pains:["Tiempo de espera largo","Papeleo excesivo"],
    gains:["Trato humano","Diagnóstico claro"]
  },
  {
    num:"05", name:"Post-visita", icon:"💊", color:"var(--stage-5)",
    persona:"Paciente en recuperación",
    goal:"Seguir el tratamiento con seguridad",
    emotion:85,
    touchpoints:["Receta / indicaciones","Seguimiento por mensaje","Próxima cita"],
    pains:["Dudas sin resolver","Sin canal de contacto"],
    gains:["Mensaje de seguimiento","Recordatorio de medicamento"]
  }
];

let activeIdx = 0;

function renderTabs() {
  const row = document.getElementById('stages-row');
  row.innerHTML = '';
  stages.forEach((s, i) => {
    const div = document.createElement('div');
    div.className = 'stage-tab' + (i === activeIdx ? ' active' : '');
    div.style.setProperty('--c', s.color);
    div.innerHTML = `<div class="tab-num">${s.num}</div><div class="tab-icon">${s.icon}</div><div class="tab-name">${s.name}</div>`;
    div.onclick = () => { activeIdx = i; renderTabs(); renderDetail(); };
    row.appendChild(div);
  });
}

function renderDetail() {
  const s = stages[activeIdx];
  const emoteColor = s.emotion >= 70 ? 'var(--gain)' : s.emotion >= 50 ? 'var(--stage-3)' : 'var(--pain)';
  const grid = document.getElementById('detail-grid');
  grid.style.animation = 'none';
  void grid.offsetWidth;
  grid.style.animation = '';

  grid.innerHTML = `
    <div class="detail-card">
      <div class="detail-card-header">
        <div class="detail-icon" style="background:${s.color}22">${s.icon}</div>
        <span class="detail-card-title">Etapa ${s.num}</span>
      </div>
      <div class="detail-stage-name">${s.name}</div>
      <div class="detail-meta"><strong>Persona:</strong> ${s.persona}</div>
      <div class="detail-meta" style="margin-top:4px"><strong>Objetivo:</strong> ${s.goal}</div>
      <div class="emotion-wrap">
        <div class="emotion-label"><span>😟 Baja</span><span>${s.emotion}% satisfacción</span><span>Alta 😊</span></div>
        <div class="emotion-track"><div class="emotion-fill" style="width:${s.emotion}%;background:${emoteColor}"></div></div>
      </div>
    </div>

    <div class="detail-card">
      <div class="detail-card-header">
        <div class="detail-icon" style="background:var(--touch-bg)">📍</div>
        <span class="detail-card-title">Touchpoints</span>
      </div>
      <div class="pills-wrap">${s.touchpoints.map(t=>`<span class="pill pill-touch">${t}</span>`).join('')}</div>
    </div>

    <div class="detail-card">
      <div class="detail-card-header">
        <div class="detail-icon" style="background:var(--pain-bg)">⚡</div>
        <span class="detail-card-title">Puntos de dolor</span>
      </div>
      <div class="pills-wrap">${s.pains.map(p=>`<span class="pill pill-pain">${p}</span>`).join('')}</div>
    </div>

    <div class="detail-card">
      <div class="detail-card-header">
        <div class="detail-icon" style="background:var(--gain-bg)">✨</div>
        <span class="detail-card-title">Momentos de alegría</span>
      </div>
      <div class="pills-wrap">${s.gains.map(g=>`<span class="pill pill-gain">${g}</span>`).join('')}</div>
    </div>
  `;
}

renderTabs();
renderDetail();
</script>
</body>
</html>
