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
  --papan:#1f4d3a; --papan-2:#2b6049; --kapur:#f2f0e6;
  --kertas:#fbfcff; --garis:#d5def2; --tinta:#1d2433; --abu:#667085;
  --stabilo:#ffe66d; --merah:#d33a2c; --hijau:#1f8a52; --biru:#2f64d6;
  --radius:10px;
}
*{box-sizing:border-box}
html,body{height:100%}
body{margin:0;font-family:Figtree,system-ui,sans-serif;color:var(--tinta);background:var(--kertas);font-size:15px;line-height:1.5}
h1,h2,h3{font-family:'Bricolage Grotesque',Figtree,sans-serif;margin:0;line-height:1.15}
button,input,select,textarea{font:inherit;color:inherit}
button{cursor:pointer}
:focus-visible{outline:3px solid var(--biru);outline-offset:2px}
 
.app{display:grid;grid-template-columns:230px 1fr;min-height:100%}
aside{background:var(--papan);color:var(--kapur);padding:20px 14px;position:sticky;top:0;height:100vh;display:flex;flex-direction:column;gap:18px}
aside .brand{font-family:'Bricolage Grotesque',sans-serif;font-size:24px;font-weight:700;padding:0 8px}
aside .brand small{display:block;font:400 12px Figtree,sans-serif;opacity:.7}
nav{display:flex;flex-direction:column;gap:2px}
nav button{background:none;border:0;color:inherit;text-align:left;padding:10px 12px;border-radius:8px;opacity:.85}
nav button:hover{background:var(--papan-2)}
nav button.on{background:var(--kapur);color:var(--papan);font-weight:600;opacity:1}
.side-note{margin-top:auto;font-size:12px;opacity:.65;padding:0 8px}
 
main{padding:22px clamp(14px,3vw,34px) 90px;max-width:1100px;width:100%}
.topbar{display:flex;gap:10px;flex-wrap:wrap;align-items:end;margin-bottom:18px;padding-bottom:14px;border-bottom:2px solid var(--garis)}
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
 
