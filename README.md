[关键词比对法训练题集-H5.html](https://github.com/user-attachments/files/28094054/-H5.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="关键词比对法训练">
<meta name="format-detection" content="telephone=no">
<meta property="og:title" content="二选一"关键词比对法"训练题集">
<meta property="og:description" content="30道法考精选易混题型 · 三步拆解 · 精准提分">
<meta property="og:type" content="website">
<meta property="og:site_name" content="法考题库">
<title>二选一"关键词比对法"训练题集</title>
<style>
:root {
  --bg: #0a0e17;
  --surface: #111827;
  --surface-2: #1a2235;
  --surface-3: #1e293b;
  --border: #1e3a5f;
  --border-active: #3b82f6;
  --text: #e2e8f0;
  --text-secondary: #94a3b8;
  --text-muted: #64748b;
  --accent: #3b82f6;
  --accent-glow: rgba(59,130,246,0.3);
  --gold: #f59e0b;
  --green: #10b981;
  --red: #ef4444;
  --red-glow: rgba(239,68,68,0.25);
  --purple: #8b5cf6;
  --cyan: #06b6d4;
  --radius: 14px;
  --radius-sm: 10px;
  --safe-bottom: env(safe-area-inset-bottom, 16px);
}

[data-theme="light"] {
  --bg: #f1f5f9;
  --surface: #ffffff;
  --surface-2: #f8fafc;
  --surface-3: #e2e8f0;
  --border: #cbd5e1;
  --border-active: #2563eb;
  --text: #0f172a;
  --text-secondary: #475569;
  --text-muted: #94a3b8;
  --accent-glow: rgba(37,99,235,0.15);
}

* { margin: 0; padding: 0; box-sizing: border-box; }
html { height: 100%; overflow: hidden; }
body {
  font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", sans-serif;
  background: var(--bg);
  color: var(--text);
  height: 100%;
  overflow: hidden;
  transition: background 0.3s ease, color 0.3s ease;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-smoothing: antialiased;
  user-select: none;
  -webkit-user-select: none;
  -webkit-overflow-scrolling: touch;
}

/* Ambient bg */
.bg-ambient {
  position: fixed; inset: 0; z-index: 0; pointer-events: none;
}
.bg-orb {
  position: absolute;
  border-radius: 50%;
  filter: blur(100px);
  opacity: 0.1;
  animation: orbFloat 25s ease-in-out infinite;
}
.bg-orb:nth-child(1) { width: 300px; height: 300px; background: var(--accent); top: -10%; left: -20%; }
.bg-orb:nth-child(2) { width: 250px; height: 250px; background: var(--purple); bottom: -10%; right: -20%; animation-delay: -8s; }
.bg-orb:nth-child(3) { width: 200px; height: 200px; background: var(--cyan); top: 40%; left: 40%; animation-delay: -16s; }
@keyframes orbFloat {
  0%, 100% { transform: translate(0, 0) scale(1); }
  33% { transform: translate(40px, -30px) scale(1.2); }
  66% { transform: translate(-30px, 40px) scale(0.85); }
}

/* Main app shell */
.app-shell {
  position: relative; z-index: 1;
  height: 100%; display: flex; flex-direction: column;
  max-width: 480px; margin: 0 auto;
}

/* Top bar */
.top-bar {
  flex-shrink: 0;
  padding: 12px 16px 8px;
  display: flex; align-items: center; justify-content: space-between;
  gap: 12px;
  background: var(--bg);
  z-index: 10;
}
.top-bar .title {
  font-size: 16px; font-weight: 700;
  background: linear-gradient(135deg, var(--text), var(--text-secondary));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.top-bar-actions {
  display: flex; gap: 8px;
}
.top-btn {
  width: 34px; height: 34px;
  border-radius: 50%;
  border: 1px solid var(--border);
  background: var(--surface);
  color: var(--text-secondary);
  cursor: pointer;
  display: flex; align-items: center; justify-content: center;
  font-size: 15px;
  transition: all 0.2s ease;
}
.top-btn:active { transform: scale(0.92); background: var(--surface-3); }

/* Progress bar thin */
.progress-strip {
  flex-shrink: 0;
  height: 3px;
  background: var(--surface-3);
  position: relative; z-index: 10;
}
.progress-strip-fill {
  height: 100%;
  background: linear-gradient(90deg, var(--accent), var(--purple), var(--cyan));
  background-size: 200% 100%;
  animation: progressShimmer 3s ease-in-out infinite;
  transition: width 0.4s ease;
}
@keyframes progressShimmer {
  0%, 100% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
}

/* Subject filter chips */
.filter-row {
  flex-shrink: 0;
  padding: 10px 16px;
  display: flex; gap: 6px;
  overflow-x: auto;
  z-index: 10;
  background: var(--bg);
  -webkit-overflow-scrolling: touch;
  scrollbar-width: none;
}
.filter-row::-webkit-scrollbar { display: none; }
.filter-chip {
  flex-shrink: 0;
  padding: 6px 14px;
  border-radius: 16px;
  border: 1px solid var(--border);
  background: var(--surface);
  color: var(--text-secondary);
  font-size: 12px; font-weight: 500;
  cursor: pointer;
  transition: all 0.2s ease;
  white-space: nowrap;
}
.filter-chip.active {
  background: var(--accent);
  border-color: var(--accent);
  color: #fff;
  box-shadow: 0 2px 12px var(--accent-glow);
}

/* Card area - scrollable */
.card-area {
  flex: 1;
  overflow-y: auto;
  padding: 0 16px;
  -webkit-overflow-scrolling: touch;
  scroll-behavior: smooth;
  z-index: 5;
}

/* Stats chips */
.stats-row {
  display: flex; gap: 8px;
  padding: 10px 0 14px;
}
.stat-chip {
  flex: 1;
  padding: 10px 8px;
  border-radius: 12px;
  background: var(--surface);
  border: 1px solid var(--border);
  text-align: center;
}
.stat-chip .val {
  font-size: 18px; font-weight: 700;
  background: linear-gradient(135deg, var(--accent), var(--cyan));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
.stat-chip .lbl {
  font-size: 10px; color: var(--text-muted);
  margin-top: 2px;
  text-transform: uppercase;
  letter-spacing: 0.03em;
}

/* Question card */
.question-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  margin-bottom: 14px;
  overflow: hidden;
  transition: all 0.3s ease;
}
.question-card.answered-correct {
  border-color: var(--green);
  box-shadow: 0 0 0 1px var(--green), 0 2px 16px rgba(16,185,129,0.12);
}
.question-card.answered-wrong {
  border-color: var(--red);
  box-shadow: 0 0 0 1px var(--red), 0 2px 16px var(--red-glow);
}

.card-top {
  padding: 16px;
  display: flex; align-items: flex-start; gap: 12px;
  cursor: pointer;
}
.card-num {
  flex-shrink: 0;
  width: 36px; height: 36px;
  border-radius: 10px;
  display: flex; align-items: center; justify-content: center;
  font-weight: 700; font-size: 14px;
  background: var(--surface-2);
  color: var(--text-secondary);
  border: 1px solid var(--border);
  transition: all 0.2s ease;
}
.question-card.answered-correct .card-num {
  background: rgba(16,185,129,0.15); color: var(--green); border-color: var(--green);
}
.question-card.answered-wrong .card-num {
  background: var(--red-glow); color: var(--red); border-color: var(--red);
}
.card-info { flex: 1; min-width: 0; }
.card-subject {
  font-size: 11px; font-weight: 600; color: var(--accent);
  letter-spacing: 0.04em; margin-bottom: 4px;
}
.card-stem {
  font-size: 14px; line-height: 1.65; color: var(--text); font-weight: 500;
}
.card-arrow {
  flex-shrink: 0; width: 28px; height: 28px;
  display: flex; align-items: center; justify-content: center;
  color: var(--text-muted); font-size: 13px;
  transition: transform 0.3s ease;
}
.question-card.expanded .card-arrow { transform: rotate(180deg); color: var(--accent); }

/* Card body */
.card-body {
  max-height: 0; overflow: hidden;
  transition: max-height 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}
.question-card.expanded .card-body { max-height: 4000px; }
.card-body-inner {
  padding: 0 16px 16px;
  border-top: 1px solid var(--border);
}

/* Options */
.options {
  display: flex; flex-direction: column; gap: 8px;
  margin: 14px 0;
}
.option-btn {
  display: flex; align-items: center; gap: 12px;
  padding: 14px 16px;
  border-radius: var(--radius-sm);
  border: 2px solid var(--border);
  background: var(--surface-2);
  cursor: pointer;
  font-size: 14px;
  text-align: left;
  color: var(--text);
  transition: all 0.15s ease;
  -webkit-tap-highlight-color: transparent;
  touch-action: manipulation;
}
.option-btn:active {
  transform: scale(0.98);
  border-color: var(--accent);
}
.option-letter {
  width: 30px; height: 30px;
  border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-weight: 700; font-size: 13px;
  flex-shrink: 0;
  background: var(--surface-3);
  color: var(--text-secondary);
  transition: all 0.15s ease;
}
.option-btn.correct-choice {
  border-color: var(--green) !important;
  background: rgba(16,185,129,0.08);
}
.option-btn.correct-choice .option-letter {
  background: var(--green); color: #fff;
  box-shadow: 0 0 12px rgba(16,185,129,0.3);
}
.option-btn.wrong-choice {
  border-color: var(--red) !important;
  background: var(--red-glow);
  animation: shake 0.5s ease;
}
.option-btn.wrong-choice .option-letter {
  background: var(--red); color: #fff;
}
@keyframes shake {
  0%, 100% { transform: translateX(0); }
  25% { transform: translateX(-5px); }
  50% { transform: translateX(5px); }
  75% { transform: translateX(-3px); }
}

/* Reveal */
.reveal-section {
  margin-top: 12px;
  opacity: 0; transform: translateY(8px);
  transition: all 0.35s cubic-bezier(0.4, 0, 0.2, 1);
}
.reveal-section.visible { opacity: 1; transform: translateY(0); }

.answer-badge {
  display: inline-flex; align-items: center; gap: 4px;
  padding: 5px 12px; border-radius: 16px;
  font-weight: 700; font-size: 12px; margin-bottom: 8px;
}
.answer-badge.correct { background: rgba(16,185,129,0.1); color: var(--green); }
.answer-badge.wrong { background: var(--red-glow); color: var(--red); }

.kw-info {
  margin-top: 8px; padding: 10px 14px;
  background: var(--surface-2); border-radius: 8px;
  font-size: 13px; color: var(--text-secondary); line-height: 1.6;
}
.kw-info .kw-label {
  font-size: 11px; font-weight: 600; color: var(--text-muted); margin-bottom: 2px;
}

.keyword-compare {
  display: grid; grid-template-columns: 1fr 1fr; gap: 8px;
  margin-top: 10px;
}
.keyword-col {
  background: var(--surface-2); border-radius: 8px;
  padding: 12px; border: 1px solid var(--border);
}
.keyword-col.col-a { border-left: 3px solid var(--accent); }
.keyword-col.col-b { border-left: 3px solid var(--purple); }
.keyword-col .col-label {
  font-size: 11px; font-weight: 700; letter-spacing: 0.03em; margin-bottom: 4px;
}
.keyword-col.col-a .col-label { color: var(--accent); }
.keyword-col.col-b .col-label { color: var(--purple); }
.keyword-col .col-kw { font-size: 12px; line-height: 1.6; color: var(--text-secondary); }

.analysis-box {
  margin-top: 10px; padding: 14px 16px;
  border-radius: 8px;
  background: rgba(245,158,11,0.06);
  border: 1px solid rgba(245,158,11,0.2);
}
.analysis-box .analysis-label {
  font-size: 11px; font-weight: 700; color: var(--gold);
  letter-spacing: 0.03em; margin-bottom: 4px;
}
.analysis-box .analysis-text { font-size: 13px; line-height: 1.75; color: var(--text-secondary); }

/* Bottom bar */
.bottom-bar {
  flex-shrink: 0;
  padding: 10px 16px calc(10px + var(--safe-bottom));
  display: flex; gap: 8px; align-items: center;
  background: var(--bg);
  border-top: 1px solid var(--border);
  z-index: 10;
}
.bottom-btn {
  flex: 1; padding: 12px;
  border-radius: 22px;
  border: 1px solid var(--border);
  background: var(--surface);
  color: var(--text);
  font-size: 13px; font-weight: 600;
  cursor: pointer;
  text-align: center;
  transition: all 0.15s ease;
  white-space: nowrap;
}
.bottom-btn:active { transform: scale(0.96); background: var(--surface-3); }
.bottom-btn.primary {
  background: var(--accent); border-color: var(--accent); color: #fff;
  box-shadow: 0 4px 16px var(--accent-glow);
}
.bottom-btn.primary:active { box-shadow: 0 2px 8px var(--accent-glow); }

/* Toast */
.toast {
  position: fixed; top: 20px; left: 50%; transform: translateX(-50%) translateY(-120px);
  z-index: 200;
  padding: 10px 20px; border-radius: 20px;
  font-weight: 600; font-size: 13px;
  background: var(--surface); border: 1px solid var(--border);
  color: var(--text);
  box-shadow: 0 8px 32px rgba(0,0,0,0.4);
  transition: transform 0.35s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  pointer-events: none;
}
.toast.show { transform: translateX(-50%) translateY(0); }

/* Confetti */
.confetti-piece {
  position: fixed; z-index: 300; pointer-events: none;
  animation: confettiFall 1.5s ease-out forwards;
}
@keyframes confettiFall {
  0% { transform: translateY(0) rotate(0deg) scale(1); opacity: 1; }
  100% { transform: translateY(100vh) rotate(720deg) scale(0); opacity: 0; }
}

/* Celebration overlay */
.celebration {
  position: fixed; inset: 0; z-index: 250; pointer-events: none;
  display: flex; align-items: center; justify-content: center;
  opacity: 0; transition: opacity 0.3s ease;
}
.celebration.show { opacity: 1; }
.celebration .emoji {
  font-size: 80px;
  animation: celebPop 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}
@keyframes celebPop {
  0% { transform: scale(0); opacity: 0; }
  60% { transform: scale(1.3); opacity: 1; }
  100% { transform: scale(1); opacity: 0; }
}

/* Empty state */
.empty-state {
  text-align: center; padding: 40px 20px;
}
.empty-state .icon { font-size: 48px; margin-bottom: 12px; }
.empty-state .msg { font-size: 14px; color: var(--text-muted); }

/* Share sheet */
.share-overlay {
  position: fixed; inset: 0; z-index: 500;
  background: rgba(0,0,0,0.6);
  display: flex; align-items: flex-end;
  opacity: 0; pointer-events: none;
  transition: opacity 0.3s ease;
}
.share-overlay.show { opacity: 1; pointer-events: auto; }
.share-sheet {
  width: 100%; max-width: 480px; margin: 0 auto;
  background: var(--surface);
  border-radius: 20px 20px 0 0;
  padding: 20px 20px calc(20px + var(--safe-bottom));
  transform: translateY(100%);
  transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}
.share-overlay.show .share-sheet { transform: translateY(0); }
.share-sheet h3 { font-size: 16px; text-align: center; margin-bottom: 16px; }
.share-actions {
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 12px;
}
.share-action {
  display: flex; flex-direction: column; align-items: center; gap: 6px;
  cursor: pointer; padding: 8px;
}
.share-action .sa-icon {
  width: 48px; height: 48px; border-radius: 14px;
  display: flex; align-items: center; justify-content: center;
  font-size: 22px;
  background: var(--surface-3);
  transition: all 0.15s ease;
}
.share-action:active .sa-icon { transform: scale(0.9); }
.share-action .sa-label { font-size: 11px; color: var(--text-secondary); }
.share-cancel {
  display: block; width: 100%; margin-top: 16px;
  padding: 12px; border-radius: 22px;
  border: 1px solid var(--border);
  background: var(--surface-2);
  color: var(--text);
  font-size: 14px; font-weight: 600;
  cursor: pointer; text-align: center;
}

/* Haptic ripple */
.ripple {
  position: absolute;
  border-radius: 50%;
  background: rgba(255,255,255,0.15);
  transform: scale(0);
  animation: ripple 0.6s ease-out;
  pointer-events: none;
}
@keyframes ripple {
  to { transform: scale(4); opacity: 0; }
}

@media (min-width: 481px) {
  .app-shell { border-left: 1px solid var(--border); border-right: 1px solid var(--border); }
}
</style>
</head>
<body>

<div class="bg-ambient">
  <div class="bg-orb"></div>
  <div class="bg-orb"></div>
  <div class="bg-orb"></div>
</div>

<div class="toast" id="toast"></div>
<div class="celebration" id="celebration"><span class="emoji"></span></div>

<div class="share-overlay" id="shareOverlay" onclick="closeShare()">
  <div class="share-sheet" onclick="event.stopPropagation()">
    <h3>分享给朋友</h3>
    <div class="share-actions">
      <div class="share-action" onclick="doShare('wechat')">
        <div class="sa-icon" style="background:#07c16022;color:#07c160;">💬</div>
        <span class="sa-label">微信好友</span>
      </div>
      <div class="share-action" onclick="doShare('moments')">
        <div class="sa-icon" style="background:#07c16022;color:#07c160;">🔄</div>
        <span class="sa-label">朋友圈</span>
      </div>
      <div class="share-action" onclick="doShare('copy')">
        <div class="sa-icon" style="background:var(--accent-glow);color:var(--accent);">📋</div>
        <span class="sa-label">复制链接</span>
      </div>
      <div class="share-action" onclick="doShare('more')">
        <div class="sa-icon" style="background:rgba(245,158,11,0.2);color:var(--gold);">⋯</div>
        <span class="sa-label">更多</span>
      </div>
    </div>
    <button class="share-cancel" onclick="closeShare()">取消</button>
  </div>
</div>

<div class="app-shell">
  <!-- Top bar -->
  <div class="top-bar">
    <span class="title">⚖️ 关键词比对法训练</span>
    <div class="top-bar-actions">
      <button class="top-btn" onclick="toggleTheme()" title="主题">🌓</button>
      <button class="top-btn" onclick="openShare()" title="分享">📤</button>
      <button class="top-btn" onclick="resetAll()" title="重置">↺</button>
    </div>
  </div>

  <!-- Progress strip -->
  <div class="progress-strip">
    <div class="progress-strip-fill" id="progressFill" style="width:0%"></div>
  </div>

  <!-- Filter chips -->
  <div class="filter-row" id="filterRow">
    <button class="filter-chip active" data-filter="all">全部</button>
    <button class="filter-chip" data-filter="刑法">刑法</button>
    <button class="filter-chip" data-filter="民法">民法</button>
    <button class="filter-chip" data-filter="刑诉法">刑诉法</button>
    <button class="filter-chip" data-filter="民诉法">民诉法</button>
    <button class="filter-chip" data-filter="行政法">行政法</button>
    <button class="filter-chip" data-filter="理论法">理论法</button>
  </div>

  <!-- Card area -->
  <div class="card-area" id="cardArea"></div>

  <!-- Bottom nav -->
  <div class="bottom-bar">
    <button class="bottom-btn" id="statBtn">
      <span id="statDone">0</span>/<span id="statTotal">30</span> · <span id="statAccuracy">—</span>
    </button>
    <button class="bottom-btn" onclick="collapseAll()">收起全部</button>
    <button class="bottom-btn primary" onclick="expandAll()">展开全部</button>
  </div>
</div>

<script>
var questions = [{"id":1,"subject":"刑法","stem":"甲为杀乙，在乙的饭菜中投毒，明知丙也会吃该饭菜，仍放任不管，最终乙、丙均中毒死亡。甲对丙的死亡主观心态是？","optionA":"直接故意","optionB":"间接故意","kwQ":"明知、放任、乙丙均死亡","kwA":"明知+希望结果发生","kwB":"明知+放任结果发生","analysis":"甲杀乙的主观心态为直接故意（积极希望乙死亡）；对丙的死亡，甲未积极追求，仅明知可能发生且放任该结果，符合间接故意的构成要件。","answer":"B"},{"id":2,"subject":"刑法","stem":"甲开车时认为自己技术好，超速行驶，未及时避让行人，致行人重伤。甲的主观心态是？","optionA":"过于自信的过失","optionB":"疏忽大意的过失","kwQ":"认为技术好、超速、未避让","kwA":"已经预见危害结果+轻信能避免","kwB":"应当预见危害结果+未预见","analysis":"甲作为机动车驾驶人，应当预见超速行驶可能引发交通事故，但其因自信自身技术好而轻信能够避免，最终导致行人重伤，符合过于自信的过失的构成要件。","answer":"A"},{"id":3,"subject":"刑法","stem":"甲趁乙不备，一把夺走乙手中价值5000元的手机，转身逃跑。甲构成？","optionA":"抢劫罪","optionB":"抢夺罪","kwQ":"趁不备、夺走、逃跑","kwA":"暴力/胁迫压制人身反抗+当场取财","kwB":"趁人不备+公然夺取财物（暴力作用于物）","analysis":"甲未使用暴力、胁迫等手段压制乙的人身反抗，仅趁乙不备公然夺取其手中手机，暴力作用于财物而非人身，符合抢夺罪的构成要件，不构成抢劫罪。","answer":"B"},{"id":4,"subject":"刑法","stem":"乙将手机落在咖啡馆，甲捡到后拒不归还，占为己有。甲构成？","optionA":"盗窃罪","optionB":"侵占罪","kwQ":"落在、捡到、拒不归还","kwA":"他人占有财物→秘密转移占有","kwB":"自己合法占有财物→变占有为所有","analysis":"乙将手机落在咖啡馆，该手机已脱离乙的占有，甲捡到后合法占有该手机，但其拒不归还、占为己有，符合侵占罪“变合法占有为非法所有”的核心要件，不构成盗窃罪。","answer":"B"},{"id":5,"subject":"刑法","stem":"甲遭歹徒持刀追杀，情急之下夺过路人乙的自行车骑车逃跑，致乙摔倒受伤。甲的行为属于？","optionA":"正当防卫","optionB":"紧急避险","kwQ":"遭追杀、夺路人自行车、乙受伤","kwA":"针对不法侵害人实施防卫行为","kwB":"针对无辜第三人的合法权益实施避险行为","analysis":"甲为躲避歹徒追杀（避免自身人身权益受侵害），不得已损害无辜路人乙的自行车所有权及人身权益，其行为针对的是无辜第三人，而非不法侵害人，符合紧急避险的构成要件。","answer":"B"},{"id":6,"subject":"刑法","stem":"甲持刀欲杀乙，举刀后因害怕坐牢，主动放下刀离开。甲属于？","optionA":"犯罪未遂","optionB":"犯罪中止","kwQ":"害怕、主动放下、离开","kwA":"已着手犯罪+意志以外原因被迫停止","kwB":"已着手犯罪+自动放弃犯罪/有效防止结果发生","analysis":"甲已持刀举刀（已着手实行杀人行为），但因主观上害怕坐牢而主动放下刀、放弃杀人行为，并非因意志以外的原因被迫停止，符合犯罪中止的构成要件。","answer":"B"},{"id":7,"subject":"民法","stem":"某商场在官网发布“新款手机5000元，现货可下单”的广告。该广告属于？","optionA":"要约","optionB":"要约邀请","kwQ":"5000元、现货可下单、内容确定","kwA":"内容具体确定+表明一经承诺即受约束","kwB":"希望他人向自己发出要约（内容不具体或无受约束意思）","analysis":"该广告明确标注手机价格、现货状态，且“可下单”表明商场愿意接受相对人的承诺（下单行为）并受其约束，内容具体确定，符合要约的构成要件，不属于要约邀请。","answer":"A"},{"id":8,"subject":"民法","stem":"甲是A公司业务员，长期代表A公司与B公司签约，后甲离职但未收回盖有A公司公章的空白合同，甲持空白合同与B公司签约。该合同效力？","optionA":"无权代理，效力待定","optionB":"表见代理，有效","kwQ":"长期代表、离职、空白合同、B公司善意","kwA":"无代理权+相对人无理由相信其有代理权","kwB":"无代理权+相对人有理由相信其有代理权","analysis":"甲虽已离职（无代理权），但长期代表A公司与B公司签约，且持有盖有A公司公章的空白合同，B公司有合理理由相信甲仍有代理权，符合表见代理的构成要件，该合同有效。","answer":"B"},{"id":9,"subject":"民法","stem":"甲将自己的汽车抵押给乙借款5万元，未交付汽车。乙享有的权利是？","optionA":"抵押权","optionB":"质权","kwQ":"抵押、未交付","kwA":"不转移抵押物占有，不动产/动产均可设定","kwB":"必须转移质押物占有，动产/权利可设定","analysis":"甲与乙约定的是抵押，且未将汽车交付给乙（未转移占有），符合抵押权“不转移占有”的核心特征；质权要求转移占有，本案不符合质权的构成要件，故乙享有的是抵押权。","answer":"A"},{"id":10,"subject":"民法","stem":"甲向乙借款，丙提供担保，约定“甲不还钱时，丙再还”。丙的保证方式是？","optionA":"一般保证","optionB":"连带责任保证","kwQ":"甲不还钱时、丙再还、先后顺序","kwA":"债务人不能履行债务时，保证人才承担保证责任（有先诉抗辩权）","kwB":"债务到期后，债权人可直接要求保证人承担保证责任（无先诉抗辩权）","analysis":"双方约定“甲不还钱时，丙再还”，明确约定了债务人甲先履行还款义务，只有在甲不能履行时，丙才承担保证责任，符合一般保证的构成要件，丙享有先诉抗辩权。","answer":"A"},{"id":11,"subject":"刑诉法","stem":"公安机关通知犯罪嫌疑人甲到案接受讯问，甲无正当理由拒不到案，公安机关强制将甲带到警局。该行为是？","optionA":"拘传","optionB":"传唤","kwQ":"强制带到","kwA":"刑事强制措施，强制犯罪嫌疑人/被告人到案","kwB":"侦查手段，通知到案，不具有强制性","analysis":"传唤仅为通知到案，无强制性；而本案中公安机关因甲拒不到案，强制将其带到警局，属于刑事强制措施中的拘传，而非传唤。","answer":"A"},{"id":12,"subject":"刑诉法","stem":"犯罪嫌疑人甲涉嫌轻罪，无社会危险性，公安机关责令甲提供保证人，甲在家居住，定期报告活动情况。该强制措施是？","optionA":"取保候审","optionB":"监视居住","kwQ":"保证人、在家居住、定期报告","kwA":"不关押，提供保证人/保证金，活动范围较大，定期报告","kwB":"限制人身自由，通常为指定居所，活动范围极小","analysis":"甲涉嫌轻罪、无社会危险性，公安机关责令其提供保证人，允许其在家居住、定期报告活动情况，符合取保候审“不关押、限制较少”的特征；监视居住限制更严格，通常为指定居所，本案不符合监视居住的要件。","answer":"A"},{"id":13,"subject":"刑诉法","stem":"被告人甲不服一审判决，向上级法院提出异议，要求二审改判。该行为是？","optionA":"上诉","optionB":"抗诉","kwQ":"被告人、不服一审、向上级法院提出","kwA":"由被告人、自诉人、附带民事诉讼当事人提出，不服一审判决/裁定","kwB":"由人民检察院提出，不服一审判决/裁定","analysis":"本案中提出异议的主体是被告人甲，而非人民检察院，其不服一审判决、向上级法院要求改判的行为，属于上诉，而非抗诉。","answer":"A"},{"id":14,"subject":"民诉法","stem":"原告起诉被告还款10万，被告主张原告还欠自己5万，要求抵消。被告的主张是？","optionA":"反诉","optionB":"反驳","kwQ":"欠自己5万、抵消、独立请求","kwA":"提出独立的诉讼请求，意图吞并/抵消本诉请求","kwB":"仅否定原告的诉讼主张，无独立的诉讼请求","analysis":"被告主张原告欠自己5万，并要求抵消原告的10万还款请求，该主张是独立于本诉（原告要求还款10万）的诉讼请求，并非单纯否定原告的主张，符合反诉的构成要件。","answer":"A"},{"id":15,"subject":"民诉法","stem":"甲起诉乙要求返还房屋，丙主张自己才是房屋所有权人，要求甲乙返还房屋。丙是？","optionA":"有独立请求权第三人","optionB":"无独立请求权第三人","kwQ":"主张所有权、独立请求（要求甲乙返还房屋）","kwA":"对原、被告争议的标的物有独立的所有权/请求权，相当于原告","kwB":"对原、被告争议无独立请求权，仅与案件结果有利害关系","analysis":"丙主张自己是房屋所有权人，要求原、被告甲乙返还房屋，其对该房屋享有独立的所有权请求权，并非仅与案件结果有利害关系，符合有独立请求权第三人的构成要件。","answer":"A"},{"id":16,"subject":"行政法","stem":"公务员甲因违纪被单位给予记过处理。该行为是？","optionA":"行政处分","optionB":"行政处罚","kwQ":"公务员、记过、单位处理（内部）","kwA":"行政机关对内部公务员的惩戒，属于内部行政行为","kwB":"行政机关对外部行政相对人的处罚，属于外部行政行为","analysis":"甲是公务员，其被单位给予记过处理，属于行政机关对内部工作人员的惩戒，是内部行政行为，符合行政处分的构成要件；行政处罚针对的是外部相对人，本案不适用。","answer":"A"},{"id":17,"subject":"行政法","stem":"市场监管局给甲颁发营业执照，允许甲经营超市。该行为是？","optionA":"行政许可","optionB":"行政确认","kwQ":"允许经营、颁发营业执照、赋予权利","kwA":"赋予行政相对人新的权利，从“无”到“有”","kwB":"确认行政相对人已有的权利/事实，从“有”到“认”","analysis":"甲原本无经营超市的合法权利，市场监管局颁发营业执照，允许其经营超市，是赋予甲新的经营权利，属于行政许可；行政确认仅为确认已有权利，本案不符合行政确认的要件。","answer":"A"},{"id":18,"subject":"刑法","stem":"甲为索要债务，将乙控制在出租屋，不让其离开，未向第三人索财。甲构成？","optionA":"绑架罪","optionB":"非法拘禁罪","kwQ":"索要债务、控制人身、无第三人索财","kwA":"控制人身自由+向第三人勒索财物/提出不法要求","kwB":"单纯剥夺人身自由，无向第三人索财/提不法要求的目的","analysis":"甲仅为索要债务，控制乙的人身自由，未向任何第三人勒索财物或提出不法要求，其核心目的是剥夺乙的人身自由，符合非法拘禁罪的构成要件；绑架罪要求向第三人索财，本案不构成绑架罪。","answer":"B"},{"id":19,"subject":"刑法","stem":"甲一枪打死乙，同时打碎乙身边的珍贵文物，一行为触犯故意杀人罪和故意毁坏财物罪。属于？","optionA":"想象竞合","optionB":"法条竞合","kwQ":"一行为、两罪、无包容关系","kwA":"一行为同时触犯数个无包容关系的罪名，择一重罪处罚","kwB":"一行为仅符合一个罪名，因法条之间有包容关系而看似触犯数罪","analysis":"甲的一个开枪行为，同时触犯故意杀人罪和故意毁坏财物罪，两罪之间无包容关系（故意杀人罪不包含故意毁坏财物罪，反之亦然），属于想象竞合；法条竞合要求法条之间有包容关系，本案不符合。","answer":"A"},{"id":20,"subject":"民法","stem":"甲故意隐瞒房屋漏水事实，将房屋卖给不知情的乙。该买卖合同？","optionA":"可撤销","optionB":"无效","kwQ":"隐瞒事实、欺诈、不知情","kwA":"因欺诈、胁迫、重大误解等情形，撤销前有效，撤销后自始无效","kwB":"违反法律强制性规定/公序良俗，自始、绝对无效","analysis":"甲故意隐瞒房屋漏水事实（欺诈行为），使乙在不知情的情况下签订买卖合同，该行为属于可撤销民事法律行为（乙可主张撤销），并非违反法律强制性规定或公序良俗的无效行为。","answer":"A"},{"id":21,"subject":"民法","stem":"甲误将乙的快递当成自己的签收使用，拒不返还。甲构成？","optionA":"不当得利","optionB":"无因管理","kwQ":"误收、使用、拒不返还、无主动管理","kwA":"无合法依据获利+他人受损，无需主动管理","kwB":"为避免他人受损主动管理，可请求费用补偿","analysis":"甲误将乙的快递当成自己的签收使用，属于无合法依据获得利益，且导致乙的财产受损，其行为未体现“主动为他人管理事务”的核心，符合不当得利的构成要件，不构成无因管理。","answer":"A"},{"id":22,"subject":"刑法","stem":"甲因盗窃被公安机关抓获后，主动如实供述自己的盗窃罪行。甲的行为是？","optionA":"自首","optionB":"坦白","kwQ":"被抓获后、如实供述、被动归案","kwA":"自动投案+如实供述自己的罪行","kwB":"被动归案+如实供述自己的罪行","analysis":"甲是被公安机关抓获后被动归案，并非主动向司法机关投案，其如实供述自己盗窃罪行的行为，符合坦白的构成要件；自首要求主动投案，本案不构成自首。","answer":"B"},{"id":23,"subject":"刑法","stem":"甲因故意伤害被逮捕后，揭发同案犯的抢劫罪行，经查证属实。甲的行为是？","optionA":"立功","optionB":"坦白","kwQ":"揭发同案犯抢劫罪行、查证属实","kwA":"揭发他人犯罪行为、提供重要线索，经查证属实","kwB":"仅如实供述自己的犯罪行为，不涉及他人","analysis":"甲揭发的是同案犯的抢劫罪行（他人犯罪行为），且经查证属实，符合立功的构成要件；坦白仅要求供述自己的罪行，不包含揭发他人犯罪，本案不构成坦白。","answer":"A"},{"id":24,"subject":"民法","stem":"甲、乙各出资50万元购买房屋，约定按出资比例享有权利、承担义务。该共有方式是？","optionA":"按份共有","optionB":"共同共有","kwQ":"各出资50万、按出资比例、明确份额","kwA":"按明确份额享有权利、承担义务，可自由处分自有份额","kwB":"不分份额，共同享有权利、承担义务，处分需全体同意","analysis":"甲、乙明确约定按出资比例享有权利、承担义务，存在明确的共有份额，符合按份共有的构成要件；共同共有不分份额，本案不符合共同共有的特征。","answer":"A"},{"id":25,"subject":"刑诉法","stem":"甲涉嫌盗窃罪，可能判处2年有期徒刑，认罪认罚，案情简单，法院适用独任制审理并当庭宣判。该程序是？","optionA":"简易程序","optionB":"速裁程序","kwQ":"可能判处2年、认罪认罚、独任制、当庭宣判","kwA":"基层法院、事实清楚、认罪，可合议/独任，不一定当庭宣判","kwB":"基层法院、3年以下、认罪认罚、速审，独任制、当庭宣判","analysis":"甲涉嫌盗窃罪，可能判处2年有期徒刑（3年以下），且认罪认罚、案情简单，法院适用独任制审理并当庭宣判，完全符合速裁程序的核心特征；简易程序可合议审理，且不一定当庭宣判，本案不适用简易程序。","answer":"B"},{"id":26,"subject":"刑诉法","stem":"甲因琐事被乙殴打，造成轻微伤，甲直接向法院起诉要求乙承担刑事责任。该案件是？","optionA":"自诉案件","optionB":"公诉案件","kwQ":"轻微伤、直接向法院起诉、轻微刑事案件","kwA":"被害人直接起诉，包括轻微刑事案件、告诉才处理的案件","kwB":"由人民检察院代表国家提起公诉，绝大多数刑事案件","analysis":"甲被乙殴打致轻微伤，属于轻微刑事案件，甲直接向法院起诉，符合自诉案件“被害人直接起诉、案件轻微”的特征；公诉案件需由检察院提起公诉，本案不构成公诉案件。","answer":"A"},{"id":27,"subject":"民诉法","stem":"原告向A法院起诉被告，被告认为A法院对本案无管辖权，向A法院提出异议。该行为是？","optionA":"管辖权异议","optionB":"移送管辖","kwQ":"被告提出、认为A法院无管辖权、向受理法院提出","kwA":"由被告向受理案件的法院提出，主张法院无管辖权","kwB":"由法院主动将案件移送给有管辖权的法院","analysis":"本案中，提出“法院无管辖权”主张的是被告，且是向受理案件的A法院提出，符合管辖权异议的构成要件；移送管辖是法院主动作出的行为，并非当事人提出，本案不构成移送管辖。","answer":"A"},{"id":28,"subject":"行政法","stem":"甲对市场监管局的罚款处罚不服，向市场监管局的上级机关申请审查。该行为是？","optionA":"行政复议","optionB":"行政诉讼","kwQ":"不服罚款、向上级机关申请审查、行政内部监督","kwA":"向作出行政行为的上级行政机关申请审查，属于行政内部监督","kwB":"向法院提起诉讼，属于司法监督","analysis":"甲不服市场监管局的罚款处罚，向其上级机关申请审查，属于行政机关内部的监督方式，符合行政复议的构成要件；行政诉讼需向法院提起，本案不构成行政诉讼。","answer":"A"},{"id":29,"subject":"理论法","stem":"“故意杀人的，处死刑、无期徒刑或者十年以上有期徒刑”，该规定属于？","optionA":"法律规则","optionB":"法律原则","kwQ":"具体明确、可直接适用、规定具体处罚","kwA":"内容具体、明确，可直接适用于具体案件，有明确的行为模式和法律后果","kwB":"内容抽象、概括，需结合案件权衡适用，无具体行为模式和法律后果","analysis":"该规定明确了“故意杀人”这一行为模式，以及对应的“死刑、无期徒刑或者十年以上有期徒刑”的法律后果，内容具体明确，可直接适用于故意杀人案件，符合法律规则的构成要件；法律原则抽象概括，无具体处罚规定，本案不符合。","answer":"A"},{"id":30,"subject":"刑法","stem":"甲因诈骗罪被判处3年有期徒刑，法院判决时决定附条件不执行原判刑罚，考验期2年。该制度是？","optionA":"缓刑","optionB":"假释","kwQ":"判决时、附条件不执行原判、考验期","kwA":"判决时作出，附条件不执行原判刑罚，考验期内无违法犯罪即不执行原判","kwB":"执行一定刑期后作出，附条件提前释放，考验期内无违法犯罪即原判执行完毕","analysis":"甲被判处3年有期徒刑，法院在判决时即决定附条件不执行原判刑罚，符合缓刑“判决时适用、不执行原判”的核心特征；假释需在刑罚执行一定刑期后适用，本案不构成假释。","answer":"A"}];

var STATE_KEY = 'kw_mobile_v1';
var state = loadState();
var currentFilter = 'all';

function loadState() {
  try { var s = localStorage.getItem(STATE_KEY); if (s) return JSON.parse(s); } catch(e) {}
  return { answers: {}, expanded: {} };
}
function saveState() {
  try { localStorage.setItem(STATE_KEY, JSON.stringify(state)); } catch(e) {}
}

function getAnswer(qid) { return state.answers[qid] || null; }
function setAnswer(qid, choice) {
  state.answers[qid] = choice;
  saveState();
  updateStats();
}
function isExpanded(qid) { return !!state.expanded[qid]; }

function renderQuestions() {
  var area = document.getElementById('cardArea');
  var filtered = currentFilter === 'all'
    ? questions
    : questions.filter(function(q) { return q.subject === currentFilter; });

  if (filtered.length === 0) {
    area.innerHTML = '<div class="empty-state"><div class="icon">📭</div><div class="msg">该分类暂无题目</div></div>';
    return;
  }

  area.innerHTML = filtered.map(function(q) {
    var userAnswer = getAnswer(q.id);
    var expanded = isExpanded(q.id) || !!userAnswer;
    var isCorrect = userAnswer === q.answer;

    var cardClass = 'question-card';
    if (expanded) cardClass += ' expanded';
    if (userAnswer && isCorrect) cardClass += ' answered-correct';
    if (userAnswer && !isCorrect) cardClass += ' answered-wrong';

    function optClass(opt) {
      if (!userAnswer) return '';
      if (opt === q.answer) return 'correct-choice';
      if (opt === userAnswer && userAnswer !== q.answer) return 'wrong-choice';
      return '';
    }

    var h = '<div class="' + cardClass + '" id="card-' + q.id + '">';
    h += '<div class="card-top" onclick="toggleCard(' + q.id + ')">';
    h += '<div class="card-num">' + String(q.id).padStart(2,'0') + '</div>';
    h += '<div class="card-info">';
    h += '<div class="card-subject">' + esc(q.subject) + '</div>';
    h += '<div class="card-stem">' + esc(q.stem) + '</div>';
    h += '</div>';
    h += '<div class="card-arrow">▼</div>';
    h += '</div>';
    h += '<div class="card-body"><div class="card-body-inner">';
    h += '<div class="options">';
    h += '<button class="option-btn ' + optClass('A') + '" ontouchstart="" onclick="event.stopPropagation();selectAnswer(' + q.id + ',\'A\')">';
    h += '<span class="option-letter">A</span><span>' + esc(q.optionA) + '</span></button>';
    h += '<button class="option-btn ' + optClass('B') + '" ontouchstart="" onclick="event.stopPropagation();selectAnswer(' + q.id + ',\'B\')">';
    h += '<span class="option-letter">B</span><span>' + esc(q.optionB) + '</span></button>';
    h += '</div>';

    if (userAnswer) {
      h += '<div class="reveal-section">';
      h += '<div class="answer-badge ' + (isCorrect ? 'correct' : 'wrong') + '">';
      h += isCorrect ? '✓ 回答正确' : '✗ 回答错误 · 正确答案 ' + q.answer;
      h += '</div>';
      h += '<div class="kw-info"><div class="kw-label">📋 题干关键词</div>' + esc(q.kwQ) + '</div>';
      h += '<div class="keyword-compare">';
      h += '<div class="keyword-col col-a"><div class="col-label">A · ' + esc(q.optionA) + '</div><div class="col-kw">' + esc(q.kwA) + '</div></div>';
      h += '<div class="keyword-col col-b"><div class="col-label">B · ' + esc(q.optionB) + '</div><div class="col-kw">' + esc(q.kwB) + '</div></div>';
      h += '</div>';
      h += '<div class="analysis-box"><div class="analysis-label">💡 解析</div><div class="analysis-text">' + esc(q.analysis) + '</div></div>';
      h += '</div>';
    }

    h += '</div></div></div>';
    return h;
  }).join('');

  requestAnimationFrame(function() {
    var reveals = document.querySelectorAll('.reveal-section');
    for (var i = 0; i < reveals.length; i++) reveals[i].classList.add('visible');
  });
}

function esc(s) {
  return s.replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;').replace(/"/g, '&quot;');
}

function toggleCard(id) {
  state.expanded[id] = !isExpanded(id);
  saveState();
  renderQuestions();
}

function selectAnswer(id, choice) {
  if (getAnswer(id)) return;
  setAnswer(id, choice);
  state.expanded[id] = true;
  saveState();

  var q = questions.find(function(qq) { return qq.id === id; });
  var isCorrect = choice === q.answer;

  showToast(isCorrect ? '✓ 正确！继续加油' : '✗ 回答错误，查看解析');

  if (isCorrect) {
    spawnConfetti();
    showCelebration();
  }

  renderQuestions();

  setTimeout(function() {
    var card = document.getElementById('card-' + id);
    if (card) card.scrollIntoView({ behavior: 'smooth', block: 'center' });
  }, 100);

  setTimeout(function() {
    var reveal = document.querySelector('#card-' + id + ' .reveal-section');
    if (reveal) reveal.classList.add('visible');
  }, 150);
}

function updateStats() {
  var total = questions.length;
  var keys = Object.keys(state.answers);
  var answered = keys.length;
  var correct = 0;
  for (var i = 0; i < keys.length; i++) {
    var q = questions.find(function(qq) { return qq.id === parseInt(keys[i]); });
    if (q && state.answers[keys[i]] === q.answer) correct++;
  }

  var acc = answered > 0 ? Math.round(correct / answered * 100) + '%' : '—';
  document.getElementById('statDone').textContent = answered;
  document.getElementById('statAccuracy').textContent = acc;
  document.getElementById('progressFill').style.width = (answered / total * 100) + '%';
}

function showToast(msg) {
  var t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  clearTimeout(t._t);
  t._t = setTimeout(function() { t.classList.remove('show'); }, 1800);
}

function showCelebration() {
  var c = document.getElementById('celebration');
  var emojis = ['🎉','✨','👏','💪','🔥','✅','🌟'];
  c.querySelector('.emoji').textContent = emojis[Math.floor(Math.random() * emojis.length)];
  c.classList.add('show');
  setTimeout(function() { c.classList.remove('show'); }, 700);
}

function spawnConfetti() {
  var colors = ['#3b82f6','#8b5cf6','#f59e0b','#10b981','#ef4444','#06b6d4','#ec4899'];
  for (var i = 0; i < 50; i++) {
    var p = document.createElement('div');
    p.className = 'confetti-piece';
    p.style.left = Math.random() * 100 + '%';
    p.style.top = -(Math.random() * 30 + 10) + 'px';
    p.style.width = (Math.random() * 8 + 5) + 'px';
    p.style.height = (Math.random() * 8 + 5) + 'px';
    p.style.background = colors[Math.floor(Math.random() * colors.length)];
    p.style.borderRadius = Math.random() > 0.5 ? '50%' : '2px';
    p.style.animationDuration = (Math.random() * 1.5 + 1.2) + 's';
    p.style.animationDelay = Math.random() * 0.3 + 's';
    document.body.appendChild(p);
    setTimeout(function() { p.remove(); }, 2200);
  }
}

// Filter
document.getElementById('filterRow').addEventListener('click', function(e) {
  if (!e.target.classList.contains('filter-chip')) return;
  var chips = document.querySelectorAll('.filter-chip');
  for (var i = 0; i < chips.length; i++) chips[i].classList.remove('active');
  e.target.classList.add('active');
  currentFilter = e.target.dataset.filter;
  renderQuestions();
});

function expandAll() {
  questions.forEach(function(q) { state.expanded[q.id] = true; });
  saveState();
  renderQuestions();
}
function collapseAll() {
  questions.forEach(function(q) { state.expanded[q.id] = false; });
  saveState();
  renderQuestions();
}
function resetAll() {
  if (confirm('确定要重置所有答题记录吗？此操作不可撤销。')) {
    state = { answers: {}, expanded: {} };
    saveState();
    renderQuestions();
    updateStats();
    showToast('已重置全部进度');
  }
}

function toggleTheme() {
  var h = document.documentElement;
  var cur = h.getAttribute('data-theme');
  h.setAttribute('data-theme', cur === 'light' ? '' : 'light');
  try { localStorage.setItem('kw_mobile_theme', cur === 'light' ? '' : 'light'); } catch(e) {}
}

// Share
function openShare() {
  document.getElementById('shareOverlay').classList.add('show');
}
function closeShare() {
  document.getElementById('shareOverlay').classList.remove('show');
}
function doShare(type) {
  var url = window.location.href;
  var title = '二选一"关键词比对法"训练题集';
  var desc = '30道法考精选易混题型 · 三步拆解 · 精准提分';
  closeShare();

  if (type === 'copy') {
    if (navigator.clipboard) {
      navigator.clipboard.writeText(url).then(function() {
        showToast('链接已复制，快去分享吧');
      });
    } else {
      var ta = document.createElement('textarea');
      ta.value = url; ta.style.position = 'fixed'; ta.style.opacity = '0';
      document.body.appendChild(ta); ta.select();
      document.execCommand('copy'); document.body.removeChild(ta);
      showToast('链接已复制，快去分享吧');
    }
  } else if (type === 'wechat' || type === 'moments') {
    showToast('请点击右上角 ··· 分享给朋友');
  } else if (type === 'more') {
    if (navigator.share) {
      navigator.share({ title: title, text: desc, url: url });
    } else {
      showToast('请点击右上角 ··· 选择分享方式');
    }
  }
}

// Swipe right on empty area to go back / collapse
var touchStartX = 0;
document.addEventListener('touchstart', function(e) { touchStartX = e.touches[0].clientX; }, {passive: true});

function init() {
  try {
    var t = localStorage.getItem('kw_mobile_theme');
    if (t) document.documentElement.setAttribute('data-theme', t);
  } catch(e) {}
  document.getElementById('statTotal').textContent = questions.length;
  renderQuestions();
  updateStats();
}

init();
</script>
</body>
</html>
