<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>KelasKu – Absensi & Nilai</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@600;700&family=Figtree:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --papan:#1457c8; --papan-2:#2a72e0; --kapur:#e6f2ff;
  --kertas:#f7fbff; --garis:#c8dcf5; --tinta:#14264a; --abu:#4a5d80;
  --stabilo:#ffe066; --merah:#e5503f; --laut:#1f6fe5; --biru:#2f64d6;
  --radius:16px;
}
*{box-sizing:border-box}
html,body{height:100%}
body{margin:0;font-family:Figtree,system-ui,sans-serif;color:var(--tinta);background:transparent;font-size:15px;line-height:1.5}
h1,h2,h3{font-family:'Bricolage Grotesque',Figtree,sans-serif;margin:0;line-height:1.15}
button,input,select,textarea{font:inherit;color:inherit}
button{cursor:pointer}
:focus-visible{outline:3px solid var(--biru);outline-offset:2px}
 
.app{display:grid;grid-template-columns:230px 1fr;min-height:100%}
aside{background:linear-gradient(180deg,#1760d4 0%,#0f46a8 55%,#0a2f78 100%);box-shadow:4px 0 22px rgba(10,45,117,.28);color:var(--kapur);padding:20px 14px;position:sticky;top:0;height:100vh;display:flex;flex-direction:column;gap:18px}
aside .brand{font-family:'Bricolage Grotesque',sans-serif;font-size:24px;font-weight:700;padding:0 8px;display:flex;align-items:center;gap:8px;line-height:1.1}
aside .brand .logo svg{width:46px;height:auto;display:block}
aside .brand small{display:block;font:400 12px Figtree,sans-serif;opacity:.7}
nav{display:flex;flex-direction:column;gap:2px}
nav button{background:none;border:0;color:inherit;text-align:left;padding:10px 12px;border-radius:8px;opacity:.85}
nav button:hover{background:var(--papan-2)}
nav button.on{background:var(--kapur);color:var(--papan);font-weight:600;opacity:1}
.side-art{margin-top:auto;display:flex;justify-content:center}
.side-art svg{width:92px;height:auto}
.side-note{margin-top:6px;font-size:12px;opacity:.75;padding:0 8px}
 
main{padding:22px clamp(14px,3vw,34px) 90px;max-width:1100px;width:100%}
.topbar{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin-bottom:16px;padding:12px 18px;background:rgba(255,255,255,.93);border:2px solid #fff;border-radius:22px;box-shadow:0 8px 24px rgba(10,45,117,.16)}
.topbar label{display:flex;flex-direction:column;font-size:12px;color:var(--abu);gap:2px}
.topbar select{min-width:140px}
.title{margin-right:auto}
.title h1{font-size:28px}
.title p{margin:2px 0 0;color:var(--abu)}
 
select,input[type=text],input[type=number],input[type=date],input[type=month],textarea{
  background:#fff;border:1.5px solid var(--garis);border-radius:8px;padding:8px 10px;min-height:38px;width:100%}
select{width:auto}
textarea{min-height:90px;resize:vertical}
.btn{background:var(--papan);color:#fff;border:0;border-radius:8px;padding:9px 14px;font-weight:600;min-height:38px}
.btn:hover{background:var(--papan-2)}
.btn.ghost{background:#fff;color:var(--papan);border:1.5px solid var(--papan)}
.btn.ghost:hover{background:var(--kapur)}
.btn.danger{background:#fff;color:var(--merah);border:1.5px solid var(--merah)}
.btn.sm{padding:4px 10px;min-height:30px;font-size:13px}
.btn:disabled{opacity:.5;cursor:default}
 
.panel{background:#fff;border:1.5px solid var(--garis);border-radius:var(--radius);padding:16px;margin-bottom:16px;box-shadow:0 3px 10px rgba(15,70,168,.07)}
.panel h2{font-size:19px;margin-bottom:10px}
.row{display:flex;gap:10px;flex-wrap:wrap;align-items:end}
.row>label{display:flex;flex-direction:column;gap:3px;font-size:13px;color:var(--abu);flex:1 1 150px}
.muted{color:var(--abu)}
.small{font-size:13px}
 
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px;margin-bottom:16px}
.stat{background:#fff;border:1.5px solid var(--garis);border-radius:var(--radius);padding:14px}
.stat b{display:block;font:700 30px 'Bricolage Grotesque',sans-serif}
.stat span{color:var(--abu);font-size:13px}
.stat.hl{background:var(--stabilo);border-color:#e6c800}
.stat.hl span{color:#5d5200}
 
.tbl-wrap{overflow-x:auto;border:1.5px solid var(--garis);border-radius:var(--radius);background:#fff}
table{border-collapse:collapse;width:100%;min-width:560px}
th,td{padding:8px 10px;text-align:left;border-bottom:1px solid var(--garis);vertical-align:middle}
th{background:var(--kapur);font-weight:600;font-size:13px;position:sticky;top:0}
tr:last-child td{border-bottom:0}
td.num,th.num{text-align:center}
td input[type=number]{width:74px;text-align:center;padding:5px;min-height:32px}
td input.low{color:var(--merah);font-weight:700;border-color:var(--merah)}
.fin{font-weight:700}
.fin.low{color:var(--merah)}
.badge{display:inline-block;font-size:11px;padding:1px 7px;border-radius:99px;background:var(--stabilo);color:#4a4000;font-weight:600}
.badge.ok{background:#d6e8ff;color:#0f3f91}
.badge.warn{background:#fff0c2;color:#7a5800}
.badge.bad{background:#fde1de;color:#9c2217}
.tiny-in{width:56px!important;min-height:26px!important;padding:2px 4px!important;font-size:12px}
 
.stamps{display:flex;gap:6px}
.stamps button{width:44px;height:36px;border-radius:8px;border:1.5px solid var(--garis);background:#fff;font-weight:700;color:var(--abu)}
.stamps button.on[data-s=H]{background:var(--laut);border-color:var(--laut);color:#fff}
.stamps button.on[data-s=I]{background:#56c2ff;border-color:#2ea9f0;color:#04304f}
.stamps button.on[data-s=S]{background:var(--stabilo);border-color:#e6c800;color:#4a4000}
.stamps button.on[data-s=A]{background:var(--merah);border-color:var(--merah);color:#fff}
 
.tabs{display:inline-flex;border:1.5px solid var(--papan);border-radius:8px;overflow:hidden;margin-bottom:12px}
.tabs button{border:0;background:#fff;padding:7px 14px;color:var(--papan);font-weight:600}
.tabs button.on{background:var(--papan);color:#fff}
.empty{padding:26px;text-align:center;color:var(--abu);border:2px dashed var(--garis);border-radius:var(--radius);background:#fff}
.drop{display:block;border:2px dashed var(--papan-2);border-radius:var(--radius);background:var(--kapur);padding:20px;text-align:center;cursor:pointer}
.drop:hover,.drop.over{background:#d6e8ff;border-color:var(--papan)}
.drop b{display:block;font:700 17px 'Bricolage Grotesque',sans-serif}
.drop input{display:none}
.scroll{max-height:320px;overflow:auto;border:1.5px solid var(--garis);border-radius:var(--radius)}
.scroll table{min-width:0}
.chips{display:flex;gap:6px;flex-wrap:wrap}
.chip{border:1.5px solid var(--garis);background:#fff;border-radius:99px;padding:5px 14px;font-weight:600;color:var(--abu)}
.chip:hover{border-color:var(--papan)}
.chip.on{background:var(--papan);border-color:var(--papan);color:#fff}
.chip:disabled{opacity:.4;cursor:default}
td .note-in{width:100%;min-width:160px;margin-top:4px;font-size:13px;text-align:left}
.grp{background:var(--papan);color:#fff;text-align:center;border-left:3px solid #fff;font-size:14px}
.grp .small{color:#cfe3ff;margin-top:2px}
.grp button{background:transparent;border:1px solid #9fc4f0;color:#fff;border-radius:6px;font-size:12px;padding:0 7px;margin-left:4px;min-height:22px}
.grp button:hover{background:var(--papan-2)}
td.tot{background:#fff8cf;font-weight:700;text-align:center}
td.tot.part{color:var(--abu);font-style:italic;font-weight:600}
td.tot.low{color:var(--merah)}
th.tot{background:var(--stabilo);color:#3d3500;text-align:center}
.stk1{position:sticky;left:0;z-index:2;background:#fff;width:46px;min-width:46px}
.stk2{position:sticky;left:46px;z-index:2;background:#fff;min-width:170px;box-shadow:1px 0 0 var(--garis)}
th.stk1,th.stk2{background:var(--kapur);z-index:3}
.steps{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:12px}
.steps span{font-size:13px;padding:3px 10px;border-radius:99px;background:var(--kapur)}
.steps span.on{background:var(--papan);color:#fff}
.note{background:#fffbe0;border-left:4px solid var(--stabilo);padding:10px 12px;border-radius:6px;font-size:13px;margin:10px 0}
 
#toast{position:fixed;left:50%;bottom:78px;transform:translateX(-50%);background:var(--papan);color:#fff;padding:9px 16px;border-radius:99px;font-size:14px;opacity:0;pointer-events:none;transition:opacity .2s;z-index:9}
#toast.show{opacity:1}
 
@media (max-width:760px){
  .app{grid-template-columns:1fr}
  aside{position:fixed;top:auto;bottom:0;left:0;right:0;height:auto;flex-direction:row;padding:6px;z-index:5;gap:0}
  aside .brand,.side-note{display:none}
  nav{flex-direction:row;width:100%;justify-content:space-around}
  nav button{padding:8px 6px;font-size:12px;text-align:center;flex:1}
  .title h1{font-size:23px}
  .side-art{display:none}
  .mascot{width:56px!important}
  #view{padding:10px;border-radius:16px}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important}}
html{background:#cfe8ff}
#scene{position:fixed;inset:0;z-index:0;overflow:hidden;pointer-events:none}
#scene svg{position:absolute;inset:0;width:100%;height:100%;display:block}
.app{position:relative;z-index:1}
#view{background:rgba(255,255,255,.82);border:2px solid rgba(255,255,255,.95);border-radius:22px;padding:16px;box-shadow:0 10px 30px rgba(10,45,117,.18);backdrop-filter:blur(5px);-webkit-backdrop-filter:blur(5px)}
.mascot{width:84px;flex:0 0 auto}
.mascot svg{width:100%;height:auto;display:block;overflow:visible}
.empty-art{display:flex;justify-content:center;margin-bottom:8px}
.empty-art svg{width:86px;height:auto}
.shore{margin-top:18px;overflow:hidden;line-height:0}
.shore svg{display:block;width:max(100%,640px);margin-left:calc((100% - max(100%,640px))/2);height:auto}
@keyframes bob{0%,100%{transform:translateY(0) rotate(-2deg)}50%{transform:translateY(-6px) rotate(2deg)}}
@keyframes bobsm{0%,100%{transform:translateY(0)}50%{transform:translateY(-4px)}}
@keyframes drift{to{transform:translateX(300px)}}
@keyframes cloudmove{to{transform:translateX(70px)}}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes twinkle{0%,100%{opacity:.25}50%{opacity:1}}
@keyframes rise{from{transform:translateY(0)}to{transform:translateY(-820px)}}
@keyframes rays{from{opacity:.05}to{opacity:.16}}
@media (prefers-reduced-motion:no-preference){
  .mascot svg{animation:bob 3.2s ease-in-out infinite}
  .bobsm{animation:bobsm 3.8s ease-in-out infinite}
  .drift{animation:drift 10s linear infinite}
  .drift.d2{animation-duration:15s;animation-direction:reverse}
  .drift.d3{animation-duration:22s}
  .cloud{animation:cloudmove 40s ease-in-out infinite alternate}
  .spin{animation:spin 80s linear infinite;transform-box:fill-box;transform-origin:center}
  .twinkle{animation:twinkle 3s ease-in-out infinite}
  .rise{animation:rise 10s linear infinite}
  .ray{animation:rays 7s ease-in-out infinite alternate}
}
</style>
</head>
<body>
<div id="scene" aria-hidden="true"></div>
<div class="app">
  <aside>
    <div class="brand">KelasKu<small>Absensi & nilai murid</small></div>
    <nav id="nav">
      <button data-t="dashboard">Beranda</button>
      <button data-t="absensi">Absensi</button>
      <button data-t="nilai">Nilai</button>
      <button data-t="impor">Impor Google Form</button>
      <button data-t="data">Data & Pengaturan</button>
    </nav>
    <div class="side-note">Data tersimpan di browser ini. Cadangkan lewat menu Data & Pengaturan.</div>
  </aside>
  <main>
    <div class="topbar">
      <div id="mascot" class="mascot" aria-hidden="true"></div>
      <div class="title"><h1 id="pageTitle"></h1><p id="pageSub"></p></div>
      <label>Kelas <select id="gClass"></select></label>
      <label>Mata pelajaran <select id="gSubject"></select></label>
      <label>Latar <select id="gBg"></select></label>
    </div>
    <div id="view"></div>
    <div class="shore" id="shore" aria-hidden="true"></div>
  </main>
</div>
<div id="toast" role="status"></div>
 
<script>
/* ============ Util ============ */
const $=(s,r=document)=>r.querySelector(s);
const esc=s=>String(s??'').replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
const uid=()=>Math.random().toString(36).slice(2,9);
const norm=s=>String(s||'').toLowerCase().replace(/[^a-z0-9 ]/g,' ').replace(/\s+/g,' ').trim();
const pad=n=>String(n).padStart(2,'0');
const today=()=>{const d=new Date();return d.getFullYear()+'-'+pad(d.getMonth()+1)+'-'+pad(d.getDate())};
const fmt=n=>n==null?'–':(Math.round(n*10)/10).toString().replace('.',',');
const JENIS=['Tugas','Catatan','Kuis','UH','PTS','PAS','Praktik','Sikap'];
const meetingsOf=(cid,subj,month)=>S.meetings.filter(m=>m.classId===cid&&m.subject===subj&&(!month||m.month===month));
const BULAN=['Januari','Februari','Maret','April','Mei','Juni','Juli','Agustus','September','Oktober','November','Desember'];
const monthLabel=m=>{const [y,mo]=String(m).split('-');return (BULAN[+mo-1]||m)+' '+y};
const compsOf=m=>S.assessments.filter(a=>a.meetingId===m.id);
const compLabel=(a,m)=>a.name&&a.name!==m.name?a.name:(a.type||'Tugas');
function meetingTotal(m,sid){
  let w=0,t=0,miss=0;
  compsOf(m).forEach(a=>{const v=S.scores[a.id]?.[sid];if(v!=null&&v!==''){w+=a.weight;t+=v*a.weight}else miss++});
  return {v:w?t/w:null,partial:miss>0&&w>0};
}
const noOf=(s,i)=>s.nis||String(i+1);
let toastT;
function toast(m){const t=$('#toast');t.textContent=m;t.classList.add('show');clearTimeout(toastT);toastT=setTimeout(()=>t.classList.remove('show'),2400)}
function download(name,text,type='text/csv'){const a=document.createElement('a');a.href=URL.createObjectURL(new Blob(['\ufeff'+text],{type}));a.download=name;a.click();setTimeout(()=>URL.revokeObjectURL(a.href),500)}
const csvCell=v=>{v=String(v??'');return /[",\n;]/.test(v)?'"'+v.replace(/"/g,'""')+'"':v};
 
/* ============ Penyimpanan (localStorage, dengan cadangan memori) ============ */
const KEY='kelasku.v1';
function seed(){
  const c1={id:'k7a',name:'VII A'},c2={id:'k8a',name:'VIII A'};
  const names=['Aditya Pratama','Bunga Lestari','Citra Maharani','Dimas Saputra','Eka Wulandari','Farhan Hakim','Gita Anjani','Hendra Wijaya','Indah Permata','Joko Santoso'];
  const students=names.map((n,i)=>({id:'s'+i,nis:String(i+1),name:n,classId:'k7a'}));
  ['Kartika Sari','Lutfi Ramadhan','Mega Putri'].forEach((n,i)=>students.push({id:'t'+i,nis:String(i+1),name:n,classId:'k8a'}));
  const meetings=[{id:'m1',classId:'k7a',subject:'Informatika',name:'Pertemuan 1'},{id:'m2',classId:'k7a',subject:'Informatika',name:'Pertemuan 2'}];
  const mk=(id,m,name,type,weight)=>({id,classId:'k7a',subject:'Informatika',meetingId:m,name,type,types:[type],weight,source:'manual',manual:{}});
  const as=[mk('a1','m1','Tugas Catatan','Catatan',70),mk('a2','m1','Kuis','Kuis',30),mk('a3','m2','Tugas Catatan','Catatan',70),mk('a4','m2','Kuis','Kuis',30)];
  const base=[88,76,92,64,80,71,95,58,84,78];
  const scores={a1:{},a2:{},a3:{},a4:{}};
  students.filter(s=>s.classId==='k7a').forEach((s,i)=>{
    scores.a1[s.id]=base[i];scores.a2[s.id]=Math.min(100,base[i]+((i*7)%11)-4);
    scores.a3[s.id]=Math.min(100,base[i]+((i*5)%9)-3);if(i<6)scores.a4[s.id]=Math.min(100,base[i]+((i*3)%7));
  });
  return {classes:[c1,c2],students,subjects:['Informatika','Matematika','IPA'],meetings,assessments:as,scores,notes:{},attendance:{},kkm:75,clientId:''};
}
function fixS(o){
  o.notes=o.notes||{};o.meetings=o.meetings||[];
  (o.assessments||[]).forEach(a=>{
    if(!a.types)a.types=[a.type||'Tugas'];
    if(!a.type)a.type=a.types[0];
    if(!(a.weight>0))a.weight=10;
    if(!a.meetingId){
      let m=o.meetings.find(x=>x.classId===a.classId&&x.subject===a.subject&&x.name===a.name);
      if(!m){m={id:'m'+Math.random().toString(36).slice(2,8),classId:a.classId,subject:a.subject,name:a.name};o.meetings.push(m)}
      a.meetingId=m.id;
    }
  });
  o.meetings.forEach(m=>{if(!m.month)m.month=today().slice(0,7)});
  o.bg=o.bg||'auto';
  return o;
}
function load(){try{const r=localStorage.getItem(KEY);if(r)return fixS(JSON.parse(r))}catch(e){}return fixS(seed())}
function save(){try{localStorage.setItem(KEY,JSON.stringify(S))}catch(e){}}
let S=load();
 
/* ============ Hitungan ============ */
const clsStudents=id=>S.students.filter(s=>s.classId===id).sort((a,b)=>{const x=parseFloat(a.nis),y=parseFloat(b.nis);if(!isNaN(x)&&!isNaN(y)&&x!==y)return x-y;return a.name.localeCompare(b.name)});
function finalGrade(cid,subj,sid,month){
  const ts=meetingsOf(cid,subj,month).map(m=>meetingTotal(m,sid).v).filter(v=>v!=null);
  return ts.length?ts.reduce((a,b)=>a+b,0)/ts.length:null;
}
function attStats(cid,sid,prefix=''){
  const c={H:0,I:0,S:0,A:0};
  for(const k in S.attendance){const [kc,d]=k.split('|');if(kc!==cid||!d.startsWith(prefix))continue;const v=S.attendance[k][sid];if(v)c[v]++}
  const tot=c.H+c.I+c.S+c.A;
  return {...c,tot,pct:tot?c.H/tot*100:null};
}
 
/* ============ State tampilan ============ */
const V={tab:'dashboard',classId:S.classes[0]?.id,subject:S.subjects[0],date:today(),month:today().slice(0,7),
  method:'api',imp:{link:'',name:'',type:'Kuis',weight:'',meetingId:'',csv:''},im:null,busy:false,err:''};
 
const TITLES={
  dashboard:['Beranda','Ringkasan kelas hari ini'],
  absensi:['Absensi','Catat kehadiran per tanggal dan lihat rekapnya'],
  nilai:['Nilai','Nilai dipisah per bulan; isi per pertemuan dan lihat nilai akhir'],
  impor:['Impor Google Form','Tarik nilai kuis langsung ke daftar nilai murid'],
  data:['Data & Pengaturan','Kelas, murid, mata pelajaran, dan cadangan']
};
 
function render(){
  $('#gClass').innerHTML=S.classes.map(c=>`<option value="${c.id}" ${c.id===V.classId?'selected':''}>${esc(c.name)}</option>`).join('');
  $('#gSubject').innerHTML=S.subjects.map(s=>`<option ${s===V.subject?'selected':''}>${esc(s)}</option>`).join('');
  document.querySelectorAll('#nav button').forEach(b=>b.classList.toggle('on',b.dataset.t===V.tab));
  $('#pageTitle').textContent=TITLES[V.tab][0];$('#pageSub').textContent=TITLES[V.tab][1];
  const needClass=['dashboard','absensi','nilai','impor'].includes(V.tab);
  $('#view').innerHTML=(needClass&&!V.classId)?`<div class="empty">Belum ada kelas. Tambahkan kelas dan murid di menu <b>Data & Pengaturan</b>.</div>`:VIEWS[V.tab]();
  decorate();
}
$('#nav').addEventListener('click',e=>{const b=e.target.closest('button');if(b){V.tab=b.dataset.t;render();scrollTo(0,0)}});
$('#gClass').addEventListener('change',e=>{V.classId=e.target.value;V.im=null;render()});
$('#gSubject').addEventListener('change',e=>{V.subject=e.target.value;V.im=null;render()});
 
/* ============ Tampilan ============ */
const VIEWS={
dashboard(){
  const st=clsStudents(V.classId),rec=S.attendance[V.classId+'|'+today()];
  const hadir=rec?st.filter(s=>rec[s.id]==='H').length:null;
  const fg=st.map(s=>finalGrade(V.classId,V.subject,s.id)).filter(v=>v!=null);
  const avg=fg.length?fg.reduce((a,b)=>a+b,0)/fg.length:null;
  const risk=st.map(s=>({s,a:attStats(V.classId,s.id),f:finalGrade(V.classId,V.subject,s.id)}))
    .filter(r=>(r.a.pct!=null&&r.a.pct<85)||(r.f!=null&&r.f<S.kkm));
  return `
  <div class="stats">
    <div class="stat"><b>${st.length}</b><span>murid di kelas ini</span></div>
    <div class="stat"><b>${hadir==null?'–':hadir+'/'+st.length}</b><span>hadir hari ini</span></div>
    <div class="stat"><b>${fmt(avg)}</b><span>rata-rata nilai akhir ${esc(V.subject)}</span></div>
    <div class="stat hl"><b>${risk.length}</b><span>murid perlu perhatian</span></div>
  </div>
  <div class="panel">
    <h2>Perlu perhatian</h2>
    ${risk.length?`<div class="tbl-wrap"><table><thead><tr><th>Nama</th><th class="num">Kehadiran</th><th class="num">Nilai akhir</th><th>Catatan</th></tr></thead><tbody>
    ${risk.map(r=>`<tr><td>${esc(r.s.name)}</td><td class="num">${r.a.pct==null?'–':fmt(r.a.pct)+'%'}</td><td class="num fin ${r.f!=null&&r.f<S.kkm?'low':''}">${fmt(r.f)}</td>
      <td>${r.a.pct!=null&&r.a.pct<85?'<span class="badge bad">Kehadiran rendah</span> ':''}${r.f!=null&&r.f<S.kkm?`<span class="badge warn">Di bawah KKM ${S.kkm}</span>`:''}</td></tr>`).join('')}
    </tbody></table></div>`:`<p class="muted">Tidak ada murid yang kehadirannya di bawah 85% atau nilainya di bawah KKM ${S.kkm}.</p>`}
  </div>
  <div class="row"><button class="btn" onclick="go('absensi')">Mulai absen hari ini</button><button class="btn ghost" onclick="go('nilai')">Buka daftar nilai</button><button class="btn ghost" onclick="go('impor')">Impor nilai kuis</button></div>`;
},
 
absensi(){
  const st=clsStudents(V.classId),key=V.classId+'|'+V.date,rec=S.attendance[key];
  const rows=st.map((s,i)=>{const cur=rec?.[s.id]||'H';return `<tr><td class="num muted" style="width:46px">${noOf(s,i)}</td><td>${esc(s.name)}</td>
    <td><div class="stamps">${['H','I','S','A'].map(x=>`<button data-s="${x}" class="${cur===x?'on':''}" onclick="setAtt('${s.id}','${x}')" aria-label="${{H:'Hadir',I:'Izin',S:'Sakit',A:'Alpa'}[x]}">${x}</button>`).join('')}</div></td></tr>`}).join('');
  const rk=st.map((s,i)=>({s,i,a:attStats(V.classId,s.id,V.month)}));
  return `
  <div class="panel">
    <div class="row">
      <label>Tanggal<input type="date" value="${V.date}" onchange="V.date=this.value;render()"></label>
      <span class="badge ${rec?'ok':'warn'}" style="align-self:center">${rec?'Tersimpan':'Belum disimpan (bawaan: Hadir)'}</span>
      <button class="btn" onclick="allHadir()">Simpan semua Hadir</button>
    </div>
    <p class="muted small" style="margin:8px 0 0">H = Hadir, I = Izin, S = Sakit, A = Alpa. Setiap ketukan langsung tersimpan.</p>
  </div>
  ${st.length?`<div class="tbl-wrap"><table><thead><tr><th class="num">No</th><th>Murid</th><th>Status</th></tr></thead><tbody>${rows}</tbody></table></div>`:`<div class="empty">Kelas ini belum punya murid.</div>`}
  <div class="panel" style="margin-top:16px">
    <div class="row"><h2 style="margin-right:auto">Rekap bulanan</h2>
      <label style="flex:0 1 170px">Bulan<input type="month" value="${V.month}" onchange="V.month=this.value;render()"></label>
      <button class="btn ghost" onclick="exportAbsen()">Ekspor CSV</button></div>
    <div class="tbl-wrap" style="margin-top:10px"><table><thead><tr><th class="num">No</th><th>Murid</th><th class="num">H</th><th class="num">I</th><th class="num">S</th><th class="num">A</th><th class="num">% Hadir</th></tr></thead><tbody>
    ${rk.map(({s,a,i})=>`<tr><td class="num muted">${noOf(s,i)}</td><td>${esc(s.name)}</td><td class="num">${a.H}</td><td class="num">${a.I}</td><td class="num">${a.S}</td><td class="num">${a.A}</td>
      <td class="num fin ${a.pct!=null&&a.pct<85?'low':''}">${a.pct==null?'–':fmt(a.pct)+'%'}</td></tr>`).join('')}
    </tbody></table></div>
  </div>`;
},
 
nilai(){
  if(V.gAll)return nilaiRekap();
  const st=clsStudents(V.classId),allMs=meetingsOf(V.classId,V.subject),ms=meetingsOf(V.classId,V.subject,V.gMonth),nm=V.nm,nc=V.nc;
  const fgs=st.map(s=>finalGrade(V.classId,V.subject,s.id,V.gMonth));
  const ok=fgs.filter(v=>v!=null),avg=ok.length?ok.reduce((a,b)=>a+b,0)/ok.length:null;
  const mSel=ms.some(m=>m.id===nc.meetingId)?nc.meetingId:(ms[ms.length-1]?.id||'');
  const avgOf=vs=>{vs=vs.filter(v=>v!=null&&v!=='');return vs.length?fmt(vs.reduce((x,y)=>x+y,0)/vs.length):'–'};
  return `${monthBar()}
  <div class="panel"><h2>Atur pertemuan di ${monthLabel(V.gMonth)}</h2>
    <div class="row">
      <label style="flex:2 1 180px">Pertemuan baru<input type="text" value="${esc(nm.name)}" placeholder="Pertemuan ${ms.length+1}" oninput="V.nm.name=this.value"></label>
      ${allMs.length?`<label style="flex:0 1 auto;flex-direction:row;align-items:center;gap:6px;color:var(--tinta);padding-bottom:8px"><input type="checkbox" style="width:auto;min-height:0" ${nm.copy?'checked':''} onchange="V.nm.copy=this.checked"> Salin komponen dari pertemuan terakhir</label>`:''}
      <button class="btn" onclick="addMeeting()">Tambah pertemuan</button>
    </div>
    ${ms.length?`<div class="row" style="margin-top:14px">
      <label>Tambah komponen ke<select style="width:100%" onchange="V.nc.meetingId=this.value">${ms.map(m=>`<option value="${m.id}" ${m.id===mSel?'selected':''}>${esc(m.name)}</option>`).join('')}</select></label>
      <label>Jenis<select style="width:100%" onchange="V.nc.jenis=this.value">${JENIS.map(j=>`<option ${j===nc.jenis?'selected':''}>${j}</option>`).join('')}</select></label>
      <label>Nama (opsional)<input type="text" value="${esc(nc.name)}" oninput="V.nc.name=this.value" placeholder="mis. Tugas Catatan"></label>
      <label style="flex:0 1 110px">Bobot (%)<input type="number" min="1" max="100" value="${esc(nc.weight)}" oninput="V.nc.weight=this.value" placeholder="sisa"></label>
      <button class="btn" onclick="addComp()">Tambah komponen</button>
    </div>`:''}
    <p class="muted small" style="margin:10px 0 0">Tiap pertemuan punya komponen sendiri (misalnya Catatan 70% + Kuis 30%) dan totalnya dihitung terpisah dari pertemuan lain. Nilai akhir bulan ini = rata-rata total semua pertemuan di ${monthLabel(V.gMonth)}. Tiap bulan dihitung terpisah.</p>
  </div>
  ${ms.length?`
  <div class="row" style="margin-bottom:8px"><span class="muted small" style="margin-right:auto">KKM ${S.kkm}. Total miring berarti ada komponen yang belum terisi.</span>
    <button class="btn ghost sm" onclick="exportNilai()">Ekspor CSV</button></div>
  <div class="tbl-wrap"><table><thead>
    <tr><th class="stk1 num" rowspan="2">No</th><th class="stk2" rowspan="2">Murid</th>
    ${ms.map(m=>{const cs=compsOf(m),tw=cs.reduce((x,a)=>x+a.weight,0);
      return `<th class="grp" colspan="${cs.length+1}">${esc(m.name)}<button onclick="renameMeeting('${m.id}')">ubah nama</button><button onclick="delMeeting('${m.id}')" aria-label="Hapus ${esc(m.name)}">×</button>
        <div class="small">${cs.length?(tw===100?'bobot 100%':'<span class="badge warn">bobot '+tw+'%, idealnya 100%</span>'):'belum ada komponen'}</div></th>`}).join('')}
    <th class="num" rowspan="2">Nilai akhir<div class="small muted" style="font-weight:400">${monthLabel(V.gMonth)}</div></th></tr>
    <tr>${ms.map(m=>compsOf(m).map(a=>`<th class="num">${esc(compLabel(a,m))}<div class="small muted" style="font-weight:400">${esc(a.type)}${a.source==='google_form'?' <span class="badge">Form</span>':''}</div>
      <div style="display:flex;gap:3px;justify-content:center;align-items:center;margin-top:3px"><input class="tiny-in" type="number" min="1" max="100" value="${a.weight}" onchange="setW('${a.id}',this.value)" aria-label="Bobot ${esc(compLabel(a,m))}">%
      <button class="btn danger sm" style="padding:0 6px;min-height:24px" onclick="delAssess('${a.id}')" aria-label="Hapus ${esc(compLabel(a,m))}">×</button></div></th>`).join('')+`<th class="tot">Total</th>`).join('')}</tr>
  </thead><tbody>
    ${st.map((s,i)=>`<tr><td class="stk1 num muted">${noOf(s,i)}</td><td class="stk2">${esc(s.name)}</td>
      ${ms.map(m=>{const t=meetingTotal(m,s.id);
        return compsOf(m).map(a=>{const v=S.scores[a.id]?.[s.id];
          return `<td class="num"><input type="number" min="0" max="100" step="any" value="${v??''}" class="${v!=null&&v!==''&&v<S.kkm?'low':''}" onchange="setScore('${a.id}','${s.id}',this.value)" aria-label="${esc(s.name)} ${esc(compLabel(a,m))}"></td>`}).join('')
          +`<td class="tot ${t.partial?'part':''} ${t.v!=null&&t.v<S.kkm?'low':''}" ${t.partial?'title="Belum semua komponen terisi"':''}>${fmt(t.v)}</td>`}).join('')}
      <td class="num fin ${fgs[i]!=null&&fgs[i]<S.kkm?'low':''}">${fmt(fgs[i])}</td></tr>`).join('')}
    <tr><td class="stk1"></td><td class="stk2"><b>Rata-rata kelas</b></td>
      ${ms.map(m=>compsOf(m).map(a=>`<td class="num muted">${avgOf(st.map(s=>S.scores[a.id]?.[s.id]))}</td>`).join('')+`<td class="tot">${avgOf(st.map(s=>meetingTotal(m,s.id).v))}</td>`).join('')}
      <td class="num fin">${fmt(avg)}</td></tr>
  </tbody></table></div>
  <p class="muted small">Total pertemuan = rata-rata tertimbang dari komponen yang sudah terisi. Angka merah berarti di bawah KKM.</p>`
  :`<div class="empty">Belum ada pertemuan ${esc(V.subject)} pada ${monthLabel(V.gMonth)}. Buat pertemuan pertama di atas, lalu tambahkan komponennya.</div>`}`;
},
 
impor(){
  const p=V.imp,im=V.im;
  const stepOn=n=>(n===1&&!im)||(n===2&&im)?'on':'';
  return `
  <div class="steps"><span class="${stepOn(1)}">1. Ambil data form</span><span class="${stepOn(2)}">2. Cek & simpan</span></div>
  <div class="note">Nilai masuk ke <b>${esc(S.classes.find(c=>c.id===V.classId)?.name||'')}</b> · <b>${esc(V.subject)}</b> · bulan <input type="month" value="${V.gMonth}" style="width:165px;min-height:30px;padding:3px 8px;display:inline-block" onchange="if(this.value){V.gMonth=this.value;V.imp.meetingId='';render()}" aria-label="Bulan penilaian">. Ganti kelas atau mapel di bagian atas jika perlu.</div>
  ${im?importPreview():`
  <div class="panel">
    <div class="row">
      <label style="flex:3 1 260px">Link Google Form (mode Kuis)<input type="text" value="${esc(p.link)}" oninput="V.imp.link=this.value" placeholder="https://docs.google.com/forms/d/…/edit"></label>
      <label style="flex:1 1 170px">Masuk ke pertemuan<select style="width:100%" onchange="V.imp.meetingId=this.value">${(()=>{const ms=meetingsOf(V.classId,V.subject,V.gMonth),pm=p.meetingId||ms[ms.length-1]?.id||'__new__';return ms.map(m=>`<option value="${m.id}" ${m.id===pm?'selected':''}>${esc(m.name)}</option>`).join('')+`<option value="__new__" ${pm==='__new__'?'selected':''}>+ Pertemuan baru</option>`})()}</select></label>
      <label style="flex:2 1 160px">Nama komponen<input type="text" value="${esc(p.name)}" oninput="V.imp.name=this.value" placeholder="mis. Kuis Bab 2"></label>
      <label style="flex:0 1 120px">Jenis<select style="width:100%" onchange="V.imp.type=this.value">${JENIS.map(t=>`<option ${t===p.type?'selected':''}>${t}</option>`).join('')}</select></label>
      <label style="flex:0 1 90px">Bobot %<input type="number" value="${esc(p.weight)}" min="1" max="100" oninput="V.imp.weight=this.value" placeholder="sisa"></label>
    </div>
  </div>
  <div class="tabs" role="tablist">
    <button class="${V.method==='api'?'on':''}" onclick="V.method='api';render()">Google Forms API</button>
    <button class="${V.method==='csv'?'on':''}" onclick="V.method='csv';render()">Unggah CSV</button>
    <button class="${V.method==='demo'?'on':''}" onclick="V.method='demo';render()">Coba dengan data contoh</button>
  </div>
  ${V.err?`<div class="note" style="border-color:var(--merah);background:#fde8e6">${esc(V.err)}</div>`:''}
  ${V.method==='api'?`
  <div class="panel">
    <div class="row"><label style="flex:3 1 260px">OAuth Client ID (Google Cloud)<input type="text" value="${esc(S.clientId)}" oninput="S.clientId=this.value;save()" placeholder="xxxx.apps.googleusercontent.com"></label>
    <button class="btn" onclick="fetchAPI()" ${V.busy?'disabled':''}>${V.busy?'Mengambil…':'Hubungkan Google & ambil nilai'}</button></div>
    <p class="muted small" style="margin:10px 0 0">Akun Google yang dipakai harus pemilik atau editor form tersebut. Halaman ini harus dibuka lewat <b>https</b> atau <b>localhost</b>, dan alamatnya didaftarkan sebagai Authorized JavaScript origin di Google Cloud. Izin yang diminta hanya baca (form dan respons).</p>
  </div>`:''}
  ${V.method==='csv'?`
  <div class="panel">
    <p class="muted small" style="margin-top:0">Di Google Form buka tab <b>Respons → Tautkan ke Sheets</b>, unduh sebagai CSV, lalu unggah atau tempel di sini. Kolom <b>Skor/Score</b> terbaca otomatis, termasuk format "8 / 10".</p>
    <input type="file" accept=".csv,text/csv" onchange="readCSVFile(this.files[0])">
    <textarea style="margin-top:8px" placeholder="…atau tempel isi CSV di sini" oninput="V.imp.csv=this.value">${esc(p.csv)}</textarea>
    <div style="margin-top:8px"><button class="btn" onclick="loadCSV()">Baca CSV</button></div>
  </div>`:''}
  ${V.method==='demo'?`
  <div class="panel"><p style="margin-top:0">Membuat respons contoh dari murid di kelas ini (termasuk satu nama salah ketik dan satu murid tidak dikenal) untuk mencoba alur pencocokan.</p>
  <button class="btn" onclick="loadDemo()">Buat data contoh</button></div>`:''}
  `}`;
},
 
data(){
  const sel=V.classId;
  return `
  <div class="panel"><h2>Kelas</h2>
    <div class="row"><label>Nama kelas baru<input type="text" id="cName" placeholder="mis. IX B"></label><button class="btn" onclick="addClass()">Tambah kelas</button>
    ${S.classes.length?`<button class="btn danger" onclick="delClass()">Hapus kelas terpilih</button>`:''}</div>
  </div>
  <div class="panel"><h2>Murid ${sel?`di ${esc(S.classes.find(c=>c.id===sel)?.name)}`:''}</h2>
    ${sel?`<div class="row"><label style="flex:0 1 100px">No<input type="text" id="sNis" placeholder="otomatis"></label><label style="flex:2 1 200px">Nama<input type="text" id="sName"></label><button class="btn" onclick="addStudent()">Tambah murid</button></div>
    <div style="margin-top:14px">
      <label class="drop" ondragover="event.preventDefault();this.classList.add('over')" ondragleave="this.classList.remove('over')" ondrop="event.preventDefault();this.classList.remove('over');readStudentFile(event.dataTransfer.files[0])">
        <b>Unggah daftar murid dari file</b>
        <span class="muted small">Seret file ke sini atau klik untuk memilih. Mendukung Excel (.xlsx, .xls) dan CSV.</span>
        <input type="file" accept=".xlsx,.xls,.csv,.txt,.tsv" onchange="readStudentFile(this.files[0])">
      </label>
      <p class="muted small" style="margin:8px 0 0">Kolom yang dibaca: <b>No</b> (nomor) dan <b>Nama</b>, judul kolom boleh ada atau tidak. Jika tidak ada nomor, murid dinomori otomatis sesuai urutan. Murid masuk ke kelas yang sedang dipilih. <a href="#" onclick="downloadStudentTemplate();return false">Unduh templat CSV</a></p>
      ${stuPreviewHTML()}
    </div>
    <label class="muted small" style="display:block;margin-top:14px">Atau tempel banyak murid sekaligus, satu baris satu murid, format <b>No,Nama</b>
      <textarea id="bulk" placeholder="1,Aditya Pratama&#10;2,Bunga Lestari"></textarea></label>
    <div style="margin:8px 0 12px"><button class="btn ghost" onclick="bulkStudents()">Impor daftar</button></div>
    <div class="tbl-wrap"><table><thead><tr><th class="num" style="width:50px">No</th><th>Nama</th><th></th></tr></thead><tbody>
    ${clsStudents(sel).map((s,i)=>`<tr><td class="num">${noOf(s,i)}</td><td>${esc(s.name)}</td><td style="text-align:right"><button class="btn danger sm" onclick="delStudent('${s.id}')">Hapus</button></td></tr>`).join('')||'<tr><td colspan="3" class="muted">Belum ada murid.</td></tr>'}
    </tbody></table></div>`:'<p class="muted">Tambahkan kelas terlebih dahulu.</p>'}
  </div>
  <div class="panel"><h2>Pengaturan</h2>
    <div class="row"><label style="flex:0 1 140px">KKM<input type="number" value="${S.kkm}" min="0" max="100" onchange="S.kkm=+this.value||75;save();render()"></label>
    <label>Tambah mata pelajaran<input type="text" id="mName" placeholder="mis. Bahasa Indonesia"></label><button class="btn" onclick="addSubject()">Tambah</button></div>
    <p class="muted small">Mapel: ${S.subjects.map(esc).join(', ')}</p>
  </div>
  <div class="panel"><h2>Cadangan data</h2>
    <div class="row"><button class="btn ghost" onclick="backup()">Unduh cadangan (.json)</button>
    <label style="flex:0 1 auto"><span class="btn ghost" style="display:inline-block">Pulihkan dari cadangan</span><input type="file" accept=".json" hidden onchange="restore(this.files[0])"></label>
    <button class="btn danger" onclick="resetAll()">Hapus semua data</button></div>
  </div>`;
}};
 
function importPreview(){
  const im=V.im,{rows,pick,missing}=computeMatches(),sts=clsStudents(V.classId);
  const matched=Object.keys(pick).length;
  return `
  <div class="panel">
    <div class="row">
      <label style="flex:2 1 220px">Kolom identitas murid<select style="width:100%" onchange="V.im.idQ=this.value;render()">${im.questions.map(q=>`<option value="${esc(q.id)}" ${q.id===im.idQ?'selected':''}>${esc(q.title)}</option>`).join('')}</select></label>
      <label style="flex:1 1 170px">Jika mengerjakan lebih dari sekali<select style="width:100%" onchange="V.im.policy=this.value;render()">
        <option value="max" ${im.policy==='max'?'selected':''}>Pakai nilai tertinggi</option><option value="last" ${im.policy==='last'?'selected':''}>Pakai yang terakhir</option><option value="first" ${im.policy==='first'?'selected':''}>Pakai yang pertama</option></select></label>
    </div>
    <p class="muted small" style="margin:10px 0 0">Skor diubah ke skala 0–100 (skor maksimum form: ${fmt(im.max)}). Pencocokan: nomor absen dulu, lalu nama.</p>
  </div>
  <div class="stats">
    <div class="stat"><b>${rows.length}</b><span>respons diterima</span></div>
    <div class="stat"><b>${matched}</b><span>murid cocok</span></div>
    <div class="stat hl"><b>${rows.filter(r=>!r.st).length}</b><span>perlu dicocokkan manual</span></div>
    <div class="stat"><b>${missing.length}</b><span>murid belum mengerjakan</span></div>
  </div>
  <div class="tbl-wrap"><table><thead><tr><th>Isian di form</th><th>Murid</th><th class="num">Nilai</th><th>Status</th></tr></thead><tbody>
  ${rows.map(r=>`<tr><td>${esc(r.raw)||'<span class="muted">(kosong)</span>'}</td>
    <td><select style="width:100%" onchange="assign(${r.i},this.value)"><option value="">– pilih murid –</option>${sts.map(s=>`<option value="${s.id}" ${r.st?.id===s.id?'selected':''}>${esc(s.name)}</option>`).join('')}</select></td>
    <td class="num">${r.score==null?'–':fmt(r.score)}</td>
    <td>${!r.st?'<span class="badge bad">Belum cocok</span>':r.how==='mirip'?'<span class="badge warn">Mirip, cek dulu</span>':'<span class="badge ok">Cocok ('+r.how+')</span>'}${r.st&&pick[r.st.id]&&pick[r.st.id].i!==r.i?' <span class="badge">Tidak dipakai</span>':''}</td></tr>`).join('')}
  </tbody></table></div>
  ${missing.length?`<p class="muted small">Belum mengerjakan (dibiarkan kosong, bukan nol): ${missing.map(m=>esc(m.name)).join(', ')}</p>`:''}
  <div class="row" style="margin-top:12px"><button class="btn" onclick="saveImport()" ${matched?'':'disabled'}>Simpan ${matched} nilai</button><button class="btn ghost" onclick="V.im=null;render()">Batal</button></div>`;
}
 
/* ============ Aksi: umum ============ */
function go(t){V.tab=t;render();scrollTo(0,0)}
 
function setAtt(sid,st){
  const key=V.classId+'|'+V.date;
  if(!S.attendance[key]){S.attendance[key]={};clsStudents(V.classId).forEach(s=>S.attendance[key][s.id]='H')}
  S.attendance[key][sid]=st;save();render();
}
function allHadir(){
  const key=V.classId+'|'+V.date;S.attendance[key]={};clsStudents(V.classId).forEach(s=>S.attendance[key][s.id]='H');save();render();toast('Absensi tersimpan: semua hadir');
}
function exportAbsen(){
  const rows=[['No','Nama','Hadir','Izin','Sakit','Alpa','% Hadir']];
  clsStudents(V.classId).forEach((s,i)=>{const a=attStats(V.classId,s.id,V.month);rows.push([noOf(s,i),s.name,a.H,a.I,a.S,a.A,a.pct==null?'':fmt(a.pct)])});
  download(`rekap-absen-${V.month}.csv`,rows.map(r=>r.map(csvCell).join(',')).join('\n'));
}
 
function monthBar(){
  const shift=d=>{const [y,m]=V.gMonth.split('-').map(Number);const dt=new Date(y,m-1+d,1);return dt.getFullYear()+'-'+pad(dt.getMonth()+1)};
  return `<div class="tabs"><button class="on">Per bulan</button><button onclick="V.gAll=true;render()">Rekap semua bulan</button></div>
  <div class="row" style="margin-bottom:14px;align-items:center">
    <button class="btn ghost sm" onclick="V.gMonth='${shift(-1)}';render()" aria-label="Bulan sebelumnya">‹</button>
    <b style="font:700 21px 'Bricolage Grotesque',sans-serif;min-width:150px;text-align:center">${monthLabel(V.gMonth)}</b>
    <button class="btn ghost sm" onclick="V.gMonth='${shift(1)}';render()" aria-label="Bulan berikutnya">›</button>
    <input type="month" value="${V.gMonth}" style="width:170px" onchange="if(this.value){V.gMonth=this.value;render()}" aria-label="Pilih bulan">
  </div>`;
}
const meanOf=arr=>{const v=arr.filter(x=>x!=null);return v.length?v.reduce((a,b)=>a+b,0)/v.length:null};
function rekapData(){
  const st=clsStudents(V.classId),ml=meetingsOf(V.classId,V.subject),months=[...new Set(ml.map(m=>m.month))].sort();
  const grid=st.map((s,i)=>{const per=months.map(mo=>finalGrade(V.classId,V.subject,s.id,mo));return {s,i,per,avg:meanOf(per)}});
  return {months,grid,count:months.map(mo=>ml.filter(m=>m.month===mo).length),colAvg:months.map((mo,j)=>meanOf(grid.map(g=>g.per[j])))};
}
function nilaiRekap(){
  const tabs=`<div class="tabs"><button onclick="V.gAll=false;render()">Per bulan</button><button class="on">Rekap semua bulan</button></div>`;
  const {months,grid,count,colAvg}=rekapData();
  if(!months.length)return tabs+`<div class="empty">Belum ada pertemuan ${esc(V.subject)} di kelas ini.</div>`;
  return tabs+`<div class="row" style="margin-bottom:8px"><span class="muted small" style="margin-right:auto">Nilai akhir tiap bulan, dihitung terpisah. Rata-rata diambil dari bulan yang sudah ada nilainya. KKM ${S.kkm}.</span>
    <button class="btn ghost sm" onclick="exportRekap()">Ekspor CSV</button></div>
  <div class="tbl-wrap"><table><thead><tr><th class="stk1 num">No</th><th class="stk2">Murid</th>
    ${months.map((mo,j)=>`<th class="num"><button class="btn ghost sm" onclick="V.gMonth='${mo}';V.gAll=false;render()" title="Buka nilai bulan ini">${monthLabel(mo)}</button><div class="small muted" style="font-weight:400">${count[j]} pertemuan</div></th>`).join('')}
    <th class="num">Rata-rata</th></tr></thead><tbody>
    ${grid.map(({s,i,per,avg})=>`<tr><td class="stk1 num muted">${noOf(s,i)}</td><td class="stk2">${esc(s.name)}</td>${per.map(v=>`<td class="num fin ${v!=null&&v<S.kkm?'low':''}">${fmt(v)}</td>`).join('')}<td class="num fin ${avg!=null&&avg<S.kkm?'low':''}">${fmt(avg)}</td></tr>`).join('')}
    <tr><td class="stk1"></td><td class="stk2"><b>Rata-rata kelas</b></td>${colAvg.map(v=>`<td class="num muted">${fmt(v)}</td>`).join('')}<td class="num fin">${fmt(meanOf(grid.map(g=>g.avg)))}</td></tr>
  </tbody></table></div>`;
}
function exportRekap(){
  const {months,grid}=rekapData();
  const rows=[['No','Nama',...months.map(monthLabel),'Rata-rata']];
  grid.forEach(({s,i,per,avg})=>rows.push([noOf(s,i),s.name,...per.map(v=>v==null?'':fmt(v)),fmt(avg)]));
  download(`rekap-nilai-${V.subject}.csv`,rows.map(r=>r.map(csvCell).join(',')).join('\n'));
}
 
function addMeeting(){
  const all=meetingsOf(V.classId,V.subject),ms=meetingsOf(V.classId,V.subject,V.gMonth);
  const name=(V.nm.name||'').trim()||'Pertemuan '+(ms.length+1);
  const m={id:uid(),classId:V.classId,subject:V.subject,month:V.gMonth,name};S.meetings.push(m);
  const prev=ms[ms.length-1]||all[all.length-1];
  if(V.nm.copy&&prev)compsOf(prev).forEach(a=>{
    const c={id:uid(),classId:a.classId,subject:a.subject,meetingId:m.id,name:a.name,type:a.type,types:[a.type],weight:a.weight,source:'manual',manual:{}};
    S.assessments.push(c);S.scores[c.id]={};
  });
  V.nm.name='';V.nc.meetingId=m.id;save();render();
}
function addComp(){
  const ms=meetingsOf(V.classId,V.subject,V.gMonth);if(!ms.length)return;
  const m=ms.find(x=>x.id===V.nc.meetingId)||ms[ms.length-1];
  const used=compsOf(m).reduce((x,a)=>x+a.weight,0),typed=Math.round(+V.nc.weight);
  const w=typed>0?typed:(100-used>0?100-used:10);
  const a={id:uid(),classId:V.classId,subject:V.subject,meetingId:m.id,name:(V.nc.name||'').trim()||V.nc.jenis,type:V.nc.jenis,types:[V.nc.jenis],weight:w,source:'manual',manual:{}};
  S.assessments.push(a);S.scores[a.id]={};V.nc.name='';V.nc.weight='';V.nc.meetingId=m.id;save();render();
}
function renameMeeting(id){const m=S.meetings.find(x=>x.id===id);const n=prompt('Nama pertemuan',m.name);if(n&&n.trim()){m.name=n.trim();save();render()}}
function delMeeting(id){
  const m=S.meetings.find(x=>x.id===id);if(!confirm(`Hapus "${m.name}" beserta semua komponen dan nilainya?`))return;
  S.assessments.filter(a=>a.meetingId===id).forEach(a=>{delete S.scores[a.id];delete S.notes[a.id]});
  S.assessments=S.assessments.filter(a=>a.meetingId!==id);S.meetings=S.meetings.filter(x=>x.id!==id);save();render();
}
function setW(id,v){const a=S.assessments.find(x=>x.id===id);a.weight=Math.max(1,+v||1);save();render()}
function delAssess(id){const a=S.assessments.find(x=>x.id===id);if(!confirm(`Hapus penilaian "${a.name}" beserta semua nilainya?`))return;
  S.assessments=S.assessments.filter(x=>x.id!==id);delete S.scores[id];delete S.notes[id];save();render()}
function setScore(aid,sid,v){
  const a=S.assessments.find(x=>x.id===aid);S.scores[aid]=S.scores[aid]||{};
  if(v===''){delete S.scores[aid][sid]}else{S.scores[aid][sid]=Math.min(100,Math.max(0,+v))}
  a.manual=a.manual||{};a.manual[sid]=true;save();render();
}
function exportNilai(){
  const ms=meetingsOf(V.classId,V.subject,V.gMonth);
  const head=['No','Nama'];
  ms.forEach(m=>{compsOf(m).forEach(a=>head.push(`${m.name} - ${compLabel(a,m)} (${a.weight}%)`));head.push(`${m.name} - Total`)});
  head.push('Nilai akhir');
  const rows=[head];
  clsStudents(V.classId).forEach((s,i)=>{const r=[noOf(s,i),s.name];
    ms.forEach(m=>{compsOf(m).forEach(a=>r.push(S.scores[a.id]?.[s.id]??''));r.push(fmt(meetingTotal(m,s.id).v))});
    r.push(fmt(finalGrade(V.classId,V.subject,s.id,V.gMonth)));rows.push(r)});
  download(`nilai-${V.subject}-${V.gMonth}.csv`,rows.map(r=>r.map(csvCell).join(',')).join('\n'));
}
 
/* ============ Aksi: data ============ */
function addClass(){const n=$('#cName').value.trim();if(!n)return;const c={id:uid(),name:n};S.classes.push(c);V.classId=c.id;save();render()}
function delClass(){const c=S.classes.find(x=>x.id===V.classId);if(!confirm(`Hapus kelas ${c.name} beserta murid, absensi, dan nilainya?`))return;
  const aid=S.assessments.filter(a=>a.classId===c.id).map(a=>a.id);aid.forEach(i=>{delete S.scores[i];delete S.notes[i]});
  S.assessments=S.assessments.filter(a=>a.classId!==c.id);S.meetings=S.meetings.filter(m=>m.classId!==c.id);S.students=S.students.filter(s=>s.classId!==c.id);
  Object.keys(S.attendance).forEach(k=>{if(k.startsWith(c.id+'|'))delete S.attendance[k]});
  S.classes=S.classes.filter(x=>x.id!==c.id);V.classId=S.classes[0]?.id;save();render()}
function addStudent(){const n=$('#sName').value.trim();if(!n)return;S.students.push({id:uid(),nis:$('#sNis').value.trim()||String(clsStudents(V.classId).length+1),name:n,classId:V.classId});save();render()}
function bulkStudents(){
  const lines=$('#bulk').value.split('\n').map(l=>l.trim()).filter(Boolean);let n=0,cnt=clsStudents(V.classId).length;
  lines.forEach(l=>{const m=l.split(/[,;\t]/);const nis=m.length>1?m[0].trim():'';const name=(m.length>1?m.slice(1).join(' '):m[0]).trim();if(name){S.students.push({id:uid(),nis:nis||String(++cnt),name,classId:V.classId});n++}});
  save();render();toast(n+' murid ditambahkan');
}
function delStudent(id){if(!confirm('Hapus murid ini?'))return;S.students=S.students.filter(s=>s.id!==id);save();render()}
function addSubject(){const n=$('#mName').value.trim();if(!n||S.subjects.includes(n))return;S.subjects.push(n);V.subject=n;save();render()}
function backup(){download('kelasku-cadangan.json',JSON.stringify(S),'application/json')}
function restore(f){if(!f)return;f.text().then(t=>{try{S=fixS(JSON.parse(t.replace(/^\ufeff/,'')));save();V.classId=S.classes[0]?.id;V.subject=S.subjects[0];render();toast('Data dipulihkan')}catch(e){toast('Berkas cadangan tidak valid')}})}
function resetAll(){if(!confirm('Hapus SEMUA data di browser ini? Tindakan ini tidak bisa dibatalkan.'))return;S={classes:[],students:[],subjects:['Informatika'],meetings:[],assessments:[],scores:{},notes:{},attendance:{},kkm:75,clientId:''};V.classId=undefined;V.subject='Informatika';save();render()}
 
/* ============ Impor Google Form ============ */
function formIdFromLink(l){const m=String(l).match(/\/forms\/d\/(?:e\/)?([\w-]{15,})/);return m?m[1]:''}
 
function getToken(clientId){
  return new Promise((res,rej)=>{
    const go=()=>{try{
      google.accounts.oauth2.initTokenClient({client_id:clientId,
        scope:'https://www.googleapis.com/auth/forms.body.readonly https://www.googleapis.com/auth/forms.responses.readonly',
        callback:r=>r.error?rej(new Error('Izin Google ditolak: '+r.error)):res(r.access_token)}).requestAccessToken();
    }catch(e){rej(e)}};
    if(window.google?.accounts?.oauth2)return go();
    const s=document.createElement('script');s.src='https://accounts.google.com/gsi/client';s.onload=go;
    s.onerror=()=>rej(new Error('Tidak bisa memuat layanan login Google. Periksa koneksi internet.'));document.head.appendChild(s);
  });
}
async function gfetch(url,token){
  const r=await fetch(url,{headers:{Authorization:'Bearer '+token}});
  if(!r.ok){let m='';try{m=(await r.json()).error.message}catch(e){}throw new Error(`Google menolak permintaan (${r.status}). ${m}`)}
  return r.json();
}
async function fetchAPI(){
  V.err='';const id=formIdFromLink(V.imp.link);
  if(!id){V.err='Link form tidak dikenali. Salin link dari bilah alamat saat membuka form di mode edit.';return render()}
  if(!S.clientId.trim()){V.err='Isi OAuth Client ID terlebih dahulu.';return render()}
  V.busy=true;render();
  try{
    const token=await getToken(S.clientId.trim());
    const form=await gfetch(`https://forms.googleapis.com/v1/forms/${id}`,token);
    const questions=[];let max=0;
    (form.items||[]).forEach(it=>{const q=it.questionItem?.question;if(!q)return;
      questions.push({id:q.questionId,title:it.title||'(tanpa judul)'});max+=q.grading?.pointValue||0});
    let resp=[],pt='';
    do{const d=await gfetch(`https://forms.googleapis.com/v1/forms/${id}/responses?pageSize=500${pt?'&pageToken='+pt:''}`,token);resp=resp.concat(d.responses||[]);pt=d.nextPageToken||''}while(pt);
    const responses=resp.map(r=>{const vals={};
      Object.entries(r.answers||{}).forEach(([qid,a])=>{vals[qid]=(a.textAnswers?.answers||[]).map(x=>x.value).join(', ')});
      if(r.respondentEmail)vals.__email=r.respondentEmail;
      return {vals,raw:r.totalScore,time:Date.parse(r.lastSubmittedTime||r.createTime)||0}}).sort((a,b)=>a.time-b.time);
    if(!max)max=100;
    responses.forEach(r=>r.score=r.raw==null?null:r.raw/max*100);
    if(responses.some(r=>r.vals.__email))questions.push({id:'__email',title:'Email responden'});
    startPreview({formId:id,title:form.info?.title||'',questions,responses,max});
  }catch(e){V.err=e.message}
  V.busy=false;render();
}
 
function parseCSV(t){
  const rows=[];let r=[],f='',q=false;
  for(let i=0;i<t.length;i++){const c=t[i];
    if(q){if(c==='"'){if(t[i+1]==='"'){f+='"';i++}else q=false}else f+=c}
    else if(c==='"')q=true;else if(c===','||c===';'){r.push(f);f=''}
    else if(c==='\n'){r.push(f);rows.push(r);r=[];f=''}else if(c!=='\r')f+=c}
  if(f!==''||r.length){r.push(f);rows.push(r)}
  return rows.filter(x=>x.some(v=>v.trim()!==''));
}
function readCSVFile(f){if(!f)return;f.text().then(t=>{V.imp.csv=t.replace(/^\ufeff/,'');loadCSV()})}
function loadCSV(){
  V.err='';const rows=parseCSV(V.imp.csv||'');
  if(rows.length<2){V.err='CSV kosong atau tidak terbaca.';return render()}
  const head=rows[0].map(h=>h.trim());
  let sc=head.findIndex(h=>/^(score|skor|nilai|poin|total)/i.test(h));
  if(sc<0){V.err='Kolom skor tidak ditemukan. Pastikan ada kolom bernama Skor/Score.';return render()}
  let max=0;const parsed=rows.slice(1).map((r,idx)=>{
    const cell=(r[sc]||'').trim(),m=cell.match(/(-?\d+(?:[.,]\d+)?)\s*\/\s*(\d+(?:[.,]\d+)?)/);
    let s=null,mx=null;
    if(m){s=+m[1].replace(',','.');mx=+m[2].replace(',','.')}else if(cell!==''&&!isNaN(+cell.replace(',','.'))){s=+cell.replace(',','.')}
    if(mx)max=Math.max(max,mx);
    const vals={};head.forEach((h,i)=>{vals[i]=(r[i]||'').trim()});
    return {vals,raw:s,time:idx}});
  if(!max)max=100;
  parsed.forEach(r=>r.score=r.raw==null?null:r.raw/max*100);
  const questions=head.map((h,i)=>({id:String(i),title:h||'(kolom '+(i+1)+')'})).filter((q,i)=>i!==sc);
  startPreview({formId:'',title:'',questions,responses:parsed,max});
  render();
}
function loadDemo(){
  const sts=clsStudents(V.classId);
  if(!sts.length){V.err='Kelas ini belum punya murid.';return render()}
  const responses=[];
  sts.forEach((s,i)=>{if(i%5===4)return;
    const sc=50+((i*13)%50);
    responses.push({vals:{nis:s.nis,nama:i%4===1?s.name.toLowerCase():s.name},raw:sc/10,time:i});
    if(i===2)responses.push({vals:{nis:s.nis,nama:s.name},raw:Math.min(10,sc/10+1.5),time:100+i})});
  responses.push({vals:{nis:'999999',nama:'Murid Tidak Dikenal'},raw:7,time:200});
  if(sts[0])responses.push({vals:{nis:'',nama:sts[0].name.split(' ')[0]+' P.'},raw:6,time:201});
  responses.forEach(r=>r.score=r.raw/10*100);
  startPreview({formId:'',title:'Kuis contoh',questions:[{id:'nis',title:'Nomor absen'},{id:'nama',title:'Nama lengkap'}],responses,max:10});
  render();
}
function startPreview(im){
  im.idQ=(im.questions.find(q=>/nomor|absen|\bnisn?\b|\bno\b/i.test(q.title))||im.questions.find(q=>/nama|name|email/i.test(q.title))||im.questions[0])?.id;
  im.policy='max';im.assign={};
  if(!V.imp.name)V.imp.name=im.title||'Kuis Google Form';
  V.im=im;
}
function assign(i,sid){V.im.assign[i]=sid||'';render()}
 
function computeMatches(){
  const im=V.im,sts=clsStudents(V.classId);
  const rows=im.responses.map((r,i)=>{
    const raw=String(r.vals[im.idQ]??'').trim();let st=null,how='';
    if(im.assign[i]){st=sts.find(s=>s.id===im.assign[i]);how='manual'}
    else if(raw){
      const rn=raw.replace(/^0+(?=\d)/,'');st=sts.find(s=>s.nis&&String(s.nis).replace(/^0+(?=\d)/,'')===rn);how=st?'No':'';
      if(!st){const n=norm(raw);
        st=sts.find(s=>norm(s.name)===n);if(st)how='nama';
        else if(n.length>=4){st=sts.find(s=>{const m=norm(s.name);return m.includes(n)||n.includes(m)});if(st)how='mirip'}}
    }
    return {i,raw,st,how,score:r.score};
  });
  const pick={};
  rows.forEach(r=>{if(!r.st||r.score==null)return;const p=pick[r.st.id];
    if(!p||(im.policy==='max'&&r.score>p.score)||im.policy==='last')pick[r.st.id]=r});
  return {rows,pick,missing:sts.filter(s=>!pick[s.id])};
}
 
function saveImport(){
  const im=V.im,p=V.imp,{pick}=computeMatches();
  let a=im.formId&&S.assessments.find(x=>x.formId===im.formId&&x.classId===V.classId&&x.subject===V.subject),m;
  if(a){m=S.meetings.find(x=>x.id===a.meetingId)}
  else{
    const ms=meetingsOf(V.classId,V.subject,V.gMonth);
    m=ms.find(x=>x.id===(p.meetingId||ms[ms.length-1]?.id));
    if(!m){m={id:uid(),classId:V.classId,subject:V.subject,month:V.gMonth,name:'Pertemuan '+(ms.length+1)};S.meetings.push(m)}
    const used=compsOf(m).reduce((x,c)=>x+c.weight,0),typed=Math.round(+p.weight);
    a={id:uid(),classId:V.classId,subject:V.subject,meetingId:m.id,name:(p.name||'').trim()||im.title||p.type,type:p.type,types:[p.type],
       weight:typed>0?typed:(100-used>0?100-used:10),source:'google_form',formId:im.formId||'',manual:{}};
    S.assessments.push(a);S.scores[a.id]={};
  }
  let n=0,skip=0;
  Object.entries(pick).forEach(([sid,r])=>{if(a.manual?.[sid]){skip++;return}S.scores[a.id][sid]=Math.round(r.score*10)/10;n++});
  a.syncedAt=Date.now();save();V.im=null;V.imp.name='';V.imp.meetingId='';V.tab='nilai';V.gAll=false;render();
  toast(`${n} nilai masuk ke ${m.name}: ${compLabel(a,m)}`+(skip?` (${skip} nilai yang diedit manual tidak ditimpa)`:''));
}
 
/* ============ Impor murid dari file ============ */
V.stu=null;V.nm={name:'',copy:true};V.nc={meetingId:'',jenis:'Catatan',name:'',weight:''};V.gMonth=today().slice(0,7);V.gAll=false;
function loadXLSX(){
  return new Promise((res,rej)=>{
    if(window.XLSX)return res();
    const s=document.createElement('script');s.src='https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js';
    s.onload=res;s.onerror=()=>rej(new Error('Pembaca Excel gagal dimuat (butuh internet). Simpan file sebagai CSV lalu unggah lagi.'));
    document.head.appendChild(s);
  });
}
function gridToStudents(grid){
  grid=grid.map(r=>r.map(c=>String(c??'').trim())).filter(r=>r.some(Boolean));
  if(!grid.length)return [];
  const h=grid[0].map(x=>x.toLowerCase());
  let ni=h.findIndex(x=>/^(no\b|nomor|nis|nisn|absen)/.test(x)),nm=h.findIndex(x=>/nama|name/.test(x)),start=0;
  if(nm>=0){start=1}
  else if(grid[0].length>1){
    ni=0;nm=1;
    if(/^\d+$/.test(grid[0][1])&&!/^\d+$/.test(grid[0][0])){ni=1;nm=0}
  }else{ni=-1;nm=0}
  return grid.slice(start).map(r=>({nis:ni>=0?(r[ni]||''):'',name:r[nm]||''})).filter(r=>r.name);
}
async function readStudentFile(f){
  if(!f)return;
  try{
    const ext=(f.name.split('.').pop()||'').toLowerCase();let grid;
    if(ext==='xlsx'||ext==='xls'){
      await loadXLSX();
      const wb=XLSX.read(await f.arrayBuffer(),{type:'array'});
      grid=XLSX.utils.sheet_to_json(wb.Sheets[wb.SheetNames[0]],{header:1,raw:false,defval:''});
    }else{
      let t=(await f.text()).replace(/^\ufeff/,'');
      if(t.includes('\t'))t=t.replace(/\t/g,',');
      grid=parseCSV(t);
    }
    const rows=gridToStudents(grid);
    if(!rows.length){toast('Tidak ada nama murid yang terbaca di file ini');return}
    V.stu={file:f.name,rows};render();
  }catch(e){toast(e.message||'File tidak bisa dibaca')}
}
function stuCompute(){
  const seenN=new Set(clsStudents(V.classId).map(s=>norm(s.name)));
  return V.stu.rows.map(r=>{
    const dup=seenN.has(norm(r.name));
    if(!dup)seenN.add(norm(r.name));
    return {...r,dup};
  });
}
function stuPreviewHTML(){
  if(!V.stu)return '';
  const rows=stuCompute(),n=rows.filter(r=>!r.dup).length,d=rows.length-n;
  return `<div class="panel" style="margin:12px 0 0;background:var(--kertas)">
    <p style="margin:0 0 8px"><b>${esc(V.stu.file)}</b>: ${rows.length} baris terbaca, <b>${n}</b> murid baru${d?`, ${d} dilewati karena namanya sudah ada`:''}.</p>
    <div class="scroll"><table><thead><tr><th class="num">No</th><th>Nama</th><th>Status</th></tr></thead><tbody>
    ${rows.map(r=>`<tr><td>${esc(r.nis)||'<span class="muted">–</span>'}</td><td>${esc(r.name)}</td><td>${r.dup?'<span class="badge warn">Sudah ada</span>':'<span class="badge ok">Baru</span>'}</td></tr>`).join('')}
    </tbody></table></div>
    <div class="row" style="margin-top:10px"><button class="btn" onclick="saveStudentImport()" ${n?'':'disabled'}>Tambahkan ${n} murid</button><button class="btn ghost" onclick="V.stu=null;render()">Batal</button></div>
  </div>`;
}
function saveStudentImport(){
  const rows=stuCompute().filter(r=>!r.dup);
  let cnt=clsStudents(V.classId).length;rows.forEach(r=>S.students.push({id:uid(),nis:r.nis||String(++cnt),name:r.name,classId:V.classId}));
  V.stu=null;save();render();toast(rows.length+' murid ditambahkan');
}
function downloadStudentTemplate(){
  download('templat-murid.csv','No,Nama\n1,Aditya Pratama\n2,Bunga Lestari');
}
 
/* ============ Tema pantai: karakter lucu & latar ============ */
const CH={
 crab:{w:100,h:80,g:`<g stroke="#e8553f" stroke-width="5" stroke-linecap="round" fill="none"><path d="M24 54 L10 62 M27 60 L16 72 M76 54 L90 62 M73 60 L84 72"/><path d="M24 42 Q8 40 10 24"/><path d="M76 42 Q92 40 90 24"/></g>
  <circle cx="11" cy="21" r="10" fill="#ff7a68"/><circle cx="89" cy="21" r="10" fill="#ff7a68"/>
  <path d="M11 11 V20 M89 11 V20" stroke="#e8553f" stroke-width="3" stroke-linecap="round"/>
  <ellipse cx="50" cy="52" rx="30" ry="21" fill="#ff7a68"/>
  <path d="M40 34 V28 M60 34 V28" stroke="#e8553f" stroke-width="4" stroke-linecap="round"/>
  <circle cx="40" cy="25" r="8" fill="#fff"/><circle cx="60" cy="25" r="8" fill="#fff"/>
  <circle cx="41" cy="26" r="4" fill="#1a2b4d"/><circle cx="59" cy="26" r="4" fill="#1a2b4d"/>
  <circle cx="42.3" cy="24.5" r="1.4" fill="#fff"/><circle cx="60.3" cy="24.5" r="1.4" fill="#fff"/>
  <circle cx="34" cy="55" r="4.5" fill="#ff9d8f"/><circle cx="66" cy="55" r="4.5" fill="#ff9d8f"/>
  <path d="M43 54 Q50 62 57 54" stroke="#1a2b4d" stroke-width="2.6" fill="none" stroke-linecap="round"/>`},
 star:{w:80,h:80,g:`<polygon points="40,12 48.2,30.7 68.5,32.7 53.3,46.3 57.6,66.3 40,56 22.4,66.3 26.7,46.3 11.5,32.7 31.8,30.7" fill="#ffb347" stroke="#ffb347" stroke-width="9" stroke-linejoin="round"/>
  <g fill="#ff8a3d"><circle cx="40" cy="21" r="1.8"/><circle cx="62" cy="35" r="1.8"/><circle cx="54" cy="61" r="1.8"/><circle cx="26" cy="61" r="1.8"/><circle cx="18" cy="35" r="1.8"/></g>
  <circle cx="34" cy="41" r="3.3" fill="#1a2b4d"/><circle cx="46" cy="41" r="3.3" fill="#1a2b4d"/>
  <circle cx="35" cy="40" r="1.1" fill="#fff"/><circle cx="47" cy="40" r="1.1" fill="#fff"/>
  <circle cx="29.5" cy="46" r="3" fill="#ff8f7a"/><circle cx="50.5" cy="46" r="3" fill="#ff8f7a"/>
  <path d="M36 47 Q40 52 44 47" stroke="#1a2b4d" stroke-width="2.2" fill="none" stroke-linecap="round"/>`},
 shell:{w:70,h:60,g:`<path d="M35 6 C12 6 4 30 5 46 Q35 60 65 46 C66 30 58 6 35 6Z" fill="#ffd0d9" stroke="#ff9fb3" stroke-width="3" stroke-linejoin="round"/>
  <g stroke="#ff9fb3" stroke-width="2.5" stroke-linecap="round"><path d="M35 50 V12 M35 50 L19 16 M35 50 L51 16 M35 50 L9 32 M35 50 L61 32"/></g>
  <rect x="26" y="48" width="18" height="8" rx="4" fill="#ffb3c2"/>
  <circle cx="28" cy="37" r="3" fill="#1a2b4d"/><circle cx="42" cy="37" r="3" fill="#1a2b4d"/>
  <circle cx="29" cy="36" r="1" fill="#fff"/><circle cx="43" cy="36" r="1" fill="#fff"/>
  <circle cx="22" cy="42" r="3" fill="#ff9aae"/><circle cx="48" cy="42" r="3" fill="#ff9aae"/>
  <path d="M31 43 Q35 47 39 43" stroke="#1a2b4d" stroke-width="2" fill="none" stroke-linecap="round"/>`},
 whale:{w:120,h:80,g:`<path d="M34 22 V11 M28 15 Q24 9 20 11 M40 15 Q44 9 48 11" stroke="#9fd0ff" stroke-width="4" stroke-linecap="round" fill="none"/>
  <path d="M90 44 Q104 42 106 28" stroke="#3b8cff" stroke-width="13" stroke-linecap="round" fill="none"/>
  <ellipse cx="99" cy="21" rx="11" ry="5.5" transform="rotate(25 99 21)" fill="#2f7cf0"/><ellipse cx="113" cy="21" rx="11" ry="5.5" transform="rotate(-25 113 21)" fill="#2f7cf0"/>
  <ellipse cx="54" cy="48" rx="46" ry="27" fill="#3b8cff"/>
  <path d="M12 58 Q54 82 96 58 Q80 74 54 74 Q30 74 12 58Z" fill="#d6ebff"/>
  <ellipse cx="58" cy="62" rx="10" ry="5" transform="rotate(-20 58 62)" fill="#2f7cf0"/>
  <circle cx="30" cy="44" r="4.2" fill="#1a2b4d"/><circle cx="31.3" cy="42.7" r="1.4" fill="#fff"/>
  <circle cx="22" cy="54" r="4.5" fill="#ff9fb0"/>
  <path d="M20 59 Q32 66 44 59" stroke="#1a2b4d" stroke-width="2.6" fill="none" stroke-linecap="round"/>`},
 sun:{w:80,h:80,g:`<g stroke="#ffc933" stroke-width="5" stroke-linecap="round"><path d="M40 4 V12 M40 68 V76 M4 40 H12 M68 40 H76 M14 14 L20 20 M60 60 L66 66 M66 14 L60 20 M14 66 L20 60"/></g>
  <circle cx="40" cy="40" r="22" fill="#ffd84a"/>
  <rect x="22" y="33" width="15" height="11" rx="4.5" fill="#1a2b4d"/><rect x="43" y="33" width="15" height="11" rx="4.5" fill="#1a2b4d"/><path d="M37 37 H43" stroke="#1a2b4d" stroke-width="2.5"/>
  <circle cx="26" cy="50" r="3.6" fill="#ffa56b"/><circle cx="54" cy="50" r="3.6" fill="#ffa56b"/>
  <path d="M33 51 Q40 58 47 51" stroke="#1a2b4d" stroke-width="2.6" fill="none" stroke-linecap="round"/>`},
 jelly:{w:70,h:90,g:`<g stroke="#8fb0fa" stroke-width="4" fill="none" stroke-linecap="round"><path d="M20 48 Q14 60 20 70 T20 86"/><path d="M35 50 Q29 62 35 72 T35 86"/><path d="M50 48 Q44 60 50 70 T50 86"/></g>
  <path d="M8 44 A27 31 0 0 1 62 44 Q52 51 44 44 Q35 53 26 44 Q18 51 8 44Z" fill="#a9c4ff" stroke="#7fa3f5" stroke-width="2"/>
  <circle cx="27" cy="31" r="3.3" fill="#1a2b4d"/><circle cx="43" cy="31" r="3.3" fill="#1a2b4d"/>
  <circle cx="28" cy="30" r="1.1" fill="#fff"/><circle cx="44" cy="30" r="1.1" fill="#fff"/>
  <circle cx="21" cy="37" r="3" fill="#ffa6c1"/><circle cx="49" cy="37" r="3" fill="#ffa6c1"/>
  <path d="M31 36 Q35 40 39 36" stroke="#1a2b4d" stroke-width="2" fill="none" stroke-linecap="round"/>`},
 fish:{w:80,h:50,g:`<path d="M64 25 L80 9 L80 41Z" fill="#ff8f3d"/>
  <path d="M4 25 Q22 2 52 8 Q66 12 72 25 Q66 38 52 42 Q22 48 4 25Z" fill="#ffb347"/>
  <path d="M34 9 Q42 25 34 41" stroke="#fff" stroke-width="5" fill="none" stroke-linecap="round"/>
  <circle cx="17" cy="21" r="4" fill="#1a2b4d"/><circle cx="18.2" cy="19.8" r="1.3" fill="#fff"/>
  <circle cx="14" cy="30" r="3" fill="#ff8f7a"/>
  <path d="M7 27 Q11 31 15 28" stroke="#1a2b4d" stroke-width="2" fill="none" stroke-linecap="round"/>`},
 umbrella:{w:90,h:110,g:`<path d="M45 12 V104" stroke="#8a5a2b" stroke-width="4" stroke-linecap="round"/>
  <ellipse cx="45" cy="106" rx="16" ry="4" fill="#f0c987"/>
  <path d="M5 54 Q45 -12 85 54 Q75 46 65 54 Q55 46 45 54 Q35 46 25 54 Q15 46 5 54Z" fill="#ff6b5e"/>
  <path d="M45 8 Q31 28 26 52 L40 52 Q43 30 45 8Z M45 8 Q59 28 64 52 L50 52 Q47 30 45 8Z" fill="#fff"/>
  <circle cx="45" cy="9" r="3.5" fill="#ffe066"/>`},
 boat:{w:120,h:110,g:`<path d="M60 84 V10" stroke="#8a5a2b" stroke-width="3.5" stroke-linecap="round"/>
  <path d="M64 14 V80 H108Z" fill="#fff"/><path d="M56 22 V80 H16Z" fill="#ffe066"/>
  <path d="M60 10 L78 16 L60 22Z" fill="#ff6b5e"/>
  <path d="M8 84 H112 L98 104 H22Z" fill="#ff6b5e"/><path d="M11 90 H109" stroke="#fff" stroke-width="3" opacity=".8"/>
  <circle cx="40" cy="95" r="3" fill="#fff"/><circle cx="60" cy="95" r="3" fill="#fff"/><circle cx="80" cy="95" r="3" fill="#fff"/>`}
};
const chSvg=n=>`<svg viewBox="0 0 ${CH[n].w} ${CH[n].h}" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">${CH[n].g}</svg>`;
const ch=(n,cx,yb,w,cls='')=>{const c=CH[n],h=w*c.h/c.w;return `<g class="${cls}"><svg x="${cx-w/2}" y="${yb-h}" width="${w}" height="${h}" viewBox="0 0 ${c.w} ${c.h}">${c.g}</svg></g>`};
const wv=(y,amp,fill,op=1,cls='')=>`<g class="drift ${cls}"><path d="M-300 ${y} q75 ${-amp} 150 0${' t150 0'.repeat(11)} V820 H-300Z" fill="${fill}" opacity="${op}"/></g>`;
const cloud=(x,y,sc=1,fill='#fff',op=.92)=>`<g transform="translate(${x} ${y}) scale(${sc})"><g class="cloud" fill="${fill}" opacity="${op}"><circle cx="28" cy="34" r="20"/><circle cx="60" cy="22" r="26"/><circle cx="92" cy="34" r="20"/><ellipse cx="60" cy="42" rx="58" ry="14"/></g></g>`;
const grad=(id,stops)=>`<linearGradient id="${id}" x1="0" y1="0" x2="0" y2="1">${stops.map(([o,c])=>`<stop offset="${o}" stop-color="${c}"/>`).join('')}</linearGradient>`;
const stars=(n,maxY,seed=7)=>Array.from({length:n},(_,i)=>{const x=(i*263+seed*37)%1200,y=(i*149+seed*53)%maxY,r=1+((i*7)%3)*.6;return `<circle class="twinkle" style="animation-delay:-${(i%7)*.5}s" cx="${x}" cy="${y}" r="${r}" fill="#fff" opacity=".85"/>`}).join('');
 
const SCENES={
siang:()=>`<defs>${grad('g',[[0,'#62b9ff'],[.6,'#bfe5ff'],[1,'#eaf7ff']])}<radialGradient id="sg"><stop offset="0" stop-color="#fff3b0"/><stop offset="1" stop-color="#ffd84a" stop-opacity="0"/></radialGradient></defs>
 <rect width="1200" height="800" fill="url(#g)"/>
 <circle cx="1010" cy="130" r="190" fill="url(#sg)"/>
 <g class="spin"><g stroke="#ffd84a" stroke-width="9" stroke-linecap="round">${Array.from({length:12},(_,i)=>{const a=i*30*Math.PI/180;return `<line x1="${1010+Math.cos(a)*84}" y1="${130+Math.sin(a)*84}" x2="${1010+Math.cos(a)*108}" y2="${130+Math.sin(a)*108}"/>`}).join('')}</g></g>
 <circle cx="1010" cy="130" r="64" fill="#ffd84a"/>
 ${cloud(120,110,1.3)}${cloud(520,200,.9)}${cloud(780,70,.8,'#fff',.8)}${cloud(300,350,.7,'#fff',.7)}
 <g fill="none" stroke="#fff" stroke-width="3" stroke-linecap="round"><path d="M700 160 q12 -14 24 0 q12 -14 24 0"/><path d="M780 230 q9 -10 18 0 q9 -10 18 0"/></g>
 <rect y="570" width="1200" height="230" fill="#46a3f5"/>
 ${wv(570,14,'#6cbcff',.95)}${wv(615,18,'#3a8fee',.95,'d2')}${wv(670,20,'#2a78e0',.95,'d3')}
 ${ch('boat',330,592,110,'bobsm')}
 <path d="M0 765 Q300 735 600 758 T1200 748 V800 H0Z" fill="#ffe3a8"/>`,
lagoon:()=>`<defs>${grad('g',[[0,'#7fd0ff'],[.55,'#c9ecff'],[1,'#f2fbff']])}</defs>
 <rect width="1200" height="800" fill="url(#g)"/>
 ${[[540,'#ff7a6b'],[516,'#ffab5e'],[492,'#ffe066'],[468,'#8ad8ff'],[444,'#4f93ff'],[420,'#a58bff']].map(([r,c])=>`<path d="M${600-r} 640 A${r} ${r} 0 0 1 ${600+r} 640" fill="none" stroke="${c}" stroke-width="24" opacity=".6"/>`).join('')}
 ${cloud(30,470,1.2)}${cloud(990,470,1.2)}${cloud(250,150,.9,'#fff',.8)}${cloud(820,110,1,'#fff',.85)}
 <g fill="#fff" opacity=".4"><circle cx="150" cy="300" r="26"/><circle cx="1090" cy="260" r="34"/><circle cx="930" cy="360" r="14"/><circle cx="260" cy="410" r="18"/></g>
 <rect y="610" width="1200" height="190" fill="#6cc4ff"/>
 ${wv(610,12,'#8fd6ff',.95)}${wv(655,16,'#4fb0f7',.95,'d2')}${wv(705,18,'#3996ef',.95,'d3')}
 ${ch('boat',900,634,95,'bobsm')}
 <g class="bobsm"><circle cx="300" cy="652" r="26" fill="none" stroke="#fff" stroke-width="12"/><circle cx="300" cy="652" r="26" fill="none" stroke="#ff6b5e" stroke-width="12" stroke-dasharray="20.4 20.4"/></g>
 <path d="M0 775 Q300 755 600 772 T1200 765 V800 H0Z" fill="#ffe9bd"/>`,
senja:()=>`<defs>${grad('g',[[0,'#1f3a9a'],[.35,'#4a5fd0'],[.58,'#a68de8'],[.78,'#ff9fba'],[1,'#ffd0a0']])}${grad('s',[[0,'#4a62c8'],[1,'#16296f']])}<radialGradient id="sg"><stop offset="0" stop-color="#ffd08a"/><stop offset="1" stop-color="#ff9f6a" stop-opacity="0"/></radialGradient></defs>
 <rect width="1200" height="800" fill="url(#g)"/>
 ${stars(22,300,3)}
 <circle cx="600" cy="610" r="230" fill="url(#sg)"/><circle cx="600" cy="610" r="92" fill="#ffb25e"/>
 ${cloud(140,260,1.2,'#ffc2d4',.75)}${cloud(880,330,1,'#ffc2d4',.7)}${cloud(520,150,.8,'#d8c6ff',.6)}
 <rect y="610" width="1200" height="190" fill="url(#s)"/>
 <g fill="#ffcf8a">${[0,1,2,3,4,5].map(i=>`<ellipse cx="600" cy="${628+i*22}" rx="${110-i*14}" ry="5" opacity="${.65-i*.08}"/>`).join('')}</g>
 ${wv(625,10,'#3149a8',.6)}${wv(680,14,'#223a92',.75,'d2')}${wv(735,16,'#15296f',.9,'d3')}
 <g transform="translate(860 590)"><g class="bobsm" fill="#15296f"><path d="M0 24 H80 L68 40 H12Z"/><path d="M40 22 V-30 L68 22Z"/><path d="M34 22 V-4 L12 22Z"/></g></g>
 <g fill="none" stroke="#2a3a8f" stroke-width="3" stroke-linecap="round"><path d="M300 200 q12 -14 24 0 q12 -14 24 0"/><path d="M380 250 q9 -10 18 0 q9 -10 18 0"/><path d="M930 170 q12 -14 24 0 q12 -14 24 0"/></g>`,
laut:()=>`<defs>${grad('g',[[0,'#47a6ff'],[.5,'#1f65d8'],[1,'#0b2c82']])}</defs>
 <rect width="1200" height="800" fill="url(#g)"/>
 <g fill="#fff">${[[180,60],[430,60],[760,70],[1000,50]].map(([x,w],i)=>`<polygon class="ray" style="animation-delay:-${i*1.5}s" points="${x},0 ${x+w},0 ${x+w*3.2},800 ${x-w*1.6},800" opacity=".09"/>`).join('')}</g>
 ${Array.from({length:16},(_,i)=>`<circle class="rise" style="animation-delay:-${(i*.9)%9}s;animation-duration:${8+(i%4)*2}s" cx="${(i*97+40)%1200}" cy="${760-(i%3)*40}" r="${4+(i%4)*3}" fill="none" stroke="#fff" stroke-width="2" opacity=".55"/>`).join('')}
 ${ch('fish',250,330,70,'bobsm')}${ch('fish',900,250,56,'bobsm')}${ch('fish',640,470,48,'bobsm')}${ch('jelly',1040,440,72,'bobsm')}${ch('jelly',160,540,52,'bobsm')}
 <path d="M0 760 Q200 735 420 755 T820 748 T1200 756 V800 H0Z" fill="#e7c27f"/>
 <g fill="none" stroke-linecap="round" stroke-width="9"><path d="M110 760 V690 M110 720 L88 696 M110 706 L134 684" stroke="#ff7a6b"/><path d="M980 758 V680 M980 716 L956 690 M980 700 L1004 674" stroke="#ff9ec1"/><path d="M620 752 V700 M620 724 L604 706 M620 716 L638 700" stroke="#a58bff"/><path d="M360 756 V716 M360 734 L346 720" stroke="#ffab5e"/></g>`,
malam:()=>`<defs>${grad('g',[[0,'#061642'],[.6,'#12307f'],[1,'#2449ad']])}<radialGradient id="mg"><stop offset="0" stop-color="#fff7d1" stop-opacity=".55"/><stop offset="1" stop-color="#fff7d1" stop-opacity="0"/></radialGradient></defs>
 <rect width="1200" height="800" fill="url(#g)"/>
 ${stars(60,520,5)}
 <circle cx="190" cy="150" r="130" fill="url(#mg)"/><circle cx="190" cy="150" r="54" fill="#fff4c4"/>
 <g fill="#f1de9b"><circle cx="172" cy="136" r="9"/><circle cx="208" cy="168" r="12"/><circle cx="196" cy="128" r="5"/></g>
 <path d="M820 90 L720 150" stroke="#fff" stroke-width="3" stroke-linecap="round" opacity=".7"/>
 ${cloud(620,240,1,'#2d4cae',.5)}${cloud(980,160,.8,'#2d4cae',.45)}
 <rect y="600" width="1200" height="200" fill="#0e2872"/>
 <g fill="#fff4c4">${[0,1,2,3].map(i=>`<ellipse cx="190" cy="${620+i*24}" rx="${70-i*12}" ry="4" opacity="${.5-i*.1}"/>`).join('')}</g>
 ${wv(612,12,'#1a3c98',.8)}${wv(670,16,'#142f82',.9,'d2')}${wv(730,18,'#0c2266',.95,'d3')}
 <polygon class="ray" points="990,440 200,380 200,520" fill="#ffe9a0" opacity=".12"/>
 <path d="M900 650 Q960 570 1020 585 Q1080 595 1100 650Z" fill="#0b1d5a"/>
 <path d="M978 590 L990 452 H1014 L1026 590Z" fill="#fff"/>
 <path d="M984 552 L986 534 H1018 L1020 552Z M989 502 L991 486 H1013 L1015 502Z" fill="#ff6b5e"/>
 <rect x="990" y="430" width="24" height="22" fill="#ffe066"/><path d="M984 430 L1002 410 L1020 430Z" fill="#ff6b5e"/>
 ${ch('whale',430,664,150,'bobsm')}`
};
const NAMA={siang:'Pantai Siang',lagoon:'Lagoon Pelangi',senja:'Senja Biru',laut:'Bawah Laut',malam:'Malam Berbintang'};
const AUTO={dashboard:'siang',absensi:'lagoon',nilai:'senja',impor:'laut',data:'malam'};
const MASCOT={dashboard:'sun',absensi:'crab',nilai:'star',impor:'jelly',data:'whale'};
const EMPTYCH=['shell','fish','star','jelly','crab'];
const SAND={siang:'#ffe3a8',lagoon:'#ffe9bd',senja:'#f7cba2',laut:'#e7c27f',malam:'#44579f'};
const SHORE={
 siang:[['crab',110,80],['star',300,56],['umbrella',520,92],['shell',740,56],['crab',900,60]],
 lagoon:[['star',90,58],['shell',270,60],['crab',470,84],['umbrella',700,90],['star',900,52]],
 senja:[['shell',120,58],['crab',320,80],['star',560,60],['crab',760,64],['shell',930,52]],
 laut:[['star',100,60],['crab',300,86],['shell',520,58],['star',700,50],['crab',900,70]],
 malam:[['crab',120,84],['star',320,58],['shell',560,58],['umbrella',760,84],['star',930,52]]
};
function shoreSvg(id){
  const sand=SAND[id];
  return `<svg viewBox="0 0 1000 150" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
   <path d="M0 96 Q125 78 250 92 T500 90 T750 94 T1000 88 V150 H0Z" fill="${sand}"/>
   <path d="M0 96 Q125 78 250 92 T500 90 T750 94 T1000 88" fill="none" stroke="#fff" stroke-width="5" opacity=".7" stroke-linecap="round"/>
   ${SHORE[id].map(([n,x,w],i)=>ch(n,x,120+(i%2)*6,w,i%2?'':'bobsm')).join('')}</svg>`;
}
const DECOR={scene:'',tab:'',shore:''};
function decorate(){
  const id=(S.bg&&S.bg!=='auto'&&SCENES[S.bg])?S.bg:AUTO[V.tab];
  if(DECOR.scene!==id){DECOR.scene=id;$('#scene').innerHTML=`<svg viewBox="0 0 1200 800" preserveAspectRatio="xMidYMax slice" xmlns="http://www.w3.org/2000/svg">${SCENES[id]()}</svg>`;document.body.dataset.bg=id}
  if(DECOR.tab!==V.tab){DECOR.tab=V.tab;$('#mascot').innerHTML=chSvg(MASCOT[V.tab])}
  if(DECOR.shore!==id){DECOR.shore=id;$('#shore').innerHTML=shoreSvg(id)}
  $('#gBg').value=S.bg&&SCENES[S.bg]?S.bg:'auto';
  document.querySelectorAll('.empty').forEach((e,i)=>e.insertAdjacentHTML('afterbegin',`<div class="empty-art">${chSvg(EMPTYCH[i%EMPTYCH.length])}</div>`));
}
$('.brand').innerHTML=`<span class="logo">${chSvg('whale')}</span><span>KelasKu<small>Absensi & nilai murid</small></span>`;
$('.side-note').insertAdjacentHTML('beforebegin',`<div class="side-art">${chSvg('crab')}</div>`);
$('#gBg').innerHTML=`<option value="auto">Otomatis (ganti tiap menu)</option>`+Object.keys(NAMA).map(k=>`<option value="${k}">${NAMA[k]}</option>`).join('');
$('#gBg').addEventListener('change',e=>{S.bg=e.target.value;save();render()});
 
render();
</script>
</body>
</html>
 
Claude selesai menulis balasan
