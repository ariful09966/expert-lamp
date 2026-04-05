<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>9Anime — Watch Anime Online Free HD</title>
<meta name="description" content="Watch anime online free in HD quality. Latest episodes updated daily."/>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;500;600;700;800;900&amp;family=Rajdhani:wght@500;600;700&amp;display=swap" rel="stylesheet"/>
<style>
:root{
  --bg0:#0a0a0a;--bg1:#111111;--bg2:#161616;--bg3:#1c1c1c;--bg4:#222222;
  --acc:#e74c3c;--acc2:#c0392b;--ora:#f39c12;--blu:#3498db;--grn:#2ecc71;
  --t1:#e8e8e8;--t2:#aaaaaa;--t3:#666666;--t4:#333333;
  --bdr:#252525;--bdr2:#2e2e2e;
  --sub:#f39c12;--dub:#3498db;
  --card-h:220px;
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{font-family:'Nunito',sans-serif;background:var(--bg0);color:var(--t1);font-size:14px;line-height:1.5;min-height:100vh;}
a{text-decoration:none;color:inherit;}
button{font-family:'Nunito',sans-serif;cursor:pointer;}
input,textarea,select{font-family:'Nunito',sans-serif;}
img{max-width:100%;display:block;}
::-webkit-scrollbar{width:5px;height:5px;}
::-webkit-scrollbar-track{background:var(--bg1);}
::-webkit-scrollbar-thumb{background:var(--bg4);border-radius:3px;}
::-webkit-scrollbar-thumb:hover{background:var(--acc);}

/* ═══ PAGE ROUTER ═══ */
.page{display:none;}
.page.show{display:block;}

/* ═══ NOTICE BAR ═══ */
.notice{background:linear-gradient(90deg,#1a0000,#200808,#1a0000);border-bottom:1px solid #3a1010;padding:5px 20px;text-align:center;font-size:11px;color:#c08080;letter-spacing:.3px;}
.notice strong{color:var(--acc);}

/* ═══ HEADER ═══ */
header{background:var(--bg1);border-bottom:1px solid var(--bdr);position:sticky;top:0;z-index:200;box-shadow:0 2px 20px rgba(0,0,0,.7);}
.hdr-inner{max-width:1300px;margin:0 auto;padding:0 18px;height:56px;display:flex;align-items:center;gap:14px;}
.logo{font-family:'Rajdhani',sans-serif;font-size:28px;font-weight:700;color:var(--acc);letter-spacing:2px;cursor:pointer;flex-shrink:0;transition:opacity .2s;}
.logo:hover{opacity:.85;}
.logo em{color:var(--t1);font-style:normal;}
.hdr-search{flex:1;max-width:480px;display:flex;align-items:center;background:var(--bg3);border:1px solid var(--bdr2);border-radius:4px;overflow:hidden;transition:border-color .2s;}
.hdr-search:focus-within{border-color:var(--acc);}
.hdr-search input{flex:1;background:none;border:none;outline:none;padding:9px 14px;color:var(--t1);font-size:13px;}
.hdr-search input::placeholder{color:var(--t3);}
.hdr-search button{background:var(--acc);border:none;padding:9px 14px;color:#fff;font-size:13px;transition:background .2s;}
.hdr-search button:hover{background:var(--acc2);}
.hdr-right{margin-left:auto;display:flex;align-items:center;gap:8px;}
.btn-adm{background:linear-gradient(135deg,#f39c12,#d68910);color:#000;border:none;padding:6px 13px;border-radius:3px;font-size:11px;font-weight:800;letter-spacing:.5px;cursor:pointer;transition:opacity .2s;text-transform:uppercase;}
.btn-adm:hover{opacity:.85;}
.btn-reg{background:var(--bg3);color:var(--t2);border:1px solid var(--bdr2);padding:6px 14px;border-radius:3px;font-size:12px;font-weight:600;cursor:pointer;transition:background .2s,color .2s;}
.btn-reg:hover{background:var(--bg4);color:var(--t1);}
.btn-log{background:var(--acc);color:#fff;border:none;padding:6px 14px;border-radius:3px;font-size:12px;font-weight:700;cursor:pointer;transition:background .2s;}
.btn-log:hover{background:var(--acc2);}

/* ═══ NAV ═══ */
nav{background:var(--bg2);border-bottom:1px solid var(--bdr);}
.nav-inner{max-width:1300px;margin:0 auto;padding:0 18px;display:flex;align-items:center;overflow-x:auto;}
.nav-inner::-webkit-scrollbar{height:0;}
.nav-link{color:var(--t2);font-size:12.5px;font-weight:700;padding:11px 13px;display:flex;align-items:center;gap:4px;white-space:nowrap;transition:color .2s,background .2s;border-bottom:2px solid transparent;}
.nav-link:hover,.nav-link.on{color:var(--acc);background:rgba(231,76,60,.06);border-bottom-color:var(--acc);}
.nav-drop{position:relative;}
.nav-drop:hover .drop-menu{display:grid;}
.drop-menu{display:none;position:absolute;top:100%;left:0;background:var(--bg2);border:1px solid var(--bdr2);border-top:2px solid var(--acc);padding:10px;grid-template-columns:repeat(4,1fr);gap:1px;z-index:300;min-width:560px;box-shadow:0 12px 30px rgba(0,0,0,.7);}
.drop-menu a{font-size:11.5px;padding:6px 10px;border-radius:3px;color:var(--t2);transition:color .2s,background .2s;display:block;}
.drop-menu a:hover{color:var(--acc);background:rgba(231,76,60,.07);}

/* ═══ LAYOUT ═══ */
.layout{max-width:1300px;margin:0 auto;padding:16px 18px;display:grid;grid-template-columns:1fr 265px;gap:18px;}
@media(max-width:900px){.layout{grid-template-columns:1fr;}}

/* ═══ HERO SLIDER ═══ */
.hero{position:relative;border-radius:6px;overflow:hidden;background:var(--bg2);margin-bottom:20px;height:370px;display:flex;align-items:center;justify-content:center;}
.hero-empty{text-align:center;color:var(--t3);}
.hero-empty svg{width:56px;height:56px;margin-bottom:14px;opacity:.15;}
.hero-empty p{font-size:13px;margin-bottom:8px;}
.hero-empty a{color:var(--acc);font-size:12px;cursor:pointer;}
.slide{display:none;position:absolute;inset:0;animation:sldIn .5s ease;}
.slide.on{display:block;}
@keyframes sldIn{from{opacity:0}to{opacity:1}}
.slide-bg{position:absolute;inset:0;background-size:cover;background-position:center;filter:brightness(.35);}
.slide-grd{position:absolute;inset:0;background:linear-gradient(to top,rgba(10,10,10,.98) 0%,rgba(10,10,10,.55) 55%,transparent 100%);}
.slide-body{position:absolute;bottom:0;left:0;right:0;padding:22px 26px;}
.slide-tags{display:flex;gap:5px;margin-bottom:8px;flex-wrap:wrap;}
.badge{font-size:9.5px;font-weight:800;padding:2px 8px;border-radius:2px;text-transform:uppercase;letter-spacing:.6px;}
.b-sub{background:var(--sub);color:#000;}
.b-dub{background:var(--dub);color:#fff;}
.b-new{background:var(--acc);color:#fff;}
.b-typ{background:#3a3a3a;color:#bbb;}
.b-hd{background:#1a4a1a;color:#4ecb4e;}
.slide-ttl{font-family:'Rajdhani',sans-serif;font-size:28px;font-weight:700;color:#fff;line-height:1.15;margin-bottom:6px;text-shadow:0 2px 8px rgba(0,0,0,.9);}
.slide-meta{font-size:11.5px;color:#999;margin-bottom:10px;display:flex;gap:14px;flex-wrap:wrap;}
.slide-desc{font-size:12px;color:#bbb;line-height:1.55;margin-bottom:14px;max-width:620px;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.slide-btns{display:flex;gap:8px;}
.btn-play{background:var(--acc);color:#fff;border:none;padding:9px 22px;border-radius:3px;font-size:13px;font-weight:800;display:flex;align-items:center;gap:6px;cursor:pointer;transition:background .2s,transform .15s;}
.btn-play:hover{background:var(--acc2);transform:translateY(-1px);}
.btn-info{background:rgba(255,255,255,.09);color:#fff;border:1px solid rgba(255,255,255,.18);padding:9px 18px;border-radius:3px;font-size:13px;font-weight:600;cursor:pointer;transition:background .2s;}
.btn-info:hover{background:rgba(255,255,255,.16);}
.hero-dots{position:absolute;bottom:12px;right:16px;display:flex;gap:5px;}
.dot{width:7px;height:7px;border-radius:50%;background:rgba(255,255,255,.25);cursor:pointer;transition:background .2s,transform .2s;}
.dot.on{background:var(--acc);transform:scale(1.3);}
.hero-arr{position:absolute;top:50%;transform:translateY(-50%);background:rgba(0,0,0,.55);border:none;color:#fff;width:36px;height:60px;border-radius:3px;font-size:18px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:background .2s;z-index:10;}
.hero-arr:hover{background:rgba(231,76,60,.7);}
.hero-arr.prev{left:8px;}
.hero-arr.next{right:8px;}

/* ═══ SECTION HEADER ═══ */
.sec-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;padding-bottom:8px;border-bottom:2px solid var(--bdr);position:relative;}
.sec-hdr::after{content:'';position:absolute;bottom:-2px;left:0;width:70px;height:2px;background:var(--acc);}
.sec-ttl{font-family:'Rajdhani',sans-serif;font-size:15px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--t1);}
.sec-more{font-size:11px;color:var(--t3);transition:color .2s;cursor:pointer;}
.sec-more:hover{color:var(--acc);}

/* ═══ ANIME GRID ═══ */
.a-grid{display:grid;grid-template-columns:repeat(6,1fr);gap:10px;margin-bottom:22px;}
@media(max-width:1100px){.a-grid{grid-template-columns:repeat(5,1fr);}}
@media(max-width:700px){.a-grid{grid-template-columns:repeat(3,1fr);}}
@media(max-width:400px){.a-grid{grid-template-columns:repeat(2,1fr);}}
.a-card{cursor:pointer;}
.a-thumb{position:relative;aspect-ratio:3/4;border-radius:4px;overflow:hidden;background:var(--bg3);margin-bottom:6px;}
.a-thumb img{width:100%;height:100%;object-fit:cover;transition:transform .35s,filter .35s;}
.a-card:hover .a-thumb img{transform:scale(1.07);filter:brightness(.65);}
.a-ov{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;opacity:0;transition:opacity .3s;}
.a-card:hover .a-ov{opacity:1;}
.a-ov-play{width:40px;height:40px;background:rgba(231,76,60,.92);border-radius:50%;display:flex;align-items:center;justify-content:center;transform:scale(.8);transition:transform .3s;}
.a-card:hover .a-ov-play{transform:scale(1);}
.a-ov-play svg{width:16px;height:16px;fill:#fff;margin-left:2px;}
.a-bgs{position:absolute;top:4px;left:4px;display:flex;gap:3px;flex-wrap:wrap;}
.a-ep{position:absolute;bottom:4px;right:4px;background:rgba(0,0,0,.82);color:#bbb;font-size:9.5px;font-weight:800;padding:2px 6px;border-radius:2px;}
.a-ep.hot{color:var(--ora);}
.a-emoji{width:100%;height:100%;display:flex;align-items:center;justify-content:center;font-size:36px;background:linear-gradient(135deg,var(--bg3),var(--bg4));}
.a-name{font-size:11.5px;font-weight:700;color:var(--t1);line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;transition:color .2s;}
.a-card:hover .a-name{color:var(--acc);}
.a-sub{font-size:10.5px;color:var(--t3);margin-top:1px;}

/* ═══ EMPTY STATE ═══ */
.empty{grid-column:1/-1;text-align:center;padding:44px 20px;color:var(--t3);}
.empty svg{width:48px;height:48px;margin-bottom:12px;opacity:.2;}
.empty p{font-size:13px;}
.empty-cta{color:var(--acc);font-size:12px;margin-top:8px;cursor:pointer;display:inline-block;}
.empty-cta:hover{text-decoration:underline;}

/* ═══ TABS ═══ */
.tabs{display:flex;border-bottom:2px solid var(--bdr);margin-bottom:14px;}
.tab{padding:9px 15px;font-size:12px;font-weight:800;color:var(--t3);cursor:pointer;font-family:'Rajdhani',sans-serif;text-transform:uppercase;letter-spacing:.5px;border-bottom:2px solid transparent;margin-bottom:-2px;transition:color .2s;}
.tab.on{color:var(--acc);border-bottom-color:var(--acc);}
.tab:hover:not(.on){color:var(--t2);}
.tab-pane{display:none;}
.tab-pane.on{display:block;}

/* ═══ SCHEDULE ═══ */
.sched-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:6px;margin-bottom:22px;}
.sched-day{}
.day-hdr{font-size:10px;font-weight:800;text-align:center;padding:5px 3px;background:var(--bg3);border-radius:3px;margin-bottom:5px;color:var(--t3);text-transform:uppercase;letter-spacing:.5px;}
.day-hdr.today{background:var(--acc);color:#fff;}
.sched-item{background:var(--bg3);border-radius:3px;padding:5px 6px;margin-bottom:4px;font-size:9.5px;color:var(--t2);border-left:2px solid transparent;cursor:pointer;transition:border-color .2s,background .2s;}
.sched-item:hover{border-left-color:var(--acc);background:var(--bg4);}
.sched-item.airing{border-left-color:var(--grn);}
.sched-t{font-size:8.5px;color:var(--t3);margin-bottom:1px;}

/* ═══ SIDEBAR ═══ */
.sb-box{background:var(--bg1);border:1px solid var(--bdr);border-radius:5px;overflow:hidden;margin-bottom:14px;}
.sb-hdr{background:var(--bg2);padding:9px 13px;font-family:'Rajdhani',sans-serif;font-size:12.5px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--t1);border-bottom:2px solid var(--acc);display:flex;align-items:center;gap:6px;}
.sb-hdr svg{width:13px;height:13px;fill:var(--acc);}
.tr-list{padding:6px 0;}
.tr-item{display:flex;align-items:center;gap:9px;padding:6px 11px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);}
.tr-item:last-child{border-bottom:none;}
.tr-item:hover{background:var(--bg2);}
.tr-rank{font-family:'Rajdhani',sans-serif;font-size:17px;font-weight:700;color:var(--bdr2);min-width:20px;text-align:center;line-height:1;}
.tr-rank.hot{color:var(--acc);}
.tr-img{width:42px;height:58px;border-radius:3px;overflow:hidden;flex-shrink:0;background:var(--bg3);display:flex;align-items:center;justify-content:center;font-size:18px;}
.tr-img img{width:100%;height:100%;object-fit:cover;}
.tr-info{flex:1;min-width:0;}
.tr-name{font-size:11.5px;font-weight:700;color:var(--t1);line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.tr-item:hover .tr-name{color:var(--acc);}
.tr-meta{font-size:10px;color:var(--t3);margin-top:2px;}
.genre-wrap{padding:10px;display:flex;flex-wrap:wrap;gap:4px;}
.g-tag{background:var(--bg3);border:1px solid var(--bdr2);color:var(--t2);font-size:10.5px;padding:3px 10px;border-radius:2px;cursor:pointer;transition:background .2s,color .2s,border-color .2s;}
.g-tag:hover{background:var(--acc);color:#fff;border-color:var(--acc);}
.rec-list{padding:4px 0;}
.rec-item{display:flex;gap:9px;padding:6px 11px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);align-items:flex-start;}
.rec-item:hover{background:var(--bg2);}
.rec-img{width:48px;height:66px;border-radius:3px;overflow:hidden;flex-shrink:0;background:var(--bg3);display:flex;align-items:center;justify-content:center;font-size:20px;}
.rec-img img{width:100%;height:100%;object-fit:cover;}
.rec-info{flex:1;min-width:0;}
.rec-name{font-size:11.5px;font-weight:700;color:var(--t1);line-height:1.3;margin-bottom:3px;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.rec-item:hover .rec-name{color:var(--acc);}
.rec-ep{font-size:10px;color:var(--t3);}
.rec-ep b{color:var(--ora);}
.sb-empty{padding:16px 11px;text-align:center;font-size:11.5px;color:var(--t3);}

/* ═══ FOOTER ═══ */
footer{background:#080808;border-top:1px solid var(--bdr);padding:28px 18px;margin-top:8px;}
.ft-inner{max-width:1300px;margin:0 auto;}
.ft-top{display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:26px;margin-bottom:22px;}
@media(max-width:700px){.ft-top{grid-template-columns:1fr 1fr;}}
.ft-logo{font-family:'Rajdhani',sans-serif;font-size:24px;font-weight:700;color:var(--acc);margin-bottom:9px;}
.ft-logo em{color:var(--t1);font-style:normal;}
.ft-desc{font-size:11.5px;color:var(--t3);line-height:1.6;}
.ft-col h5{font-family:'Rajdhani',sans-serif;font-size:12px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--t1);margin-bottom:9px;padding-bottom:5px;border-bottom:1px solid var(--bdr);}
.ft-col ul{list-style:none;}
.ft-col ul li{margin-bottom:5px;}
.ft-col ul li a{font-size:11.5px;color:var(--t3);transition:color .2s;}
.ft-col ul li a:hover{color:var(--acc);}
.ft-btm{border-top:1px solid var(--bdr);padding-top:14px;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:8px;}
.ft-copy{font-size:11px;color:var(--t3);}
.ft-links{display:flex;gap:12px;}
.ft-links a{font-size:11px;color:var(--t3);transition:color .2s;}
.ft-links a:hover{color:var(--acc);}

/* ═══ WATCH PAGE ═══ */
.watch-wrap{max-width:1300px;margin:0 auto;padding:14px 18px;display:grid;grid-template-columns:1fr 290px;gap:18px;}
@media(max-width:900px){.watch-wrap{grid-template-columns:1fr;}}
.back-btn{display:inline-flex;align-items:center;gap:6px;color:var(--t3);font-size:12.5px;padding:10px 18px;cursor:pointer;transition:color .2s;}
.back-btn:hover{color:var(--acc);}
.bc{font-size:11.5px;color:var(--t3);margin-bottom:12px;display:flex;align-items:center;gap:5px;flex-wrap:wrap;}
.bc a{color:var(--t2);transition:color .2s;cursor:pointer;}
.bc a:hover{color:var(--acc);}
.player-box{background:#000;border-radius:5px;overflow:hidden;margin-bottom:12px;position:relative;}
.player-box iframe,.player-box video{width:100%;aspect-ratio:16/9;display:block;border:none;}
.player-hold{width:100%;aspect-ratio:16/9;display:flex;flex-direction:column;align-items:center;justify-content:center;background:#050505;gap:14px;}
.player-hold svg{width:60px;height:60px;fill:var(--acc);opacity:.35;animation:pulse 2s infinite;}
@keyframes pulse{0%,100%{opacity:.25}50%{opacity:.7}}
.player-hold p{font-size:13px;color:var(--t3);}
.srv-bar{background:var(--bg2);border:1px solid var(--bdr);border-radius:4px;padding:9px 13px;margin-bottom:12px;display:flex;align-items:center;gap:9px;flex-wrap:wrap;}
.srv-lbl{font-size:10.5px;font-weight:800;color:var(--t3);text-transform:uppercase;letter-spacing:.5px;white-space:nowrap;}
.srv-btn{background:var(--bg3);border:1px solid var(--bdr2);color:var(--t2);font-size:11.5px;padding:5px 13px;border-radius:3px;cursor:pointer;transition:background .2s,color .2s,border-color .2s;}
.srv-btn.on,.srv-btn:hover{background:var(--acc);color:#fff;border-color:var(--acc);}
.ep-box{background:var(--bg2);border:1px solid var(--bdr);border-radius:4px;overflow:hidden;margin-bottom:12px;}
.ep-hdr{background:var(--bg3);padding:9px 13px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--bdr);}
.ep-hdr-ttl{font-family:'Rajdhani',sans-serif;font-size:12.5px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
.ep-hdr-ct{font-size:10.5px;color:var(--t3);}
.ep-body{padding:9px;display:flex;flex-wrap:wrap;gap:4px;max-height:155px;overflow-y:auto;}
.ep-n{background:var(--bg3);border:1px solid var(--bdr2);color:var(--t2);font-size:11.5px;font-weight:700;padding:4px 9px;border-radius:3px;cursor:pointer;transition:background .2s,color .2s;min-width:40px;text-align:center;}
.ep-n:hover{background:var(--bg4);color:var(--t1);}
.ep-n.on{background:var(--acc);color:#fff;border-color:var(--acc);}
.w-info{background:var(--bg2);border:1px solid var(--bdr);border-radius:5px;padding:16px;margin-bottom:12px;}
.w-badges{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:9px;}
.w-title{font-family:'Rajdhani',sans-serif;font-size:22px;font-weight:700;color:var(--t1);margin-bottom:8px;line-height:1.2;}
.w-metas{display:flex;flex-wrap:wrap;gap:12px;margin-bottom:10px;}
.w-meta{font-size:11.5px;color:var(--t3);display:flex;align-items:center;gap:3px;}
.w-meta strong{color:var(--t2);}
.w-desc{font-size:12.5px;color:var(--t2);line-height:1.65;}
.rel-list{padding:5px 0;}
.rel-item{display:flex;gap:9px;padding:7px 11px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);}
.rel-item:hover{background:var(--bg2);}
.rel-item:last-child{border-bottom:none;}
.rel-img{width:78px;height:52px;border-radius:3px;overflow:hidden;flex-shrink:0;background:var(--bg3);display:flex;align-items:center;justify-content:center;font-size:20px;}
.rel-img img{width:100%;height:100%;object-fit:cover;}
.rel-info{flex:1;min-width:0;}
.rel-name{font-size:11.5px;font-weight:700;color:var(--t1);line-height:1.3;margin-bottom:3px;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.rel-item:hover .rel-name{color:var(--acc);}
.rel-meta{font-size:10.5px;color:var(--t3);}

/* ═══ ADMIN PAGE ═══ */
.adm-wrap{max-width:980px;margin:0 auto;padding:22px 18px;}
.adm-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:22px;}
.adm-title{font-family:'Rajdhani',sans-serif;font-size:20px;font-weight:700;display:flex;align-items:center;gap:9px;color:var(--t1);}
.adm-title svg{width:20px;height:20px;fill:var(--acc);}
.adm-live{font-size:11px;color:var(--grn);}
.adm-stats{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-bottom:22px;}
@media(max-width:600px){.adm-stats{grid-template-columns:repeat(2,1fr);}}
.s-card{background:var(--bg2);border:1px solid var(--bdr);border-radius:5px;padding:14px;border-left:3px solid var(--acc);}
.s-num{font-family:'Rajdhani',sans-serif;font-size:26px;font-weight:700;color:var(--acc);line-height:1;}
.s-lbl{font-size:10.5px;color:var(--t3);text-transform:uppercase;letter-spacing:.5px;margin-top:3px;}
.adm-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px;}
@media(max-width:720px){.adm-grid{grid-template-columns:1fr;}}
.form-box{background:var(--bg2);border:1px solid var(--bdr);border-radius:5px;overflow:hidden;}
.fb-hdr{background:var(--bg3);padding:11px 16px;border-bottom:2px solid var(--acc);display:flex;align-items:center;gap:7px;}
.fb-hdr svg{width:14px;height:14px;fill:var(--acc);}
.fb-hdr span{font-family:'Rajdhani',sans-serif;font-size:13.5px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
.fb-body{padding:16px;}
.fg{margin-bottom:12px;}
.fg label{display:block;font-size:11px;font-weight:800;color:var(--t2);margin-bottom:4px;text-transform:uppercase;letter-spacing:.3px;}
.fg input,.fg textarea,.fg select{width:100%;background:var(--bg3);border:1px solid var(--bdr2);color:var(--t1);padding:8px 11px;border-radius:3px;font-size:12.5px;outline:none;transition:border-color .2s;}
.fg input:focus,.fg textarea:focus,.fg select:focus{border-color:var(--acc);}
.fg textarea{resize:vertical;min-height:76px;}
.fg select option{background:var(--bg3);}
.fg-hint{font-size:10.5px;color:var(--t3);margin-top:3px;}
.fg-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.btn-post{background:var(--acc);color:#fff;border:none;padding:10px 22px;border-radius:3px;font-size:13px;font-weight:800;cursor:pointer;transition:background .2s,transform .15s;display:flex;align-items:center;gap:6px;width:100%;justify-content:center;text-transform:uppercase;letter-spacing:.5px;}
.btn-post:hover{background:var(--acc2);transform:translateY(-1px);}
.cancel-lnk{display:none;text-align:center;margin-top:8px;font-size:11.5px;color:var(--t3);cursor:pointer;transition:color .2s;}
.cancel-lnk:hover{color:var(--acc);}
.posted-box{background:var(--bg2);border:1px solid var(--bdr);border-radius:5px;overflow:hidden;}
.pb-hdr{background:var(--bg3);padding:11px 16px;border-bottom:2px solid var(--acc);display:flex;align-items:center;gap:7px;}
.pb-hdr svg{width:14px;height:14px;fill:var(--acc);}
.pb-hdr span{font-family:'Rajdhani',sans-serif;font-size:13.5px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
.posted-list{max-height:520px;overflow-y:auto;}
.p-item{display:flex;align-items:center;gap:10px;padding:9px 13px;border-bottom:1px solid rgba(255,255,255,.04);transition:background .2s;}
.p-item:hover{background:var(--bg3);}
.p-thumb{width:52px;height:38px;border-radius:3px;overflow:hidden;flex-shrink:0;background:var(--bg3);display:flex;align-items:center;justify-content:center;font-size:16px;}
.p-thumb img{width:100%;height:100%;object-fit:cover;}
.p-info{flex:1;min-width:0;}
.p-name{font-size:12px;font-weight:700;color:var(--t1);white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.p-sub{font-size:10px;color:var(--t3);margin-top:2px;}
.p-acts{display:flex;gap:5px;flex-shrink:0;}
.btn-ic{background:var(--bg3);border:1px solid var(--bdr2);color:var(--t3);padding:4px 8px;border-radius:3px;cursor:pointer;font-size:11px;transition:background .2s,color .2s,border-color .2s;white-space:nowrap;}
.btn-ic:hover{background:var(--acc);color:#fff;border-color:var(--acc);}
.btn-ic.del:hover{background:#c0392b;border-color:#c0392b;}
.p-empty{padding:22px;text-align:center;font-size:12.5px;color:var(--t3);}

/* ═══ TOAST ═══ */
.toast{position:fixed;bottom:22px;right:22px;background:var(--bg2);border:1px solid var(--bdr2);border-left:4px solid var(--grn);color:var(--t1);padding:11px 18px;border-radius:4px;font-size:12.5px;font-weight:600;z-index:9999;opacity:0;transform:translateY(8px);transition:opacity .3s,transform .3s;pointer-events:none;max-width:280px;box-shadow:0 6px 24px rgba(0,0,0,.6);}
.toast.show{opacity:1;transform:translateY(0);}

/* ═══ MODAL ═══ */
.modal-bg{position:fixed;inset:0;background:rgba(0,0,0,.78);z-index:500;display:flex;align-items:center;justify-content:center;opacity:0;pointer-events:none;transition:opacity .25s;}
.modal-bg.show{opacity:1;pointer-events:all;}
.modal{background:var(--bg2);border:1px solid var(--bdr2);border-top:3px solid var(--acc);border-radius:5px;padding:22px;max-width:350px;width:92%;}
.modal h3{font-family:'Rajdhani',sans-serif;font-size:18px;font-weight:700;margin-bottom:8px;}
.modal p{font-size:12.5px;color:var(--t2);margin-bottom:18px;line-height:1.5;}
.modal-btns{display:flex;gap:8px;}
.btn-cancel{background:var(--bg3);border:1px solid var(--bdr2);color:var(--t2);padding:7px 18px;border-radius:3px;cursor:pointer;font-size:12.5px;transition:background .2s;}
.btn-cancel:hover{background:var(--bg4);}
.btn-del{background:#c0392b;border:none;color:#fff;padding:7px 18px;border-radius:3px;cursor:pointer;font-size:12.5px;font-weight:700;transition:background .2s;}
.btn-del:hover{background:#a93226;}

/* ═══ SEARCH RESULTS ═══ */
.search-wrap{max-width:1300px;margin:0 auto;padding:16px 18px;}
.search-ttl{font-family:'Rajdhani',sans-serif;font-size:18px;font-weight:700;margin-bottom:16px;color:var(--t1);}
.search-ttl em{color:var(--acc);font-style:normal;}
</style>
</head>
<body>

<!-- TOAST -->
<div class="toast" id="toast"></div>

<!-- DELETE MODAL -->
<div class="modal-bg" id="delModal">
  <div class="modal">
    <h3>🗑 Delete Stream?</h3>
    <p>This action is permanent and cannot be undone. The stream will be removed from all sections.</p>
    <div class="modal-btns">
      <button class="btn-cancel" onclick="closeModal()">Cancel</button>
      <button class="btn-del" onclick="doDelete()">Yes, Delete</button>
    </div>
  </div>
</div>

<!-- ══════ SHARED HEADER ══════ -->
<div class="notice">⚠ Use <strong>AdBlock</strong> for a better experience &#160;|&#160; Bookmark: <strong>9anime.to</strong></div>

<header>
  <div class="hdr-inner">
    <div class="logo" onclick="nav('home')">9<em>ANIME</em></div>
    <div class="hdr-search">
      <input type="text" id="sInput" placeholder="Search anime title..." oninput="searchQ(this.value)" onkeydown="if(event.key==='Enter')searchQ(this.value)"/>
      <button onclick="searchQ(document.getElementById('sInput').value)">
        <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.5" width="13" height="13"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.3-4.3"/></svg>
      </button>
    </div>
    <div class="hdr-right">
      <button class="btn-adm" onclick="nav('admin')">⚙ Admin</button>
      <button class="btn-reg">Register</button>
      <button class="btn-log">Login</button>
    </div>
  </div>
</header>

<nav>
  <div class="nav-inner">
    <a class="nav-link on" onclick="nav('home')">
      <svg viewBox="0 0 24 24" fill="currentColor" width="12" height="12"><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>Home
    </a>
    <a class="nav-link">New Season</a>
    <a class="nav-link">Movies</a>
    <a class="nav-link">TV Series</a>
    <a class="nav-link">OVA</a>
    <a class="nav-link">ONA</a>
    <a class="nav-link">Specials</a>
    <div class="nav-drop">
      <a class="nav-link">Genre ▾</a>
      <div class="drop-menu">
        <a>Action</a><a>Adventure</a><a>Comedy</a><a>Drama</a>
        <a>Ecchi</a><a>Fantasy</a><a>Harem</a><a>Horror</a>
        <a>Isekai</a><a>Josei</a><a>Magic</a><a>Mecha</a>
        <a>Military</a><a>Music</a><a>Mystery</a><a>Parody</a>
        <a>Psychological</a><a>Romance</a><a>Sci-Fi</a><a>Seinen</a>
        <a>Shoujo</a><a>Shounen</a><a>Slice of Life</a><a>Sports</a>
        <a>Super Power</a><a>Supernatural</a><a>Thriller</a><a>Vampire</a>
      </div>
    </div>
    <a class="nav-link">Schedule</a>
    <a class="nav-link" onclick="nav('admin')" style="color:var(--ora);">🎬 Post Stream</a>
  </div>
</nav>

<!-- ══════════════════════════════
     PAGE: HOME
══════════════════════════════ -->
<div class="page show" id="pg-home">
  <div class="layout">
    <main>

      <!-- Hero Slider -->
      <div class="hero" id="heroBox">
        <div class="hero-empty" id="heroEmpty">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M18 4l2 4h-3l-2-4h-2l2 4h-3l-2-4H8l2 4H7L5 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V4h-4z"/></svg>
          <p>No streams posted yet.</p>
          <a onclick="nav('admin')">➕ Post your first stream →</a>
        </div>
        <div id="slidesWrap"></div>
        <div class="hero-dots" id="heroDots"></div>
        <button class="hero-arr prev" id="heroPrev" onclick="moveSlide(-1)" style="display:none">❮</button>
        <button class="hero-arr next" id="heroNext" onclick="moveSlide(1)" style="display:none">❯</button>
      </div>

      <!-- Recently Updated -->
      <div class="sec-hdr">
        <div class="sec-ttl">Recently Updated</div>
        <span class="sec-more">View All →</span>
      </div>
      <div class="a-grid" id="recentGrid"></div>

      <!-- Tabs -->
      <div class="tabs">
        <div class="tab on" onclick="switchTab(this,'tp-trending')">Trending</div>
        <div class="tab" onclick="switchTab(this,'tp-popular')">Popular</div>
        <div class="tab" onclick="switchTab(this,'tp-movies')">Movies</div>
        <div class="tab" onclick="switchTab(this,'tp-completed')">Completed</div>
      </div>
      <div class="tab-pane on" id="tp-trending"><div class="a-grid" id="gridTrend"></div></div>
      <div class="tab-pane" id="tp-popular"><div class="a-grid" id="gridPop"></div></div>
      <div class="tab-pane" id="tp-movies"><div class="a-grid" id="gridMov"></div></div>
      <div class="tab-pane" id="tp-completed"><div class="a-grid" id="gridComp"></div></div>

      <!-- Weekly Schedule -->
      <div class="sec-hdr" style="margin-top:6px;">
        <div class="sec-ttl">Weekly Schedule</div>
        <span class="sec-more">Full Schedule →</span>
      </div>
      <div class="sched-grid">
        <div class="sched-day"><div class="day-hdr">Mon</div></div>
        <div class="sched-day"><div class="day-hdr">Tue</div></div>
        <div class="sched-day"><div class="day-hdr">Wed</div></div>
        <div class="sched-day"><div class="day-hdr today">Thu ★</div></div>
        <div class="sched-day"><div class="day-hdr">Fri</div></div>
        <div class="sched-day"><div class="day-hdr">Sat</div></div>
        <div class="sched-day"><div class="day-hdr">Sun</div></div>
      </div>

    </main>

    <!-- Sidebar -->
    <aside>
      <div class="sb-box">
        <div class="sb-hdr">
          <svg viewBox="0 0 24 24"><path d="M17.66 18.66A8 8 0 0 1 4 12c0-2.21.9-4.21 2.34-5.66L12 12l5.66 6.66z"/></svg>
          Top Airing
        </div>
        <div class="tr-list" id="sbAiring"><div class="sb-empty">No streams yet.</div></div>
      </div>

      <div class="sb-box">
        <div class="sb-hdr">
          <svg viewBox="0 0 24 24"><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>
          Genres
        </div>
        <div class="genre-wrap">
          <span class="g-tag">Action</span><span class="g-tag">Adventure</span><span class="g-tag">Comedy</span>
          <span class="g-tag">Drama</span><span class="g-tag">Fantasy</span><span class="g-tag">Horror</span>
          <span class="g-tag">Isekai</span><span class="g-tag">Magic</span><span class="g-tag">Mecha</span>
          <span class="g-tag">Mystery</span><span class="g-tag">Romance</span><span class="g-tag">Sci-Fi</span>
          <span class="g-tag">Shounen</span><span class="g-tag">Supernatural</span><span class="g-tag">Thriller</span>
        </div>
      </div>

      <div class="sb-box">
        <div class="sb-hdr">
          <svg viewBox="0 0 24 24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
          Recently Added
        </div>
        <div class="rec-list" id="sbRecent"><div class="sb-empty">Nothing here yet.</div></div>
      </div>
    </aside>
  </div>

  <footer>
    <div class="ft-inner">
      <div class="ft-top">
        <div>
          <div class="ft-logo">9<em>ANIME</em></div>
          <p class="ft-desc">Watch anime online free in HD quality. Latest episodes and movies updated daily. The best anime streaming experience.</p>
        </div>
        <div class="ft-col"><h5>Anime</h5><ul><li><a>New Season</a></li><li><a>Movies</a></li><li><a>OVA</a></li><li><a>TV Series</a></li><li><a>Completed</a></li></ul></div>
        <div class="ft-col"><h5>Community</h5><ul><li><a>Forum</a></li><li><a>Discord</a></li><li><a>Request Anime</a></li><li><a>Report Issue</a></li></ul></div>
        <div class="ft-col"><h5>Info</h5><ul><li><a>About Us</a></li><li><a>DMCA</a></li><li><a>Privacy Policy</a></li><li><a>Terms of Use</a></li><li><a>Contact</a></li></ul></div>
      </div>
      <div class="ft-btm">
        <div class="ft-copy">© 2024 9Anime — Watch Anime Online. All Rights Reserved.</div>
        <div class="ft-links"><a>Home</a><a>Privacy</a><a>DMCA</a><a>Contact</a></div>
      </div>
    </div>
  </footer>
</div>

<!-- ══════════════════════════════
     PAGE: SEARCH
══════════════════════════════ -->
<div class="page" id="pg-search">
  <div class="back-btn" onclick="nav('home')">← Back to Home</div>
  <div class="search-wrap">
    <div class="search-ttl" id="searchTitle">Results for <em>""</em></div>
    <div class="a-grid" id="searchGrid"></div>
  </div>
</div>

<!-- ══════════════════════════════
     PAGE: WATCH
══════════════════════════════ -->
<div class="page" id="pg-watch">
  <div class="back-btn" onclick="nav('home')">← Back to Home</div>
  <div class="watch-wrap">
    <div>
      <div class="bc"><a onclick="nav('home')">Home</a> › <span id="wBC">Watch</span></div>
      <div class="player-box" id="playerBox">
        <div class="player-hold">
          <svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg>
          <p>Loading player...</p>
        </div>
      </div>
      <div class="srv-bar">
        <span class="srv-lbl">Servers:</span>
        <button class="srv-btn on" onclick="pickSrv(this)">▶ Server 1</button>
        <button class="srv-btn" onclick="pickSrv(this)">▶ Server 2</button>
        <button class="srv-btn" onclick="pickSrv(this)">▶ Server 3</button>
      </div>
      <div class="ep-box">
        <div class="ep-hdr">
          <span class="ep-hdr-ttl">Episodes</span>
          <span class="ep-hdr-ct" id="epCt"></span>
        </div>
        <div class="ep-body" id="epBody"></div>
      </div>
      <div class="w-info">
        <div class="w-badges" id="wBadges"></div>
        <div class="w-title" id="wTitle"></div>
        <div class="w-metas" id="wMetas"></div>
        <div class="w-desc" id="wDesc"></div>
      </div>
    </div>
    <div>
      <div class="sb-box">
        <div class="sb-hdr">
          <svg viewBox="0 0 24 24"><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>
          More Streams
        </div>
        <div class="rel-list" id="relList"></div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════
     PAGE: ADMIN
══════════════════════════════ -->
<div class="page" id="pg-admin">
  <div class="back-btn" onclick="nav('home')">← Back to Home</div>
  <div class="adm-wrap">
    <div class="adm-hdr">
      <div class="adm-title">
        <svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 14.5v-9l6 4.5-6 4.5z"/></svg>
        Admin — Streaming Manager
      </div>
      <div class="adm-live">🟢 Live Dashboard</div>
    </div>

    <!-- Stats -->
    <div class="adm-stats">
      <div class="s-card"><div class="s-num" id="aStat0">0</div><div class="s-lbl">Total Streams</div></div>
      <div class="s-card" style="border-color:var(--ora)"><div class="s-num" style="color:var(--ora)" id="aStat1">0</div><div class="s-lbl">Ongoing</div></div>
      <div class="s-card" style="border-color:var(--blu)"><div class="s-num" style="color:var(--blu)" id="aStat2">0</div><div class="s-lbl">Movies</div></div>
      <div class="s-card" style="border-color:var(--grn)"><div class="s-num" style="color:var(--grn)" id="aStat3">0</div><div class="s-lbl">Completed</div></div>
    </div>

    <div class="adm-grid">
      <!-- POST FORM -->
      <div class="form-box">
        <div class="fb-hdr">
          <svg viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
          <span id="fmHead">Post New Stream</span>
        </div>
        <div class="fb-body">
          <input type="hidden" id="fEid"/>

          <div class="fg">
            <label>Anime Title *</label>
            <input type="text" id="fTitle" placeholder="e.g. Demon Slayer Season 3"/>
          </div>

          <div class="fg">
            <label>Thumbnail URL</label>
            <input type="text" id="fThumb" placeholder="https://... (leave blank for auto emoji)"/> 
            <div class="fg-hint">Paste a direct image URL. Emoji auto-generated if blank.</div>
          </div>

          <div class="fg">
            <label>Video / Stream URL *</label>
            <input type="text" id="fVideo" placeholder="YouTube, iframe URL, or direct .mp4 link"/>
            <div class="fg-hint">✅ YouTube links auto-convert • iframe URLs • direct .mp4/.webm</div>
          </div>

          <div class="fg-row">
            <div class="fg">
              <label>Type</label>
              <select id="fType"><option>TV</option><option>Movie</option><option>OVA</option><option>ONA</option><option>Special</option></select>
            </div>
            <div class="fg">
              <label>Status</label>
              <select id="fStatus"><option>Ongoing</option><option>Completed</option><option>Upcoming</option></select>
            </div>
          </div>

          <div class="fg-row">
            <div class="fg">
              <label>Episodes</label>
              <input type="number" id="fEps" placeholder="e.g. 12" min="1"/>
            </div>
            <div class="fg">
              <label>Year</label>
              <input type="number" id="fYear" placeholder="e.g. 2024"/>
            </div>
          </div>

          <div class="fg-row">
            <div class="fg">
              <label>Audio</label>
              <select id="fAudio"><option>SUB</option><option>DUB</option><option value="BOTH">SUB+DUB</option></select>
            </div>
            <div class="fg">
              <label>Genre Tags</label>
              <input type="text" id="fGenre" placeholder="Action, Fantasy..."/>
            </div>
          </div>

          <div class="fg">
            <label>Synopsis / Description</label>
            <textarea id="fDesc" placeholder="Brief synopsis of the anime series..."></textarea>
          </div>

          <button class="btn-post" onclick="submitStream()">
            <svg viewBox="0 0 24 24" fill="#fff" width="13" height="13"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
            <span id="fmBtn">Post Stream</span>
          </button>
          <div class="cancel-lnk" id="cancelLnk" onclick="resetForm()">✕ Cancel Edit</div>
        </div>
      </div>

      <!-- POSTED LIST -->
      <div class="posted-box">
        <div class="pb-hdr">
          <svg viewBox="0 0 24 24"><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>
          <span>Posted Streams</span>
        </div>
        <div class="posted-list" id="postedList">
          <div class="p-empty">No streams posted yet. Use the form!</div>
        </div>
      </div>
    </div>
  </div>
</div>

<script>
// ─────────────────────────────────────────────────────
// DATA STORE
// ─────────────────────────────────────────────────────
const KEY = '9anime_v2';
const EMOJIS = ['🌸','⚔️','🔥','🌊','⚡','🌙','🎭','🧿','🐲','🌺','💥','🦋','🌀','🎯','🏮','🗡️','🌟','🔮','🐉','🎌','🦊','🌈','⛩️','🎋','🧨'];

const load = () => { try{ return JSON.parse(localStorage.getItem(KEY)) || []; }catch(e){ return []; } };
const save = d => localStorage.setItem(KEY, JSON.stringify(d));
const uid  = () => Date.now().toString(36) + Math.random().toString(36).slice(2,5);
const em   = i  => EMOJIS[Math.abs(i || 0) % EMOJIS.length];

// ─────────────────────────────────────────────────────
// NAVIGATION
// ─────────────────────────────────────────────────────
function nav(pg){
  document.querySelectorAll('.page').forEach(p => p.classList.remove('show'));
  document.getElementById('pg-' + pg).classList.add('show');
  window.scrollTo(0, 0);
  if(pg === 'home')  renderHome();
  if(pg === 'admin') renderAdmin();
}

// ─────────────────────────────────────────────────────
// TABS
// ─────────────────────────────────────────────────────
function switchTab(el, id){
  document.querySelectorAll('.tab').forEach(t => t.classList.remove('on'));
  document.querySelectorAll('.tab-pane').forEach(p => p.classList.remove('on'));
  el.classList.add('on');
  document.getElementById(id).classList.add('on');
}

// ─────────────────────────────────────────────────────
// BADGE BUILDER
// ─────────────────────────────────────────────────────
function audioBadge(a){
  if(a === 'BOTH') return `<span class="badge b-sub">SUB</span><span class="badge b-dub">DUB</span>`;
  if(a === 'DUB')  return `<span class="badge b-dub">DUB</span>`;
  return `<span class="badge b-sub">SUB</span>`;
}

// ─────────────────────────────────────────────────────
// CARD HTML
// ─────────────────────────────────────────────────────
function card(s, i){
  const hot = s.status === 'Ongoing';
  const epLbl = s.type === 'Movie' ? 'Movie' : 'EP ' + (s.eps || '?');
  const thumbHTML = s.thumb
    ? `<img src="${s.thumb}" alt="${s.title}" loading="lazy" onerror="this.parentElement.innerHTML='<div class=a-emoji>${em(i)}</div>'">`
    : `<div class="a-emoji">${em(i)}</div>`;
  return `<div class="a-card" onclick="openWatch('${s.id}')">
    <div class="a-thumb">
      ${thumbHTML}
      <div class="a-ov"><div class="a-ov-play"><svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg></div></div>
      <div class="a-bgs">${audioBadge(s.audio)}<span class="badge b-typ">${s.type||'TV'}</span></div>
      <div class="a-ep${hot?' hot':''}">${epLbl}</div>
    </div>
    <div class="a-name">${s.title}</div>
    <div class="a-sub">${s.type||'TV'}${s.status ? ' • '+s.status : ''}</div>
  </div>`;
}

function fillGrid(id, arr, emptyMsg, cta){
  const el = document.getElementById(id);
  if(!el) return;
  el.innerHTML = arr.length
    ? arr.map((s,i) => card(s,i)).join('')
    : `<div class="empty">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M18 4l2 4h-3l-2-4h-2l2 4h-3l-2-4H8l2 4H7L5 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V4h-4z"/></svg>
        <p>${emptyMsg}</p>${cta ? `<span class="empty-cta" onclick="nav('admin')">${cta}</span>` : ''}
      </div>`;
}

// ─────────────────────────────────────────────────────
// HERO SLIDER
// ─────────────────────────────────────────────────────
let sTimer=null, sIdx=0, sTotal=0;

function buildHero(all){
  const heroEmpty = document.getElementById('heroEmpty');
  const sw = document.getElementById('slidesWrap');
  const hd = document.getElementById('heroDots');
  const prev = document.getElementById('heroPrev');
  const next = document.getElementById('heroNext');
  sw.innerHTML = ''; hd.innerHTML = '';
  if(sTimer) clearInterval(sTimer);
  sIdx = 0;

  if(!all.length){
    heroEmpty.style.display = 'block';
    prev.style.display = next.style.display = 'none';
    return;
  }
  heroEmpty.style.display = 'none';
  const feat = all.slice(-6).reverse();
  sTotal = feat.length;

  feat.forEach((s,i) => {
    const bgStyle = s.thumb
      ? `background-image:url('${s.thumb}');background-color:#111;`
      : `background:linear-gradient(135deg,hsl(${i*55%360},38%,10%),hsl(${(i*55+80)%360},32%,16%));`;
    sw.innerHTML += `<div class="slide${i===0?' on':''}" id="sl${i}">
      <div class="slide-bg" style="${bgStyle}"></div>
      <div class="slide-grd"></div>
      <div class="slide-body">
        <div class="slide-tags">${audioBadge(s.audio)}<span class="badge b-new">NEW</span><span class="badge b-typ">${s.type||'TV'}</span><span class="badge b-hd">HD</span></div>
        <div class="slide-ttl">${s.title}</div>
        <div class="slide-meta">
          <span>📺 Eps: ${s.eps||'?'}</span>
          <span>🎬 ${s.type||'TV'}</span>
          <span>📅 ${s.year||'2024'}</span>
          <span>🏷 ${s.status||'Ongoing'}</span>
          ${s.genre ? `<span>🎭 ${s.genre.split(',')[0]}</span>` : ''}
        </div>
        <div class="slide-desc">${s.desc || 'No description available for this title.'}</div>
        <div class="slide-btns">
          <button class="btn-play" onclick="openWatch('${s.id}')">▶ Watch Now</button>
          <button class="btn-info" onclick="openWatch('${s.id}')">Detail</button>
        </div>
      </div>
    </div>`;
    hd.innerHTML += `<div class="dot${i===0?' on':''}" onclick="goSlide(${i})"></div>`;
  });

  prev.style.display = next.style.display = sTotal > 1 ? 'flex' : 'none';
  if(sTotal > 1) sTimer = setInterval(() => goSlide((sIdx+1) % sTotal), 5000);
}

function goSlide(n){
  document.querySelectorAll('.slide').forEach((s,i) => s.classList.toggle('on', i===n));
  document.querySelectorAll('.dot').forEach((d,i) => d.classList.toggle('on', i===n));
  sIdx = n;
}
function moveSlide(dir){ goSlide((sIdx + dir + sTotal) % sTotal); }

// ─────────────────────────────────────────────────────
// RENDER HOME
// ─────────────────────────────────────────────────────
function renderHome(){
  const all = load();
  buildHero(all);

  fillGrid('recentGrid',  [...all].reverse().slice(0,6), 'No streams added yet.', '➕ Add via Admin Panel');
  fillGrid('gridTrend',   all.slice(0,6),                'No trending streams yet.');
  fillGrid('gridPop',     [...all].sort((a,b)=>a.title.localeCompare(b.title)).slice(0,6), 'No streams yet.');
  fillGrid('gridMov',     all.filter(s=>s.type==='Movie').slice(0,6), 'No movies added yet.');
  fillGrid('gridComp',    all.filter(s=>s.status==='Completed').slice(0,6), 'No completed series yet.');

  // Sidebar Top Airing
  const sa = document.getElementById('sbAiring');
  sa.innerHTML = all.length
    ? all.slice(0,8).map((s,i) => `
      <div class="tr-item" onclick="openWatch('${s.id}')">
        <div class="tr-rank${i<3?' hot':''}">${i+1}</div>
        <div class="tr-img">${s.thumb ? `<img src="${s.thumb}" loading="lazy">` : em(i)}</div>
        <div class="tr-info">
          <div class="tr-name">${s.title}</div>
          <div class="tr-meta">EP ${s.eps||'?'} • ${s.audio||'SUB'}</div>
        </div>
      </div>`).join('')
    : '<div class="sb-empty">No streams posted yet.</div>';

  // Sidebar Recently Added
  const sr = document.getElementById('sbRecent');
  sr.innerHTML = all.length
    ? [...all].reverse().slice(0,4).map((s,i) => `
      <div class="rec-item" onclick="openWatch('${s.id}')">
        <div class="rec-img">${s.thumb ? `<img src="${s.thumb}" loading="lazy">` : em(i)}</div>
        <div class="rec-info">
          <div class="rec-name">${s.title}</div>
          <div class="rec-ep">Ep <b>${s.eps||'?'}</b> • ${s.status||'Ongoing'}</div>
        </div>
      </div>`).join('')
    : '<div class="sb-empty">Nothing here yet.</div>';
}

// ─────────────────────────────────────────────────────
// WATCH PAGE
// ─────────────────────────────────────────────────────
function openWatch(id){
  const all = load();
  const s = all.find(x => x.id === id);
  if(!s) return;

  // Breadcrumb + title
  document.getElementById('wBC').textContent = s.title;
  document.getElementById('wTitle').textContent = s.title;

  // Badges
  document.getElementById('wBadges').innerHTML =
    `${audioBadge(s.audio)}<span class="badge b-typ">${s.type||'TV'}</span><span class="badge b-new">${s.status||'Ongoing'}</span>`;

  // Meta
  document.getElementById('wMetas').innerHTML = `
    <div class="w-meta">🎬 <strong>Type:</strong> ${s.type||'TV'}</div>
    <div class="w-meta">📺 <strong>Episodes:</strong> ${s.eps||'?'}</div>
    <div class="w-meta">📅 <strong>Year:</strong> ${s.year||'—'}</div>
    <div class="w-meta">🏷 <strong>Genre:</strong> ${s.genre||'—'}</div>
    <div class="w-meta">🔊 <strong>Audio:</strong> ${s.audio||'SUB'}</div>`;

  document.getElementById('wDesc').textContent = s.desc || 'No description available.';

  // Player
  loadPlayer(s.video);

  // Episodes
  const epCount = Math.min(parseInt(s.eps)||1, 500);
  document.getElementById('epCt').textContent = epCount + ' Episode' + (epCount!==1?'s':'');
  document.getElementById('epBody').innerHTML = Array.from({length:epCount},(_,i) =>
    `<button class="ep-n${i===0?' on':''}" onclick="pickEp(this,${i+1})">${i+1}</button>`
  ).join('');

  // Related
  const rel = all.filter(x => x.id !== id).slice(0, 8);
  document.getElementById('relList').innerHTML = rel.length
    ? rel.map((r,i) => `
      <div class="rel-item" onclick="openWatch('${r.id}')">
        <div class="rel-img">${r.thumb ? `<img src="${r.thumb}" loading="lazy">` : em(i)}</div>
        <div class="rel-info">
          <div class="rel-name">${r.title}</div>
          <div class="rel-meta">${r.type||'TV'} • ${r.status||'Ongoing'}</div>
        </div>
      </div>`).join('')
    : '<div style="padding:16px;text-align:center;font-size:12px;color:var(--t3)">No other streams yet.</div>';

  nav('watch');
}

function loadPlayer(url){
  const box = document.getElementById('playerBox');
  if(!url){
    box.innerHTML = `<div class="player-hold"><svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg><p>No video URL provided.</p></div>`;
    return;
  }
  // YouTube auto-convert
  const yt = url.match(/(?:youtube\.com\/watch\?v=|youtu\.be\/)([a-zA-Z0-9_-]{11})/);
  if(yt){ url = `https://www.youtube.com/embed/${yt[1]}?rel=0&autoplay=0`; }

  if(/\.(mp4|webm|ogg)(\?.*)?$/i.test(url)){
    box.innerHTML = `<video controls src="${url}" style="width:100%;aspect-ratio:16/9;display:block;background:#000;"></video>`;
  } else {
    box.innerHTML = `<iframe src="${url}" style="width:100%;aspect-ratio:16/9;display:block;" frameborder="0" allowfullscreen allow="autoplay;encrypted-media;picture-in-picture"></iframe>`;
  }
}

function pickEp(btn, n){
  document.querySelectorAll('.ep-n').forEach(b => b.classList.remove('on'));
  btn.classList.add('on');
  toast('▶ Playing Episode ' + n);
}

function pickSrv(btn){
  document.querySelectorAll('.srv-btn').forEach(b => b.classList.remove('on'));
  btn.classList.add('on');
  toast('Switched to ' + btn.textContent.trim());
}

// ─────────────────────────────────────────────────────
// SEARCH
// ─────────────────────────────────────────────────────
function searchQ(q){
  if(!q || !q.trim()) return;
  const all = load();
  const r = all.filter(s => s.title.toLowerCase().includes(q.toLowerCase().trim()));
  document.getElementById('searchTitle').innerHTML = `Results for <em>"${q}"</em> — ${r.length} found`;
  const sg = document.getElementById('searchGrid');
  sg.innerHTML = r.length
    ? r.map((s,i) => card(s,i)).join('')
    : `<div class="empty"><p>No results for "<strong>${q}</strong>"</p><span class="empty-cta" onclick="nav('home')">← Back to Home</span></div>`;
  nav('search');
}

// ─────────────────────────────────────────────────────
// ADMIN
// ─────────────────────────────────────────────────────
function renderAdmin(){
  const all = load();
  document.getElementById('aStat0').textContent = all.length;
  document.getElementById('aStat1').textContent = all.filter(s=>s.status==='Ongoing').length;
  document.getElementById('aStat2').textContent = all.filter(s=>s.type==='Movie').length;
  document.getElementById('aStat3').textContent = all.filter(s=>s.status==='Completed').length;

  const pl = document.getElementById('postedList');
  if(!all.length){ pl.innerHTML = '<div class="p-empty">No streams posted yet. Use the form above!</div>'; return; }

  pl.innerHTML = [...all].reverse().map((s,i) => `
    <div class="p-item">
      <div class="p-thumb">${s.thumb ? `<img src="${s.thumb}" loading="lazy">` : em(i)}</div>
      <div class="p-info">
        <div class="p-name">${s.title}</div>
        <div class="p-sub">${s.type||'TV'} • ${s.status||'Ongoing'} • ${s.audio||'SUB'} • EP ${s.eps||'?'} • ${s.year||'—'}</div>
      </div>
      <div class="p-acts">
        <button class="btn-ic" onclick="openWatch('${s.id}')">▶</button>
        <button class="btn-ic" onclick="editStream('${s.id}')">✏</button>
        <button class="btn-ic del" onclick="askDel('${s.id}')">🗑</button>
      </div>
    </div>`).join('');
}

function submitStream(){
  const title = document.getElementById('fTitle').value.trim();
  const video = document.getElementById('fVideo').value.trim();
  if(!title){ toast('⚠️ Title is required!', true); return; }
  if(!video){ toast('⚠️ Video URL is required!', true); return; }

  const eid = document.getElementById('fEid').value;
  const all = load();
  const obj = {
    id:     eid || uid(),
    title,  video,
    thumb:  document.getElementById('fThumb').value.trim(),
    type:   document.getElementById('fType').value,
    status: document.getElementById('fStatus').value,
    eps:    document.getElementById('fEps').value,
    year:   document.getElementById('fYear').value,
    audio:  document.getElementById('fAudio').value,
    genre:  document.getElementById('fGenre').value.trim(),
    desc:   document.getElementById('fDesc').value.trim(),
    ts:     eid ? (all.find(s=>s.id===eid)||{}).ts || Date.now() : Date.now()
  };

  if(eid){
    const idx = all.findIndex(s => s.id === eid);
    if(idx > -1) all[idx] = obj; else all.push(obj);
    toast('✅ Stream updated successfully!');
  } else {
    all.push(obj);
    toast('✅ Stream posted successfully!');
  }
  save(all);
  resetForm();
  renderAdmin();
}

function editStream(id){
  const s = load().find(x => x.id === id);
  if(!s) return;
  document.getElementById('fEid').value    = s.id;
  document.getElementById('fTitle').value  = s.title;
  document.getElementById('fThumb').value  = s.thumb || '';
  document.getElementById('fVideo').value  = s.video || '';
  document.getElementById('fType').value   = s.type || 'TV';
  document.getElementById('fStatus').value = s.status || 'Ongoing';
  document.getElementById('fEps').value    = s.eps || '';
  document.getElementById('fYear').value   = s.year || '';
  document.getElementById('fAudio').value  = s.audio || 'SUB';
  document.getElementById('fGenre').value  = s.genre || '';
  document.getElementById('fDesc').value   = s.desc || '';
  document.getElementById('fmHead').textContent = 'Edit Stream';
  document.getElementById('fmBtn').textContent  = 'Update Stream';
  document.getElementById('cancelLnk').style.display = 'block';
  document.querySelector('.form-box').scrollIntoView({behavior:'smooth'});
}

function resetForm(){
  document.getElementById('fEid').value = '';
  ['fTitle','fThumb','fVideo','fEps','fYear','fGenre','fDesc'].forEach(id => document.getElementById(id).value = '');
  document.getElementById('fType').value   = 'TV';
  document.getElementById('fStatus').value = 'Ongoing';
  document.getElementById('fAudio').value  = 'SUB';
  document.getElementById('fmHead').textContent = 'Post New Stream';
  document.getElementById('fmBtn').textContent  = 'Post Stream';
  document.getElementById('cancelLnk').style.display = 'none';
}

// Delete
let delId = null;
function askDel(id){ delId = id; document.getElementById('delModal').classList.add('show'); }
function closeModal(){ delId = null; document.getElementById('delModal').classList.remove('show'); }
function doDelete(){
  if(!delId) return;
  save(load().filter(s => s.id !== delId));
  closeModal();
  toast('🗑 Stream deleted.');
  renderAdmin();
}

// ─────────────────────────────────────────────────────
// TOAST
// ─────────────────────────────────────────────────────
let tTimer;
function toast(msg, warn=false){
  const el = document.getElementById('toast');
  el.textContent = msg;
  el.style.borderLeftColor = warn ? 'var(--ora)' : 'var(--grn)';
  el.classList.add('show');
  clearTimeout(tTimer);
  tTimer = setTimeout(() => el.classList.remove('show'), 2800);
}

// ─────────────────────────────────────────────────────
// BOOT
// ─────────────────────────────────────────────────────
renderHome();
</script>
</body>
</html>
