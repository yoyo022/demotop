[index (2).html](https://github.com/user-attachments/files/35307508/index.2.html)
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>TokoKu – Stok, Penjualan, Invoice & Pajak</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;700;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#F1F4F6;--card:#fff;--ink:#17262E;--mut:#46586A;--line:#C5D0D8;--pri:#0E5A6B;--pri-t:#fff;--soft:#E1EFF2;--warn:#B45F06;--warnbg:#FCEBD3;--bad:#B3261E;--ok:#1B7A46;--okbg:#DDF1E5;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0F1A20;--card:#17262E;--ink:#E8EEF1;--mut:#B4C3CC;--line:#3B5764;--pri:#4FB6CB;--pri-t:#08232A;--soft:#1B3A44;--warn:#F2B35E;--warnbg:#3A2C14;--bad:#F2877F;--ok:#6FD39A;--okbg:#17352450;color-scheme:dark}}
*{box-sizing:border-box}html,body{margin:0}
body{background:var(--bg);color:var(--ink);font:15px/1.5 "Plus Jakarta Sans",system-ui,sans-serif}
.app{display:grid;grid-template-columns:210px 1fr;min-height:100vh}
nav{background:var(--card);border-right:1px solid var(--line);padding:18px 12px;position:sticky;top:0;height:100vh}
.brand{font-weight:800;font-size:20px;padding:0 10px 16px;color:var(--pri)}
nav button{display:block;width:100%;text-align:left;border:0;background:none;color:var(--ink);padding:10px 12px;border-radius:8px;font:inherit;cursor:pointer;margin-bottom:2px}
nav button.on{background:var(--soft);color:var(--pri);font-weight:700}
nav button:focus-visible,button:focus-visible,input:focus-visible,select:focus-visible{outline:2px solid var(--pri);outline-offset:2px}
main{padding:24px;max-width:1000px;width:100%}
h1{font-size:24px;margin:0 0 4px;font-weight:800}h2{font-size:16px;margin:0 0 10px}
.sub{color:var(--mut);margin:0 0 18px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:12px;margin-bottom:16px}
.card{background:var(--card);border:1px solid var(--line);border-radius:10px;padding:16px;margin-bottom:16px}
.grid .card{margin:0}
.k{color:var(--mut);font-size:13px}.v{font-size:22px;font-weight:800;margin-top:2px}
.hero .v{font-size:30px;color:var(--pri)}
table{width:100%;border-collapse:collapse}th,td{padding:9px 8px;border-bottom:1px solid var(--line);text-align:left;vertical-align:middle;color:var(--ink)}
th{color:var(--ink);font-weight:700;font-size:13px;background:var(--soft)}
main table,main tr,main td,main th{background:transparent!important;border-left:0!important;border-right:0!important;border-top:0!important;box-shadow:none!important}
main th{background:var(--soft)!important}
main td,main th{border-bottom:1px solid var(--line)!important;color:var(--ink)!important}
main h1,main h2{border:0!important;padding:0!important;margin-top:0!important}
main h1{font-size:24px!important}main h2{font-size:16px!important}td.r,th.r{text-align:right}
.tw{overflow-x:auto}
input,select{font:inherit;color:var(--ink);background:var(--bg);border:1px solid var(--line);border-radius:8px;padding:8px 10px;min-width:0}
.row{display:flex;gap:8px;flex-wrap:wrap;align-items:flex-end;margin-bottom:10px}
.row label{display:flex;flex-direction:column;gap:3px;font-size:13px;color:var(--mut)}
.btn{background:var(--pri);color:var(--pri-t);border:0;border-radius:8px;padding:9px 14px;font:inherit;font-weight:700;cursor:pointer}
.btn.g{background:none;color:var(--pri);border:1px solid var(--line)}
.btn.sm{padding:2px 9px;font-size:12px;font-weight:600;margin-left:6px}
.tag{display:inline-block;padding:2px 9px;border-radius:99px;font-size:12px;font-weight:700}
.t-ok{background:var(--okbg);color:var(--ok)}.t-w{background:var(--warnbg);color:var(--warn)}
.bars{display:flex;align-items:flex-end;gap:5px;height:110px}
.bars div{flex:1;background:var(--pri);border-radius:3px 3px 0 0;min-height:2px;opacity:.85}
.prog{height:10px;background:var(--soft);border-radius:9px;overflow:hidden}.prog i{display:block;height:100%;background:var(--pri)}
.note{background:var(--warnbg);color:var(--warn);border-radius:8px;padding:10px 12px;font-size:13px}
.modal{position:fixed;inset:0;background:#0009;display:flex;align-items:flex-start;justify-content:center;overflow:auto;padding:20px;z-index:20}
.inv{background:#fff;color:#111;max-width:640px;width:100%;border-radius:10px;padding:28px}
.inv table td,.inv table th{border-color:#ddd;color:#111}.inv th{background:#eee;color:#222}
.toast{position:fixed;left:50%;transform:translateX(-50%);bottom:84px;background:var(--ink);color:var(--bg);padding:10px 16px;border-radius:8px;z-index:30}
@media(max-width:720px){
.app{grid-template-columns:1fr}
nav{position:fixed;bottom:0;left:0;right:0;top:auto;height:auto;display:flex;border-right:0;border-top:1px solid var(--line);padding:6px 4px calc(6px + env(safe-area-inset-bottom,0px));z-index:10}
.brand{display:none}nav button{text-align:center;font-size:11px;padding:8px 2px;margin:0}
main{padding:16px 14px 90px}}
@media print{body *{visibility:hidden}.modal,.modal *{visibility:visible}.modal{position:absolute;background:none;padding:0}.noprint{display:none!important}}
</style>
</head>
<body>
<div class="app">
<nav id="nav"></nav>
<main id="main"></main>
</div>
<div id="modal"></div>
<script>
const $=s=>document.querySelector(s);
const rp=n=>(n<0?'-':'')+'Rp '+Math.round(Math.abs(n)).toLocaleString('id-ID');
const fd=d=>new Date(d).toLocaleDateString('id-ID',{day:'2-digit',month:'2-digit',year:'numeric'});
const fdt=d=>new Date(d).toLocaleString('id-ID',{day:'2-digit',month:'2-digit',year:'numeric',hour:'2-digit',minute:'2-digit'});
const iso=o=>{const d=new Date();d.setDate(d.getDate()-o);return d.toISOString().slice(0,10)};
const esc=s=>String(s).replace(/[&<>"]/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;'}[c]));
function terbilang(n){n=Math.floor(n);const s=['','satu','dua','tiga','empat','lima','enam','tujuh','delapan','sembilan','sepuluh','sebelas'];
const t=n=>{if(n<12)return s[n];if(n<20)return t(n-10)+' belas';if(n<100)return s[Math.floor(n/10)]+' puluh '+t(n%10);if(n<200)return 'seratus '+t(n-100);if(n<1e3)return s[Math.floor(n/100)]+' ratus '+t(n%100);if(n<2e3)return 'seribu '+t(n-1e3);if(n<1e6)return t(Math.floor(n/1e3))+' ribu '+t(n%1e3);if(n<1e9)return t(Math.floor(n/1e6))+' juta '+t(n%1e6);return t(Math.floor(n/1e9))+' miliar '+t(n%1e9)};
const r=n?t(n).replace(/\s+/g,' ').trim():'nol';return r.charAt(0).toUpperCase()+r.slice(1)+' rupiah'}

let S;
const seed=()=>({
 set:{nama:'Toko Berkah Jaya',alamat:'Jl. Dago No. 12, Bandung',npwp:'12.345.678.9-421.000',bank:'BCA 123 456 7890 a.n. Berkah Jaya',pkp:true,ppn:11,pph:0.5},
 items:[
  {id:1,sku:'CT30-01',warna:'Merah Maroon',name:'Cotton Combed 30s',unit:'kg',buy:78000,sell:92000,stock:312.4,ctn:13,min:100},
  {id:2,sku:'CT30-02',warna:'Biru Navy',name:'Cotton Combed 30s',unit:'kg',buy:78000,sell:92000,stock:74.85,ctn:3,min:100},
  {id:3,sku:'PL40-10',warna:'Putih',name:'Polyester 40s',unit:'kg',buy:42000,sell:51000,stock:518.3,ctn:26,min:150},
  {id:4,sku:'AC24-05',warna:'Hijau Botol',name:'Akrilik 24s',unit:'kg',buy:65000,sell:78000,stock:180.15,ctn:7,min:80},
  {id:5,sku:'RY30-07',warna:'Hitam',name:'Rayon 30s',unit:'kg',buy:58000,sell:70000,stock:90.6,ctn:4,min:100}],
 sales:[
  {no:'INV/2026/11/0001',date:iso(9),cust:'Konveksi Maju Jaya',lines:[{id:1,name:'CT30-01 · Merah Maroon',qty:125,price:92000,cost:78000}],paid:true},
  {no:'INV/2026/11/0002',date:iso(5),cust:'Pabrik Kaos Sinar',lines:[{id:3,name:'PL40-10 · Putih',qty:200,price:51000,cost:42000},{id:2,name:'CT30-02 · Biru Navy',qty:50,price:92000,cost:78000}],paid:false},
  {no:'INV/2026/11/0003',date:iso(1),cust:'Toko Rajut Ibu Ani',lines:[{id:4,name:'AC24-05 · Hijau Botol',qty:37.5,price:78000,cost:65000}],paid:true}],
 buys:[
  {date:iso(12),sup:'PT Benang Nusantara',lines:[{id:1,name:'CT30-01 · Merah Maroon',qty:500,price:78000}],paid:true},
  {date:iso(7),sup:'CV Serat Prima',lines:[{id:3,name:'PL40-10 · Putih',qty:400,price:42000}],paid:false}]
});
try{S=JSON.parse(localStorage.getItem('tokoku3')||'null')}catch(e){}
if(!S)S=seed();
const save=()=>{try{localStorage.setItem('tokoku3',JSON.stringify(S))}catch(e){}};
const calc=(lines,pkp,rate)=>{const sub=lines.reduce((a,l)=>a+Math.round(l.qty*l.price),0);const ppn=pkp?Math.round(sub*rate/100):0;return{sub,ppn,total:sub+ppn}};
const tot=t=>calc(t.lines,S.set.pkp,S.set.ppn);
const toast=m=>{const e=document.createElement('div');e.className='toast';e.textContent=m;document.body.appendChild(e);setTimeout(()=>e.remove(),2200)};

let D={s:iso(0),b:iso(0)},F={q:'',j:'',low:false,s:''},view='dash',cart=[],bcart=[],month=new Date().toISOString().slice(0,7);
const tabs=[['dash','Ringkasan'],['items','Barang'],['sell','Penjualan'],['buy','Pembelian'],['tax','Pajak']];
function nav(){$('#nav').innerHTML='<div class="brand">TokoKu</div>'+tabs.map(([k,l])=>`<button class="${view===k?'on':''}" onclick="go('${k}')">${l}</button>`).join('')}
function go(v){view=v;render()}
const lbl=i=>i.sku+' · '+i.warna;
const kg=n=>(+n).toLocaleString('id-ID',{minimumFractionDigits:2,maximumFractionDigits:2})+' kg';
const pk=i=>i.ctn!=null?`${i.ctn} karung`:'';
const sum=a=>a.reduce((x,y)=>x+y,0),r2=n=>Math.round(n*100)/100;
const parseW=s=>(s||'').split(/[+;\s]+/).map(x=>parseFloat(x.replace(',','.'))).filter(x=>x>0);
function pv(p){const w=parseW($('#'+p+'_w').value),el=$('#'+p+'_pv'),pr=$('#'+p+'_price'),q=r2(sum(w));el.textContent=w.length?`${w.length} karung = ${kg(q)}`+(pr?` · total ${rp(q*pr.value)}`:''):''}
const act=()=>S.sales.filter(s=>!s.batal);
const opts=()=>S.items.map(i=>`<option value="${i.id}">${esc(lbl(i))} – ${esc(i.name)} (stok ${kg(i.stock)})</option>`).join('');
const tagp=p=>p?'<span class="tag t-ok">Lunas</span>':'<span class="tag t-w">Belum lunas</span>';

function dash(){
 const m=new Date().toISOString().slice(0,7);
 const ms=act().filter(s=>s.date.startsWith(m)),mb=S.buys.filter(s=>s.date.startsWith(m));
 const sj=ms.reduce((a,s)=>a+calc(s.lines,0,0).sub,0),bj=mb.reduce((a,s)=>a+calc(s.lines,0,0).sub,0);
 const hpp=ms.reduce((a,s)=>a+s.lines.reduce((x,l)=>x+l.qty*l.cost,0),0);
 const nilai=S.items.reduce((a,i)=>a+i.stock*i.buy,0);
 const days=[...Array(14)].map((_,i)=>{const d=iso(13-i);return act().filter(s=>s.date===d).reduce((a,s)=>a+calc(s.lines,0,0).sub,0)});
 const mx=Math.max(...days,1);
 const low=S.items.filter(i=>i.stock<=i.min);
 const unpaid=act().filter(s=>!s.paid);
 return `<h1>Ringkasan</h1><p class="sub">${esc(S.set.nama)} · bulan ini</p>
 <div class="grid"><div class="card hero"><div class="k">Penjualan</div><div class="v">${rp(sj)}</div></div>
 <div class="card"><div class="k">Pembelian</div><div class="v">${rp(bj)}</div></div>
 <div class="card"><div class="k">Laba kotor</div><div class="v">${rp(sj-hpp)}</div></div>
 <div class="card"><div class="k">Nilai stok · ${kg(S.items.reduce((a,i)=>a+i.stock,0))}</div><div class="v">${rp(nilai)}</div></div></div>
 <div class="card"><h2>Penjualan 14 hari terakhir</h2><div class="bars">${days.map(d=>`<div title="${rp(d)}" style="height:${d/mx*100}%"></div>`).join('')}</div></div>
 <div class="grid" style="grid-template-columns:repeat(auto-fit,minmax(280px,1fr))">
 <div class="card"><h2>Stok menipis</h2>${low.length?low.map(i=>`<div class="row" style="justify-content:space-between;margin:0 0 6px"><span>${esc(i.name)}</span><span class="tag t-w">sisa ${kg(i.stock)}</span></div>`).join(''):'<p class="sub">Semua stok aman.</p>'}</div>
 <div class="card"><h2>Invoice belum dibayar</h2>${unpaid.length?unpaid.map(s=>`<div class="row" style="justify-content:space-between;margin:0 0 6px"><a href="#" onclick="inv('${s.no}');return false">${s.no}</a><span>${rp(tot(s).total)}</span></div>`).join(''):'<p class="sub">Tidak ada tagihan tertunda.</p>'}</div></div>`}

function items(){return `<h1>Barang & stok</h1><p class="sub">Satu baris = satu kode + warna. Stok dicatat dari berat tiap karung (kg, 2 desimal); jumlah karung dihitung otomatis.</p>
 <div class="card"><h2>Tambah barang</h2><div class="row">
 <label>Kode<input id="n_sku" size="8"></label><label>Warna<input id="n_warna" size="12"></label><label>Jenis benang<input id="n_name" size="14"></label>
 <label>Stok awal: berat tiap karung (kg)<input id="n_w" placeholder="24,85 + 25,10 + 24,90" style="width:260px" oninput="pv('n')"></label><span class="k" id="n_pv"></span>
 <label>Harga beli/kg<input id="n_buy" type="number" min="0" style="width:100px"></label><label>Harga jual/kg<input id="n_sell" type="number" min="0" style="width:100px"></label>
 <label>Stok min (kg)<input id="n_min" type="number" min="0" style="width:90px" value="50"></label><button class="btn" onclick="addItem()">Simpan barang</button></div></div>
 <div class="card"><div class="row" style="margin:0"><label>Cari kode / warna<input id="f_q" value="${esc(F.q)}" oninput="fl()" placeholder="mis. maroon atau CT30"></label>
 <label>Jenis benang<select id="f_j" onchange="fl()"><option value="">Semua</option>${[...new Set(S.items.map(i=>i.name))].map(n=>`<option ${F.j===n?'selected':''}>${esc(n)}</option>`).join('')}</select></label>
 <label>Urutkan<select id="f_s" onchange="fl()"><option value="">Bawaan</option><option value="hi" ${F.s==='hi'?'selected':''}>Stok terbanyak</option><option value="lo" ${F.s==='lo'?'selected':''}>Stok tersedikit</option></select></label>
 <label style="flex-direction:row;align-items:center;gap:6px;padding-bottom:9px"><input type="checkbox" id="f_l" ${F.low?'checked':''} onchange="fl()">Stok menipis saja</label></div></div>
 <div class="card tw"><table><tr><th>Kode</th><th>Warna</th><th class="r">Beli/kg</th><th class="r">Jual/kg</th><th class="r">Stok</th></tr>
 <tbody id="irows">${itemRows()}</tbody></table></div>`}
function itemRows(){const q=F.q.toLowerCase();
 let a=S.items.filter(i=>(!q||(i.sku+' '+i.warna+' '+i.name).toLowerCase().includes(q))&&(!F.j||i.name===F.j)&&(!F.low||i.stock<=i.min));
 if(F.s==='hi')a.sort((x,y)=>y.stock-x.stock);if(F.s==='lo')a.sort((x,y)=>x.stock-y.stock);
 const gs=[...new Set(a.map(i=>i.name))];return a.length?gs.map(g=>{const m=a.filter(i=>i.name===g);return `<tr><td colspan="5" style="background:var(--soft);color:var(--pri);font-weight:700">${esc(g)} <span class="k">· ${m.length} warna · ${kg(sum(m.map(i=>i.stock)))}</span></td></tr>`+m.map(i=>`<tr><td>${esc(i.sku)}</td><td>${esc(i.warna)}</td><td class="r">${rp(i.buy)}</td><td class="r">${rp(i.sell)}</td><td class="r">${i.stock<=i.min?`<span class="tag t-w">${kg(i.stock)}</span>`:kg(i.stock)}<div class="k">${pk(i).trim()}</div></td></tr>`).join('')}).join(''):'<tr><td colspan="5" class="k">Tidak ada barang yang cocok.</td></tr>'}
function fl(){F.q=$('#f_q').value;F.j=$('#f_j').value;F.low=$('#f_l').checked;F.s=$('#f_s').value;$('#irows').innerHTML=itemRows()}
function addItem(){const g=k=>$('#n_'+k).value.trim();if(!g('sku')||!g('warna'))return toast('Isi kode dan warna dulu');
 S.items.push({id:Date.now(),sku:g('sku'),warna:g('warna'),name:g('name')||'-',unit:'kg',buy:+g('buy')||0,sell:+g('sell')||0,stock:r2(sum(parseW(g('w')))),ctn:parseW(g('w')).length,min:+g('min')||0});save();toast('Barang disimpan');render()}

function cartTable(c,k){const t=calc(c,k==='sell'&&S.set.pkp,S.set.ppn);const t2=k==='buy'?calc(c,S.set.pkp,S.set.ppn):t;
 return c.length?`<div class="tw"><table>${c.map((l,i)=>`<tr><td>${esc(l.name)}</td><td class="r">${l.n?l.n+' karung · ':''}${kg(l.qty)} × ${rp(l.price)}/kg</td><td class="r">${rp(l.qty*l.price)}</td><td><button class="btn g" onclick="${k}Cart.splice(${i},1);render()">Hapus</button></td></tr>`).join('')}
 <tr><td colspan="2" class="r">PPN ${S.set.pkp?S.set.ppn+'%':'(non-PKP)'}</td><td class="r">${rp(t2.ppn)}</td><td></td></tr><tr><td colspan="2" class="r"><b>Total</b></td><td class="r"><b>${rp(t2.total)}</b></td><td></td></tr></table></div>`:'<p class="sub">Belum ada barang di daftar.</p>'}
function sell(){return `<h1>Penjualan</h1><p class="sub">Simpan transaksi untuk membuat invoice dan mengurangi stok.</p>
 <div class="card"><h2>Transaksi baru</h2><div class="row"><label>Tanggal<input type="date" value="${D.s}" onchange="D.s=this.value"></label><label>Pelanggan<input id="s_cust" placeholder="Nama pelanggan" value="Pelanggan Umum"></label>
 <label>Barang<select id="s_item" onchange="$('#s_price').value=S.items.find(i=>i.id==this.value).sell">${opts()}</select></label>
 <label>Berat tiap karung (kg)<input id="s_w" placeholder="24,85 + 25,10 + 24,90" style="width:260px" oninput="pv('s')"></label>
 <label>Harga/kg<input id="s_price" type="number" style="width:110px" value="${S.items[0]?S.items[0].sell:0}"></label><button class="btn g" onclick="addLine('sell')">Tambah</button></div><div class="k" id="s_pv" style="margin:-4px 0 8px"></div>
 ${cartTable(cart,'sell')}
 <div class="row" style="margin-top:12px"><label>Pembayaran<select id="s_paid"><option value="1">Lunas (tunai/transfer/QRIS)</option><option value="0">Tempo (piutang)</option></select></label><button class="btn" onclick="saveSale()">Simpan & buat invoice</button></div></div>
 <div class="card tw"><h2>Riwayat penjualan</h2><table><tr><th>Invoice</th><th>Tanggal</th><th>Pelanggan</th><th class="r">Total</th><th>Status</th></tr>
 ${[...S.sales].reverse().map(s=>`<tr><td><a href="#" onclick="inv('${s.no}');return false">${s.no}</a></td><td>${fd(s.date)}</td><td>${esc(s.cust)}</td><td class="r">${rp(tot(s).total)}</td><td>${s.batal?'<span class="tag t-w">Batal</span>':tagp(s.paid)+(s.paid&&s.paidAt?` <span class="k">${fdt(s.paidAt)}</span>`:'')}</td></tr>`).join('')}</table></div>`}
function buy(){return `<h1>Pembelian</h1><p class="sub">Catat barang masuk dari supplier. Stok dan harga beli ikut diperbarui.</p>
 <div class="card"><h2>Pembelian baru</h2><div class="row"><label>Tanggal<input type="date" value="${D.b}" onchange="D.b=this.value"></label><label>Supplier<input id="b_sup" placeholder="Nama supplier"></label>
 <label>Barang<select id="b_item" onchange="$('#b_price').value=S.items.find(i=>i.id==this.value).buy">${opts()}</select></label>
 <label>Berat tiap karung (kg)<input id="b_w" placeholder="24,85 + 25,10 + 24,90" style="width:260px" oninput="pv('b')"></label>
 <label>Harga beli/kg<input id="b_price" type="number" style="width:110px" value="${S.items[0]?S.items[0].buy:0}"></label><button class="btn g" onclick="addLine('buy')">Tambah</button></div><div class="k" id="b_pv" style="margin:-4px 0 8px"></div>
 ${cartTable(bcart,'buy')}
 <div class="row" style="margin-top:12px"><label>Pembayaran<select id="b_paid"><option value="1">Lunas</option><option value="0">Hutang</option></select></label><button class="btn" onclick="saveBuy()">Simpan pembelian</button></div></div>
 <div class="card tw"><h2>Riwayat pembelian</h2><table><tr><th>Tanggal</th><th>Supplier</th><th class="r">Total</th><th>Status</th></tr>
 ${[...S.buys].reverse().map(b=>`<tr><td>${fd(b.date)}</td><td>${esc(b.sup)}</td><td class="r">${rp(tot(b).total)}</td><td>${tagp(b.paid)}${b.paid?(b.paidAt?` <span class="k">${fdt(b.paidAt)}</span>`:'')+` <button class="btn g sm" onclick="payB(${S.buys.indexOf(b)},false)">Batal lunas</button>`:` <button class="btn g sm" onclick="payB(${S.buys.indexOf(b)},true)">Tandai lunas</button>`}</td></tr>`).join('')}</table></div>`}
function addLine(k){const p=k==='sell'?'s':'b',it=S.items.find(i=>i.id==$('#'+p+'_item').value),price=+$('#'+p+'_price').value;
 const w=parseW($('#'+p+'_w').value),qty=r2(sum(w)),n=w.length;
 if(!it||!(qty>0))return;const c=k==='sell'?cart:bcart;
 if(k==='sell'&&(c.filter(l=>l.id===it.id).reduce((a,l)=>a+l.qty,0)+qty>it.stock+0.001||c.filter(l=>l.id===it.id).reduce((a,l)=>a+l.n,0)+n>(it.ctn||0)))return toast('Stok '+lbl(it)+' tidak cukup (sisa '+kg(it.stock)+', '+(it.ctn||0)+' karung)');
 c.push({id:it.id,name:lbl(it),qty,n,price,cost:it.buy});const v=($('#s_cust')||{}).value,sp=($('#b_sup')||{}).value;render();if(v)$('#s_cust').value=v;if(sp)$('#b_sup').value=sp}
function saveSale(){if(!cart.length)return toast('Tambahkan barang dulu');
 const d=new Date((D.s||iso(0))+'T00:00:00'),pre=`INV/${d.getFullYear()}/${String(d.getMonth()+1).padStart(2,'0')}/`;
 const n=S.sales.filter(s=>s.no.startsWith(pre)).length+1,no=pre+String(n).padStart(4,'0');
 cart.forEach(l=>{const i=S.items.find(i=>i.id===l.id);i.stock=r2(i.stock-l.qty);i.ctn-=l.n});
 S.sales.push({no,date:D.s||iso(0),cust:$('#s_cust').value||'Pelanggan Umum',lines:cart,paid:$('#s_paid').value==='1'});cart=[];save();render();inv(no)}
function saveBuy(){if(!bcart.length)return toast('Tambahkan barang dulu');
 bcart.forEach(l=>{const i=S.items.find(i=>i.id===l.id);i.stock=r2(i.stock+l.qty);i.ctn=(i.ctn||0)+l.n;i.buy=l.price});
 S.buys.push({date:D.b||iso(0),sup:$('#b_sup').value||'Supplier',lines:bcart.map(({id,name,qty,n,price})=>({id,name,qty,n,price})),paid:$('#b_paid').value==='1'});bcart=[];save();toast('Pembelian disimpan, stok bertambah');render()}

function inv(no){const s=S.sales.find(x=>x.no===no),t=tot(s);
 $('#modal').innerHTML=`<div class="modal" onclick="if(event.target===this)closeM()"><div class="inv">
 <div style="display:flex;justify-content:space-between;gap:12px;flex-wrap:wrap"><div><b style="font-size:18px">${esc(S.set.nama)}</b><br>${esc(S.set.alamat)}<br>NPWP ${esc(S.set.npwp)}</div><div style="text-align:right"><b style="font-size:18px">INVOICE</b><br>${s.no}<br>${fd(s.date)}<br>${s.batal?'<b style="color:#B3261E">BATAL</b>':s.paid?'<b style="color:#1B7A46">LUNAS</b>'+(s.paidAt?'<br><small>'+fdt(s.paidAt)+'</small>':''):'<b style="color:#B3261E">BELUM LUNAS</b>'}</div></div>
 <p>Kepada: <b>${esc(s.cust)}</b></p>
 <table><tr><th>Kode · Warna</th><th class="r">Qty (kg)</th><th class="r">Harga/kg</th><th class="r">Jumlah</th></tr>${s.lines.map(l=>`<tr><td>${esc(l.name)}${l.n?` <small>(${l.n} karung)</small>`:''}</td><td class="r">${kg(l.qty).replace(' kg','')}</td><td class="r">${rp(l.price)}</td><td class="r">${rp(l.qty*l.price)}</td></tr>`).join('')}
 <tr><td colspan="3" class="r">Subtotal</td><td class="r">${rp(t.sub)}</td></tr><tr><td colspan="3" class="r">PPN ${S.set.pkp?S.set.ppn+'%':'(non-PKP)'}</td><td class="r">${rp(t.ppn)}</td></tr><tr><td colspan="3" class="r"><b>Total</b></td><td class="r"><b>${rp(t.total)}</b></td></tr></table>
 <p><i>Terbilang: ${terbilang(t.total)}</i></p><p>Pembayaran ke: ${esc(S.set.bank)}</p>
 <div class="row noprint" style="margin-top:16px"><button class="btn" onclick="window.print()">Cetak / simpan PDF</button>
 <button class="btn g" style="color:#0E5A6B" onclick="wa('${s.no}')">Kirim lewat WhatsApp</button>
 ${s.batal?'':s.paid?`<button class="btn g" style="color:#0E5A6B" onclick="pay('${s.no}',false)">Batal lunas</button>`:`<button class="btn g" style="color:#0E5A6B" onclick="pay('${s.no}',true)">Tandai lunas</button>`}
 ${s.batal?`<span style="color:#B3261E">Dibatalkan: ${esc(s.alasan||'')}</span>`:`<input id="alasan" placeholder="Alasan pembatalan" style="background:#fff;color:#111"><button class="btn g" style="color:#B3261E" onclick="cancelInv('${s.no}')">Batalkan invoice</button>`}
 <button class="btn g" style="color:#444" onclick="closeM()">Tutup</button></div></div></div>`}
const closeM=()=>$('#modal').innerHTML='';
function payB(i,v){S.buys[i].paid=v;S.buys[i].paidAt=v?new Date().toISOString():null;save();render();toast(v?'Pembelian ditandai lunas':'Status lunas dibatalkan')}
function cancelInv(no){const s=S.sales.find(x=>x.no===no),a=($('#alasan')||{value:''}).value.trim();if(!a)return toast('Isi alasan pembatalan dulu');
 s.lines.forEach(l=>{const i=S.items.find(i=>i.id===l.id);if(i){i.stock=r2(i.stock+l.qty);i.ctn=(i.ctn||0)+(l.n||0)}});
 s.batal=true;s.alasan=a;save();render();inv(no);toast('Invoice dibatalkan, stok dikembalikan')}
function pay(no,v){const s=S.sales.find(s=>s.no===no);s.paid=v;s.paidAt=v?new Date().toISOString():null;save();render();inv(no);toast(v?'Invoice ditandai lunas':'Status lunas dibatalkan')}
function wa(no){const s=S.sales.find(x=>x.no===no);const m=`Halo ${s.cust}, berikut tagihan ${s.no} dari ${S.set.nama} sebesar ${rp(tot(s).total)}. Pembayaran ke ${S.set.bank}. Terima kasih.`;window.open('https://wa.me/?text='+encodeURIComponent(m),'_blank')}

function tax(){
 const ms=act().filter(s=>s.date.startsWith(month)),mb=S.buys.filter(s=>s.date.startsWith(month));
 const out=ms.reduce((a,s)=>a+tot(s).ppn,0),inn=mb.reduce((a,s)=>a+tot(s).ppn,0);
 const omzet=ms.reduce((a,s)=>a+calc(s.lines,0,0).sub,0);
 const ytd=act().filter(s=>s.date.slice(0,4)===month.slice(0,4)&&s.date.slice(0,7)<=month).reduce((a,s)=>a+calc(s.lines,0,0).sub,0);
 const pph=Math.round(omzet*S.set.pph/100),lim=4.8e9;
 return `<h1>Pajak</h1><p class="sub">Rekap otomatis dari transaksi. Pilih bulan:</p>
 <div class="row"><label>Bulan<input type="month" value="${month}" onchange="month=this.value;render()"></label>
 <label>Status usaha<select onchange="S.set.pkp=this.value==='1';save();render()"><option value="1" ${S.set.pkp?'selected':''}>PKP (kena PPN)</option><option value="0" ${S.set.pkp?'':'selected'}>Non-PKP</option></select></label>
 <label>Tarif PPN (%)<input type="number" value="${S.set.ppn}" style="width:80px" onchange="S.set.ppn=+this.value;save();render()"></label>
 <label>Tarif PPh final (%)<input type="number" step="0.1" value="${S.set.pph}" style="width:90px" onchange="S.set.pph=+this.value;save();render()"></label></div>
 <div class="grid"><div class="card"><div class="k">PPN keluaran (penjualan)</div><div class="v">${rp(out)}</div></div>
 <div class="card"><div class="k">PPN masukan (pembelian)</div><div class="v">${rp(inn)}</div></div>
 <div class="card hero"><div class="k">${out-inn>=0?'PPN kurang bayar':'PPN lebih bayar'}</div><div class="v">${rp(Math.abs(out-inn))}</div></div></div>
 <div class="card"><h2>PPh final UMKM</h2><p>Omzet bruto bulan ini <b>${rp(omzet)}</b> × ${S.set.pph}% = <b>${rp(pph)}</b></p>
 <div class="k" style="margin-bottom:6px">Omzet kumulatif tahun ${month.slice(0,4)}: ${rp(ytd)} dari batas ${rp(lim)}</div><div class="prog"><i style="width:${Math.min(ytd/lim*100,100)}%"></i></div></div>
 <div class="note">Prototipe ini hanya alat bantu rekap, bukan pengganti konsultan pajak. Cek tarif dan aturan terbaru di DJP sebelum dipakai untuk pelaporan resmi.</div>
 <div class="row" style="margin-top:12px"><button class="btn g" onclick="csv()">Unduh rekap (CSV)</button><button class="btn g" onclick="if(confirm('Kembalikan ke data contoh?')){S=seed();save();render()}">Reset data contoh</button></div>`}
function csv(){const rows=[['Tanggal','Invoice','Pelanggan','DPP','PPN','Total']];act().filter(s=>s.date.startsWith(month)).forEach(s=>{const t=tot(s);rows.push([s.date,s.no,s.cust,t.sub,t.ppn,t.total])});
 const text=rows.map(r=>r.join(',')).join('\n');try{const a=document.createElement('a');a.href='data:text/csv;charset=utf-8,'+encodeURIComponent(text);a.download='rekap-pajak-'+month+'.csv';a.click()}catch(e){}toast('Rekap pajak diunduh (jika browser mengizinkan)')}

function render(){nav();$('#main').innerHTML={dash,items,sell,buy,tax}[view]();window.scrollTo(0,0)}
render();
</script>
</body>
</html>
