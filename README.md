<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>9Anime - Watch Anime Online Free HD</title>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800;900&family=Rajdhani:wght@500;600;700&display=swap" rel="stylesheet">
<style>
  :root {
    --bg-primary:#0d0d0d; --bg-secondary:#141414; --bg-card:#1a1a1a; --bg-hover:#222;
    --accent:#e74c3c; --accent-orange:#f39c12; --accent-blue:#3498db; --accent-green:#2ecc71;
    --text-primary:#e0e0e0; --text-secondary:#999; --text-muted:#666;
    --border:#2a2a2a; --border-light:#333; --header-bg:#111;
    --badge-sub:#f39c12; --badge-dub:#3498db;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  body{font-family:'Nunito',sans-serif;background:var(--bg-primary);color:var(--text-primary);font-size:14px;line-height:1.5;}
  a{text-decoration:none;color:inherit;cursor:pointer;}
  .page{display:none;} .page.active{display:block;}

  /* NOTICE */
  .notice-bar{background:linear-gradient(90deg,#1a0505,#1e1010,#1a0505);border-bottom:1px solid #3a1515;padding:6px 20px;text-align:center;font-size:12px;color:#cc9090;}
  .notice-bar strong{color:var(--accent);}

  /* HEADER */
  header{background:var(--header-bg);border-bottom:1px solid var(--border);position:sticky;top:0;z-index:100;box-shadow:0 2px 10px rgba(0,0,0,.5);}
  .header-top{display:flex;align-items:center;padding:0 20px;height:54px;max-width:1280px;margin:0 auto;gap:16px;}
  .logo{font-family:'Rajdhani',sans-serif;font-size:26px;font-weight:700;color:var(--accent);letter-spacing:1px;flex-shrink:0;cursor:pointer;}
  .logo span{color:var(--text-primary);}
  .search-bar{flex:1;max-width:460px;display:flex;align-items:center;background:#1e1e1e;border:1px solid var(--border-light);border-radius:4px;overflow:hidden;}
  .search-bar input{flex:1;background:none;border:none;padding:8px 14px;color:var(--text-primary);font-size:13px;outline:none;font-family:'Nunito',sans-serif;}
  .search-bar input::placeholder{color:var(--text-muted);}
  .search-bar button{background:var(--accent);border:none;padding:8px 14px;color:#fff;cursor:pointer;font-size:14px;transition:background .2s;}
  .search-bar button:hover{background:#c0392b;}
  .header-actions{margin-left:auto;display:flex;align-items:center;gap:10px;}
  .btn-admin{background:linear-gradient(135deg,#f39c12,#e67e22);color:#000;padding:6px 14px;border-radius:3px;font-size:12px;font-weight:700;cursor:pointer;display:flex;align-items:center;gap:5px;transition:opacity .2s;}
  .btn-admin:hover{opacity:.85;}
  .btn-login{background:var(--accent);color:#fff;padding:6px 16px;border-radius:3px;font-size:13px;font-weight:600;transition:background .2s;}
  .btn-login:hover{background:#c0392b;}
  .btn-register{background:#2a2a2a;color:var(--text-primary);padding:6px 16px;border-radius:3px;font-size:13px;font-weight:600;border:1px solid var(--border-light);transition:background .2s;}
  .btn-register:hover{background:#333;}

  /* NAV */
  nav{background:#161616;border-bottom:1px solid var(--border);}
  .nav-inner{max-width:1280px;margin:0 auto;padding:0 20px;display:flex;align-items:center;gap:2px;}
  .nav-inner a{color:#ccc;font-size:13px;font-weight:600;padding:10px 14px;transition:color .2s,background .2s;letter-spacing:.3px;display:flex;align-items:center;gap:5px;}
  .nav-inner a:hover,.nav-inner a.active{color:var(--accent);background:rgba(231,76,60,.08);}
  .nav-genre{position:relative;}
  .nav-genre:hover .genre-dropdown{display:grid;}
  .genre-dropdown{display:none;position:absolute;top:100%;left:0;background:#1a1a1a;border:1px solid var(--border-light);border-top:2px solid var(--accent);padding:12px;grid-template-columns:repeat(4,140px);gap:2px;z-index:200;box-shadow:0 8px 24px rgba(0,0,0,.5);min-width:580px;}
  .genre-dropdown a{font-size:12px;padding:6px 10px;border-radius:3px;color:var(--text-secondary);}
  .genre-dropdown a:hover{color:var(--accent);background:rgba(231,76,60,.08);}

  /* LAYOUT */
  .page-wrapper{max-width:1280px;margin:0 auto;padding:16px 20px;display:grid;grid-template-columns:1fr 260px;gap:20px;}

  /* SECTION HEADER */
  .section-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;padding-bottom:8px;border-bottom:2px solid var(--border);position:relative;}
  .section-header::after{content:'';position:absolute;bottom:-2px;left:0;width:80px;height:2px;background:var(--accent);}
  .section-title{font-family:'Rajdhani',sans-serif;font-size:16px;font-weight:700;color:var(--text-primary);letter-spacing:.5px;text-transform:uppercase;}
  .view-all{font-size:12px;color:var(--text-muted);transition:color .2s;}
  .view-all:hover{color:var(--accent);}

  /* GRID + CARDS */
  .anime-grid{display:grid;grid-template-columns:repeat(6,1fr);gap:12px;margin-bottom:24px;min-height:40px;}
  .anime-card{position:relative;cursor:pointer;}
  .anime-thumb{position:relative;border-radius:4px;overflow:hidden;aspect-ratio:3/4;background:#1c1c1c;margin-bottom:7px;}
  .anime-thumb img{width:100%;height:100%;object-fit:cover;transition:transform .3s,filter .3s;}
  .anime-card:hover .anime-thumb img{transform:scale(1.06);filter:brightness(.7);}
  .anime-thumb-overlay{position:absolute;inset:0;background:rgba(0,0,0,0);display:flex;align-items:center;justify-content:center;transition:background .3s;}
  .anime-card:hover .anime-thumb-overlay{background:rgba(0,0,0,.35);}
  .play-icon{width:36px;height:36px;background:rgba(231,76,60,.9);border-radius:50%;display:flex;align-items:center;justify-content:center;opacity:0;transform:scale(.8);transition:opacity .3s,transform .3s;}
  .play-icon svg{width:16px;height:16px;fill:#fff;margin-left:2px;}
  .anime-card:hover .play-icon{opacity:1;transform:scale(1);}
  .thumb-badges{position:absolute;top:5px;left:5px;display:flex;gap:3px;flex-wrap:wrap;}
  .badge{font-size:10px;font-weight:700;padding:2px 8px;border-radius:2px;text-transform:uppercase;letter-spacing:.5px;}
  .badge-sub{background:var(--badge-sub);color:#000;}
  .badge-dub{background:var(--badge-dub);color:#fff;}
  .badge-new{background:var(--accent);color:#fff;}
  .badge-tv{background:#555;color:#fff;}
  .ep-count{position:absolute;bottom:5px;right:5px;background:rgba(0,0,0,.78);color:#ccc;font-size:10px;padding:2px 6px;border-radius:2px;font-weight:700;}
  .ep-count.new-ep{color:var(--accent-orange);}
  .thumb-placeholder{width:100%;height:100%;display:flex;align-items:center;justify-content:center;font-size:32px;}
  .anime-name{font-size:12px;font-weight:700;color:var(--text-primary);line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;transition:color .2s;}
  .anime-card:hover .anime-name{color:var(--accent);}
  .anime-type{font-size:11px;color:var(--text-muted);margin-top:2px;}

  /* EMPTY STATE */
  .empty-state{grid-column:1/-1;text-align:center;padding:40px 20px;color:var(--text-muted);}
  .empty-state svg{width:44px;height:44px;margin-bottom:10px;opacity:.25;}
  .empty-state p{font-size:13px;}
  .add-hint{color:var(--accent);font-size:12px;margin-top:8px;cursor:pointer;}
  .add-hint:hover{text-decoration:underline;}

  /* TABS */
  .tab-bar{display:flex;border-bottom:2px solid var(--border);margin-bottom:14px;}
  .tab{padding:8px 16px;font-size:13px;font-weight:700;color:var(--text-muted);cursor:pointer;transition:color .2s;font-family:'Rajdhani',sans-serif;text-transform:uppercase;letter-spacing:.5px;border-bottom:2px solid transparent;margin-bottom:-2px;}
  .tab.active{color:var(--accent);border-bottom-color:var(--accent);}
  .tab:hover{color:var(--text-primary);}

  /* HERO */
  .hero-slider{position:relative;border-radius:6px;overflow:hidden;background:#1a1a1a;margin-bottom:22px;height:360px;display:flex;align-items:center;justify-content:center;}
  .hero-empty{text-align:center;color:var(--text-muted);}
  .hero-empty svg{width:52px;height:52px;margin-bottom:12px;opacity:.2;}
  .hero-empty p{font-size:14px;margin-bottom:6px;}
  .hero-empty span{color:var(--accent);cursor:pointer;font-size:12px;}
  .hero-empty span:hover{text-decoration:underline;}
  .slide{display:none;position:absolute;inset:0;animation:fadeIn .5s ease;}
  .slide.active{display:block;}
  @keyframes fadeIn{from{opacity:0}to{opacity:1}}
  .slide-bg-div{position:absolute;inset:0;}
  .slide-content{position:absolute;bottom:0;left:0;right:0;padding:24px 28px;background:linear-gradient(to top,rgba(0,0,0,.92) 0%,rgba(0,0,0,.5) 60%,transparent 100%);}
  .slide-badges{display:flex;gap:6px;margin-bottom:8px;}
  .slide-title{font-family:'Rajdhani',sans-serif;font-size:26px;font-weight:700;color:#fff;line-height:1.2;margin-bottom:6px;text-shadow:0 2px 6px rgba(0,0,0,.8);}
  .slide-meta{font-size:12px;color:#aaa;margin-bottom:10px;display:flex;gap:14px;}
  .slide-desc{font-size:12px;color:#bbb;line-height:1.5;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;margin-bottom:14px;max-width:600px;}
  .slide-actions{display:flex;gap:8px;}
  .btn-watch{background:var(--accent);color:#fff;padding:8px 20px;border-radius:3px;font-size:13px;font-weight:700;display:flex;align-items:center;gap:6px;transition:background .2s,transform .1s;cursor:pointer;border:none;font-family:'Nunito',sans-serif;}
  .btn-watch:hover{background:#c0392b;transform:translateY(-1px);}
  .btn-detail{background:rgba(255,255,255,.1);color:#fff;padding:8px 18px;border-radius:3px;font-size:13px;font-weight:600;border:1px solid rgba(255,255,255,.2);transition:background .2s;cursor:pointer;font-family:'Nunito',sans-serif;}
  .btn-detail:hover{background:rgba(255,255,255,.18);}
  .slider-dots{position:absolute;bottom:14px;right:18px;display:flex;gap:5px;}
  .dot{width:8px;height:8px;border-radius:50%;background:rgba(255,255,255,.3);cursor:pointer;transition:background .2s,transform .2s;}
  .dot.active{background:var(--accent);transform:scale(1.25);}

  /* SCHEDULE */
  .schedule-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:8px;margin-bottom:20px;}
  .day-label{font-size:11px;font-weight:700;text-align:center;padding:5px 4px;background:#1e1e1e;border-radius:3px;margin-bottom:6px;color:var(--text-muted);text-transform:uppercase;letter-spacing:.5px;}

  /* SIDEBAR */
  .sidebar-box{background:var(--bg-secondary);border:1px solid var(--border);border-radius:5px;overflow:hidden;margin-bottom:16px;}
  .sidebar-box-header{background:#1e1e1e;padding:10px 14px;font-family:'Rajdhani',sans-serif;font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--text-primary);border-bottom:2px solid var(--accent);display:flex;align-items:center;gap:7px;}
  .sidebar-box-header svg{width:14px;height:14px;fill:var(--accent);}
  .trending-list{padding:8px 0;}
  .trending-item{display:flex;align-items:center;gap:10px;padding:7px 12px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);}
  .trending-item:last-child{border-bottom:none;}
  .trending-item:hover{background:#1e1e1e;}
  .rank-num{font-family:'Rajdhani',sans-serif;font-size:18px;font-weight:700;color:var(--border-light);min-width:22px;text-align:center;}
  .rank-num.top3{color:var(--accent);}
  .t-thumb{width:44px;height:60px;border-radius:3px;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:20px;overflow:hidden;background:#1e1e1e;}
  .t-thumb img{width:100%;height:100%;object-fit:cover;}
  .trending-info{flex:1;min-width:0;}
  .trending-name{font-size:12px;font-weight:700;color:var(--text-primary);line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
  .trending-item:hover .trending-name{color:var(--accent);}
  .trending-meta{font-size:10px;color:var(--text-muted);margin-top:2px;}
  .genre-tags{padding:12px;display:flex;flex-wrap:wrap;gap:5px;}
  .genre-tag{background:#1e1e1e;border:1px solid var(--border-light);color:var(--text-secondary);font-size:11px;padding:4px 10px;border-radius:2px;cursor:pointer;transition:background .2s,color .2s,border-color .2s;}
  .genre-tag:hover{background:var(--accent);color:#fff;border-color:var(--accent);}
  .recent-list{padding:6px 0;}
  .recent-item{display:flex;gap:10px;padding:7px 12px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);align-items:flex-start;}
  .recent-item:hover{background:#1e1e1e;}
  .r-thumb{width:50px;height:70px;border-radius:3px;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:22px;overflow:hidden;background:#1e1e1e;}
  .r-thumb img{width:100%;height:100%;object-fit:cover;}
  .recent-info{flex:1;min-width:0;}
  .recent-name{font-size:12px;font-weight:700;color:var(--text-primary);line-height:1.3;margin-bottom:3px;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
  .recent-item:hover .recent-name{color:var(--accent);}
  .recent-ep{font-size:10px;color:var(--text-muted);}
  .recent-ep strong{color:var(--accent-orange);}
  .sidebar-empty{padding:18px 12px;text-align:center;color:var(--text-muted);font-size:12px;}

  /* FOOTER */
  footer{background:#0a0a0a;border-top:1px solid var(--border);padding:30px 20px;margin-top:10px;}
  .footer-inner{max-width:1280px;margin:0 auto;}
  .footer-top{display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:28px;margin-bottom:24px;}
  .footer-logo{font-family:'Rajdhani',sans-serif;font-size:22px;font-weight:700;color:var(--accent);margin-bottom:10px;}
  .footer-logo span{color:var(--text-primary);}
  .footer-desc{font-size:12px;color:var(--text-muted);line-height:1.6;}
  .footer-col h4{font-family:'Rajdhani',sans-serif;font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--text-primary);margin-bottom:10px;padding-bottom:6px;border-bottom:1px solid var(--border);}
  .footer-col ul{list-style:none;}
  .footer-col ul li{margin-bottom:6px;}
  .footer-col ul li a{font-size:12px;color:var(--text-muted);transition:color .2s;}
  .footer-col ul li a:hover{color:var(--accent);}
  .footer-bottom{border-top:1px solid var(--border);padding-top:16px;display:flex;align-items:center;justify-content:space-between;}
  .footer-copy{font-size:11px;color:var(--text-muted);}
  .footer-links{display:flex;gap:14px;}
  .footer-links a{font-size:11px;color:var(--text-muted);transition:color .2s;}
  .footer-links a:hover{color:var(--accent);}

  /* ══ WATCH PAGE ══ */
  .watch-wrapper{max-width:1280px;margin:0 auto;padding:16px 20px;display:grid;grid-template-columns:1fr 300px;gap:20px;}
  .breadcrumb{font-size:12px;color:var(--text-muted);margin-bottom:14px;display:flex;align-items:center;gap:6px;}
  .breadcrumb a{color:var(--text-secondary);transition:color .2s;}
  .breadcrumb a:hover{color:var(--accent);}
  .player-box{background:#000;border-radius:6px;overflow:hidden;margin-bottom:14px;}
  .player-box iframe,.player-box video{width:100%;aspect-ratio:16/9;display:block;border:none;}
  .player-loading{width:100%;aspect-ratio:16/9;display:flex;align-items:center;justify-content:center;background:#0a0a0a;flex-direction:column;gap:12px;}
  .player-loading svg{width:56px;height:56px;fill:var(--accent);opacity:.4;animation:pulse 2s infinite;}
  .player-loading p{font-size:13px;color:var(--text-muted);}
  @keyframes pulse{0%,100%{opacity:.3}50%{opacity:.8}}
  .server-bar{background:#1a1a1a;border:1px solid var(--border);border-radius:4px;padding:10px 14px;margin-bottom:14px;display:flex;align-items:center;gap:10px;flex-wrap:wrap;}
  .server-label{font-size:11px;font-weight:700;color:var(--text-muted);text-transform:uppercase;letter-spacing:.5px;}
  .server-btn{background:#242424;border:1px solid var(--border-light);color:var(--text-secondary);font-size:12px;padding:5px 14px;border-radius:3px;cursor:pointer;transition:background .2s,color .2s;font-family:'Nunito',sans-serif;}
  .server-btn.active,.server-btn:hover{background:var(--accent);color:#fff;border-color:var(--accent);}
  .ep-list-box{background:#1a1a1a;border:1px solid var(--border);border-radius:4px;overflow:hidden;margin-bottom:14px;}
  .ep-list-header{background:#1e1e1e;padding:10px 14px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--border);}
  .ep-list-header span{font-family:'Rajdhani',sans-serif;font-size:13px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
  .ep-list-body{padding:10px;display:flex;flex-wrap:wrap;gap:5px;max-height:160px;overflow-y:auto;}
  .ep-btn{background:#242424;border:1px solid var(--border-light);color:var(--text-secondary);font-size:12px;font-weight:700;padding:5px 10px;border-radius:3px;cursor:pointer;transition:background .2s,color .2s;min-width:44px;text-align:center;font-family:'Nunito',sans-serif;}
  .ep-btn:hover{background:#333;color:var(--text-primary);}
  .ep-btn.active{background:var(--accent);color:#fff;border-color:var(--accent);}
  .watch-info{background:#1a1a1a;border:1px solid var(--border);border-radius:6px;padding:18px;margin-bottom:14px;}
  .watch-title{font-family:'Rajdhani',sans-serif;font-size:22px;font-weight:700;color:var(--text-primary);margin-bottom:8px;line-height:1.2;}
  .watch-meta-row{display:flex;flex-wrap:wrap;gap:14px;margin-bottom:10px;}
  .watch-meta-item{font-size:12px;color:var(--text-muted);display:flex;align-items:center;gap:4px;}
  .watch-meta-item strong{color:var(--text-secondary);}
  .watch-desc{font-size:13px;color:var(--text-secondary);line-height:1.6;}
  .watch-badges{display:flex;gap:6px;margin-bottom:10px;}
  .related-list{padding:8px 0;}
  .related-item{display:flex;gap:10px;padding:8px 12px;cursor:pointer;transition:background .2s;border-bottom:1px solid rgba(255,255,255,.03);}
  .related-item:hover{background:#1e1e1e;}
  .related-item:last-child{border-bottom:none;}
  .rel-thumb{width:80px;height:54px;border-radius:3px;flex-shrink:0;display:flex;align-items:center;justify-content:center;overflow:hidden;background:#1e1e1e;}
  .rel-thumb img{width:100%;height:100%;object-fit:cover;}
  .related-info{flex:1;min-width:0;}
  .related-name{font-size:12px;font-weight:700;color:var(--text-primary);line-height:1.3;margin-bottom:3px;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
  .related-item:hover .related-name{color:var(--accent);}
  .related-meta{font-size:11px;color:var(--text-muted);}

  /* ══ ADMIN ══ */
  .admin-wrapper{max-width:960px;margin:0 auto;padding:24px 20px;}
  .admin-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:24px;}
  .admin-title{font-family:'Rajdhani',sans-serif;font-size:22px;font-weight:700;color:var(--text-primary);display:flex;align-items:center;gap:10px;}
  .admin-title svg{width:22px;height:22px;fill:var(--accent);}
  .admin-stats{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-bottom:24px;}
  .stat-card{background:#1a1a1a;border:1px solid var(--border);border-radius:6px;padding:16px;border-left:3px solid var(--accent);}
  .stat-num{font-family:'Rajdhani',sans-serif;font-size:28px;font-weight:700;color:var(--accent);}
  .stat-label{font-size:11px;color:var(--text-muted);text-transform:uppercase;letter-spacing:.5px;margin-top:2px;}
  .admin-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
  .form-box{background:#1a1a1a;border:1px solid var(--border);border-radius:6px;overflow:hidden;}
  .form-box-header{background:#1e1e1e;padding:12px 18px;border-bottom:2px solid var(--accent);display:flex;align-items:center;gap:8px;}
  .form-box-header span{font-family:'Rajdhani',sans-serif;font-size:14px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
  .form-box-header svg{width:16px;height:16px;fill:var(--accent);}
  .form-body{padding:18px;}
  .form-group{margin-bottom:14px;}
  .form-group label{display:block;font-size:12px;font-weight:700;color:var(--text-secondary);margin-bottom:5px;text-transform:uppercase;letter-spacing:.3px;}
  .form-group input,.form-group textarea,.form-group select{width:100%;background:#242424;border:1px solid var(--border-light);color:var(--text-primary);padding:9px 12px;border-radius:3px;font-size:13px;outline:none;font-family:'Nunito',sans-serif;transition:border-color .2s;}
  .form-group input:focus,.form-group textarea:focus,.form-group select:focus{border-color:var(--accent);}
  .form-group textarea{resize:vertical;min-height:80px;}
  .form-group select option{background:#242424;}
  .input-hint{font-size:11px;color:var(--text-muted);margin-top:4px;}
  .form-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
  .btn-submit{background:var(--accent);color:#fff;border:none;padding:10px 24px;border-radius:3px;font-size:13px;font-weight:700;cursor:pointer;transition:background .2s,transform .1s;font-family:'Nunito',sans-serif;display:flex;align-items:center;gap:6px;width:100%;justify-content:center;}
  .btn-submit:hover{background:#c0392b;transform:translateY(-1px);}
  .posted-box{background:#1a1a1a;border:1px solid var(--border);border-radius:6px;overflow:hidden;}
  .posted-list-header{background:#1e1e1e;padding:12px 18px;border-bottom:2px solid var(--accent);display:flex;align-items:center;gap:8px;}
  .posted-list-header span{font-family:'Rajdhani',sans-serif;font-size:14px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;}
  .posted-item{display:flex;align-items:center;gap:12px;padding:10px 14px;border-bottom:1px solid rgba(255,255,255,.04);transition:background .2s;}
  .posted-item:last-child{border-bottom:none;}
  .posted-item:hover{background:#1e1e1e;}
  .p-thumb{width:54px;height:40px;border-radius:3px;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:18px;overflow:hidden;background:#242424;}
  .p-thumb img{width:100%;height:100%;object-fit:cover;}
  .posted-info{flex:1;min-width:0;}
  .posted-name{font-size:12px;font-weight:700;color:var(--text-primary);white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
  .posted-sub{font-size:10px;color:var(--text-muted);margin-top:2px;}
  .posted-actions{display:flex;gap:6px;}
  .btn-icon{background:#242424;border:1px solid var(--border-light);color:var(--text-muted);padding:5px 8px;border-radius:3px;cursor:pointer;font-size:11px;transition:background .2s,color .2s;font-family:'Nunito',sans-serif;}
  .btn-icon:hover{background:var(--accent);color:#fff;border-color:var(--accent);}
  .btn-icon.del:hover{background:#c0392b;border-color:#c0392b;color:#fff;}
  .posted-empty{padding:24px;text-align:center;color:var(--text-muted);font-size:13px;}

  /* BACK BTN */
  .back-btn{display:inline-flex;align-items:center;gap:6px;color:var(--text-muted);font-size:13px;padding:10px 20px;cursor:pointer;transition:color .2s;}
  .back-btn:hover{color:var(--accent);}

  /* TOAST */
  .toast{position:fixed;bottom:24px;right:24px;background:#1a1a1a;border:1px solid var(--border-light);border-left:4px solid var(--accent-green);color:var(--text-primary);padding:12px 18px;border-radius:4px;font-size:13px;font-weight:600;z-index:9999;opacity:0;transform:translateY(10px);transition:opacity .3s,transform .3s;pointer-events:none;display:flex;align-items:center;gap:8px;max-width:300px;}
  .toast.show{opacity:1;transform:translateY(0);}

  /* MODAL */
  .modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,.75);z-index:500;display:flex;align-items:center;justify-content:center;opacity:0;pointer-events:none;transition:opacity .2s;}
  .modal-overlay.show{opacity:1;pointer-events:all;}
  .modal{background:#1a1a1a;border:1px solid var(--border-light);border-top:3px solid var(--accent);border-radius:6px;padding:24px;max-width:360px;width:90%;}
  .modal h3{font-family:'Rajdhani',sans-serif;font-size:18px;font-weight:700;margin-bottom:8px;}
  .modal p{font-size:13px;color:var(--text-secondary);margin-bottom:18px;}
  .modal-btns{display:flex;gap:10px;}
  .btn-cancel-m{background:#242424;border:1px solid var(--border-light);color:var(--text-secondary);padding:8px 18px;border-radius:3px;cursor:pointer;font-size:13px;font-family:'Nunito',sans-serif;transition:background .2s;}
  .btn-cancel-m:hover{background:#333;}
  .btn-confirm-del{background:#c0392b;border:none;color:#fff;padding:8px 18px;border-radius:3px;cursor:pointer;font-size:13px;font-weight:700;font-family:'Nunito',sans-serif;transition:background .2s;}
  .btn-confirm-del:hover{background:#a93226;}

  ::-webkit-scrollbar{width:6px;height:6px;}
  ::-webkit-scrollbar-track{background:#1a1a1a;}
  ::-webkit-scrollbar-thumb{background:#333;border-radius:3px;}
  ::-webkit-scrollbar-thumb:hover{background:#555;}
</style>
</head>
<body>

<!-- TOAST -->
<div class="toast" id="toast"><span id="toastMsg"></span></div>

<!-- DELETE MODAL -->
<div class="modal-overlay" id="deleteModal">
  <div class="modal">
    <h3>🗑 Delete Stream?</h3>
    <p>This will permanently remove this stream. This action cannot be undone.</p>
    <div class="modal-btns">
      <button class="btn-cancel-m" onclick="closeDelModal()">Cancel</button>
      <button class="btn-confirm-del" onclick="confirmDelete()">Yes, Delete</button>
    </div>
  </div>
</div>

<!-- ── SHARED HEADER ── -->
<div class="notice-bar">⚠️ Use <strong>AdBlock</strong> for a better experience. Bookmark us: <strong>9anime.to</strong></div>

<header>
  <div class="header-top">
    <div class="logo" onclick="showPage('home')">9<span>ANIME</span></div>
    <div class="search-bar">
      <input type="text" id="searchInput" placeholder="Search anime..." oninput="liveSearch(this.value)">
      <button onclick="liveSearch(document.getElementById('searchInput').value)">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" width="14" height="14"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>
      </button>
    </div>
    <div class="header-actions">
      <div class="btn-admin" onclick="showPage('admin')">⚙ Admin Panel</div>
      <a href="#" class="btn-register">Register</a>
      <a href="#" class="btn-login">Login</a>
    </div>
  </div>
</header>

<nav>
  <div class="nav-inner">
    <a href="#" class="active" onclick="showPage('home');return false;">
      <svg viewBox="0 0 24 24" fill="currentColor" width="14" height="14"><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>Home
    </a>
    <a href="#">New Season</a><a href="#">Movies</a><a href="#">TV Series</a>
    <a href="#">OVA</a><a href="#">ONA</a><a href="#">Specials</a>
    <div class="nav-genre">
      <a href="#">Genre <svg viewBox="0 0 24 24" fill="currentColor" width="10" height="10"><path d="M7 10l5 5 5-5z"/></svg></a>
      <div class="genre-dropdown">
        <a href="#">Action</a><a href="#">Adventure</a><a href="#">Comedy</a><a href="#">Drama</a>
        <a href="#">Ecchi</a><a href="#">Fantasy</a><a href="#">Harem</a><a href="#">Horror</a>
        <a href="#">Isekai</a><a href="#">Josei</a><a href="#">Magic</a><a href="#">Mecha</a>
        <a href="#">Military</a><a href="#">Music</a><a href="#">Mystery</a><a href="#">Parody</a>
        <a href="#">Psychological</a><a href="#">Romance</a><a href="#">Sci-Fi</a><a href="#">Seinen</a>
        <a href="#">Shoujo</a><a href="#">Shounen</a><a href="#">Slice of Life</a><a href="#">Sports</a>
        <a href="#">Super Power</a><a href="#">Supernatural</a><a href="#">Thriller</a><a href="#">Vampire</a>
      </div>
    </div>
    <a href="#">Schedule</a>
    <a href="#" onclick="showPage('admin');return false;">🎬 Post Stream</a>
  </div>
</nav>

<!-- ════ PAGE: HOME ════ -->
<div class="page active" id="page-home">
  <div class="page-wrapper">
    <main>
      <!-- Hero -->
      <div class="hero-slider" id="heroSlider">
        <div class="hero-empty" id="heroEmpty">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M18 4l2 4h-3l-2-4h-2l2 4h-3l-2-4H8l2 4H7L5 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V4h-4z"/></svg>
          <p>No streams posted yet.</p>
          <span onclick="showPage('admin')">➕ Post your first stream →</span>
        </div>
        <div id="slidesContainer"></div>
        <div class="slider-dots" id="sliderDots"></div>
      </div>

      <!-- Recently Updated -->
      <div class="section-header">
        <div class="section-title">Recently Updated</div>
        <a href="#" class="view-all">View All →</a>
      </div>
      <div class="anime-grid" id="recentGrid"></div>

      <!-- Tabs -->
      <div class="tab-bar">
        <div class="tab active" onclick="switchTab(this,'tab-trending')">Trending</div>
        <div class="tab" onclick="switchTab(this,'tab-popular')">Popular</div>
        <div class="tab" onclick="switchTab(this,'tab-movies')">Movies</div>
        <div class="tab" onclick="switchTab(this,'tab-completed')">Completed</div>
      </div>
      <div id="tab-trending"><div class="anime-grid" id="trendingGrid"></div></div>
      <div id="tab-popular" style="display:none"><div class="anime-grid" id="popularGrid"></div></div>
      <div id="tab-movies" style="display:none"><div class="anime-grid" id="moviesGrid"></div></div>
      <div id="tab-completed" style="display:none"><div class="anime-grid" id="completedGrid"></div></div>

      <!-- Schedule -->
      <div class="section-header" style="margin-top:8px;">
        <div class="section-title">Weekly Schedule</div>
        <a href="#" class="view-all">Full Schedule →</a>
      </div>
      <div class="schedule-grid">
        <div><div class="day-label">Mon</div></div>
        <div><div class="day-label">Tue</div></div>
        <div><div class="day-label">Wed</div></div>
        <div><div class="day-label" style="background:var(--accent);color:#fff;">Thu ★</div></div>
        <div><div class="day-label">Fri</div></div>
        <div><div class="day-label">Sat</div></div>
        <div><div class="day-label">Sun</div></div>
      </div>
    </main>

    <aside>
      <div class="sidebar-box">
        <div class="sidebar-box-header">
          <svg viewBox="0 0 24 24"><path d="M17.657 18.657A8 8 0 0 1 4 12c0-2.21.9-4.21 2.343-5.657L12 12l5.657 6.657z"/></svg>Top Airing
        </div>
        <div class="trending-list" id="topAiringList"><div class="sidebar-empty">No streams yet.</div></div>
      </div>
      <div class="sidebar-box">
        <div class="sidebar-box-header"><svg viewBox="0 0 24 24"><path d="M4 6h16M4 12h16M4 18h16"/></svg>Genres</div>
        <div class="genre-tags">
          <span class="genre-tag">Action</span><span class="genre-tag">Adventure</span><span class="genre-tag">Comedy</span><span class="genre-tag">Drama</span>
          <span class="genre-tag">Fantasy</span><span class="genre-tag">Horror</span><span class="genre-tag">Isekai</span><span class="genre-tag">Magic</span>
          <span class="genre-tag">Mecha</span><span class="genre-tag">Mystery</span><span class="genre-tag">Romance</span><span class="genre-tag">Sci-Fi</span>
          <span class="genre-tag">Shounen</span><span class="genre-tag">Supernatural</span><span class="genre-tag">Thriller</span>
        </div>
      </div>
      <div class="sidebar-box">
        <div class="sidebar-box-header"><svg viewBox="0 0 24 24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>Recently Added</div>
        <div class="recent-list" id="recentSidebar"><div class="sidebar-empty">Nothing here yet.</div></div>
      </div>
    </aside>
  </div>

  <footer>
    <div class="footer-inner">
      <div class="footer-top">
        <div>
          <div class="footer-logo">9<span>ANIME</span></div>
          <p class="footer-desc">Watch anime online free in HD quality. Latest episodes and movies updated daily. The best anime streaming site.</p>
        </div>
        <div class="footer-col"><h4>Anime</h4><ul><li><a href="#">New Season</a></li><li><a href="#">Movies</a></li><li><a href="#">OVA</a></li><li><a href="#">TV Series</a></li></ul></div>
        <div class="footer-col"><h4>Community</h4><ul><li><a href="#">Forum</a></li><li><a href="#">Discord</a></li><li><a href="#">Request Anime</a></li></ul></div>
        <div class="footer-col"><h4>Info</h4><ul><li><a href="#">About Us</a></li><li><a href="#">DMCA</a></li><li><a href="#">Privacy Policy</a></li><li><a href="#">Contact</a></li></ul></div>
      </div>
      <div class="footer-bottom">
        <div class="footer-copy">© 2024 9Anime — Watch Anime Online. All Rights Reserved.</div>
        <div class="footer-links"><a href="#">Home</a><a href="#">Privacy</a><a href="#">DMCA</a><a href="#">Contact</a></div>
      </div>
    </div>
  </footer>
</div>

<!-- ════ PAGE: WATCH ════ -->
<div class="page" id="page-watch">
  <div class="back-btn" onclick="showPage('home')">← Back to Home</div>
  <div class="watch-wrapper">
    <div>
      <div class="breadcrumb"><a onclick="showPage('home')">Home</a> › <span id="wBreadcrumb">Watch</span></div>
      <div class="player-box" id="playerBox">
        <div class="player-loading"><svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg><p>Loading player...</p></div>
      </div>
      <div class="server-bar">
        <span class="server-label">Servers:</span>
        <button class="server-btn active" onclick="swServer(this)">▶ Server 1</button>
        <button class="server-btn" onclick="swServer(this)">▶ Server 2</button>
        <button class="server-btn" onclick="swServer(this)">▶ Server 3</button>
      </div>
      <div class="ep-list-box">
        <div class="ep-list-header">
          <span>Episodes</span>
          <span id="epCountLabel" style="font-size:11px;color:var(--text-muted);"></span>
        </div>
        <div class="ep-list-body" id="epListBody"></div>
      </div>
      <div class="watch-info">
        <div class="watch-badges" id="wBadges"></div>
        <div class="watch-title" id="wTitle"></div>
        <div class="watch-meta-row" id="wMeta"></div>
        <div class="watch-desc" id="wDesc"></div>
      </div>
    </div>
    <div>
      <div class="sidebar-box">
        <div class="sidebar-box-header"><svg viewBox="0 0 24 24" style="fill:var(--accent)"><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>More Streams</div>
        <div class="related-list" id="relatedList"></div>
      </div>
    </div>
  </div>
</div>

<!-- ════ PAGE: ADMIN ════ -->
<div class="page" id="page-admin">
  <div class="back-btn" onclick="showPage('home')">← Back to Home</div>
  <div class="admin-wrapper">
    <div class="admin-header">
      <div class="admin-title">
        <svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 14.5v-9l6 4.5-6 4.5z"/></svg>
        Admin Panel — Streaming Manager
      </div>
      <div style="font-size:12px;color:var(--accent-green);">🟢 Live</div>
    </div>

    <div class="admin-stats">
      <div class="stat-card"><div class="stat-num" id="sTot">0</div><div class="stat-label">Total Streams</div></div>
      <div class="stat-card" style="border-color:var(--accent-orange)"><div class="stat-num" style="color:var(--accent-orange)" id="sOng">0</div><div class="stat-label">Ongoing</div></div>
      <div class="stat-card" style="border-color:var(--accent-blue)"><div class="stat-num" style="color:var(--accent-blue)" id="sMov">0</div><div class="stat-label">Movies</div></div>
      <div class="stat-card" style="border-color:var(--accent-green)"><div class="stat-num" style="color:var(--accent-green)" id="sCom">0</div><div class="stat-label">Completed</div></div>
    </div>

    <div class="admin-grid">
      <!-- FORM -->
      <div class="form-box">
        <div class="form-box-header">
          <svg viewBox="0 0 24 24"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
          <span id="formHeading">Post New Stream</span>
        </div>
        <div class="form-body">
          <input type="hidden" id="editId">

          <div class="form-group">
            <label>Anime Title *</label>
            <input type="text" id="fTitle" placeholder="e.g. Demon Slayer Season 3">
          </div>

          <div class="form-group">
            <label>Thumbnail Image URL</label>
            <input type="text" id="fThumb" placeholder="https://... (optional — emoji used if blank)">
            <div class="input-hint">Paste a direct image URL. Leave blank for auto emoji.</div>
          </div>

          <div class="form-group">
            <label>Video / Stream URL *</label>
            <input type="text" id="fVideo" placeholder="YouTube link, iframe URL, or direct .mp4">
            <div class="input-hint">✅ Supports YouTube links, any iframe-embed URL, or direct .mp4/.webm</div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label>Type</label>
              <select id="fType"><option>TV</option><option>Movie</option><option>OVA</option><option>ONA</option><option>Special</option></select>
            </div>
            <div class="form-group">
              <label>Status</label>
              <select id="fStatus"><option>Ongoing</option><option>Completed</option><option>Upcoming</option></select>
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label>Episodes</label>
              <input type="number" id="fEps" placeholder="e.g. 12" min="1">
            </div>
            <div class="form-group">
              <label>Year</label>
              <input type="number" id="fYear" placeholder="e.g. 2024">
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label>Audio</label>
              <select id="fAudio"><option>SUB</option><option>DUB</option><option value="SUB+DUB">SUB + DUB</option></select>
            </div>
            <div class="form-group">
              <label>Genre Tags</label>
              <input type="text" id="fGenre" placeholder="Action, Fantasy...">
            </div>
          </div>

          <div class="form-group">
            <label>Description / Synopsis</label>
            <textarea id="fDesc" placeholder="Brief synopsis of the anime..."></textarea>
          </div>

          <button class="btn-submit" onclick="submitStream()">
            <svg viewBox="0 0 24 24" fill="#fff" width="14" height="14"><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
            <span id="submitLabel">Post Stream</span>
          </button>
          <div style="text-align:center;margin-top:10px;">
            <span id="cancelEditBtn" style="display:none;font-size:12px;color:var(--text-muted);cursor:pointer;" onclick="cancelEdit()">✕ Cancel Edit</span>
          </div>
        </div>
      </div>

      <!-- POSTED LIST -->
      <div class="posted-box">
        <div class="posted-list-header">
          <svg viewBox="0 0 24 24" style="width:16px;height:16px;fill:var(--accent)"><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>
          <span>Posted Streams</span>
        </div>
        <div id="postedList"><div class="posted-empty">No streams yet. Use the form to post one!</div></div>
      </div>
    </div>
  </div>
</div>

<script>
const KEY = '9anime_data';
const EMOJIS = ['🌸','⚔️','🔥','🌊','⚡','🌙','🎭','🧿','🐲','🌺','💥','🦋','🌀','🎯','🏮','🗡️','🌟','🔮','🐉','🎌'];

const getStreams = () => { try{ return JSON.parse(localStorage.getItem(KEY))||[]; }catch(e){ return []; } };
const saveStreams = d => localStorage.setItem(KEY, JSON.stringify(d));
const emoji = i => EMOJIS[Math.abs(i) % EMOJIS.length];

// ── PAGE NAV ──
function showPage(name){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.getElementById('page-'+name).classList.add('active');
  window.scrollTo(0,0);
  if(name==='home') renderHome();
  if(name==='admin') renderAdmin();
}

// ── TABS ──
function switchTab(el, id){
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  ['tab-trending','tab-popular','tab-movies','tab-completed'].forEach(t=>document.getElementById(t).style.display='none');
  document.getElementById(id).style.display='block';
}

// ── BUILD CARD ──
function card(s, i){
  const ab = s.audio==='SUB+DUB'?`<span class="badge badge-sub">SUB</span><span class="badge badge-dub">DUB</span>`:
             s.audio==='DUB'?`<span class="badge badge-dub">DUB</span>`:`<span class="badge badge-sub">SUB</span>`;
  const thumb = s.thumb
    ? `<img src="${s.thumb}" alt="${s.title}" onerror="this.parentElement.innerHTML='<div class=\\'thumb-placeholder\\'>${emoji(i)}</div>'">`
    : `<div class="thumb-placeholder">${emoji(i)}</div>`;
  return `<div class="anime-card" onclick="openWatch('${s.id}')">
    <div class="anime-thumb">
      ${thumb}
      <div class="anime-thumb-overlay"><div class="play-icon"><svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg></div></div>
      <div class="thumb-badges">${ab}<span class="badge badge-tv">${s.type||'TV'}</span></div>
      <div class="ep-count${s.status==='Ongoing'?' new-ep':''}">${s.type==='Movie'?'Movie':'EP '+(s.eps||'?')}</div>
    </div>
    <div class="anime-name">${s.title}</div>
    <div class="anime-type">${s.type||'TV'}${s.status?' • '+s.status:''}</div>
  </div>`;
}

function emptyGrid(msg, hint){
  return `<div class="empty-state">
    <svg viewBox="0 0 24 24" fill="currentColor"><path d="M18 4l2 4h-3l-2-4h-2l2 4h-3l-2-4H8l2 4H7L5 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V4h-4z"/></svg>
    <p>${msg}</p>${hint?`<div class="add-hint" onclick="showPage('admin')">${hint}</div>`:''}
  </div>`;
}

function fillGrid(id, list, emptyMsg, hint){
  const el = document.getElementById(id);
  el.innerHTML = list.length ? list.map((s,i)=>card(s,i)).join('') : emptyGrid(emptyMsg, hint);
}

// ── RENDER HOME ──
let slideTimer=null, curSlide=0, totalSlides=0;

function renderHome(){
  const all = getStreams();

  // Hero
  const heroEmpty = document.getElementById('heroEmpty');
  const sc = document.getElementById('slidesContainer');
  const sd = document.getElementById('sliderDots');
  sc.innerHTML=''; sd.innerHTML='';
  if(!all.length){
    heroEmpty.style.display='block';
  } else {
    heroEmpty.style.display='none';
    const feat = all.slice(-5).reverse();
    feat.forEach((s,i)=>{
      const bgStyle = s.thumb
        ? `background:url('${s.thumb}') center/cover no-repeat;filter:brightness(.38);`
        : `background:linear-gradient(135deg,hsl(${(i*47)%360},40%,12%),hsl(${(i*47+60)%360},35%,18%));`;
      const ab = s.audio==='SUB+DUB'?`<span class="badge badge-sub">SUB</span><span class="badge badge-dub">DUB</span>`:
                 s.audio==='DUB'?`<span class="badge badge-dub">DUB</span>`:`<span class="badge badge-sub">SUB</span>`;
      sc.innerHTML += `<div class="slide${i===0?' active':''}" id="slide-${i}">
        <div class="slide-bg-div" style="${bgStyle}"></div>
        <div class="slide-content">
          <div class="slide-badges">${ab}<span class="badge badge-new">NEW</span><span class="badge badge-tv">${s.type||'TV'}</span></div>
          <div class="slide-title">${s.title}</div>
          <div class="slide-meta"><span>📺 Eps: ${s.eps||'?'}</span><span>🎬 ${s.type||'TV'}</span><span>📅 ${s.year||'2024'}</span><span>🏷 ${s.status||'Ongoing'}</span></div>
          <div class="slide-desc">${s.desc||'No description available.'}</div>
          <div class="slide-actions">
            <button class="btn-watch" onclick="openWatch('${s.id}')">▶ Watch Now</button>
            <button class="btn-detail" onclick="openWatch('${s.id}')">Detail</button>
          </div>
        </div>
      </div>`;
      sd.innerHTML += `<div class="dot${i===0?' active':''}" onclick="goSlide(${i})"></div>`;
    });
    if(slideTimer) clearInterval(slideTimer);
    curSlide=0; totalSlides=feat.length;
    if(totalSlides>1) slideTimer = setInterval(()=>goSlide((curSlide+1)%totalSlides),4800);
  }

  // Grids
  fillGrid('recentGrid', [...all].reverse().slice(0,6), 'No streams yet.', '➕ Post via Admin Panel');
  fillGrid('trendingGrid', all.slice(0,6), 'No streams yet.', '➕ Post via Admin Panel');
  fillGrid('popularGrid', [...all].sort((a,b)=>a.title.localeCompare(b.title)).slice(0,6), 'No streams yet.');
  fillGrid('moviesGrid', all.filter(s=>s.type==='Movie').slice(0,6), 'No movies added yet.');
  fillGrid('completedGrid', all.filter(s=>s.status==='Completed').slice(0,6), 'No completed series yet.');

  // Top Airing sidebar
  const tal = document.getElementById('topAiringList');
  tal.innerHTML = all.length ? all.slice(0,8).map((s,i)=>`
    <div class="trending-item" onclick="openWatch('${s.id}')">
      <div class="rank-num${i<3?' top3':''}">${i+1}</div>
      <div class="t-thumb">${s.thumb?`<img src="${s.thumb}">`:emoji(i)}</div>
      <div class="trending-info">
        <div class="trending-name">${s.title}</div>
        <div class="trending-meta">EP ${s.eps||'?'} • ${s.audio||'SUB'}</div>
      </div>
    </div>`).join('')
  : '<div class="sidebar-empty">No streams posted yet.</div>';

  // Recent sidebar
  const rs = document.getElementById('recentSidebar');
  rs.innerHTML = all.length ? [...all].reverse().slice(0,4).map((s,i)=>`
    <div class="recent-item" onclick="openWatch('${s.id}')">
      <div class="r-thumb">${s.thumb?`<img src="${s.thumb}">`:emoji(i)}</div>
      <div class="recent-info">
        <div class="recent-name">${s.title}</div>
        <div class="recent-ep">Ep <strong>${s.eps||'?'}</strong> • ${s.status||'Ongoing'}</div>
      </div>
    </div>`).join('')
  : '<div class="sidebar-empty">Nothing here yet.</div>';
}

function goSlide(n){
  document.querySelectorAll('.slide').forEach((s,i)=>s.classList.toggle('active',i===n));
  document.querySelectorAll('.dot').forEach((d,i)=>d.classList.toggle('active',i===n));
  curSlide=n;
}

// ── WATCH PAGE ──
function openWatch(id){
  const all = getStreams();
  const s = all.find(x=>x.id===id);
  if(!s) return;

  document.getElementById('wBreadcrumb').textContent = s.title;
  document.getElementById('wTitle').textContent = s.title;

  const ab = s.audio==='SUB+DUB'?`<span class="badge badge-sub">SUB</span><span class="badge badge-dub">DUB</span>`:
             s.audio==='DUB'?`<span class="badge badge-dub">DUB</span>`:`<span class="badge badge-sub">SUB</span>`;
  document.getElementById('wBadges').innerHTML=`${ab}<span class="badge badge-tv">${s.type||'TV'}</span><span class="badge badge-new">${s.status||'Ongoing'}</span>`;
  document.getElementById('wMeta').innerHTML=`
    <div class="watch-meta-item">🎬 <strong>Type:</strong> ${s.type||'TV'}</div>
    <div class="watch-meta-item">📺 <strong>Episodes:</strong> ${s.eps||'?'}</div>
    <div class="watch-meta-item">📅 <strong>Year:</strong> ${s.year||'2024'}</div>
    <div class="watch-meta-item">🏷 <strong>Genre:</strong> ${s.genre||'—'}</div>
    <div class="watch-meta-item">🔊 <strong>Audio:</strong> ${s.audio||'SUB'}</div>`;
  document.getElementById('wDesc').textContent = s.desc||'No description available.';

  // Player
  const box = document.getElementById('playerBox');
  if(!s.video){
    box.innerHTML=`<div class="player-loading"><svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"/></svg><p>No video URL provided.</p></div>`;
  } else {
    let url = s.video;
    const yt = url.match(/(?:youtube\.com\/watch\?v=|youtu\.be\/)([a-zA-Z0-9_-]{11})/);
    if(yt) url=`https://www.youtube.com/embed/${yt[1]}?rel=0`;
    if(/\.(mp4|webm|ogg)$/i.test(url)){
      box.innerHTML=`<video controls src="${url}" style="width:100%;aspect-ratio:16/9;display:block;"></video>`;
    } else {
      box.innerHTML=`<iframe src="${url}" style="width:100%;aspect-ratio:16/9;display:block;" frameborder="0" allowfullscreen allow="autoplay;encrypted-media;picture-in-picture"></iframe>`;
    }
  }

  // Episodes
  const epCount = Math.min(parseInt(s.eps)||1, 200);
  document.getElementById('epCountLabel').textContent=`${epCount} Episode${epCount!==1?'s':''}`;
  document.getElementById('epListBody').innerHTML = Array.from({length:epCount},(_,i)=>
    `<button class="ep-btn${i===0?' active':''}" onclick="pickEp(this,${i+1})">${i+1}</button>`).join('');

  // Related
  const rel = all.filter(x=>x.id!==id).slice(0,8);
  document.getElementById('relatedList').innerHTML = rel.length ? rel.map((r,i)=>`
    <div class="related-item" onclick="openWatch('${r.id}')">
      <div class="rel-thumb">${r.thumb?`<img src="${r.thumb}">`:emoji(i)}</div>
      <div class="related-info">
        <div class="related-name">${r.title}</div>
        <div class="related-meta">${r.type||'TV'} • ${r.status||'Ongoing'}</div>
      </div>
    </div>`).join('')
  : '<div style="padding:16px;text-align:center;font-size:12px;color:var(--text-muted);">No other streams yet.</div>';

  showPage('watch');
}

function pickEp(btn, n){
  document.querySelectorAll('.ep-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  toast(`▶ Playing Episode ${n}`);
}
function swServer(btn){
  document.querySelectorAll('.server-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  toast(`Switched to ${btn.textContent.trim()}`);
}

// ── SEARCH ──
function liveSearch(q){
  if(!q.trim()) return;
  const all = getStreams();
  const r = all.filter(s=>s.title.toLowerCase().includes(q.toLowerCase()));
  const el = document.getElementById('recentGrid');
  el.innerHTML = r.length
    ? r.map((s,i)=>card(s,i)).join('')
    : `<div class="empty-state"><p>No results for "<strong>${q}</strong>"</p><div class="add-hint" onclick="clearSearch()">✕ Clear</div></div>`;
}
function clearSearch(){ document.getElementById('searchInput').value=''; renderHome(); }

// ── ADMIN ──
function renderAdmin(){
  const all = getStreams();
  document.getElementById('sTot').textContent=all.length;
  document.getElementById('sOng').textContent=all.filter(s=>s.status==='Ongoing').length;
  document.getElementById('sMov').textContent=all.filter(s=>s.type==='Movie').length;
  document.getElementById('sCom').textContent=all.filter(s=>s.status==='Completed').length;

  const pl = document.getElementById('postedList');
  if(!all.length){ pl.innerHTML='<div class="posted-empty">No streams posted yet. Use the form to add one!</div>'; return; }
  pl.innerHTML = [...all].reverse().map((s,i)=>`
    <div class="posted-item">
      <div class="p-thumb">${s.thumb?`<img src="${s.thumb}">`:emoji(i)}</div>
      <div class="posted-info">
        <div class="posted-name">${s.title}</div>
        <div class="posted-sub">${s.type||'TV'} • ${s.status||'Ongoing'} • ${s.audio||'SUB'} • EP ${s.eps||'?'} • ${s.year||'—'}</div>
      </div>
      <div class="posted-actions">
        <button class="btn-icon" onclick="openWatch('${s.id}')">▶</button>
        <button class="btn-icon" onclick="editStream('${s.id}')">✏</button>
        <button class="btn-icon del" onclick="askDelete('${s.id}')">🗑</button>
      </div>
    </div>`).join('');
}

function submitStream(){
  const title = document.getElementById('fTitle').value.trim();
  const video = document.getElementById('fVideo').value.trim();
  if(!title){ toast('⚠️ Title is required!', true); return; }
  if(!video){ toast('⚠️ Video URL is required!', true); return; }

  const eid = document.getElementById('editId').value;
  const all = getStreams();
  const obj = {
    id: eid||Date.now().toString(36)+Math.random().toString(36).slice(2,6),
    title, video,
    thumb: document.getElementById('fThumb').value.trim(),
    type: document.getElementById('fType').value,
    status: document.getElementById('fStatus').value,
    eps: document.getElementById('fEps').value,
    year: document.getElementById('fYear').value,
    audio: document.getElementById('fAudio').value,
    genre: document.getElementById('fGenre').value.trim(),
    desc: document.getElementById('fDesc').value.trim(),
    at: eid?(all.find(s=>s.id===eid)||{}).at||Date.now():Date.now()
  };

  if(eid){
    const idx=all.findIndex(s=>s.id===eid);
    if(idx>-1) all[idx]=obj; else all.push(obj);
    toast('✅ Stream updated!');
  } else {
    all.push(obj);
    toast('✅ Stream posted successfully!');
  }
  saveStreams(all);
  resetForm();
  renderAdmin();
}

function editStream(id){
  const s = getStreams().find(x=>x.id===id);
  if(!s) return;
  document.getElementById('editId').value=s.id;
  document.getElementById('fTitle').value=s.title;
  document.getElementById('fThumb').value=s.thumb||'';
  document.getElementById('fVideo').value=s.video||'';
  document.getElementById('fType').value=s.type||'TV';
  document.getElementById('fStatus').value=s.status||'Ongoing';
  document.getElementById('fEps').value=s.eps||'';
  document.getElementById('fYear').value=s.year||'';
  document.getElementById('fAudio').value=s.audio||'SUB';
  document.getElementById('fGenre').value=s.genre||'';
  document.getElementById('fDesc').value=s.desc||'';
  document.getElementById('formHeading').textContent='Edit Stream';
  document.getElementById('submitLabel').textContent='Update Stream';
  document.getElementById('cancelEditBtn').style.display='inline';
  document.querySelector('.form-box').scrollIntoView({behavior:'smooth'});
}

function cancelEdit(){ resetForm(); toast('Edit cancelled.'); }

function resetForm(){
  document.getElementById('editId').value='';
  ['fTitle','fThumb','fVideo','fEps','fYear','fGenre','fDesc'].forEach(id=>document.getElementById(id).value='');
  document.getElementById('fType').value='TV';
  document.getElementById('fStatus').value='Ongoing';
  document.getElementById('fAudio').value='SUB';
  document.getElementById('formHeading').textContent='Post New Stream';
  document.getElementById('submitLabel').textContent='Post Stream';
  document.getElementById('cancelEditBtn').style.display='none';
}

// Delete
let delTarget=null;
function askDelete(id){ delTarget=id; document.getElementById('deleteModal').classList.add('show'); }
function closeDelModal(){ delTarget=null; document.getElementById('deleteModal').classList.remove('show'); }
function confirmDelete(){
  if(!delTarget) return;
  saveStreams(getStreams().filter(s=>s.id!==delTarget));
  closeDelModal(); toast('🗑 Stream deleted.'); renderAdmin();
}

// Toast
let toastT;
function toast(msg, warn=false){
  const el=document.getElementById('toast');
  document.getElementById('toastMsg').textContent=msg;
  el.style.borderLeftColor=warn?'var(--accent-orange)':'var(--accent-green)';
  el.classList.add('show');
  clearTimeout(toastT);
  toastT=setTimeout(()=>el.classList.remove('show'),2800);
}

// Init
renderHome();
</script>
</body>
</html>
