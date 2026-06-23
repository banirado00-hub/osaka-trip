<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>오사카 with 탱파 🇯🇵</title>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: -apple-system, 'Noto Sans KR', sans-serif; background: #f7f5f0; color: #1a1a1a; min-height: 100vh; }
  .top { background: #fff; text-align: center; padding: 24px 16px 16px; border-bottom: 1px solid #eee; }
  .top h1 { font-size: 20px; font-weight: 600; }
  .top .sub { font-size: 13px; color: #888; margin-top: 4px; }
  .info-bar { background: #fff; margin: 12px 16px; border-radius: 12px; padding: 12px 16px; border: 1px solid #eee; }
  .info-row { display: flex; gap: 10px; font-size: 13px; color: #555; margin-bottom: 6px; }
  .info-row:last-child { margin-bottom: 0; }
  .info-label { font-weight: 600; color: #1a1a1a; min-width: 28px; }
  .tabs { display: flex; gap: 8px; padding: 12px 16px; }
  .tab { flex: 1; padding: 10px 0; border-radius: 10px; background: #fff; border: 1px solid #e0ddd6; font-size: 14px; font-weight: 500; color: #888; cursor: pointer; text-align: center; transition: all 0.15s; }
  .tab.active { background: #1a9e60; color: #fff; border-color: #1a9e60; }
  .section { display: none; padding: 0 16px 100px; }
  .section.active { display: block; }
  .day-label { font-size: 12px; font-weight: 600; color: #888; margin-bottom: 16px; padding-bottom: 8px; border-bottom: 1px solid #e8e5de; }
  .timeline { position: relative; padding-left: 76px; }
  .timeline::before { content: ''; position: absolute; left: 58px; top: 4px; bottom: 4px; width: 1.5px; background: #e0ddd6; }
  .event { position: relative; margin-bottom: 12px; }
  .event-time { position: absolute; left: -76px; width: 52px; text-align: right; font-size: 11px; font-weight: 700; color: #1a9e60; padding-top: 3px; }
  .event-dot { position: absolute; left: -22px; top: 6px; width: 10px; height: 10px; border-radius: 50%; background: #1a9e60; border: 2.5px solid #f7f5f0; z-index: 1; }
  .event-dot.hl { background: #d85a30; }
  .event-card { background: #fff; border: 1px solid #eee; border-radius: 10px; padding: 9px 14px; display: flex; justify-content: space-between; align-items: center; }
  .event-card.hl { border-color: #f0997b; background: #fff8f5; }
  .event-info { flex: 1; }
  .event-title { font-size: 14px; font-weight: 500; color: #1a1a1a; }
  .event-card.hl .event-title { color: #c04020; }
  .event-note { font-size: 12px; color: #888; margin-top: 3px; }
  .event-card.hl .event-note { color: #d85a30; }
  .event-del { font-size: 16px; color: #ccc; padding: 4px 4px 4px 10px; flex-shrink: 0; display: none; cursor: pointer; }
  .edit-mode .event-del { display: block; }
  .event-del:hover { color: #e74c3c; }
  .badge { display: inline-block; font-size: 10px; font-weight: 700; padding: 2px 7px; border-radius: 20px; margin-left: 6px; background: #1a9e60; color: #fff; vertical-align: middle; }
  .badge.red { background: #d85a30; }
  .add-btn { display: flex; align-items: center; justify-content: center; gap: 8px; background: #fff; border: 1.5px dashed #ccc; border-radius: 10px; padding: 10px 14px; color: #aaa; font-size: 13px; cursor: pointer; margin-top: 8px; width: 100%; }
  .add-btn:hover { border-color: #1a9e60; color: #1a9e60; }
  .bottom-bar { position: fixed; bottom: 0; left: 0; right: 0; background: #fff; border-top: 1px solid #eee; padding: 10px 16px 6px; display: flex; flex-direction: column; gap: 6px; }
  .bottom-btns { display: flex; gap: 8px; }
  .edit-toggle { flex: 1; padding: 10px; border-radius: 10px; border: 1px solid #e0ddd6; background: #fff; font-size: 14px; font-weight: 500; color: #555; cursor: pointer; }
  .edit-toggle.on { background: #fff3e0; border-color: #ffb74d; color: #e65100; }
  .map-btn { flex: 1; display: flex; align-items: center; justify-content: center; padding: 10px; border-radius: 10px; background: #e8f5ee; border: 1px solid #a3d4b8; font-size: 14px; font-weight: 500; color: #1a6640; text-decoration: none; }
  .map-btn:hover { background: #d0edde; }
  .sync-status { font-size: 11px; color: #aaa; text-align: center; padding: 2px 0; }
  .sync-status.ok { color: #1a9e60; }
  .sync-status.err { color: #e74c3c; }
  .sync-status { font-size: 11px; color: #aaa; text-align: center; padding: 4px 0 0; }
  .sync-status.ok { color: #1a9e60; }
  .sync-status.err { color: #e74c3c; }
  .modal-bg { display: none; position: fixed; inset: 0; background: rgba(0,0,0,0.4); z-index: 100; align-items: flex-end; }
  .modal-bg.show { display: flex; }
  .modal { background: #fff; border-radius: 20px 20px 0 0; padding: 24px 20px 40px; width: 100%; }
  .modal h3 { font-size: 16px; font-weight: 600; margin-bottom: 4px; }
  .modal label { font-size: 12px; color: #888; display: block; margin-bottom: 4px; margin-top: 12px; }
  .modal input { width: 100%; padding: 10px 12px; border-radius: 8px; border: 1px solid #ddd; font-size: 14px; background: #fff; }
  .modal-row { display: flex; gap: 8px; margin-top: 16px; }
  .modal-btn { flex: 1; padding: 12px; border-radius: 10px; border: none; font-size: 14px; font-weight: 600; cursor: pointer; }
  .modal-btn.cancel { background: #f5f5f5; color: #555; }
  .modal-btn.save { background: #1a9e60; color: #fff; }
  .hl-toggle { display: flex; align-items: center; gap: 8px; margin-top: 12px; }
  .hl-toggle input[type=checkbox] { width: auto; }
  .hl-toggle label { margin: 0; font-size: 14px; color: #555; }
  .loading { text-align: center; padding: 40px; color: #aaa; font-size: 14px; }
</style>
</head>
<body>

<div class="top">
  <h1>🇯🇵 오사카 with 탱파</h1>
  <div class="sub">2026년 7월 10일(금) – 12일(일) &nbsp;·&nbsp; 2박 3일</div>
</div>

<div class="info-bar">
  <div class="info-row"><span class="info-label">✈️</span><span>제주항공 7C1325 (08:10→10:00) / 7C1328 (16:30→18:15)</span></div>
  <div class="info-row"><span class="info-label">🏠</span><span>신이마미애역 근처 에어비앤비</span></div>
</div>

<div class="tabs">
  <div class="tab active" onclick="showDay(0,this)">7/10 금</div>
  <div class="tab" onclick="showDay(1,this)">7/11 토</div>
  <div class="tab" onclick="showDay(2,this)">7/12 일</div>
</div>

<div class="section active" id="day-0">
  <div class="day-label">7월 10일 (금) — 출발</div>
  <div class="timeline" id="tl-0"><div class="loading">불러오는 중...</div></div>
  <button class="add-btn" onclick="openModal(0)">＋ 일정 추가</button>
</div>
<div class="section" id="day-1">
  <div class="day-label">7월 11일 (토) — 관광</div>
  <div class="timeline" id="tl-1"><div class="loading">불러오는 중...</div></div>
  <button class="add-btn" onclick="openModal(1)">＋ 일정 추가</button>
</div>
<div class="section" id="day-2">
  <div class="day-label">7월 12일 (일) — 귀국</div>
  <div class="timeline" id="tl-2"><div class="loading">불러오는 중...</div></div>
  <button class="add-btn" onclick="openModal(2)">＋ 일정 추가</button>
</div>

<div class="bottom-bar">
  <div class="bottom-btns">
    <a href="https://maps.app.goo.gl/tDschPfNyMwpn5fv8?g_st=i" target="_blank" class="map-btn">🗺 구글맵 보기</a>
    <button class="edit-toggle" id="edit-toggle" onclick="toggleEdit()">✏️ 편집 모드</button>
  </div>
  <div class="sync-status" id="sync-status">실시간 연결 중...</div>
</div>

<div class="modal-bg" id="modal-bg" onclick="closeModal(event)">
  <div class="modal">
    <h3 id="modal-title">일정 추가</h3>
    <label>시간</label>
    <input type="time" id="inp-time" />
    <label>일정</label>
    <input type="text" id="inp-title" placeholder="예: 도톤보리 산책" />
    <label>비고 (선택)</label>
    <input type="text" id="inp-note" placeholder="예: 지하철 4번 출구" />
    <div class="hl-toggle">
      <input type="checkbox" id="inp-hl" />
      <label for="inp-hl">🟠 예약 완료 표시</label>
    </div>
    <div class="modal-row">
      <button class="modal-btn cancel" onclick="document.getElementById('modal-bg').classList.remove('show')">취소</button>
      <button class="modal-btn save" onclick="saveEvent()">저장</button>
    </div>
  </div>
</div>

<script>
const DB = 'https://osaka-2e208-default-rtdb.firebaseio.com/schedule';

const DEFAULT = [
  [
    {time:'05:00',title:'집에서 출발',note:'택시 이용',hl:false},
    {time:'06:00',title:'김포공항 도착',note:'',hl:false},
    {time:'08:10',title:'김포공항 출발',note:'7C1325',hl:false},
    {time:'10:00',title:'간사이공항 T2 도착',note:'',hl:false},
    {time:'12:00',title:'난카이항선 탑승',note:'1T 이동',hl:false},
    {time:'13:00',title:'호텔 짐 보관',note:'',hl:false},
  ],
  [
    {time:'09:00',title:'숙소 출발',note:'',hl:false},
    {time:'10:00',title:'나카자키초 스냅촬영',note:'4번 출구 / 약 1시간 소요',hl:false},
    {time:'11:30',title:'점심',note:'',hl:false},
    {time:'18:30',title:'Wagyu Yakiniku Hishimekiya',note:'주문 예약 완료',hl:true},
  ],
  [
    {time:'13:30',title:'숙소 → 공항 출발',note:'',hl:false},
    {time:'14:30',title:'간사이공항 2T 도착',note:'',hl:false},
    {time:'16:30',title:'간사이공항 T2 출발',note:'7C1328',hl:false},
    {time:'18:15',title:'김포공항 도착',note:'',hl:false},
  ]
];

let data = [[], [], []];
let editMode = false;
let modalDay = 0;
let editKey = null;

function setStatus(msg, cls) {
  const el = document.getElementById('sync-status');
  el.textContent = msg;
  el.className = 'sync-status' + (cls ? ' '+cls : '');
}

// Firebase REST API로 실시간 감지 (SSE)
function startListen() {
  const es = new EventSource(DB + '.json');
  es.onopen = () => setStatus('🟢 실시간 연결됨', 'ok');
  es.onmessage = (e) => {
    try {
      const parsed = JSON.parse(e.data);
      if (!parsed || !parsed.data) return;
      const raw = JSON.parse(parsed.data);
      if (raw && Array.isArray(raw)) {
        data = raw;
        render();
      }
    } catch(err) {}
  };
  es.onerror = () => {
    setStatus('⚠️ 연결 끊김 — 새로고침 해주세요', 'err');
    es.close();
    setTimeout(startListen, 3000);
  };
}

// 데이터 저장
function pushData() {
  setStatus('저장 중...', '');
  fetch(DB + '.json', {
    method: 'PUT',
    headers: {'Content-Type': 'application/json'},
    body: JSON.stringify(data)
  })
  .then(r => r.json())
  .then(() => setStatus('🟢 저장 완료', 'ok'))
  .catch(() => setStatus('❌ 저장 실패', 'err'));
}

// 초기 데이터 로드 (처음 한 번)
fetch(DB + '.json')
  .then(r => r.json())
  .then(raw => {
    if (raw && Array.isArray(raw)) {
      data = raw;
    } else {
      // 첫 실행 — 기본 데이터 업로드
      data = DEFAULT;
      pushData();
    }
    render();
    startListen();
  })
  .catch(() => {
    data = DEFAULT;
    render();
    setStatus('❌ Firebase 연결 실패', 'err');
  });

function render() {
  data.forEach((evts, di) => {
    const tl = document.getElementById('tl-'+di);
    if (!evts || evts.length === 0) { tl.innerHTML = ''; return; }
    const sorted = [...evts].map((e,i) => ({...e, _i:i})).sort((a,b) => a.time.localeCompare(b.time));
    tl.innerHTML = sorted.map(e =>
      '<div class="event">'
      + '<div class="event-time"' + (e.hl?' style="color:#d85a30"':'') + '>' + e.time + '</div>'
      + '<div class="event-dot' + (e.hl?' hl':'') + '"></div>'
      + '<div class="event-card' + (e.hl?' hl':'') + '" onclick="' + (editMode?'openModal('+di+','+e._i+')':'') + '">'
      + '<div class="event-info">'
      + '<div class="event-title">' + e.title + (e.hl?'<span class="badge red">예약완료</span>':'') + '</div>'
      + (e.note?'<div class="event-note">'+e.note+'</div>':'')
      + '</div>'
      + '<span class="event-del" onclick="event.stopPropagation();delEvent('+di+','+e._i+')">✕</span>'
      + '</div></div>'
    ).join('');
    if (editMode) tl.classList.add('edit-mode');
    else tl.classList.remove('edit-mode');
  });
}

function showDay(idx, el) {
  document.querySelectorAll('.section').forEach((s,i) => s.classList.toggle('active', i===idx));
  document.querySelectorAll('.tab').forEach((t,i) => t.classList.toggle('active', i===idx));
}

function toggleEdit() {
  editMode = !editMode;
  const btn = document.getElementById('edit-toggle');
  btn.textContent = editMode ? '✅ 편집 완료' : '✏️ 편집 모드';
  btn.className = 'edit-toggle' + (editMode?' on':'');
  render();
}

function openModal(day, idx=null) {
  if (!editMode) return;
  modalDay = day; editKey = idx;
  document.getElementById('modal-title').textContent = idx===null ? '일정 추가' : '일정 수정';
  if (idx !== null) {
    const e = data[day][idx];
    document.getElementById('inp-time').value = e.time;
    document.getElementById('inp-title').value = e.title;
    document.getElementById('inp-note').value = e.note;
    document.getElementById('inp-hl').checked = e.hl;
  } else {
    document.getElementById('inp-time').value = '';
    document.getElementById('inp-title').value = '';
    document.getElementById('inp-note').value = '';
    document.getElementById('inp-hl').checked = false;
  }
  document.getElementById('modal-bg').classList.add('show');
}

function closeModal(e) {
  if (e && e.target !== document.getElementById('modal-bg')) return;
  document.getElementById('modal-bg').classList.remove('show');
}

function saveEvent() {
  const time = document.getElementById('inp-time').value;
  const title = document.getElementById('inp-title').value.trim();
  if (!time || !title) { alert('시간과 일정을 입력해주세요'); return; }
  const ev = {time, title, note: document.getElementById('inp-note').value.trim(), hl: document.getElementById('inp-hl').checked};
  if (editKey !== null) data[modalDay][editKey] = ev;
  else data[modalDay].push(ev);
  pushData();
  render();
  document.getElementById('modal-bg').classList.remove('show');
}

function delEvent(day, idx) {
  if (!confirm('이 일정을 삭제할까요?')) return;
  data[day].splice(idx, 1);
  pushData();
  render();
}
</script>
</body>
</html>