.panel{background:#fff;border:1.5px solid var(--garis);border-radius:var(--radius);padding:16px;margin-bottom:16px}
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
.badge.ok{background:#d9f3e4;color:#14633a}
.badge.warn{background:#fff0c2;color:#7a5800}
.badge.bad{background:#fde1de;color:#9c2217}
.tiny-in{width:56px!important;min-height:26px!important;padding:2px 4px!important;font-size:12px}
 
.stamps{display:flex;gap:6px}
.stamps button{width:44px;height:36px;border-radius:8px;border:1.5px solid var(--garis);background:#fff;font-weight:700;color:var(--abu)}
.stamps button.on[data-s=H]{background:var(--hijau);border-color:var(--hijau);color:#fff}
.stamps button.on[data-s=I]{background:var(--biru);border-color:var(--biru);color:#fff}
.stamps button.on[data-s=S]{background:var(--stabilo);border-color:#e6c800;color:#4a4000}
.stamps button.on[data-s=A]{background:var(--merah);border-color:var(--merah);color:#fff}
 
.tabs{display:inline-flex;border:1.5px solid var(--papan);border-radius:8px;overflow:hidden;margin-bottom:12px}
.tabs button{border:0;background:#fff;padding:7px 14px;color:var(--papan);font-weight:600}
.tabs button.on{background:var(--papan);color:#fff}
.empty{padding:26px;text-align:center;color:var(--abu);border:2px dashed var(--garis);border-radius:var(--radius);background:#fff}
.drop{display:block;border:2px dashed var(--papan-2);border-radius:var(--radius);background:var(--kapur);padding:20px;text-align:center;cursor:pointer}
.drop:hover,.drop.over{background:#e8efe0;border-color:var(--papan)}
.drop b{display:block;font:700 17px 'Bricolage Grotesque',sans-serif}
.drop input{display:none}
.scroll{max-height:320px;overflow:auto;border:1.5px solid var(--garis);border-radius:var(--radius)}
.scroll table{min-width:0}
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
}
@media (prefers-reduced-motion:reduce){*{transition:none!important}}
</style>
</head>
<body>
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
      <div class="title"><h1 id="pageTitle"></h1><p id="pageSub"></p></div>
      <label>Kelas <select id="gClass"></select></label>
      <label>Mata pelajaran <select id="gSubject"></select></label>
    </div>
    <div id="view"></div>
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
let toastT;
function toast(m){const t=$('#toast');t.textContent=m;t.classList.add('show');clearTimeout(toastT);toastT=setTimeout(()=>t.classList.remove('show'),2400)}
function download(name,text,type='text/csv'){const a=document.createElement('a');a.href=URL.createObjectURL(new Blob(['\ufeff'+text],{type}));a.download=name;a.click();setTimeout(()=>URL.revokeObjectURL(a.href),500)}
const csvCell=v=>{v=String(v??'');return /[",\n;]/.test(v)?'"'+v.replace(/"/g,'""')+'"':v};
 
/* ============ Penyimpanan (localStorage, dengan cadangan memori) ============ */
const KEY='kelasku.v1';
function seed(){
  const c1={id:'k7a',name:'VII A'},c2={id:'k8a',name:'VIII A'};
  const names=['Aditya Pratama','Bunga Lestari','Citra Maharani','Dimas Saputra','Eka Wulandari','Farhan Hakim','Gita Anjani','Hendra Wijaya','Indah Permata','Joko Santoso'];
  const students=names.map((n,i)=>({id:'s'+i,nis:'2024'+pad(i+1)+'0',name:n,classId:'k7a'}));
  ['Kartika Sari','Lutfi Ramadhan','Mega Putri'].forEach((n,i)=>students.push({id:'t'+i,nis:'2023'+pad(i+1)+'0',name:n,classId:'k8a'}));
  const as=[{id:'a1',classId:'k7a',subject:'Informatika',name:'Kuis 1',type:'Kuis',weight:15,source:'manual',manual:{}},
            {id:'a2',classId:'k7a',subject:'Informatika',name:'Tugas Praktik',type:'Tugas',weight:25,source:'manual',manual:{}},
            {id:'a3',classId:'k7a',subject:'Informatika',name:'UH 1',type:'UH',weight:60,source:'manual',manual:{}}];
  const base=[88,76,92,64,80,71,95,58,84,78];
  const scores={a1:{},a2:{},a3:{}};
  students.filter(s=>s.classId==='k7a').forEach((s,i)=>{scores.a1[s.id]=base[i];scores.a2[s.id]=Math.min(100,base[i]+((i*7)%11)-4);scores.a3[s.id]=Math.min(100,base[i]+((i*5)%9)-5)});
  return {classes:[c1,c2],students,subjects:['Informatika','Matematika','IPA'],assessments:as,scores,attendance:{},kkm:75,clientId:''};
}
function load(){try{const r=localStorage.getItem(KEY);if(r)return JSON.parse(r)}catch(e){}return seed()}
function save(){try{localStorage.setItem(KEY,JSON.stringify(S))}catch(e){}}
let S=load();
 
/* ============ Hitungan ============ */
const clsStudents=id=>S.students.filter(s=>s.classId===id).sort((a,b)=>a.name.localeCompare(b.name));
function finalGrade(cid,subj,sid){
  let w=0,t=0;
  S.assessments.filter(a=>a.classId===cid&&a.subject===subj).forEach(a=>{
    const v=S.scores[a.id]?.[sid]; if(v!=null&&v!==''){w+=a.weight;t+=v*a.weight}
  });
  return w?t/w:null;
}
function attStats(cid,sid,prefix=''){
  const c={H:0,I:0,S:0,A:0};
  for(const k in S.attendance){const [kc,d]=k.split('|');if(kc!==cid||!d.startsWith(prefix))continue;const v=S.attendance[k][sid];if(v)c[v]++}
  const tot=c.H+c.I+c.S+c.A;
  return {...c,tot,pct:tot?c.H/tot*100:null};
}
 
/* ============ State tampilan ============ */
const V={tab:'dashboard',classId:S.classes[0]?.id,subject:S.subjects[0],date:today(),month:today().slice(0,7),
  method:'api',imp:{link:'',name:'',type:'Kuis',weight:10,csv:''},im:null,busy:false,err:''};
 
const TITLES={
  dashboard:['Beranda','Ringkasan kelas hari ini'],
  absensi:['Absensi','Catat kehadiran per tanggal dan lihat rekapnya'],
  nilai:['Nilai','Isi nilai, atur bobot, dan lihat nilai akhir'],
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
  const rows=st.map(s=>{const cur=rec?.[s.id]||'H';return `<tr><td>${esc(s.name)}<div class="muted small">${esc(s.nis)}</div></td>
    <td><div class="stamps">${['H','I','S','A'].map(x=>`<button data-s="${x}" class="${cur===x?'on':''}" onclick="setAtt('${s.id}','${x}')" aria-label="${{H:'Hadir',I:'Izin',S:'Sakit',A:'Alpa'}[x]}">${x}</button>`).join('')}</div></td></tr>`}).join('');
  const rk=st.map(s=>({s,a:attStats(V.classId,s.id,V.month)}));
  return `
  <div class="panel">
    <div class="row">
      <label>Tanggal<input type="date" value="${V.date}" onchange="V.date=this.value;render()"></label>
      <span class="badge ${rec?'ok':'warn'}" style="align-self:center">${rec?'Tersimpan':'Belum disimpan (bawaan: Hadir)'}</span>
      <button class="btn" onclick="allHadir()">Simpan semua Hadir</button>
    </div>
    <p class="muted small" style="margin:8px 0 0">H = Hadir, I = Izin, S = Sakit, A = Alpa. Setiap ketukan langsung tersimpan.</p>
  </div>
  ${st.length?`<div class="tbl-wrap"><table><thead><tr><th>Murid</th><th>Status</th></tr></thead><tbody>${rows}</tbody></table></div>`:`<div class="empty">Kelas ini belum punya murid.</div>`}
  <div class="panel" style="margin-top:16px">
    <div class="row"><h2 style="margin-right:auto">Rekap bulanan</h2>
      <label style="flex:0 1 170px">Bulan<input type="month" value="${V.month}" onchange="V.month=this.value;render()"></label>
      <button class="btn ghost" onclick="exportAbsen()">Ekspor CSV</button></div>
    <div class="tbl-wrap" style="margin-top:10px"><table><thead><tr><th>Murid</th><th class="num">H</th><th class="num">I</th><th class="num">S</th><th class="num">A</th><th class="num">% Hadir</th></tr></thead><tbody>
    ${rk.map(({s,a})=>`<tr><td>${esc(s.name)}</td><td class="num">${a.H}</td><td class="num">${a.I}</td><td class="num">${a.S}</td><td class="num">${a.A}</td>
      <td class="num fin ${a.pct!=null&&a.pct<85?'low':''}">${a.pct==null?'–':fmt(a.pct)+'%'}</td></tr>`).join('')}
    </tbody></table></div>
  </div>`;
},
 
nilai(){
  const st=clsStudents(V.classId),as=S.assessments.filter(a=>a.classId===V.classId&&a.subject===V.subject);
  const tw=as.reduce((x,a)=>x+a.weight,0);
  const fgs=st.map(s=>finalGrade(V.classId,V.subject,s.id));
  const ok=fgs.filter(v=>v!=null);const avg=ok.length?ok.reduce((a,b)=>a+b,0)/ok.length:null;
  return `
  <div class="panel">
    <h2>Tambah penilaian</h2>
    <div class="row">
      <label style="flex:2 1 180px">Nama<input type="text" id="nName" placeholder="mis. Kuis 2"></label>
      <label>Jenis<select id="nType" style="width:100%"><option>Tugas</option><option>Kuis</option><option>UH</option><option>PTS</option><option>PAS</option><option>Praktik</option><option>Sikap</option></select></label>
      <label style="flex:0 1 100px">Bobot (%)<input type="number" id="nW" value="10" min="1" max="100"></label>
      <button class="btn" onclick="addAssess()">Tambah</button>
    </div>
  </div>
  ${as.length?`
  <div class="row" style="margin-bottom:8px"><span class="muted small" style="margin-right:auto">KKM ${S.kkm} · total bobot <b ${tw!==100?'style="color:var(--merah)"':''}>${tw}%</b>${tw!==100?' (idealnya 100%)':''}</span>
    <button class="btn ghost sm" onclick="exportNilai()">Ekspor CSV</button></div>
  <div class="tbl-wrap"><table><thead><tr><th>Murid</th>
    ${as.map(a=>`<th class="num">${esc(a.name)}<div class="small muted" style="font-weight:400">${esc(a.type)} ${a.source==='google_form'?'<span class="badge">Form</span>':''}</div>
      <div style="display:flex;gap:3px;justify-content:center;align-items:center;margin-top:3px"><input class="tiny-in" type="number" min="1" max="100" value="${a.weight}" onchange="setW('${a.id}',this.value)" aria-label="Bobot ${esc(a.name)}">%
      <button class="btn danger sm" style="padding:0 6px;min-height:24px" onclick="delAssess('${a.id}')" aria-label="Hapus ${esc(a.name)}">×</button></div></th>`).join('')}
    <th class="num">Nilai akhir</th></tr></thead><tbody>
    ${st.map((s,i)=>`<tr><td>${esc(s.name)}</td>
      ${as.map(a=>{const v=S.scores[a.id]?.[s.id];return `<td class="num"><input type="number" min="0" max="100" step="any" value="${v??''}" class="${v!=null&&v!==''&&v<S.kkm?'low':''}" onchange="setScore('${a.id}','${s.id}',this.value)" aria-label="${esc(s.name)} ${esc(a.name)}"></td>`}).join('')}
      <td class="num fin ${fgs[i]!=null&&fgs[i]<S.kkm?'low':''}">${fmt(fgs[i])}</td></tr>`).join('')}
    <tr><td><b>Rata-rata kelas</b></td>${as.map(a=>{const vs=st.map(s=>S.scores[a.id]?.[s.id]).filter(v=>v!=null&&v!=='');return `<td class="num muted">${vs.length?fmt(vs.reduce((x,y)=>x+y,0)/vs.length):'–'}</td>`}).join('')}<td class="num fin">${fmt(avg)}</td></tr>
  </tbody></table></div>
  <p class="muted small">Nilai akhir = rata-rata tertimbang dari penilaian yang sudah terisi. Angka merah berarti di bawah KKM.</p>`
  :`<div class="empty">Belum ada penilaian untuk ${esc(V.subject)} di kelas ini. Tambahkan di atas, atau impor dari Google Form.</div>`}`;
},
 
impor(){
  const p=V.imp,im=V.im;
  const stepOn=n=>(n===1&&!im)||(n===2&&im)?'on':'';
  return `
  <div class="steps"><span class="${stepOn(1)}">1. Ambil data form</span><span class="${stepOn(2)}">2. Cek & simpan</span></div>
  <div class="note">Nilai masuk ke <b>${esc(S.classes.find(c=>c.id===V.classId)?.name||'')}</b> · <b>${esc(V.subject)}</b>. Ganti kelas atau mapel di bagian atas jika perlu.</div>
  ${im?importPreview():`
  <div class="panel">
    <div class="row">
      <label style="flex:3 1 260px">Link Google Form (mode Kuis)<input type="text" value="${esc(p.link)}" oninput="V.imp.link=this.value" placeholder="https://docs.google.com/forms/d/…/edit"></label>
      <label style="flex:2 1 160px">Nama penilaian<input type="text" value="${esc(p.name)}" oninput="V.imp.name=this.value" placeholder="mis. Kuis Bab 2"></label>
      <label style="flex:0 1 120px">Jenis<select style="width:100%" onchange="V.imp.type=this.value">${['Kuis','Tugas','UH','PTS','PAS','Praktik'].map(t=>`<option ${t===p.type?'selected':''}>${t}</option>`).join('')}</select></label>
      <label style="flex:0 1 90px">Bobot %<input type="number" value="${p.weight}" min="1" max="100" oninput="V.imp.weight=this.value"></label>
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
    ${sel?`<div class="row"><label>NIS<input type="text" id="sNis"></label><label style="flex:2 1 200px">Nama<input type="text" id="sName"></label><button class="btn" onclick="addStudent()">Tambah murid</button></div>
    <div style="margin-top:14px">
      <label class="drop" ondragover="event.preventDefault();this.classList.add('over')" ondragleave="this.classList.remove('over')" ondrop="event.preventDefault();this.classList.remove('over');readStudentFile(event.dataTransfer.files[0])">
        <b>Unggah daftar murid dari file</b>
        <span class="muted small">Seret file ke sini atau klik untuk memilih. Mendukung Excel (.xlsx, .xls) dan CSV.</span>
        <input type="file" accept=".xlsx,.xls,.csv,.txt,.tsv" onchange="readStudentFile(this.files[0])">
      </label>
      <p class="muted small" style="margin:8px 0 0">Kolom yang dibaca: <b>NIS</b> dan <b>Nama</b> (judul kolom boleh ada atau tidak). Murid masuk ke kelas yang sedang dipilih. <a href="#" onclick="downloadStudentTemplate();return false">Unduh templat CSV</a></p>
      ${stuPreviewHTML()}
    </div>
    <label class="muted small" style="display:block;margin-top:14px">Atau tempel banyak murid sekaligus, satu baris satu murid, format <b>NIS,Nama</b>
      <textarea id="bulk" placeholder="2024010,Aditya Pratama&#10;2024020,Bunga Lestari"></textarea></label>
    <div style="margin:8px 0 12px"><button class="btn ghost" onclick="bulkStudents()">Impor daftar</button></div>
    <div class="tbl-wrap"><table><thead><tr><th>NIS</th><th>Nama</th><th></th></tr></thead><tbody>
    ${clsStudents(sel).map(s=>`<tr><td>${esc(s.nis)}</td><td>${esc(s.name)}</td><td style="text-align:right"><button class="btn danger sm" onclick="delStudent('${s.id}')">Hapus</button></td></tr>`).join('')||'<tr><td colspan="3" class="muted">Belum ada murid.</td></tr>'}
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
    <p class="muted small" style="margin:10px 0 0">Skor diubah ke skala 0–100 (skor maksimum form: ${fmt(im.max)}). Pencocokan: NIS dulu, lalu nama.</p>
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
  const rows=[['Nama','NIS','Hadir','Izin','Sakit','Alpa','% Hadir']];
  clsStudents(V.classId).forEach(s=>{const a=attStats(V.classId,s.id,V.month);rows.push([s.name,s.nis,a.H,a.I,a.S,a.A,a.pct==null?'':fmt(a.pct)])});
  download(`rekap-absen-${V.month}.csv`,rows.map(r=>r.map(csvCell).join(',')).join('\n'));
}
 
function addAssess(){
  const name=$('#nName').value.trim();if(!name){toast('Isi nama penilaian dulu');return}
  const a={id:uid(),classId:V.classId,subject:V.subject,name,type:$('#nType').value,weight:+$('#nW').value||10,source:'manual',manual:{}};
  S.assessments.push(a);S.scores[a.id]={};save();render();
}
function setW(id,v){const a=S.assessments.find(x=>x.id===id);a.weight=Math.max(1,+v||1);save();render()}
function delAssess(id){const a=S.assessments.find(x=>x.id===id);if(!confirm(`Hapus penilaian "${a.name}" beserta semua nilainya?`))return;
  S.assessments=S.assessments.filter(x=>x.id!==id);delete S.scores[id];save();render()}
function setScore(aid,sid,v){
  const a=S.assessments.find(x=>x.id===aid);S.scores[aid]=S.scores[aid]||{};
  if(v===''){delete S.scores[aid][sid]}else{S.scores[aid][sid]=Math.min(100,Math.max(0,+v))}
  a.manual=a.manual||{};a.manual[sid]=true;save();render();
}
function exportNilai(){
  const as=S.assessments.filter(a=>a.classId===V.classId&&a.subject===V.subject);
  const rows=[['Nama','NIS',...as.map(a=>`${a.name} (${a.weight}%)`),'Nilai akhir']];
  clsStudents(V.classId).forEach(s=>rows.push([s.name,s.nis,...as.map(a=>S.scores[a.id]?.[s.id]??''),fmt(finalGrade(V.classId,V.subject,s.id))]));
  download(`nilai-${V.subject}.csv`,rows.map(r=>r.map(csvCell).join(',')).join('\n'));
}
 
/* ============ Aksi: data ============ */
function addClass(){const n=$('#cName').value.trim();if(!n)return;const c={id:uid(),name:n};S.classes.push(c);V.classId=c.id;save();render()}
function delClass(){const c=S.classes.find(x=>x.id===V.classId);if(!confirm(`Hapus kelas ${c.name} beserta murid, absensi, dan nilainya?`))return;
  const aid=S.assessments.filter(a=>a.classId===c.id).map(a=>a.id);aid.forEach(i=>delete S.scores[i]);
  S.assessments=S.assessments.filter(a=>a.classId!==c.id);S.students=S.students.filter(s=>s.classId!==c.id);
  Object.keys(S.attendance).forEach(k=>{if(k.startsWith(c.id+'|'))delete S.attendance[k]});
  S.classes=S.classes.filter(x=>x.id!==c.id);V.classId=S.classes[0]?.id;save();render()}
function addStudent(){const n=$('#sName').value.trim();if(!n)return;S.students.push({id:uid(),nis:$('#sNis').value.trim(),name:n,classId:V.classId});save();render()}
function bulkStudents(){
  const lines=$('#bulk').value.split('\n').map(l=>l.trim()).filter(Boolean);let n=0;
  lines.forEach(l=>{const m=l.split(/[,;\t]/);const nis=m.length>1?m[0].trim():'';const name=(m.length>1?m.slice(1).join(' '):m[0]).trim();if(name){S.students.push({id:uid(),nis,name,classId:V.classId});n++}});
  save();render();toast(n+' murid ditambahkan');
}
function delStudent(id){if(!confirm('Hapus murid ini?'))return;S.students=S.students.filter(s=>s.id!==id);save();render()}
function addSubject(){const n=$('#mName').value.trim();if(!n||S.subjects.includes(n))return;S.subjects.push(n);V.subject=n;save();render()}
function backup(){download('kelasku-cadangan.json',JSON.stringify(S),'application/json')}
function restore(f){if(!f)return;f.text().then(t=>{try{S=JSON.parse(t.replace(/^\ufeff/,''));save();V.classId=S.classes[0]?.id;V.subject=S.subjects[0];render();toast('Data dipulihkan')}catch(e){toast('Berkas cadangan tidak valid')}})}
function resetAll(){if(!confirm('Hapus SEMUA data di browser ini? Tindakan ini tidak bisa dibatalkan.'))return;S={classes:[],students:[],subjects:['Informatika'],assessments:[],scores:{},attendance:{},kkm:75,clientId:''};V.classId=undefined;V.subject='Informatika';save();render()}
 
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
  startPreview({formId:'',title:'Kuis contoh',questions:[{id:'nis',title:'NIS'},{id:'nama',title:'Nama lengkap'}],responses,max:10});
  render();
}
function startPreview(im){
  im.idQ=(im.questions.find(q=>/nis|nisn/i.test(q.title))||im.questions.find(q=>/nama|name|email/i.test(q.title))||im.questions[0])?.id;
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
      st=sts.find(s=>s.nis&&s.nis===raw);how=st?'NIS':'';
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
  let a=im.formId&&S.assessments.find(x=>x.formId===im.formId&&x.classId===V.classId&&x.subject===V.subject);
  if(!a){a={id:uid(),classId:V.classId,subject:V.subject,name:p.name||'Kuis Google Form',type:p.type,weight:+p.weight||10,source:'google_form',formId:im.formId||'',manual:{}};
    S.assessments.push(a);S.scores[a.id]={}}
  let n=0,skip=0;
  Object.entries(pick).forEach(([sid,r])=>{if(a.manual?.[sid]){skip++;return}S.scores[a.id][sid]=Math.round(r.score*10)/10;n++});
  a.syncedAt=Date.now();save();V.im=null;V.imp.name='';V.tab='nilai';render();
  toast(`${n} nilai masuk ke ${a.name}`+(skip?` (${skip} nilai yang diedit manual tidak ditimpa)`:''));
}
 
/* ============ Impor murid dari file ============ */
V.stu=null;
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
  let ni=h.findIndex(x=>/^(nis|nisn|no\.? ?induk)/.test(x)),nm=h.findIndex(x=>/nama|name/.test(x)),start=0;
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
  const cur=clsStudents(V.classId),seenN=new Set(cur.map(s=>norm(s.name))),seenI=new Set(cur.filter(s=>s.nis).map(s=>s.nis));
  return V.stu.rows.map(r=>{
    const dup=(r.nis&&seenI.has(r.nis))||seenN.has(norm(r.name));
    if(!dup){seenN.add(norm(r.name));if(r.nis)seenI.add(r.nis)}
    return {...r,dup};
  });
}
function stuPreviewHTML(){
  if(!V.stu)return '';
  const rows=stuCompute(),n=rows.filter(r=>!r.dup).length,d=rows.length-n;
  return `<div class="panel" style="margin:12px 0 0;background:var(--kertas)">
    <p style="margin:0 0 8px"><b>${esc(V.stu.file)}</b>: ${rows.length} baris terbaca, <b>${n}</b> murid baru${d?`, ${d} dilewati karena sudah ada`:''}.</p>
    <div class="scroll"><table><thead><tr><th>NIS</th><th>Nama</th><th>Status</th></tr></thead><tbody>
    ${rows.map(r=>`<tr><td>${esc(r.nis)||'<span class="muted">–</span>'}</td><td>${esc(r.name)}</td><td>${r.dup?'<span class="badge warn">Sudah ada</span>':'<span class="badge ok">Baru</span>'}</td></tr>`).join('')}
    </tbody></table></div>
    <div class="row" style="margin-top:10px"><button class="btn" onclick="saveStudentImport()" ${n?'':'disabled'}>Tambahkan ${n} murid</button><button class="btn ghost" onclick="V.stu=null;render()">Batal</button></div>
  </div>`;
}
function saveStudentImport(){
  const rows=stuCompute().filter(r=>!r.dup);
  rows.forEach(r=>S.students.push({id:uid(),nis:r.nis,name:r.name,classId:V.classId}));
  V.stu=null;save();render();toast(rows.length+' murid ditambahkan');
}
function downloadStudentTemplate(){
  download('templat-murid.csv','NIS,Nama\n2024010,Aditya Pratama\n2024020,Bunga Lestari');
}
 
render();
</script>
</body>
</html>
 
Claude selesai menulis balasan
# Management-Teacher
