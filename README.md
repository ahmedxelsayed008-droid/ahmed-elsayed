<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>\u0623\u062d\u0645\u062f \u0627\u0644\u0633\u064a\u062f \u2014 \u0645\u0635\u0645\u0645 \u062c\u0631\u0627\u0641\u064a\u0643</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;900&family=Syne:wght@700;800&family=DM+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
/* =========================================================
   SCREEN STYLES
   ========================================================= */
*, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }

:root {
  --gold:    #B8963E;
  --gold2:   #D4AF55;
  --dark:    #0F0F0F;
  --charcoal:#1C1C1C;
  --card:    #181818;
  --border:  rgba(184,150,62,0.22);
  --text:    #E2DAC8;
  --muted:   #888;
  --white:   #FAFAF8;
}

body {
  background: var(--dark);
  color: var(--text);
  font-family: 'Tajawal', sans-serif;
  line-height: 1.7;
}

/* ---- Print button ---- */
.print-bar {
  background: #111;
  border-bottom: 1px solid var(--border);
  padding: 12px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky; top: 0; z-index: 99;
}
.print-bar span {
  font-family: 'DM Sans', sans-serif;
  font-size: 13px;
  color: var(--muted);
}
.print-btn {
  cursor: pointer;
  background: linear-gradient(135deg, var(--gold), #8B6914);
  border: none;
  color: #fff;
  font-family: 'DM Sans', sans-serif;
  font-size: 13px;
  font-weight: 600;
  padding: 9px 24px;
  border-radius: 30px;
  letter-spacing: .5px;
  transition: opacity .2s;
}
.print-btn:hover { opacity:.85; }

/* ---- Page wrapper ---- */
.page {
  max-width: 900px;
  margin: 36px auto 60px;
  padding: 0 24px;
}

/* ---- Cover ---- */
.cover {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 52px 48px 44px;
  position: relative;
  overflow: hidden;
  margin-bottom: 28px;
}
.cover::before {
  content:'';
  position:absolute;
  top:-80px; left:-80px;
  width:320px; height:320px;
  background: radial-gradient(circle, rgba(184,150,62,.18) 0%, transparent 70%);
  pointer-events:none;
}
.cover::after {
  content:'';
  position:absolute;
  bottom:-60px; right:-60px;
  width:260px; height:260px;
  background: radial-gradient(circle, rgba(184,150,62,.10) 0%, transparent 70%);
  pointer-events:none;
}
.cover-inner { position:relative; z-index:1; }

.name-block { margin-bottom: 20px; }
.name-ar {
  font-family: 'Tajawal', sans-serif;
  font-weight: 900;
  font-size: 48px;
  background: linear-gradient(135deg, #F0D080, var(--gold), #F0D080);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1.1;
}
.name-en {
  font-family: 'Syne', sans-serif;
  font-size: 18px;
  font-weight: 700;
  color: var(--muted);
  letter-spacing: 2px;
  margin-top: 4px;
}
.title-badge {
  display: inline-block;
  background: rgba(184,150,62,.12);
  border: 1px solid var(--border);
  color: var(--gold2);
  font-size: 13px;
  font-weight: 500;
  padding: 5px 16px;
  border-radius: 20px;
  margin-bottom: 28px;
}
.tagline {
  font-size: 17px;
  color: #C8BFA8;
  max-width: 580px;
  font-weight: 400;
  line-height: 1.8;
  margin-bottom: 32px;
}

/* Contact chips */
.contacts {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}
.chip {
  display: flex;
  align-items: center;
  gap: 8px;
  background: rgba(255,255,255,.04);
  border: 1px solid var(--border);
  border-radius: 30px;
  padding: 7px 16px;
  font-size: 13px;
  color: var(--text);
  text-decoration: none;
  font-family: 'DM Sans', sans-serif;
  transition: border-color .2s, background .2s;
}
.chip:hover { border-color: var(--gold); background: rgba(184,150,62,.08); }
.chip .icon { font-size: 15px; }

/* ---- Stats row ---- */
.stats {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
  margin-bottom: 28px;
}
.stat-card {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 24px 20px;
  text-align: center;
}
.stat-num {
  font-family: 'Syne', sans-serif;
  font-size: 36px;
  font-weight: 800;
  background: linear-gradient(135deg, #F0D080, var(--gold));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1;
  margin-bottom: 6px;
}
.stat-label {
  font-size: 13px;
  color: var(--muted);
  font-weight: 500;
}

/* ---- Section ---- */
.section {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 30px 32px;
  margin-bottom: 20px;
}
.sec-title {
  font-family: 'Tajawal', sans-serif;
  font-weight: 700;
  font-size: 20px;
  color: var(--gold2);
  margin-bottom: 20px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.sec-title::after {
  content:'';
  flex:1;
  height:1px;
  background: var(--border);
}

/* Services grid */
.services {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 14px;
}
.service-item {
  background: rgba(255,255,255,.03);
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 18px 20px;
  display: flex;
  gap: 14px;
  align-items: flex-start;
}
.svc-icon {
  font-size: 24px;
  line-height: 1;
  flex-shrink:0;
}
.svc-name {
  font-weight: 700;
  font-size: 15px;
  margin-bottom: 4px;
}
.svc-desc {
  font-size: 13px;
  color: var(--muted);
  line-height: 1.6;
}

/* Pricing table */
.price-table { width: 100%; border-collapse: collapse; }
.price-table th {
  text-align: right;
  padding: 10px 16px;
  font-size: 12px;
  color: var(--muted);
  font-weight: 500;
  border-bottom: 1px solid var(--border);
  font-family: 'DM Sans', sans-serif;
  letter-spacing: .5px;
  text-transform: uppercase;
}
.price-table td {
  padding: 14px 16px;
  border-bottom: 1px solid rgba(184,150,62,.08);
  font-size: 14px;
  vertical-align: middle;
}
.price-table tr:last-child td { border-bottom: none; }
.price-table tr:hover td { background: rgba(184,150,62,.04); }
.pkg-name { font-weight: 700; color: var(--text); }
.pkg-desc { font-size: 12px; color: var(--muted); margin-top: 2px; }
.price-tag {
  font-family: 'Syne', sans-serif;
  font-size: 18px;
  font-weight: 800;
  color: var(--gold2);
  white-space: nowrap;
}
.price-note { font-size: 11px; color: var(--muted); }
.badge {
  display: inline-block;
  font-size: 11px;
  padding: 3px 10px;
  border-radius: 20px;
  font-family: 'DM Sans', sans-serif;
  font-weight: 500;
}
.badge-fast  { background: rgba(111,207,151,.12); color: #6FCF97; border: 1px solid rgba(111,207,151,.2); }
.badge-value { background: rgba(184,150,62,.12);  color: var(--gold2); border: 1px solid var(--border); }
.badge-pro   { background: rgba(187,107,217,.12); color: #BB6BD9; border: 1px solid rgba(187,107,217,.2); }

/* Why me */
.why-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 14px;
}
.why-item {
  display: flex;
  gap: 12px;
  align-items: flex-start;
  padding: 16px;
  border-radius: 12px;
  background: rgba(255,255,255,.02);
  border: 1px solid var(--border);
}
.why-icon { font-size: 22px; flex-shrink:0; }
.why-text strong { display:block; font-size:14px; font-weight:700; margin-bottom:3px; }
.why-text span { font-size:12px; color:var(--muted); }

/* Footer strip */
.footer-strip {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 16px;
  padding: 28px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 16px;
}
.footer-text strong { display:block; font-size:18px; font-weight:700; color:var(--gold2); margin-bottom:4px; }
.footer-text span { font-size:13px; color:var(--muted); }
.cta-btn {
  background: linear-gradient(135deg, var(--gold), #8B6914);
  color: #fff;
  text-decoration: none;
  padding: 12px 28px;
  border-radius: 30px;
  font-family: 'DM Sans', sans-serif;
  font-weight: 600;
  font-size: 14px;
}

/* =========================================================
   PRINT STYLES
   ========================================================= */
@media print {
  @page {
    size: A4;
    margin: 10mm 12mm;
  }

  body {
    background: #fff !important;
    color: #111 !important;
    -webkit-print-color-adjust: exact;
    print-color-adjust: exact;
  }

  .print-bar { display: none !important; }

  .page {
    max-width: 100%;
    margin: 0;
    padding: 0;
  }

  :root {
    --card:   #F8F6F0;
    --border: rgba(140,100,20,.18);
    --text:   #1A1A1A;
    --muted:  #666;
    --dark:   #fff;
  }

  .cover, .section, .stat-card, .service-item, .why-item, .footer-strip {
    break-inside: avoid;
  }

  .name-ar, .stat-num, .price-tag {
    -webkit-text-fill-color: var(--gold) !important;
    color: var(--gold) !important;
  }

  a { color: inherit; text-decoration: none; }
}
</style>
</head>
<body>

<!-- Print bar -->
<div class="print-bar">
  <span>\ud83d\udcc4 \u0627\u0641\u062a\u062d \u0641\u064a \u0627\u0644\u0645\u062a\u0635\u0641\u062d \u2190 \u0627\u0636\u063a\u0637 \u0627\u0644\u0632\u0631 \u0644\u062a\u062d\u0645\u064a\u0644 \u0643\u0640 PDF</span>
  <button class="print-btn" onclick="window.print()">\ud83d\udda8\ufe0f \u062d\u0641\u0638 \u0643\u0640 PDF</button>
</div>

<div class="page">

  <!-- ===== COVER ===== -->
  <div class="cover">
    <div class="cover-inner">
      <div class="name-block">
        <div class="name-ar">\u0623\u062d\u0645\u062f \u0627\u0644\u0633\u064a\u062f</div>
        <div class="name-en">AHMED EL-SAYED</div>
      </div>
      <div class="title-badge">\u2726 \u0645\u0635\u0645\u0645 \u062c\u0631\u0627\u0641\u064a\u0643 \u0645\u062d\u062a\u0631\u0641 \u00b7 Graphic Designer</div>
      <p class="tagline">
        \u0623\u0635\u0645\u0645 \u0647\u0648\u064a\u0627\u062a \u0628\u0635\u0631\u064a\u0629 \u062a\u062a\u0631\u0643 \u0623\u062b\u0631\u0627\u064b \u2014 \u0644\u0648\u062c\u0648\u060c \u0628\u0631\u0627\u0646din\u062c\u060c \u0648\u062a\u0635\u0627\u0645\u064a\u0645 \u062a\u0639\u0643\u0633 \u0631\u0648\u062d \u0639\u0644\u0627\u0645\u062a\u0643 \u0627\u0644\u062a\u062c\u0627\u0631\u064a\u0629 \u0628\u062f\u0642\u0629 \u0648\u0627\u062d\u062a\u0631\u0627\u0641\u064a\u0629 \u0639\u0627\u0644\u064a\u0629.
      </p>
      <div class="contacts">
        <a class="chip" href="https://wa.me/+201550021262" target="_blank">
          <span class="icon">\ud83d\udcac</span> \u0648\u0627\u062a\u0633\u0627\u0628: +201550021262
        </a>
        <a class="chip" href="https://behance.net/ahmedelsayed2025" target="_blank">
          <span class="icon">\ud83c\udfa8</span> behance.net/ahmedelsayed2025
        </a>
        <span class="chip">
          <span class="icon">\ud83d\udccd</span> \u0645\u062a\u0627\u062d \u0644\u0644\u0639\u0645\u0644 \u0639\u0646 \u0628\u064f\u0639\u062f \u2014 \u062f\u0648\u0644\u064a\u0627\u064b
        </span>
      </div>
    </div>
  </div>

  <!-- ===== STATS ===== -->
  <div class="stats">
    <div class="stat-card">
      <div class="stat-num">+5</div>
      <div class="stat-label">\u0633\u0646\u0648\u0627\u062a \u062e\u0628\u0631\u0629</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">+100</div>
      <div class="stat-label">\u0645\u0634\u0631\u0648\u0639 \u0645\u0646\u062c\u0632</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">2\u20133</div>
      <div class="stat-label">\u0623\u064a\u0627\u0645 \u062a\u0633\u0644\u064a\u0645</div>
    </div>
  </div>

  <!-- ===== SERVICES ===== -->
  <div class="section">
    <div class="sec-title">\ud83c\udfa8 \u062e\u062f\u0645\u0627\u062a\u064a</div>
    <div class="services">
      <div class="service-item">
        <div class="svc-icon">\ud83c\udff7</div>
        <div>
          <div class="svc-name">\u062a\u0635\u0645\u064a\u0645 \u0627\u0644\u0644\u0648\u062c\u0648</div>
          <div class="svc-desc">\u0644\u0648\u062c\u0648 \u0627\u062d\u062a\u0631\u0627\u0641\u064a \u064a\u0639\u0628\u0651\u0631 \u0639\u0646 \u0647\u0648\u064a\u062a\u0643 \u0648\u064a\u0628\u0642\u0649 \u0641\u064a \u0627\u0644\u0630\u0627\u0643\u0631\u0629 \u2014 \u0645\u0644\u0641\u0627\u062a \u0628\u062c\u0645\u064a\u0639 \u0627\u0644\u0635\u064a\u063a</div>
        </div>
      </div>
      <div class="service-item">
        <div class="svc-icon">\ud83c\udfe2</div>
        <div>
          <div class="svc-name">\u0627\u0644\u0647\u0648\u064a\u0629 \u0627\u0644\u0628\u0635\u0631\u064a\u0629 \u0627\u0644\u0643\u0627\u0645\u0644\u0629</div>
          <div class="svc-desc">\u0644\u0648\u062c\u0648 + \u0623\u0644\u0648\u0627\u0646 + \u062e\u0637\u0648\u0637 + \u062f\u0644\u064a\u0644 \u0627\u0633\u062a\u062e\u062f\u0627\u0645 + \u062a\u0637\u0628\u064a\u0642\u0627\u062a \u0639\u0644\u0649 \u0627\u0644\u0645\u0637\u0628\u0648\u0639\u0627\u062a</div>
        </div>
      </div>
      <div class="service-item">
        <div class="svc-icon">\ud83d\udcf1</div>
        <div>
          <div class="svc-name">\u062a\u0635\u0627\u0645\u064a\u0645 \u0627\u0644\u0633\u0648\u0634\u064a\u0627\u0644 \u0645\u064a\u062f\u064a\u0627</div>
          <div class="svc-desc">\u0628\u0648\u0633\u062a\u0627\u062a\u060c \u0642\u0635\u0635\u060c \u063a\u0644\u0627\u0641 \u0635\u0641\u062d\u0629 \u2014 \u0645\u062d\u062a\u0648\u0649 \u0628\u0635\u0631\u064a \u062c\u0627\u0647\u0632 \u0644\u0644\u0646\u0634\u0631</div>
        </div>
      </div>
      <div class="service-item">
        <div class="svc-icon">\ud83e\udea7</div>
        <div>
          <div class="svc-name">\u0644\u0627\u0641\u062a\u0627\u062a \u0648\u0633\u062a\u064a\u0643\u0631\u0627\u062a</div>
          <div class="svc-desc">\u062a\u0635\u0627\u0645\u064a\u0645 \u0637\u0628\u0627\u0639\u064a\u0629 \u0627\u062d\u062a\u0631\u0627\u0641\u064a\u0629 \u2014 \u0645\u062d\u0644\u0627\u062a\u060c \u0634\u0631\u0643\u0627\u062a\u060c \u0641\u0639\u0627\u0644\u064a\u0627\u062a</div>
        </div>
      </div>
    </div>
  </div>

  <!-- ===== PRICING ===== -->
  <div class="section">
    <div class="sec-title">\ud83d\udcb0 \u0627\u0644\u0623\u0633\u0639\u0627\u0631</div>
    <table class="price-table">
      <thead>
        <tr>
          <th>\u0627\u0644\u0628\u0627\u0642\u0629</th>
          <th>\u064a\u0634\u0645\u0644</th>
          <th>\u0627\u0644\u0633\u0639\u0631</th>
          <th>\u0627\u0644\u062a\u0633\u0644\u064a\u0645</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>
            <div class="pkg-name">\u0644\u0648\u062c\u0648 \u0623\u0633\u0627\u0633\u064a</div>
            <div class="pkg-desc">\u0644\u0644\u0645\u0634\u0627\u0631\u064a\u0639 \u0627\u0644\u0646\u0627\u0634\u0626\u0629 \u0648\u0627\u0644\u0623\u0641\u0631\u0627\u062f</div>
          </td>
          <td>\u0644\u0648\u062c\u0648 + 2 \u062a\u0639\u062f\u064a\u0644 + PNG/PDF</td>
          <td><span class="price-tag">$30</span><br><span class="price-note">\u064a\u0628\u062f\u0623 \u0645\u0646</span></td>
          <td><span class="badge badge-fast">2 \u0623\u064a\u0627\u0645</span></td>
        </tr>
        <tr>
          <td>
            <div class="pkg-name">\u0644\u0648\u062c\u0648 \u0645\u062a\u0642\u062f\u0645</div>
            <div class="pkg-desc">\u0644\u0644\u0645\u062d\u0644\u0627\u062a \u0648\u0627\u0644\u0645\u0624\u0633\u0633\u0627\u062a \u0627\u0644\u0635\u063a\u064a\u0631\u0629</div>
          </td>
          <td>\u0644\u0648\u062c\u0648 + \u062a\u0639\u062f\u064a\u0644\u0627\u062a \u063a\u064a\u0631 \u0645\u062d\u062f\u0648\u062f\u0629 + \u062c\u0645\u064a\u0639 \u0627\u0644\u0635\u064a\u063a</td>
          <td><span class="price-tag">$60</span><br><span class="price-note">\u064a\u0628\u062f\u0623 \u0645\u0646</span></td>
          <td><span class="badge badge-value">3 \u0623\u064a\u0627\u0645</span></td>
        </tr>
        <tr>
          <td>
            <div class="pkg-name">\u0647\u0648\u064a\u0629 \u0628\u0635\u0631\u064a\u0629 \u0643\u0627\u0645\u0644\u0629</div>
            <div class="pkg-desc">\u0628\u0631\u0627\u0646\u062f\u064a\u0646\u062c \u0627\u062d\u062a\u0631\u0627\u0641\u064a \u0634\u0627\u0645\u0644</div>
          </td>
          <td>\u0644\u0648\u062c\u0648 + \u0647\u0648\u064a\u0629 + \u062f\u0644\u064a\u0644 \u0627\u0633\u062a\u062e\u062f\u0627\u0645 + \u062a\u0637\u0628\u064a\u0642\u0627\u062a</td>
          <td><span class="price-tag">$150</span><br><span class="price-note">\u064a\u0628\u062f\u0623 \u0645\u0646</span></td>
          <td><span class="badge badge-pro">5\u20137 \u0623\u064a\u0627\u0645</span></td>
        </tr>
        <tr>
          <td>
            <div class="pkg-name">\u062a\u0635\u0627\u0645\u064a\u0645 \u0627\u0644\u0633\u0648\u0634\u064a\u0627\u0644</div>
            <div class="pkg-desc">\u062d\u0645\u0644\u0629 \u0628\u0635\u0631\u064a\u0629 \u0645\u062a\u0643\u0627\u0645\u0644\u0629</div>
          </td>
          <td>10 \u062a\u0635\u0627\u0645\u064a\u0645 + \u0637\u0628\u0642 \u0639\u0644\u0649 \u0627\u0644\u0628\u0631\u0627\u0646\u062f</td>
          <td><span class="price-tag">$50</span><br><span class="price-note">\u064a\u0628\u062f\u0623 \u0645\u0646</span></td>
          <td><span class="badge badge-fast">3 \u0623\u064a\u0627\u0645</span></td>
        </tr>
      </tbody>
    </table>
  </div>

  <!-- ===== WHY ME ===== -->
  <div class="section">
    <div class="sec-title">\u2b50 \u0644\u064a\u0634 \u0623\u062e\u062a\u0627\u0631\u0646\u064a\u061f</div>
    <div class="why-grid">
      <div class="why-item">
        <div class="why-icon">\u26a1</div>
        <div class="why-text">
          <strong>\u062a\u0633\u0644\u064a\u0645 \u0641\u0627\u0626\u0642 \u0627\u0644\u0633\u0631\u0639\u0629</strong>
          <span>\u0645\u0639\u0638\u0645 \u0627\u0644\u0645\u0634\u0627\u0631\u064a\u0639 \u062a\u064f\u0633\u0644\u064e\u0651\u0645 \u062e\u0644\u0627\u0644 2\u20133 \u0623\u064a\u0627\u0645 \u0639\u0645\u0644</span>
        </div>
      </div>
      <div class="why-item">
        <div class="why-icon">\ud83d\udcb0</div>
        <div class="why-text">
          <strong>\u0623\u0633\u0639\u0627\u0631 \u062a\u0646\u0627\u0641\u0633\u064a\u0629</strong>
          <span>\u062c\u0648\u062f\u0629 \u0639\u0627\u0644\u064a\u0629 \u0628\u0623\u0633\u0639\u0627\u0631 \u062a\u0646\u0627\u0633\u0628 \u0643\u0644 \u0627\u0644\u0645\u064a\u0632\u0627\u0646\u064a\u0627\u062a</span>
        </div>
      </div>
      <div class="why-item">
        <div class="why-icon">\ud83d\udd04</div>
        <div class="why-text">
          <strong>\u062a\u0639\u062f\u064a\u0644\u0627\u062a \u0645\u062c\u0627\u0646\u064a\u0629</strong>
          <span>\u062d\u062a\u0649 \u062a\u0643\u0648\u0646 \u0631\u0627\u0636\u064a\u0627
