<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, minimum-scale=1, user-scalable=no, viewport-fit=cover">
<meta name="theme-color" content="#F5F6FA">
<title>Learnify — Study Platform</title>
<link rel="preconnect" href="https://i.ytimg.com" crossorigin>
<link rel="preconnect" href="https://i9.ytimg.com" crossorigin>
<link rel="preconnect" href="https://www.youtube-nocookie.com" crossorigin>
<link rel="preconnect" href="https://www.youtube.com">
<link rel="preconnect" href="https://www.instagram.com">
<link rel="preconnect" href="https://scontent.cdninstagram.com">
<link rel="preconnect" href="https://googlevideo.com" crossorigin>
<link rel="preconnect" href="https://www.gstatic.com" crossorigin>
<link rel="dns-prefetch" href="https://player.vimeo.com">
<link rel="dns-prefetch" href="https://firebasestorage.googleapis.com">
<link rel="dns-prefetch" href="https://i.ytimg.com">
<script>
(function(){
  var nav = navigator;
  var lowEnd = (nav.hardwareConcurrency && nav.hardwareConcurrency <= 4) ||
               (nav.deviceMemory && nav.deviceMemory <= 4) ||
               /Android|iPhone|iPad|iPod/i.test(nav.userAgent);
  window.__LOW_END = lowEnd;
  window.__t0 = performance.now();
  var opts = {passive:true, capture:true};
  document.addEventListener('touchstart', function(){}, opts);
  document.addEventListener('touchmove',  function(){}, opts);
  document.addEventListener('wheel',      function(){}, opts);
  if(lowEnd){
    var r = document.documentElement.style;
    r.setProperty('--ease','ease-out');
    r.setProperty('--spring','ease-out');
    r.setProperty('--nav-shadow','0 6px 18px rgba(16,18,28,.14)');
  }
  requestAnimationFrame(function(){ window.__firstPaint = performance.now() - window.__t0; });
})();
</script>
<style>
html,body{
  -webkit-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;
  touch-action:manipulation;
  -webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;
  -webkit-touch-callout:none;-webkit-tap-highlight-color:transparent;
}
input,textarea{-webkit-user-select:text;-moz-user-select:text;-ms-user-select:text;user-select:text;-webkit-touch-callout:default;}
img,video,svg,canvas{
  -webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;
  -webkit-touch-callout:none;-webkit-user-select:none;user-select:none;
}
.art-img,.app-ico img,.hero-media img{pointer-events:none;}

.shorts-item .play-icon,
.channel-short-play {
  display: none !important;
}

/* FORCE HIDE NATIVE VIDEO CONTROLS (PLAY/PAUSE BUTTON) */
.short-reel-media video::-webkit-media-controls,
.short-reel-media video::-webkit-media-controls-enclosure,
.short-reel-media video::-webkit-media-controls-panel,
.short-reel-media video::-webkit-media-controls-play-button,
.short-reel-media video::-webkit-media-controls-start-playback-button,
.short-reel-media video::-webkit-media-controls-overlay-play-button {
  display: none !important;
  -webkit-appearance: none !important;
  opacity: 0 !important;
  pointer-events: none !important;
  width: 0 !important;
  height: 0 !important;
}

:root{
  --bg:#F5F6FA; --surface:#FFFFFF; --surface-2:#EFF1F7;
  --ink:#0E1016; --ink-2:#3A3F4B; --muted:#7A8194; --line:#E7E9F0;
  --brand:#5B4CF0; --brand-2:#7C6BFF; --brand-soft:#EEECFE;
  --gold:#C9821C; --gold-soft:#FDF4E6;
  --green:#0F9D58; --green-soft:#E7F7EF;
  --red:#E5484D; --red-soft:#FDECEC;

  --nav-bg: rgba(255,255,255,.70);
  --nav-border: rgba(255,255,255,.75);
  --nav-text: #8A90A2;
  --nav-active: #5B4CF0;
  --nav-shadow: 0 14px 34px rgba(16,18,28,.16), 0 2px 8px rgba(16,18,28,.05);
  --glass-bg: rgba(255,255,255,.72);
  --glass-border: rgba(255,255,255,.55);
  --soft-white: rgba(255,255,255,.92);
  --soft-white-2: rgba(255,255,255,.85);
  --float-bg: rgba(255,255,255,.92);
  --float-border: rgba(255,255,255,.75);
  --search-bg: #FFFFFF;
  --search-border: #E7E9F0;
  --search-text: #0E1016;
  --search-placeholder: #A6ACBD;
  --shorts-chip-bg: rgba(255,255,255,.92);
  --shorts-chip-text: #0E1016;
  --shorts-play-bg: rgba(255,255,255,.85);
  --thumb-play-bg: rgba(255,255,255,.92);

  --r-xs:8px; --r-sm:12px; --r-md:16px; --r-lg:22px; --r-xl:28px; --r-full:999px;
  --sh-1:0 1px 2px rgba(16,18,28,.05), 0 1px 3px rgba(16,18,28,.04);
  --sh-2:0 4px 18px rgba(16,18,28,.08);
  --sh-3:0 14px 38px rgba(16,18,28,.16);
  --ease:cubic-bezier(.22,.9,.3,1);
  --spring:cubic-bezier(.34,1.4,.64,1);
}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html,body{margin:0;padding:0;height:100%;width:100%}
body{
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Inter,Roboto,"Helvetica Neue",Arial,sans-serif;
  background:#0A0B10;color:var(--ink);
  display:flex;align-items:center;justify-content:center;
  min-height:100vh;min-height:100dvh;
  overflow:hidden;
  -webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;
}
body::before{
  content:"";position:fixed;inset:0;pointer-events:none;z-index:0;
  background:
    radial-gradient(58% 46% at 12% 6%, rgba(91,76,240,.30), transparent 62%),
    radial-gradient(48% 42% at 88% 88%, rgba(201,130,28,.16), transparent 62%),
    radial-gradient(42% 40% at 76% 10%, rgba(16,157,88,.10), transparent 62%);
}
button{font:inherit;color:inherit}
img{max-width:100%}
::-webkit-scrollbar{width:0;height:0}

.app{
  position:relative;z-index:1;
  width:100%;max-width:430px;
  height:100vh;height:100dvh;
  background:var(--bg);display:flex;flex-direction:column;
  overflow:hidden;
  background-size:cover;background-position:center center;background-repeat:no-repeat;
}
@media(min-width:520px){
  .app{height:min(880px,94vh);height:min(880px,94dvh);border-radius:42px;
    box-shadow:0 0 0 9px #15161d, 0 0 0 11px #262833, 0 40px 90px rgba(0,0,0,.65);}
}
@media(min-width:900px){ .app{max-width:452px} }
.screens{position:relative;flex:1;overflow:hidden}
.screen{
  position:absolute;inset:0;
  overflow-y:auto;overflow-x:hidden;
  overscroll-behavior:contain;display:none;
  padding-bottom:118px;-webkit-overflow-scrolling:touch;
  transform:translateZ(0);backface-visibility:hidden;
}
.screen.active{display:block;animation:screenInFast .14s ease-out}
@keyframes screenInFast{from{opacity:.4}to{opacity:1}}
#s-ai.active{display:flex;flex-direction:column;overflow:hidden;padding-bottom:0}
#s-playlist.active{padding-bottom:0}

h1,h2,h3,h4{margin:0;letter-spacing:-.022em;line-height:1.25}
.h1{font-size:26px;font-weight:800}
.h2{font-size:19px;font-weight:800}
.sec-title{font-size:16.5px;font-weight:750;letter-spacing:-.025em}
.sec-link{font-size:12.5px;font-weight:650;color:var(--brand);background:none;border:0;padding:0;cursor:pointer}
.meta{font-size:12px;color:var(--muted);font-weight:500}
.sub{font-size:13.5px;color:var(--muted);line-height:1.5}

.float-back{
  position:absolute;top:calc(14px + env(safe-area-inset-top));left:14px;z-index:90;
  width:42px;height:42px;border-radius:50%;
  background:var(--float-bg);
  -webkit-backdrop-filter:blur(10px) saturate(140%);backdrop-filter:blur(10px) saturate(140%);
  border:1px solid var(--float-border);
  box-shadow:0 8px 22px rgba(16,18,28,.18), 0 2px 6px rgba(16,18,28,.08);
  display:grid;place-items:center;color:var(--ink-2);cursor:pointer;
  transition:transform .14s var(--ease);
}
.float-back:active{transform:scale(.9)}
.float-back svg{width:20px;height:20px}

.icon-btn{
  width:40px;height:40px;flex:0 0 auto;border-radius:14px;border:1px solid var(--line);
  background:var(--surface);display:grid;place-items:center;cursor:pointer;
  color:var(--ink-2);transition:transform .14s var(--ease),background .14s,box-shadow .14s;
  box-shadow:var(--sh-1);
}
.icon-btn:active{transform:scale(.92)}
.icon-btn svg{width:20px;height:20px}
.icon-btn.glass{
  background:var(--glass-bg);border:1px solid var(--glass-border);
  -webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);
  color:#fff;box-shadow:0 4px 14px rgba(0,0,0,.18);
}

.btn{
  display:inline-flex;align-items:center;justify-content:center;gap:8px;
  height:48px;padding:0 22px;border-radius:var(--r-full);border:0;
  font-weight:700;font-size:14.5px;letter-spacing:-.01em;cursor:pointer;
  transition:transform .14s var(--ease),box-shadow .18s,background .18s,opacity .18s;white-space:nowrap;
}
.btn:active{transform:scale(.965)}
.btn svg{width:18px;height:18px;flex:0 0 auto}
.btn-primary{background:var(--brand);color:#fff;box-shadow:0 8px 22px rgba(91,76,240,.32)}
.btn-secondary{background:var(--surface);color:var(--ink);border:1px solid var(--line);box-shadow:var(--sh-1)}
.btn-ghost{background:transparent;color:var(--brand);padding:0 12px}
.btn-danger{background:var(--red-soft);color:var(--red)}
.btn-gold{background:linear-gradient(135deg,#F0B84A,#D8871E);color:#2B1A00;box-shadow:0 8px 22px rgba(216,135,30,.32)}
.btn-sm{height:38px;padding:0 16px;font-size:13px;border-radius:var(--r-full)}
.btn-sm svg{width:16px;height:16px}
.btn-lg{height:54px;font-size:15.5px}
.btn-block{width:100%}
.btn:disabled{opacity:.55;pointer-events:none}

.badge{
  display:inline-flex;align-items:center;gap:4px;height:21px;padding:0 8px;
  border-radius:999px;font-size:9.5px;font-weight:850;letter-spacing:.055em;
  text-transform:uppercase;white-space:nowrap;
}
.badge.premium{background:linear-gradient(135deg,#F5C55C,#DD8E1E);color:#2E1C00}
.badge.unlocked{background:var(--green-soft);color:var(--green)}
.badge.featured{background:var(--brand-soft);color:#4A3BE0}
.on-art{position:absolute;top:8px;left:8px;z-index:3;box-shadow:0 2px 8px rgba(0,0,0,.18)}

.art{position:relative;border-radius:16px;overflow:hidden;background:#2B3550;isolation:isolate;}
.art::before{content:"";position:absolute;inset:0;z-index:1;background:linear-gradient(180deg,rgba(0,0,0,.10) 0%,transparent 45%);pointer-events:none;}
.art::after{content:"";position:absolute;inset:0;z-index:2;background:linear-gradient(180deg,transparent 42%,rgba(5,6,14,.55));pointer-events:none;}
.art-img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;z-index:0;display:block;background:#1a1d29;}

.ar-169{aspect-ratio:16/9}
@supports not (aspect-ratio: 1 / 1){
  .ar-169{height:180px}
  .hero-card{height:440px}
  .player-art{height:220px}
  .pd-player-header{height:220px}
  .vcard .art.ar-169{height:105px}
}
.chip-dur{position:absolute;bottom:8px;right:8px;z-index:3;background:rgba(8,9,18,.78);color:#fff;font-size:10.5px;font-weight:700;padding:3px 7px;border-radius:7px;backdrop-filter:blur(6px);}
.play-fab{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);z-index:4;width:44px;height:44px;border-radius:50%;border:0;cursor:pointer;background:var(--soft-white);color:#111;display:grid;place-items:center;backdrop-filter:blur(8px);box-shadow:0 6px 18px rgba(0,0,0,.24);}
.play-fab svg{width:16px;height:16px;margin-left:2px}

.pad{padding:0 16px}
.sec{margin-top:24px}
.sec-head{display:flex;align-items:center;justify-content:space-between;gap:12px;padding:0 16px;margin-bottom:12px}
.hscroll{display:flex;gap:12px;overflow-x:auto;padding:2px 16px 6px;scrollbar-width:none;scroll-snap-type:x proximity;transform:translateZ(0);backface-visibility:hidden;overscroll-behavior-x:contain}
.hscroll::-webkit-scrollbar{display:none}
.hscroll>*{flex:0 0 auto;scroll-snap-align:start}

.page-title{padding:14px 16px 4px;font-size:22px;font-weight:800;letter-spacing:-.03em;}
.page-subtitle{padding:0 16px 4px;font-size:13px;color:var(--muted);font-weight:500;}

.hero{margin-top:14px;position:relative}
.hero-track{display:flex;overflow-x:auto;scroll-snap-type:x mandatory;scrollbar-width:none;-ms-overflow-style:none;transform:translateZ(0);backface-visibility:hidden}
.hero-track::-webkit-scrollbar{display:none}
.hero-slide{flex:0 0 100%;padding:0 16px;scroll-snap-align:start}
.hero-card{position:relative;border-radius:24px;overflow:hidden;isolation:isolate;box-shadow:0 16px 40px rgba(16,18,28,.22);aspect-ratio: 4/5;background:#2B3550;cursor:pointer;transition:transform .18s var(--ease);}
.hero-card:active{transform:scale(.985)}
.hero-media{position:absolute;inset:0;z-index:0;background:#2B3550}
.hero-media img{width:100%;height:100%;object-fit:cover;display:block;}
.hero-scrim{position:absolute;inset:0;z-index:2;background:linear-gradient(180deg,rgba(4,5,12,.20) 0%,rgba(4,5,12,.05) 40%,rgba(4,5,12,.72) 100%);pointer-events:none;}
.hero-body{position:absolute;left:0;right:0;bottom:0;z-index:5;padding:16px;color:#fff;pointer-events:none;}
.hero-title{font-size:20px;font-weight:800;letter-spacing:-.03em;line-height:1.2;margin:0 0 4px;text-shadow:0 1px 12px rgba(0,0,0,.45);display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.hero-desc{font-size:13px;opacity:.88;margin:0;font-weight:500;text-shadow:0 1px 8px rgba(0,0,0,.5);display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.hero-foot{display:flex;align-items:center;justify-content:center;gap:10px;margin-top:12px;position:relative;z-index:30;}
.dots{display:flex;align-items:center;gap:6px}
.dot{width:6px;height:6px;border-radius:999px;background:#C9CDDB;border:0;padding:0;cursor:pointer;transition:all .18s var(--ease);}
.dot.on{width:20px;background:var(--brand)}

.vcard{width:180px;cursor:pointer;transition:transform .14s var(--ease)}
.vcard:active{transform:scale(.975)}
.vcard h4{font-size:13.5px;font-weight:650;margin:9px 0 3px;line-height:1.32;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;}
.vcard .meta{font-size:11.5px}

.pcard{width:252px;background:var(--surface);border-radius:20px;overflow:hidden;border:1px solid var(--line);box-shadow:var(--sh-1);cursor:pointer;contain:layout style paint;}
.pcard .art{border-radius:0}
.pcard-body{padding:12px}
.pcard-body h4{font-size:14.5px;font-weight:700;margin-bottom:4px;line-height:1.3}
.pcard-foot{display:flex;align-items:center;justify-content:space-between;gap:10px}
.price{font-size:16px;font-weight:800;}

.app-ico{border-radius:16px;display:grid;place-items:center;color:#fff;font-weight:850;flex:0 0 auto;width:56px;height:56px;font-size:22px;box-shadow:none;position:relative;overflow:hidden;background:transparent;}
.app-ico.sm{width:46px;height:46px;font-size:18px;border-radius:14px}
.app-ico.lg{width:84px;height:84px;font-size:34px;border-radius:24px}
.app-ico.xl{width:96px;height:96px;font-size:38px;border-radius:26px}
.app-ico img{width:100%;height:100%;object-fit:cover;position:relative;z-index:2;border-radius:inherit;box-shadow:0 4px 12px rgba(0,0,0,.12);}
.app-ico.fallback{background:linear-gradient(140deg,#2B3550,#5B4CF0);box-shadow:0 6px 16px rgba(16,18,28,.16);}

.acard-v{width:154px;background:var(--surface);border:1px solid var(--line);border-radius:20px;padding:14px;box-shadow:var(--sh-1);cursor:pointer;contain:layout style paint;}
.acard-v h4{font-size:13.5px;font-weight:700;margin:10px 0 3px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.acard-v .meta{font-size:11px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}

.app-row{display:flex;align-items:center;gap:13px;padding:12px 16px;cursor:pointer;transition:background .12s;contain:layout style paint;background:transparent !important;}
.app-row:active{background:rgba(0,0,0,0.05) !important;}
.app-row-txt{flex:1;min-width:0}
.app-row-txt h4{font-size:14.5px;font-weight:680;margin:0 0 3px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.app-row-txt .meta{font-size:11.5px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}

.searchbar{display:flex;align-items:center;gap:10px;height:50px;padding:0 6px 0 15px;background:var(--search-bg);border:1px solid var(--search-border);border-radius:var(--r-full);box-shadow:var(--sh-1);}
.searchbar:focus-within{border-color:var(--brand);box-shadow:0 0 0 4px rgba(91,76,240,.10)}
.searchbar svg{width:19px;height:19px;color:var(--muted);flex:0 0 auto}
.searchbar input{flex:1;border:0;outline:0;background:transparent;font:inherit;font-size:14.5px;font-weight:500;color:var(--search-text);min-width:0;}
.searchbar input::placeholder{color:var(--search-placeholder);font-weight:450}
.clear-btn{width:28px;height:28px;border-radius:50%;border:0;background:var(--surface-2);display:grid;place-items:center;cursor:pointer;color:var(--muted);flex:0 0 auto;margin-right:8px;}
.clear-btn svg{width:13px;height:13px;}

.rcard{display:flex;gap:13px;padding:12px 16px;cursor:pointer;transition:background .12s;align-items:center;contain:layout style paint;}
.rcard:active{background:var(--surface-2)}
.rcard .art{width:104px;height:66px;border-radius:13px;flex:0 0 auto}
.rcard .app-ico{width:60px;height:60px;border-radius:17px;font-size:23px}
.rcard-txt{flex:1;min-width:0}
.rcard-txt h4{font-size:14px;font-weight:660;margin:0 0 4px;line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden}
.rcard-tags{display:flex;align-items:center;gap:6px;margin-top:6px;flex-wrap:wrap}
.tag-mini{font-size:10px;font-weight:700;color:var(--muted);background:var(--surface-2);padding:2px 7px;border-radius:6px;}

.group{background:var(--surface);border:1px solid var(--line);border-radius:20px;margin:0 16px;overflow:hidden;box-shadow:var(--sh-1);}
#appsContent .group { background: transparent !important; border: none !important; box-shadow: none !important; margin: 0 !important; }

.row-item{display:flex;align-items:center;gap:13px;padding:13px 15px;cursor:pointer;transition:background .12s;position:relative;}
.row-item + .row-item::before{content:"";position:absolute;top:0;left:58px;right:0;height:1px;background:var(--line);}
.row-item:active{background:var(--surface-2)}
.ri-ico{width:38px;height:38px;border-radius:12px;display:grid;place-items:center;background:var(--brand-soft);color:var(--brand);flex:0 0 auto;}
.ri-ico svg{width:19px;height:19px}
.ri-ico.gold{background:var(--gold-soft);color:var(--gold)}
.ri-ico.red{background:var(--red-soft);color:var(--red)}
.ri-txt{flex:1;min-width:0}
.ri-txt h4{font-size:14px;font-weight:620;margin:0 0 2px}
.ri-txt p{font-size:11.5px;color:var(--muted);margin:0;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.ri-chev{color:#C2C7D6;flex:0 0 auto}
.ri-chev svg{width:18px;height:18px}

.section-label{font-size:12px;font-weight:750;color:var(--muted);text-transform:uppercase;letter-spacing:.075em;padding:0 16px;margin:24px 0 10px;}

.nav{
  position:absolute;left:12px;right:12px;bottom:calc(12px + env(safe-area-inset-bottom));z-index:80;
  display:grid;grid-template-columns:repeat(5,1fr);align-items:center;height:68px;padding:0 5px;
  border-radius:26px;background:var(--nav-bg);backdrop-filter:blur(16px) saturate(160%);
  -webkit-backdrop-filter:blur(16px) saturate(160%);
  border:1px solid var(--nav-border);box-shadow:var(--nav-shadow);
}
.nav-item{position:relative;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;height:56px;border-radius:19px;border:0;background:none;color:var(--nav-text);cursor:pointer;transition:color .16s var(--ease);}
.nav-item::before{content:"";position:absolute;top:5px;right:7px;bottom:5px;left:7px;border-radius:16px;background:var(--brand-soft);opacity:0;transform:scale(.72);transition:opacity .16s var(--ease),transform .22s var(--spring);}
.nav-item svg{width:22px;height:22px;position:relative;z-index:1;}
.nav-item span{font-size:8.5px;font-weight:680;position:relative;z-index:1}
.nav-item.active{color:var(--nav-active)}
.nav-item.active::before{opacity:1;transform:scale(1)}
.nav-item.pulse svg{animation:navPop .32s var(--spring)}
@keyframes navPop{0%{transform:scale(.8)}55%{transform:scale(1.16)}100%{transform:scale(1.05)}}

.ai-top{position:sticky;top:0;z-index:40;display:flex;align-items:center;justify-content:space-between;gap:10px;padding:13px 14px;background:var(--nav-bg);backdrop-filter:blur(12px);-webkit-backdrop-filter:blur(12px);border-bottom:1px solid var(--line);flex:0 0 auto;}
.ai-id{display:flex;align-items:center;gap:10px;min-width:0}
.ai-mark{width:38px;height:38px;border-radius:13px;flex:0 0 auto;display:grid;place-items:center;background:linear-gradient(140deg,#5B4CF0,#9B5BF0 55%,#E85CA8);color:#fff;box-shadow:0 6px 16px rgba(91,76,240,.32);}
.ai-mark svg{width:19px;height:19px}
.ai-name{font-size:15px;font-weight:750;}
.ai-status{font-size:11px;color:var(--muted);display:flex;align-items:center;gap:5px;margin-top:1px;font-weight:550}

.chat{flex:1;overflow-y:auto;padding:18px 16px 8px;display:flex;flex-direction:column;gap:14px}
.msg{display:flex;gap:9px;max-width:100%;animation:msgIn .18s ease-out}
@keyframes msgIn{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}
.msg.me{justify-content:flex-end}
.ai-av{width:28px;height:28px;border-radius:10px;flex:0 0 auto;display:grid;place-items:center;background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff;margin-top:2px;}
.ai-av svg{width:14px;height:14px}
.bubble{padding:11px 14px;border-radius:18px;font-size:14px;line-height:1.5;max-width:280px;word-wrap:break-word;}
.msg.ai .bubble{background:var(--surface);border:1px solid var(--line);border-top-left-radius:6px;box-shadow:var(--sh-1);color:var(--ink)}
.msg.me .bubble{background:linear-gradient(140deg,var(--brand),#7C5BF5);color:#fff;border-top-right-radius:6px;box-shadow:0 6px 18px rgba(91,76,240,.28);}
.ts{font-size:10.5px;color:#A9AFC0;margin-top:5px;padding:0 4px;font-weight:550}

.typing{display:flex;gap:4px;padding:14px}
.typing i{width:6px;height:6px;border-radius:50%;background:#C4C9D8;animation:bounce 1.3s infinite}
.typing i:nth-child(2){animation-delay:.16s}
.typing i:nth-child(3){animation-delay:.32s}
@keyframes bounce{0%,60%,100%{transform:translateY(0);opacity:.5}30%{transform:translateY(-5px);opacity:1}}

.suggest-wrap{padding:0 16px 10px}
.suggest-title{font-size:12.5px;font-weight:700;color:var(--muted);margin-bottom:10px;}
.suggest{display:block;width:100%;text-align:left;padding:13px 15px;margin-bottom:9px;background:var(--surface);border:1px solid var(--line);border-radius:15px;font-size:13.5px;font-weight:550;cursor:pointer;box-shadow:var(--sh-1);color:var(--ink-2);}
.suggest span{color:var(--brand);font-weight:700;display:block;font-size:11.5px;margin-bottom:3px;text-transform:uppercase;}

.composer{flex:0 0 auto;padding:10px 14px calc(96px + env(safe-area-inset-bottom));background:linear-gradient(180deg,rgba(245,246,250,0),var(--bg) 26%);}
.composer-inner{display:flex;align-items:flex-end;gap:8px;padding:6px 6px 6px 16px;background:var(--surface);border:1px solid var(--line);border-radius:24px;box-shadow:0 6px 22px rgba(16,18,28,.09);}
.composer textarea{flex:1;border:0;outline:0;resize:none;background:transparent;font:inherit;font-size:14.5px;line-height:1.45;padding:10px 0;max-height:96px;min-height:22px;color:var(--ink);}
.send-btn{width:40px;height:40px;border-radius:50%;border:0;flex:0 0 auto;cursor:pointer;background:var(--brand);color:#fff;display:grid;place-items:center;box-shadow:0 6px 16px rgba(91,76,240,.32);}
.send-btn svg{width:18px;height:18px}

.ad-hero{position:relative;height:172px;overflow:hidden;border-radius:0 0 30px 30px}
.ad-hero-art{position:absolute;inset:0;background:#2B3550}
.ad-hero-art img{width:100%;height:100%;object-fit:cover}
.ad-hero-art::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(245,246,250,.05) 0%,rgba(245,246,250,.55) 62%,var(--bg) 100%);}
.ad-hero .back-abs{position:absolute;top:14px;left:14px;z-index:5}
.ad-head{margin-top:-52px;position:relative;z-index:6;padding:0 16px;text-align:center;cursor:pointer;}
.ad-head .app-ico{margin:0 auto 12px;box-shadow:0 14px 32px rgba(16,18,28,.24)}
.ad-head h1{font-size:22px;font-weight:820;letter-spacing:-.035em;margin-bottom:5px}
.ad-tagline{font-size:13.5px;color:var(--muted);line-height:1.45;max-width:300px;margin:0 auto 10px;}
.ad-meta{font-size:12px;color:var(--ink-2);font-weight:600;display:flex;align-items:center;justify-content:center;gap:8px;flex-wrap:wrap}
.ad-meta .sep{width:3px;height:3px;border-radius:50%;background:#C6CAD8}
.star{color:#E8A33D}
.ad-cta{padding:18px 16px 0}
.ad-cta-sub{text-align:center;font-size:11.5px;color:var(--muted);margin-top:9px;font-weight:550}
.ad-stats{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;margin:22px 16px 0;background:var(--line);border-radius:18px;overflow:hidden;border:1px solid var(--line);}
.ad-stat{background:var(--surface);padding:14px 10px;text-align:center}
.ad-stat b{display:block;font-size:14.5px;font-weight:780;}
.ad-stat span{display:block;font-size:10.5px;color:var(--muted);margin-top:3px;font-weight:600;text-transform:uppercase;letter-spacing:.05em}

.sec-h2 {padding: 24px 16px 12px; font-size: 16px; font-weight: 800; color: var(--ink); letter-spacing: -.02em;}
.app-screenshots {display: flex; gap: 12px; overflow-x: auto; padding: 0 16px 24px; scrollbar-width: none;}
.app-screenshots::-webkit-scrollbar {display: none;}
.app-screenshot-card {flex: 0 0 auto; width: 260px; aspect-ratio: 16/10; border-radius: 16px; overflow: hidden; background: var(--surface); border: 1px solid var(--line); box-shadow: var(--sh-1); display: grid; place-items: center;}
.app-screenshot-card img {width: 100%; height: 100%; object-fit: cover; display: block;}

.pd-player-header{position:relative;background:#000;aspect-ratio:16/9;overflow:hidden;}
.pd-player-header .pd-player-inner{position:absolute;inset:0;background:#000;overflow:hidden;}
.pd-player-header .pd-player-inner iframe,
.pd-player-header .pd-player-inner video{position:absolute;inset:0;width:100%;height:100%;border:0;background:#000;display:block;}
.pd-player-header .pd-player-inner video{object-fit:contain}
.pd-player-header .pd-back{position:absolute;top:12px;left:12px;z-index:10;}
.pd-player-header .pd-empty{position:absolute;inset:0;display:grid;place-items:center;color:#fff;font-size:13px;background:linear-gradient(135deg,#2B3550,#5B4CF0);}

.pd-info, .pd-desc, .pd-list-head { display: none !important; }

.pd-actions{
  display:flex;
  align-items:center;
  gap:10px;
  padding:12px 16px;
  background:var(--pd-actions-bg, var(--surface));
  border-bottom:1px solid var(--line);
  box-shadow:0 4px 12px rgba(0,0,0,0.03);
  flex-wrap:wrap;
  position:relative;
  z-index:5;
  transition: background 0.3s ease;
}
.pd-action-btn{display:inline-flex;align-items:center;gap:7px;height:38px;padding:0 14px;border-radius:999px;border:1px solid var(--line);background:var(--surface-2);color:var(--ink-2);font-size:13px;font-weight:700;cursor:pointer;box-shadow:var(--sh-1);transition:transform .14s var(--ease),background .16s,color .16s,border-color .16s;}
.pd-action-btn:active{transform:scale(.95);}
.pd-action-btn svg{width:16px;height:16px;}
.pd-action-btn.liked{background:#FDECEC;border-color:#F5A3A5;color:#E5484D;}
.pd-action-btn.liked svg{fill:#E5484D;stroke:#E5484D;}
.pd-action-btn.subscribed{background:var(--surface-2);color:var(--muted);pointer-events:none;}
.pd-action-btn.primary{background:var(--brand);color:#fff;border-color:var(--brand);}
.pd-action-count{font-weight:800;font-size:12.5px;}
.pd-actions-spacer{flex:1;}

.pd-list{
  padding:16px;
  display:flex;
  flex-direction:column;
  padding-bottom:120px;
  background:transparent !important;
}
.pd-video-item{
  display:flex;
  flex-direction:column;
  padding:0;
  margin-bottom:20px;
  background:transparent !important;
  border:none !important;
  box-shadow:none !important;
  cursor:pointer;
  transition:transform .14s var(--ease);
  position:relative;
}
.pd-video-item:active{transform:scale(.98);}
.pd-video-item.active{background:transparent !important;}
.pd-video-item.active::before{display:none;}

.pd-video-thumb{
  width:100%;
  height:auto;
  aspect-ratio:16/9;
  border-radius:14px;
  position:relative;
  background:#2B3550;
  overflow:hidden;
}
.pd-video-thumb img{
  width:100%;
  height:100%;
  object-fit:cover;
  display:block;
}
.pd-video-thumb .pd-dur{
  position:absolute;
  bottom:8px;
  right:8px;
  z-index:3;
  background:rgba(8,9,18,.82);
  color:#fff;
  font-size:11px;
  font-weight:700;
  padding:3px 8px;
  border-radius:6px;
}
.pd-video-thumb .pd-play, .pd-video-thumb .pd-lock{
  position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);z-index:3;width:44px;height:44px;border-radius:50%;display:grid;place-items:center;box-shadow:0 4px 12px rgba(0,0,0,.3);
}
.pd-video-thumb .pd-play{background:var(--thumb-play-bg);color:#111;}
.pd-video-thumb .pd-play svg{width:18px;height:18px;margin-left:2px;}
.pd-video-thumb .pd-lock{background:rgba(20,15,4,.85);color:#F5C55C;}
.pd-video-thumb .pd-lock svg{width:20px;height:20px;}

.pd-video-item.active .pd-video-thumb::after {
  content: "";
  position: absolute;
  inset: 0;
  background: rgba(0, 0, 0, 0.45);
  z-index: 4;
}
.audio-visualizer {
  position: absolute;
  bottom: 8px;
  left: 8px;
  z-index: 5;
  display: flex;
  align-items: flex-end;
  gap: 3px;
  height: 16px;
}
.audio-visualizer span {
  width: 3px;
  background: #fff;
  border-radius: 2px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.5);
  animation: eq-bounce 1.2s ease-in-out infinite alternate;
}
.audio-visualizer span:nth-child(1) { height: 6px; animation-delay: 0s; }
.audio-visualizer span:nth-child(2) { height: 16px; animation-delay: 0.3s; }
.audio-visualizer span:nth-child(3) { height: 10px; animation-delay: 0.6s; }

@keyframes eq-bounce {
  0% { height: 4px; }
  100% { height: 16px; }
}

.pd-video-info{
  padding:10px 0 0 0;
  background:transparent !important;
}
.pd-video-info h4{
  font-size:15px;
  font-weight:700;
  line-height:1.32;
  margin:0 0 4px;
  color:var(--ink);
  display:-webkit-box;
  -webkit-line-clamp:2;
  -webkit-box-orient:vertical;
  overflow:hidden;
}
.pd-video-info .pd-creator{
  font-size:12px;
  color:var(--muted);
  margin:0 0 2px;
  font-weight:550;
}

.pd-unlock-bar{position:sticky;bottom:0;z-index:30;margin-top:8px;padding:12px 16px calc(112px + env(safe-area-inset-bottom));background:linear-gradient(180deg,rgba(245,246,250,0),var(--bg) 22%);}
.pd-unlock-inner{display:flex;align-items:center;gap:14px;padding:12px 14px;background:var(--surface);border:1px solid var(--line);border-radius:22px;box-shadow:0 12px 30px rgba(16,18,28,.14);}
.pd-unlock-price b{display:block;font-size:19px;font-weight:820;line-height:1}
.pd-unlock-price span{display:block;font-size:11px;color:var(--muted);margin-top:3px;font-weight:600}

.pd-ad-slot{
  position:absolute;
  top:0; left:0; right:0;
  z-index:8;
  display:none;
  padding:8px 66px 0 60px;
  pointer-events:none;
}
.pd-ad-slot.on{display:block;animation:adSlide .25s var(--ease);}
@keyframes adSlide{from{opacity:0;transform:translateY(-8px)}to{opacity:1;transform:none}}
.pd-ad-card{
  pointer-events:auto;
  display:flex;
  align-items:center;
  gap:8px;
  height:36px;
  padding:0 10px 0 6px;
  border-radius:10px;
  background:rgba(255,255,255,.95);
  box-shadow:0 3px 14px rgba(0,0,0,.35);
  cursor:pointer;
  overflow:hidden;
  -webkit-backdrop-filter:blur(10px);
  backdrop-filter:blur(10px);
  transition:transform .14s var(--ease);
}
.pd-ad-card:active{transform:scale(.97);}
.pd-ad-card img{width:48px;height:26px;object-fit:cover;border-radius:6px;flex:0 0 auto;display:block;background:#222;}
.pd-ad-card .ad-label{font-size:8px;font-weight:900;letter-spacing:.08em;color:#B0B4C2;flex:0 0 auto;padding:1px 4px;border:1px solid #D6D9E3;border-radius:4px;line-height:1;}
.pd-ad-card .ad-title{flex:1;min-width:0;font-size:12px;font-weight:700;color:#111;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;line-height:1;}
.pd-ad-card .ad-cta{font-size:11px;font-weight:800;color:var(--brand);flex:0 0 auto;white-space:nowrap;}

.player-wrap{padding:12px 12px 0}
.player-art{position:relative;border-radius:22px;overflow:hidden;aspect-ratio:16/9;box-shadow:0 16px 38px rgba(16,18,28,.28);background:#000;}
.player-media-mount{position:absolute;inset:0;overflow:hidden;}
.player-art iframe,.player-art video{position:absolute;inset:0;width:100%;height:100%;border:0;z-index:2;background:#000;display:block;}
.player-art video{object-fit:contain}
.player-art .back-abs{position:absolute;top:12px;left:12px;z-index:6}
.yt-shield{position:absolute;inset:0;z-index:5;pointer-events:none;}
.yt-shield::before{content:"";position:absolute;top:0;right:0;width:150px;height:48px;pointer-events:auto;}
.player-art .yt-shield .back-abs,
.pd-player-header .yt-shield .back-abs{pointer-events:auto;position:absolute;z-index:10;}
.player-title{padding:18px 16px 0}
.player-title h1{font-size:19px;font-weight:800;line-height:1.3;margin-bottom:8px}
.player-meta{display:flex;align-items:center;gap:9px;flex-wrap:wrap;font-size:12px;color:var(--muted);font-weight:550}

.profile-hero{padding:66px 16px 24px;text-align:center;background:linear-gradient(170deg,var(--brand-soft) 0%,transparent 100%);}
.profile-av{width:88px;height:88px;border-radius:30px;margin:0 auto 14px;background:linear-gradient(140deg,#2B3550,#5B4CF0 60%,#9B5BF0);display:grid;place-items:center;color:#fff;font-size:30px;font-weight:850;box-shadow:0 14px 34px rgba(91,76,240,.30);position:relative;overflow:hidden;}
.profile-av img{width:100%;height:100%;object-fit:cover;}
.profile-av .edit-dot{position:absolute;right:-4px;bottom:-4px;width:30px;height:30px;border-radius:50%;background:var(--surface);border:1px solid var(--line);display:grid;place-items:center;color:var(--brand);box-shadow:var(--sh-2);}
.profile-av .edit-dot svg{width:14px;height:14px}
.profile-hero h1{font-size:20px;font-weight:800;margin-bottom:4px}
.profile-hero p{font-size:13px;color:var(--muted);margin:0 0 16px}
.stat-row{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;padding:0 16px;margin-top:-8px}
.stat-cell{background:var(--surface);border:1px solid var(--line);border-radius:18px;padding:14px 10px;text-align:center;box-shadow:var(--sh-1);}
.stat-cell b{display:block;font-size:17px;font-weight:820;}
.stat-cell span{display:block;font-size:10.5px;color:var(--muted);margin-top:3px;font-weight:650;text-transform:uppercase;letter-spacing:.05em}

.field{margin-bottom:14px}
.field label{display:block;font-size:12.5px;font-weight:680;color:var(--ink-2);margin-bottom:7px;}
.input{width:100%;height:52px;padding:0 16px;border-radius:16px;border:1px solid var(--line);background:var(--surface);font:inherit;font-size:14.5px;font-weight:500;color:var(--ink);outline:0;transition:border-color .16s,box-shadow .16s;}
.input:focus{border-color:var(--brand);box-shadow:0 0 0 4px rgba(91,76,240,.10)}
.input.error{border-color:#F5A3A5;box-shadow:0 0 0 4px rgba(229,72,77,.08)}
.err-msg{font-size:11.5px;color:var(--red);margin-top:6px;font-weight:600;display:flex;align-items:center;gap:5px}

.empty{display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding:52px 32px;}
.empty-ico{width:76px;height:76px;border-radius:26px;background:var(--surface-2);display:grid;place-items:center;color:#A9AFC0;margin-bottom:18px;}
.empty-ico svg{width:32px;height:32px}
.empty h3{font-size:16.5px;font-weight:750;margin-bottom:7px}
.empty p{font-size:13.5px;color:var(--muted);line-height:1.55;margin:0 0 20px;max-width:270px}

.toast-wrap{position:absolute;left:12px;right:12px;bottom:calc(96px + env(safe-area-inset-bottom));z-index:200;display:flex;flex-direction:column;gap:8px;pointer-events:none;}
.toast{display:flex;align-items:center;gap:11px;padding:13px 15px;border-radius:18px;background:rgba(20,22,32,.94);color:#fff;backdrop-filter:blur(12px);-webkit-backdrop-filter:blur(12px);box-shadow:0 12px 30px rgba(0,0,0,.3);font-size:13.5px;font-weight:600;animation:toastIn .22s var(--spring);}
.toast.out{animation:toastOut .18s var(--ease) forwards}
@keyframes toastIn{from{opacity:0;transform:translateY(16px) scale(.96)}to{opacity:1;transform:none}}
@keyframes toastOut{to{opacity:0;transform:translateY(10px) scale(.97)}}
.toast i{width:22px;height:22px;border-radius:50%;display:grid;place-items:center;flex:0 0 auto;}
.toast i svg{width:12px;height:12px}
.toast.success i{background:#12A150;color:#fff}
.toast.error i{background:#E5484D;color:#fff}
.toast.info i{background:var(--brand);color:#fff}

.overlay{position:absolute;inset:0;z-index:300;display:none;align-items:center;justify-content:center;padding:24px;background:rgba(10,11,18,.5);backdrop-filter:blur(6px);overflow-y:auto;}
.overlay.on{display:flex;animation:fadeIn .16s ease}
@keyframes fadeIn{from{opacity:0}to{opacity:1}}
.modal{width:100%;max-width:330px;background:var(--surface);border-radius:26px;padding:24px 22px 18px;box-shadow:0 30px 70px rgba(0,0,0,.4);animation:modalIn .22s var(--spring);max-height:92vh;overflow-y:auto;}
@keyframes modalIn{from{opacity:0;transform:translateY(20px) scale(.94)}to{opacity:1;transform:none}}
.modal h3{font-size:17.5px;font-weight:780;margin-bottom:8px}
.modal p{font-size:13.5px;color:var(--muted);line-height:1.55;margin:0 0 20px}
.modal-actions{display:flex;gap:9px}
.modal-actions .btn{flex:1;height:46px;font-size:14px}
.unlock-badge{width:64px;height:64px;border-radius:22px;margin:0 auto 14px;background:linear-gradient(140deg,#F5C55C,#DD8E1E);display:grid;place-items:center;color:#2E1C00;font-size:28px;box-shadow:0 12px 28px rgba(216,135,30,.35);}
.auth-tabs{display:flex;gap:4px;padding:4px;background:var(--surface-2);border-radius:12px;margin-bottom:14px;}
.auth-tab{flex:1;height:38px;border:0;background:none;border-radius:9px;font-size:13px;font-weight:700;color:var(--muted);cursor:pointer;}
.auth-tab.active{background:var(--surface);color:var(--brand);box-shadow:0 2px 8px rgba(16,18,28,.08);}
.spin{width:16px;height:16px;border:2px solid rgba(255,255,255,.35);border-top-color:#fff;border-radius:50%;animation:spin 0.8s linear infinite;display:inline-block;}
@keyframes spin{to{transform:rotate(360deg)}}
.bg-preview{width:100%;height:90px;border-radius:14px;background-size:cover;background-position:center;border:1px solid var(--line);display:grid;place-items:center;color:var(--muted);font-size:11.5px;font-weight:600;background-color:var(--surface-2);position:relative;overflow:hidden;}
.bg-preview::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(0,0,0,.05),rgba(0,0,0,.35));pointer-events:none;}
.bg-preview span{position:relative;z-index:2;color:#fff;background:rgba(8,9,18,.55);padding:5px 12px;border-radius:999px;backdrop-filter:blur(8px);font-size:11px;}
.home-brand{display:flex;align-items:center;justify-content:space-between;gap:11px;padding:14px 16px 6px;}
.home-brand .brand-mark{width:38px;height:38px;border-radius:13px;flex:0 0 auto;background:linear-gradient(140deg,var(--brand),#9B5BF0 60%,#E85CA8);color:#fff;display:grid;place-items:center;font-weight:900;font-size:16px;box-shadow:0 6px 16px rgba(91,76,240,.34);position:relative;overflow:hidden;}
.home-brand .brand-hello{font-size:11px;color:var(--muted);font-weight:600;}
.home-brand .brand-name{font-size:16px;font-weight:800;letter-spacing:-.03em;margin-top:-1px}

.home-banner-wrapper {
  flex: 1;
  margin-left: 12px;
  height: 38px;
  border-radius: 8px;
  overflow: hidden;
  background: var(--surface-2);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  cursor: pointer;
  border: 1px solid var(--line);
  max-width: 160px;
}
.home-banner-track {
  display: flex;
  flex-direction: column;
  width: 100%;
  transition: transform 0.6s cubic-bezier(0.25, 1, 0.5, 1);
}
.home-banner-img {
  width: 100%;
  height: 38px;
  object-fit: cover;
  display: block;
}

.shorts-row{display:flex;gap:12px;padding:2px 16px 6px;scrollbar-width:none;overflow:hidden;}
.shorts-row::-webkit-scrollbar{display:none}
.shorts-item{flex:1;min-width:0;aspect-ratio:9/16;border-radius:18px;overflow:hidden;position:relative;background:#111;cursor:pointer;box-shadow:0 4px 16px rgba(0,0,0,.18);contain:layout style paint;}
.shorts-item img{width:100%;height:100%;object-fit:cover;display:block;}
.shorts-item .thumb-fallback{width:100%;height:100%;display:grid;place-items:center;font-size:34px;background:linear-gradient(140deg,#2B3550,#5B4CF0);}
.shorts-item .short-overlay{position:absolute;left:0;right:0;bottom:0;padding:12px 10px 10px;background:linear-gradient(0deg,rgba(0,0,0,.85) 0%,transparent 100%);z-index:2;}
.shorts-item .short-label{font-size:12px;font-weight:700;color:#fff;line-height:1.3;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;text-shadow:0 1px 8px rgba(0,0,0,.6);}
.shorts-item .short-views{font-size:10px;color:rgba(255,255,255,.75);font-weight:600;margin-top:2px;}
.shorts-item .short-tag{position:absolute;top:8px;left:8px;z-index:3;background:var(--shorts-chip-bg);color:var(--shorts-chip-text);font-size:10px;font-weight:800;padding:3px 8px;border-radius:999px;}
.shorts-item .play-icon{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:34px;height:34px;border-radius:50%;background:var(--shorts-play-bg);display:grid;place-items:center;z-index:3;pointer-events:none;}
.shorts-item .play-icon svg{width:14px;height:14px;margin-left:2px}

.playlist-large{width:100%;margin-bottom:16px;border-radius:16px;overflow:hidden;position:relative;background:#2B3550;cursor:pointer;box-shadow:0 4px 16px rgba(0,0,0,.12);contain:layout style paint;}
.playlist-large .art{border-radius:16px;aspect-ratio:16/9;width:100%;}
.playlist-large .playlist-overlay{position:absolute;left:0;right:0;bottom:0;padding:16px;background:linear-gradient(0deg,rgba(0,0,0,.85) 0%,transparent 100%);color:#fff;z-index:3;}
.playlist-large .playlist-title{font-size:16px;font-weight:800;margin-bottom:4px;text-shadow:0 1px 4px rgba(0,0,0,.5);display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;line-height:1.3;}
.playlist-large .playlist-meta{font-size:12px;opacity:.85;font-weight:500;display:flex;align-items:center;gap:6px;flex-wrap:wrap;}
.playlist-large .playlist-meta svg{width:14px;height:14px;fill:currentColor;}

.premium-photo-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;padding:0 16px 8px;}
.premium-photo-item{position:relative;aspect-ratio:3/4;border-radius:14px;overflow:hidden;background:linear-gradient(135deg,#2B3550,#14162a);cursor:pointer;border:1px solid var(--line);box-shadow:0 2px 10px rgba(16,18,28,.08);transition:transform .14s var(--ease),box-shadow .18s;isolation:isolate;contain:layout style paint;}
.premium-photo-item:active{transform:scale(.97);box-shadow:0 4px 18px rgba(16,18,28,.16);}
.premium-photo-item img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;display:block;background:#14162a;z-index:0;}
.premium-photo-item::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,transparent 55%,rgba(0,0,0,.55));pointer-events:none;z-index:1;}
.premium-photo-item .pp-title{position:absolute;left:0;right:0;bottom:0;padding:18px 10px 10px;color:#fff;font-size:11.5px;font-weight:700;line-height:1.3;z-index:2;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;text-shadow:0 1px 4px rgba(0,0,0,.7);}
.premium-photo-item .pp-badge{position:absolute;top:6px;left:6px;z-index:3;background:var(--shorts-chip-bg);color:var(--shorts-chip-text);font-size:9px;font-weight:800;padding:2px 7px;border-radius:999px;text-transform:uppercase;letter-spacing:.04em;box-shadow:0 2px 6px rgba(0,0,0,.15);}

#s-shortplayer.active { padding-bottom: 0; display: block; overflow: hidden; background: #000; }
.shorts-reels {position: absolute; inset: 0; width: 100%; height: 100%;overflow-y: scroll; overflow-x: hidden;scroll-snap-type: y mandatory; scroll-snap-stop: always;-webkit-overflow-scrolling: touch;overscroll-behavior-y: contain;scrollbar-width: none; -ms-overflow-style: none;background: #000; touch-action: pan-y;transform:translateZ(0);backface-visibility:hidden;}
.shorts-reels::-webkit-scrollbar { display: none; }
.short-reel {position: relative; width: 100%; height: 100%;scroll-snap-align: start; scroll-snap-stop: always;overflow: hidden; background: #000; isolation: isolate;}
.short-reel-media { position: absolute; inset: 0; z-index: 1; background: #000; overflow: hidden; }
.short-reel-lqip {position: absolute; inset: 0;width: 100%; height: 100%;object-fit: cover;z-index: 0;filter: blur(20px);transform: scale(1.15) translateZ(0);opacity: 0.9;transition: opacity .2s ease;background: linear-gradient(135deg, #0a0b14, #14162a);pointer-events: none;}
.short-reel-media.playing .short-reel-lqip { opacity: 0; }
.short-reel-thumb {position: absolute; inset: 0;width: 100%; height: 100%;object-fit: cover;z-index: 1;opacity: 1;transition: opacity .16s ease;background: linear-gradient(135deg, #0a0b14, #14162a);pointer-events: none;filter: none !important;will-change: opacity;transform: translateZ(0);backface-visibility: hidden;}
.short-reel-media.playing .short-reel-thumb { opacity: 0; }
.short-reel-media iframe, .short-reel-media video {width: 100%; height: 100%; object-fit: cover; border: 0; background: #000; display: block;position: relative;z-index: 2;}
.short-reel-media iframe[data-media-type="instagram"] {position: absolute;inset: 0;width: 100%;height: 100%;transform: scale(2.35);transform-origin: 50% 22%;border: 0;background: #000;pointer-events: auto;}
.short-reel-ui { position: absolute; inset: 0; z-index: 3; pointer-events: none; }
.short-reel-ui > * { pointer-events: auto; }
.short-reel-info {position: absolute; left: 16px; right: 88px; bottom: 24px;color: #fff; z-index: 4; pointer-events: auto;}
.short-reel-channel { display: flex; align-items: center; gap: 8px; margin-bottom: 12px; }
.short-reel-channel-avatar {width: 32px; height: 32px; border-radius: 50%;background: var(--brand); display: grid; place-items: center;font-size: 14px; font-weight: 800; border: 2px solid #fff;cursor: pointer; transition: transform .14s var(--ease);overflow:hidden;position:relative;}
.short-reel-channel-avatar img{width:100%;height:100%;object-fit:cover;border-radius:50%;display:block;}
.short-reel-channel-avatar:active { transform: scale(.9); }
.short-reel-channel > span {font-size: 13px; font-weight: 700;text-shadow: 0 1px 3px rgba(0,0,0,.8);cursor: pointer;}
.short-reel-subscribe {background: #ff0033; color: #fff; border: none;padding: 6px 16px; border-radius: 20px; font-size: 12px;font-weight: 800; cursor: pointer;transition: transform .14s var(--ease), background .16s, color .16s;}
.short-reel-subscribe:active { transform: scale(.95); }
.short-reel-info h3 {font-size: 16px; font-weight: 700; margin-bottom: 6px;text-shadow: 0 1px 4px rgba(0,0,0,.8);display: -webkit-box; -webkit-line-clamp: 2;-webkit-box-orient: vertical; overflow: hidden;}
.short-reel-info p {font-size: 13px; opacity: .9;text-shadow: 0 1px 3px rgba(0,0,0,.8);display: -webkit-box; -webkit-line-clamp: 2;-webkit-box-orient: vertical; overflow: hidden;}
.short-reel-actions {position: absolute; right: 12px; bottom: 100px;display: flex; flex-direction: column; gap: 24px;align-items: center; z-index: 4; pointer-events: auto;}
.short-reel-action-btn {display: flex; flex-direction: column; align-items: center; gap: 4px;background: none; border: none; color: #fff; cursor: pointer;transition: transform .14s var(--ease);}
.short-reel-action-btn:active { transform: scale(.9); }
.short-reel-action-btn svg {width: 32px; height: 32px;filter: drop-shadow(0 2px 4px rgba(0,0,0,.5));transition: fill .16s, stroke .16s;}
.short-reel-action-btn span {font-size: 11px; font-weight: 600;text-shadow: 0 1px 3px rgba(0,0,0,.8);transition: color .16s;}
.shorts-global-back {position: absolute;top: calc(16px + env(safe-area-inset-top)); left: 16px;z-index: 100; width: 44px; height: 44px;border-radius: 50%; background: rgba(0,0,0,.45);backdrop-filter: blur(6px); -webkit-backdrop-filter: blur(6px);color: #fff; display: grid; place-items: center;cursor: pointer; border: none;transition: transform .14s var(--ease);}
.shorts-global-back:active { transform: scale(.9); }
.shorts-global-back svg { width: 24px; height: 24px; }

.sound-toggle{position:absolute;right:12px;bottom:12px;z-index:12;width:42px;height:42px;border-radius:50%;border:0;cursor:pointer;background:rgba(8,9,18,.75);color:#fff;display:grid;place-items:center;backdrop-filter:blur(10px);-webkit-backdrop-filter:blur(10px);box-shadow:0 4px 14px rgba(0,0,0,.35);transition:transform .14s var(--ease),background .16s;}
.sound-toggle:active{transform:scale(.9)}
.sound-toggle svg{width:20px;height:20px}
.sound-toggle.on{background:rgba(91,76,240,.95)}
.shorts-sound-toggle{position:absolute;top:calc(16px + env(safe-area-inset-top));right:16px;z-index:100;width:44px;height:44px;border-radius:50%;background:rgba(0,0,0,.5);backdrop-filter:blur(8px);-webkit-backdrop-filter:blur(8px);color:#fff;display:grid;place-items:center;cursor:pointer;border:none;transition:transform .14s var(--ease),background .16s;}
.shorts-sound-toggle:active{transform:scale(.9)}
.shorts-sound-toggle svg{width:22px;height:22px}
.shorts-sound-toggle.on{background:rgba(91,76,240,.9)}

.short-reel-cat {position: absolute;top: calc(20px + env(safe-area-inset-top));left: 50%; transform: translateX(-50%);background: rgba(0,0,0,.55);backdrop-filter: blur(8px); -webkit-backdrop-filter: blur(8px);color: #fff; font-size: 11px; font-weight: 700;padding: 6px 14px; border-radius: 999px;letter-spacing: .03em; z-index: 5; pointer-events: none;border: 1px solid rgba(255,255,255,.15);text-shadow: 0 1px 4px rgba(0,0,0,.5);white-space: nowrap;}
.shorts-progress {position: absolute; top: 0; left: 0; right: 0;height: 2px; background: rgba(255,255,255,.15);z-index: 110; pointer-events: none;}
.shorts-progress i {display: block; height: 100%; width: 0%;background: #fff; transition: width .16s ease;border-radius: 0 2px 2px 0;}
.short-reel-spinner {position: absolute; inset: 0; z-index: 2;display: flex; flex-direction: column;align-items: center; justify-content: center;color: rgba(255,255,255,.6);font-size: 13px; font-weight: 600;opacity: 0;transition: opacity .16s;pointer-events: none;background: linear-gradient(90deg, #0a0b14 0%, #1a1d2e 50%, #0a0b14 100%);background-size: 200% 100%;animation: skeletonShimmer 1.2s ease-in-out infinite;}
.short-reel-media:not(.playing) .short-reel-spinner { opacity: 1; }
.short-reel-spinner::before { display: none; }
@keyframes skeletonShimmer {0%{background-position:200% 0}100%{background-position:-200% 0}}
.shorts-reels.scrolling .short-reel-cat,
.shorts-reels.scrolling .short-reel-info,
.shorts-reels.scrolling .short-reel-subscribe,
.shorts-reels.scrolling .shorts-global-back,
.shorts-reels.scrolling .shorts-sound-toggle,
.shorts-reels.scrolling .short-reel-actions {backdrop-filter: none !important;-webkit-backdrop-filter: none !important;}
.shorts-reels.scrolling .short-reel-media {filter: none !important;}
.shorts-reels.scrolling .short-reel-lqip {filter: none !important;}
.shorts-reels.scrolling .short-reel-action-btn svg {filter: none !important;}
.short-reel.is-active {will-change: transform;transform: translateZ(0);backface-visibility: hidden;contain: layout style paint;}
.short-reel:not(.is-active) {will-change: auto;}
.short-reel-placeholder { background: #000; }
.short-reel-placeholder:not([data-filled="true"]) > * { display: none; }
.channel-hero{padding: 76px 16px 20px;text-align: center;background: linear-gradient(170deg,var(--brand-soft) 0%,transparent 100%);}
.channel-avatar{width: 96px; height: 96px;border-radius: 50%;background: linear-gradient(140deg,#5B4CF0,#9B5BF0 60%,#E85CA8);color: #fff;display: grid; place-items: center;font-size: 38px; font-weight: 800;margin: 0 auto 14px;box-shadow: 0 14px 34px rgba(91,76,240,.30);position:relative;overflow:hidden;cursor:pointer;user-select:none;}
.channel-avatar img{width:100%;height:100%;object-fit:cover;border-radius:50%;display:block;position:absolute;inset:0;}
.channel-name{font-size: 22px; font-weight: 800;letter-spacing: -.03em;margin: 0 0 4px;}
.channel-meta{font-size: 13px; color: var(--muted);margin: 0 0 16px; font-weight: 500;}
.channel-subscribe-btn{height: 42px; padding: 0 26px;font-size: 14px; font-weight: 800;border-radius: var(--r-full);display: inline-flex; align-items: center;justify-content: center; gap: 6px;transition: transform .14s var(--ease), background .16s, color .16s;}
.channel-subscribe-btn:active { transform: scale(.95); }
.channel-subscribe-btn.subscribed{background: var(--surface-2) !important;color: var(--muted) !important;box-shadow: none !important;border: 1px solid var(--line) !important;pointer-events:none;}
.channel-section-label{font-size: 13px; font-weight: 750;color: var(--muted);text-transform: uppercase;letter-spacing: .07em;padding: 0 16px;margin: 22px 0 12px;}
.channel-grid{display: grid;grid-template-columns: repeat(3, 1fr);gap: 8px;padding: 0 16px 120px;}
.channel-short{ cursor: pointer; transition: transform .14s var(--ease); contain:layout style paint;}
.channel-short:active { transform: scale(.96); }
.channel-short-thumb{position: relative; aspect-ratio: 9/16;border-radius: 12px; overflow: hidden;background: #111;box-shadow: 0 4px 12px rgba(0,0,0,.10);}
.channel-short-thumb img{ width: 100%; height: 100%; object-fit: cover; display: block; }
.channel-short-fallback{width: 100%; height: 100%;display: grid; place-items: center;font-size: 32px;background: linear-gradient(140deg,#2B3550,#5B4CF0);}
.channel-short-play{position: absolute; bottom: 6px; left: 6px;width: 24px; height: 24px;border-radius: 50%;background: var(--shorts-play-bg);display: grid; place-items: center;pointer-events: none;}
.channel-short-play svg{ width: 10px; height: 10px; margin-left: 1px; }
.channel-short-info{ padding: 6px 2px 0; }
.channel-short-title{font-size: 11.5px; font-weight: 600;line-height: 1.3; color: var(--ink);display: -webkit-box; -webkit-line-clamp: 2;-webkit-box-orient: vertical; overflow: hidden;}
.channel-short-views{font-size: 10px; color: var(--muted);margin-top: 2px; font-weight: 500;}

#homeFeed > .sec,
#premiumContent > .sec{content-visibility:auto;contain-intrinsic-size:1px 350px;}
.short-reel,.channel-short,.shorts-item,.rcard,.playlist-large,.pcard,.acard-v{content-visibility:auto;}
.channel-short { contain-intrinsic-size: 120px 200px; }
.shorts-item { contain-intrinsic-size: 160px 280px; }
.rcard { contain-intrinsic-size: 100% 80px; }
.playlist-large { contain-intrinsic-size: 100% 220px; }
.pcard { contain-intrinsic-size: 252px 200px; }
.acard-v { contain-intrinsic-size: 154px 180px; }
img{image-rendering:-webkit-optimize-contrast;}

.short-reel-anim {position: fixed; top: 50%; left: 50%;transform: translate(-50%, -50%);width: 200px; height: 200px; z-index: 9999;pointer-events: none; display: none;align-items: center; justify-content: center;}
.short-reel-anim.show { display: flex; }
.short-reel-anim video {width: 100%; height: 100%; object-fit: contain;animation: likePop 1.3s cubic-bezier(.34,1.4,.64,1) forwards;}
@keyframes likePop {0%{transform:scale(0) rotate(-15deg);opacity:0}20%{transform:scale(1.25) rotate(5deg);opacity:1}35%{transform:scale(1) rotate(0);opacity:1}75%{transform:scale(1.05);opacity:1}100%{transform:scale(1.3);opacity:0}}
.sub-anim {position: fixed; top: 50%; left: 50%;transform: translate(-50%, -50%);z-index: 9999; pointer-events: none; display: none;flex-direction: column; align-items: center; gap: 14px;}
.sub-anim.show { display: flex; }
.sub-anim .sub-bell {width: 110px; height: 110px; border-radius: 50%;background: linear-gradient(135deg, #ff0033, #d1002a);display: grid; place-items: center;color: #fff; font-size: 54px; line-height: 1;box-shadow: 0 20px 60px rgba(255,0,51,.5);animation: bellPop 1.25s cubic-bezier(.34,1.4,.64,1) forwards;}
@keyframes bellPop {0%{transform:scale(0) rotate(-30deg);opacity:0;box-shadow:0 0 0 0 rgba(255,0,51,.85)}20%{transform:scale(1.2) rotate(8deg);opacity:1;box-shadow:0 0 0 25px rgba(255,0,51,0)}40%{transform:scale(1) rotate(0)}50%{transform:scale(1) rotate(-8deg)}60%{transform:scale(1) rotate(6deg)}70%{transform:scale(1) rotate(0)}85%{transform:scale(1.08);opacity:1}100%{transform:scale(1.2);opacity:0}}
.sub-anim .sub-text {color: #fff; font-size: 15px; font-weight: 800;letter-spacing: .1em; text-transform: uppercase;padding: 8px 20px; background: rgba(255,0,51,.92);border-radius: 999px;text-shadow: 0 2px 6px rgba(0,0,0,.4);animation: subTextPop 1.25s ease forwards;white-space: nowrap;}
@keyframes subTextPop {0%{opacity:0;transform:translateY(14px) scale(.85)}25%{opacity:1;transform:translateY(0) scale(1)}80%{opacity:1;transform:translateY(0)}100%{opacity:0;transform:translateY(-14px)}}
.short-reel-action-btn.liked svg {fill: #ff3b5c; stroke: #ff3b5c;animation: heartBeat .5s var(--spring);filter: drop-shadow(0 0 10px rgba(255,59,92,.65)) drop-shadow(0 2px 4px rgba(0,0,0,.5));}
@keyframes heartBeat {0%{transform:scale(1)}30%{transform:scale(1.35)}55%{transform:scale(.92)}100%{transform:scale(1)}}
.short-reel-action-btn.liked span { color: #ff3b5c; font-weight: 800; }
.short-reel-subscribe.subscribed {background: #303030 !important;color: #bdbdbd !important;cursor: default;pointer-events:none;}
.player-art iframe[data-media-type="instagram"],
.pd-player-inner iframe[data-media-type="instagram"] {position: absolute;inset: 0;width: 100%;height: 100%;transform: scale(1.9);transform-origin: 50% 30%;border: 0;background: #000;}
.google-btn{display:inline-flex;align-items:center;justify-content:center;gap:10px;background:var(--surface);color:var(--ink);border:1px solid var(--line);font-weight:600;}
.google-btn:hover{background:var(--surface-2);}
.switch{width:46px;height:28px;border-radius:999px;background:#DFE2EC;position:relative;transition:background .18s var(--ease);flex:0 0 auto;border:0;cursor:pointer;padding:0;}
.switch::after{content:"";position:absolute;top:3px;left:3px;width:22px;height:22px;border-radius:50%;background:#fff;box-shadow:0 1px 4px rgba(0,0,0,.22);transition:transform .22s var(--spring);}
.switch.on{background:var(--brand)}
.switch.on::after{transform:translateX(18px)}
.lightbox{position:absolute;inset:0;z-index:400;display:none;align-items:center;justify-content:center;background:rgba(6,7,14,.94);backdrop-filter:blur(10px);padding:28px;}
.lightbox.on{display:flex;}
.lb-close{position:absolute;top:22px;right:22px;width:42px;height:42px;border-radius:50%;background:rgba(255,255,255,.14);border:1px solid rgba(255,255,255,.2);color:#fff;display:grid;place-items:center;cursor:pointer;font-size:20px;}

.subs-hero{padding:66px 16px 20px;text-align:center;background:linear-gradient(170deg,var(--brand-soft) 0%,transparent 100%);background-size:cover;background-position:center;position:relative;}
.subs-hero::before{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(0,0,0,0.1) 0%,transparent 100%);pointer-events:none;}
.subs-icon{width:76px;height:76px;border-radius:24px;margin:0 auto 14px;background:linear-gradient(140deg,#5B4CF0,#9B5BF0);display:grid;place-items:center;color:#fff;box-shadow:0 14px 34px rgba(91,76,240,.30);position:relative;z-index:2;}
.subs-icon svg{width:34px;height:34px;}
.subs-hero h1{font-size:20px;font-weight:800;margin-bottom:4px;position:relative;z-index:2;}
.subs-hero p{font-size:13px;color:var(--muted);margin:0;position:relative;z-index:2;}

.chip-row{display:flex;gap:8px;overflow-x:auto;padding:2px 16px 6px;scrollbar-width:none;}
.chip-row::-webkit-scrollbar{display:none;}
.chip{flex:0 0 auto;display:inline-flex;align-items:center;gap:8px;height:38px;padding:0 14px 0 6px;border-radius:999px;background:var(--surface);border:1px solid var(--line);cursor:pointer;font-size:13px;font-weight:700;color:var(--ink);box-shadow:var(--sh-1);transition:transform .14s var(--ease);}
.chip:active{transform:scale(.95);}
.chip.active{background:var(--brand-soft);border-color:var(--brand);color:var(--brand);}
.chip-av{width:26px;height:26px;border-radius:50%;background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff;display:grid;place-items:center;font-size:11px;font-weight:800;overflow:hidden;flex:0 0 auto;}
.chip-av img{width:100%;height:100%;object-fit:cover;display:block;}

.banner-ad-wrap{position:relative;display:flex;justify-content:center;align-items:center;width:100%;min-height:60px;padding:8px 12px;box-sizing:border-box;overflow:hidden;}
.banner-ad-wrap iframe{width:100%;max-width:400px;height:60px;border:0;display:block;background:transparent;border-radius:10px;}
.banner-ad-wrap.banner-ad-tight{ padding:6px 12px; }

.premium-photo-grid .premium-banner-ad{position:relative;grid-column:1 / -1;display:flex;justify-content:center;align-items:center;min-height:60px;border-radius:14px;overflow:hidden;background:var(--surface);border:1px solid var(--line);box-shadow:var(--sh-1);}
.premium-photo-grid .premium-banner-ad iframe{width:100%;height:60px;border:0;display:block;background:transparent;}

.ad-hit-overlay{position:absolute;inset:0;z-index:10;background:transparent;cursor:pointer;}

/* BOTTOM SHEET */
.bottom-sheet-overlay {
  position: absolute; inset: 0; z-index: 500;
  background: rgba(10,11,18,0.5); backdrop-filter: blur(4px);
  display: flex; align-items: flex-end;
  opacity: 0; pointer-events: none; transition: opacity 0.2s ease;
}
.bottom-sheet-overlay.on {
  opacity: 1; pointer-events: auto;
}
.bottom-sheet {
  width: 100%; background: var(--surface);
  border-radius: 24px 24px 0 0;
  padding: 24px; max-height: 50vh; overflow-y: auto;
  transform: translateY(100%); transition: transform 0.3s cubic-bezier(0.22, 0.9, 0.3, 1);
}
.bottom-sheet-overlay.on .bottom-sheet {
  transform: translateY(0);
}
.lang-option {
  display: flex; align-items: center; justify-content: space-between;
  padding: 16px; border-bottom: 1px solid var(--line);
  cursor: pointer; font-size: 15px; font-weight: 600; color: var(--ink);
}
.lang-option:last-child { border-bottom: none; }
.lang-option.active { color: var(--brand); }
.lang-option.active::after { content: "✓"; font-weight: 800; }

/* LOGIN SCREEN CSS */
#s-mobile-login {
  display: none;
  flex-direction: column;
  background: #000;
  color: #fff;
  height: 100%;
  width: 100%;
  position: absolute;
  inset: 0;
  z-index: 999;
}
#s-mobile-login.active { display: flex; }
.login-video-container {
  flex: 1;
  width: 100%;
  position: relative;
  background: #000;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.login-video-container video,
.login-video-container iframe {
  width: 100%;
  height: 100%;
  object-fit: cover;
  pointer-events: none; /* To allow tap events on container */
}
.login-form-container {
  padding: 24px 24px calc(40px + env(safe-area-inset-bottom));
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #000;
  position: relative;
  z-index: 2;
}
.login-input {
  width: 100%;
  max-width: 320px;
  height: 54px;
  background: #111;
  border: 2px solid #333;
  border-radius: 12px;
  color: #fff;
  font-size: 18px;
  font-weight: 600;
  text-align: center;
  outline: none;
  margin-bottom: 12px;
  letter-spacing: 1px;
}
.login-input:focus { border-color: #5B4CF0; }
.login-input::placeholder { color: #555; letter-spacing: normal; }
.login-btn {
  width: 100%;
  max-width: 320px;
  height: 54px;
  background: #5B4CF0;
  color: #fff;
  font-size: 18px;
  font-weight: 800;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  box-shadow: 0 8px 20px rgba(91,76,240,0.4);
  transition: transform 0.1s;
  text-transform: uppercase;
  margin-top: 8px;
}
.login-btn:active { transform: scale(0.96); }

body.dark-theme {
  --bg: #0A0B10; --surface: #141724; --surface-2: #1D2130;
  --ink: #F5F6FA; --ink-2: #A9AFC0; --muted: #7A8194; --line: #2A2F42;
  --brand: #7C6BFF; --brand-soft: #2A2550;
  --nav-bg: rgba(20,23,36,.70); --nav-border: rgba(255,255,255,.10);
  --search-bg: #141724; --search-border: #2A2F42;
  --float-bg: #1D2130; --float-border: #2A2F42;
  --shorts-chip-bg: #141724; --shorts-chip-text: #F5F6FA;
  --glass-bg: rgba(20,23,36,.72); --glass-border: rgba(255,255,255,.1);
  background: #0A0B10;
}
body.dark-theme .app { background: #0A0B10; }
body.dark-theme .screen { background: #0A0B10; }
body.dark-theme .playlist-large,
body.dark-theme .pcard,
body.dark-theme .app-ico.fallback,
body.dark-theme .shorts-item,
body.dark-theme .short-reel-cat,
body.dark-theme .channel-short-thumb,
body.dark-theme .pd-video-thumb,
body.dark-theme .ad-hero-art,
body.dark-theme .pd-unlock-inner,
body.dark-theme .bg-preview { background: #141724; }
body.dark-theme .app-ico img { box-shadow: 0 4px 12px rgba(0,0,0,.6); }
body.dark-theme .ad-hero-art::after { background:linear-gradient(180deg,rgba(10,11,16,.05) 0%,rgba(10,11,16,.55) 62%,var(--bg) 100%); }

@media (prefers-reduced-motion:reduce){
  *,*::before,*::after{animation-duration:.001s !important;transition-duration:.001s !important;}
}
</style>

<script>
if('serviceWorker' in navigator && location.protocol === 'https:'){
  const swCode = `
    const CACHE = 'learnify-thumbs-v2';
    const DB_NAME = 'learnify-idb';
    const STORE = 'thumbs';
    function idb(){return new Promise((res,rej)=>{const r=indexedDB.open(DB_NAME,1);r.onupgradeneeded=()=>r.result.createObjectStore(STORE);r.onsuccess=()=>res(r.result);r.onerror=()=>rej(r.error);});}
    async function idbGet(key){try{const db=await idb();return new Promise(res=>{const tx=db.transaction(STORE,'readonly');const req=tx.objectStore(STORE).get(key);req.onsuccess=()=>res(req.result);req.onerror=()=>res(null);});}catch(e){return null;}}
    async function idbPut(key,val){try{const db=await idb();return new Promise(res=>{const tx=db.transaction(STORE,'readwrite');tx.objectStore(STORE).put(val,key);tx.oncomplete=()=>res(true);tx.onerror=()=>res(false);});}catch(e){return false;}}
    self.addEventListener('install',e=>self.skipWaiting());
    self.addEventListener('activate',e=>e.waitUntil(clients.claim()));
    self.addEventListener('fetch',e=>{
      const url=e.request.url;
      const isImg=e.request.destination==='image'||/\\.(jpg|jpeg|png|webp|gif|avif)(\\?|$)/i.test(url);
      if(!isImg)return;
      e.respondWith((async()=>{
        const cache=await caches.open(CACHE);
        const hit=await cache.match(e.request);
        if(hit)return hit;
        const idbHit=await idbGet(url);
        if(idbHit){try{cache.put(e.request,new Response(idbHit));}catch(_){}return new Response(idbHit);}
        try{const res=await fetch(e.request);if(res&&res.ok){const clone=res.clone();try{cache.put(e.request,res.clone());}catch(_){}clone.blob().then(b=>idbPut(url,b)).catch(()=>{});}return res;}catch(err){return hit||Response.error();}
      })());
    });
  `;
  try{
    const blob = new Blob([swCode], {type:'application/javascript'});
    const url = URL.createObjectURL(blob);
    navigator.serviceWorker.register(url).catch(()=>{});
  }catch(e){}
}
</script>
</head>
<body>

<div class="app" id="app">
  <div class="screens" id="screens">

    <!-- NEW MOBILE LOGIN SCREEN -->
    <section class="screen" id="s-mobile-login">
      <div class="login-video-container" id="loginVideoContainer">
        <!-- Video injected here -->
      </div>
      <div class="login-form-container">
        <input type="text" id="userNameInput" class="login-input" placeholder="Enter Your Name">
        <input type="tel" id="mobileNumberInput" class="login-input" placeholder="Enter Mobile Number" maxlength="10" inputmode="numeric" pattern="[0-9]*">
        <button class="login-btn" id="goBtn" onclick="attemptMobileLogin()">GO</button>
      </div>
    </section>

    <section class="screen active" id="s-home">
      <div class="home-brand">
        <div class="brand-mark" id="homeBrandMark">N</div>
        <div>
          <div class="brand-hello">Welcome to Learnify</div>
          <div class="brand-name" id="homeBrandName">LEARNIFY</div>
        </div>
        <div class="home-banner-wrapper" id="homeBannerWrapper">
          <div class="home-banner-track" id="homeBannerTrack"></div>
        </div>
      </div>
      <div class="hero" id="homeHero" style="display:none">
        <div class="hero-track" id="heroTrack"></div>
        <div class="hero-foot"><div class="dots" id="heroDots"></div></div>
      </div>
      <div id="homeFeed"></div>
      <div id="homeEmpty" style="display:none">
        <div class="empty" style="padding-top:70px">
          <div class="empty-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="5" width="18" height="14" rx="3"/><path d="m10 9 5 3-5 3V9Z"/></svg></div>
          <h3>No content available</h3>
          <p>Content will appear here once it is uploaded.</p>
        </div>
      </div>
    </section>

    <!-- USER SETTINGS SCREEN -->
    <section class="screen" id="s-user-settings">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <div style="padding:64px 16px 20px">
        <h2 style="font-size:22px;font-weight:800;letter-spacing:-.03em">User Settings</h2>
        <p class="meta">Manage your profile and preferences</p>
      </div>
      <div class="group" style="margin-top: 10px;">
        <div style="padding: 16px;">
           <div class="field">
             <label>Full Name</label>
             <input id="usrName" class="input" type="text" placeholder="Enter your name">
           </div>
           <div class="field">
             <label>Mobile Number</label>
             <input id="usrPhone" class="input" type="tel" placeholder="Enter 10-digit number" maxlength="10" inputmode="numeric">
           </div>
           <div class="field">
             <label>Language</label>
             <button class="btn btn-secondary btn-block" onclick="showLanguageSheet()" id="usrLangBtn" style="justify-content: space-between;">Select Language <span>›</span></button>
           </div>
           <div class="field" style="display:flex; justify-content:space-between; align-items:center; margin-top:20px; padding: 10px 0;">
              <label style="margin-bottom:0;">Dark Mode</label>
              <button class="switch" id="usrThemeToggle" onclick="toggleTheme()"></button>
           </div>
           <button class="btn btn-primary btn-block" style="margin-top: 20px;" onclick="saveUserSettings()">Save Changes</button>
        </div>
      </div>
    </section>

    <section class="screen" id="s-search">
      <div class="banner-ad-wrap banner-ad-tight" data-ad-key="search-top"><iframe src="https://uplcm.com/4/11998765" loading="lazy" scrolling="no" frameborder="0"></iframe></div>
      <div class="page-title" style="padding-top:8px" id="searchTitle">Search</div>
      <div class="pad" style="margin-top:8px">
        <div class="searchbar">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="11" cy="11" r="7"/><path d="m20 20-3.2-3.2"/></svg>
          <input id="searchInput" placeholder="Search videos, shorts, playlists, apps..." autocomplete="off" autofocus>
          <button class="clear-btn" id="clearSearch" style="display:none" onclick="clearSearchInput()" aria-label="Clear"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.6" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg></button>
        </div>
      </div>
      <div id="searchInline"></div>
    </section>

    <section class="screen" id="s-results">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <div class="pad" style="padding-top:16px">
        <div class="searchbar">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="11" cy="11" r="7"/><path d="m20 20-3.2-3.2"/></svg>
          <input id="resultsInput" placeholder="Search..." autocomplete="off">
        </div>
      </div>
      <div id="resultsBody"></div>
    </section>

    <section class="screen" id="s-premium">
      <div class="banner-ad-wrap banner-ad-tight" data-ad-key="premium-top"><iframe src="https://uplcm.com/4/11998765" loading="lazy" scrolling="no" frameborder="0"></iframe></div>
      <div class="page-title" style="padding-top:8px" id="premiumTitle">Premium</div>
      <div class="page-subtitle" id="premiumSubtitle">Courses &amp; masterclasses</div>
      <div class="sec" id="secPhotoGrid" style="display:none">
        <div class="sec-head"><h2 class="sec-title">Explore</h2></div>
        <div class="premium-photo-grid" id="premiumPhotoGrid"></div>
      </div>
      <div id="premiumContent" style="display:none">
        <div class="sec" id="secPopPremium"><div class="sec-head"><h2 class="sec-title">Popular Premium</h2></div><div class="hscroll" id="rowPopPremium"></div></div>
        <div class="sec" id="secNewPremium"><div class="sec-head"><h2 class="sec-title">Premium Playlists</h2></div><div id="premiumList" style="padding: 0 16px 8px;"></div></div>
      </div>
    </section>

    <section class="screen" id="s-playlist">
      <div class="banner-ad-wrap banner-ad-tight" data-ad-key="playlist-top"><iframe src="https://uplcm.com/4/11998765" loading="lazy" scrolling="no" frameborder="0"></iframe></div>
      <div class="pd-player-header" id="pdPlayerHeader">
        <div class="pd-player-inner" id="pdPlayerInner"></div>
        <div class="pd-ad-slot" id="pdAdSlot"></div>
        <button class="icon-btn glass pd-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      </div>
      
      <div class="pd-actions" id="pdActionsBar"></div>
      
      <div class="pd-info"><h1 id="pdTitle">Playlist</h1><div class="pd-info-meta" id="pdInfoMeta"></div></div>
      <div class="pd-desc" id="pdDesc"></div>
      <div class="pd-list-head"><h2>Videos</h2><span id="pdListCount"></span></div>
      
      <div class="pd-list" id="pdList"></div>
      <div id="pdUnlockWrap"></div>
    </section>

    <section class="screen" id="s-player"><div id="playerBody"></div></section>
    <section class="screen" id="s-shortplayer"><div id="shortPlayerBody"></div></section>

    <section class="screen" id="s-channel">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <div id="channelBody"></div>
    </section>

    <section class="screen" id="s-subscriptions">
      <div class="banner-ad-wrap banner-ad-tight" data-ad-key="subs-top"><iframe src="https://uplcm.com/4/11998765" loading="lazy" scrolling="no" frameborder="0"></iframe></div>
      
      <div class="subs-hero" id="subsHero">
        <div class="subs-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg></div>
        <h1>Subscriptions</h1>
        <p>Channels you follow &amp; their content</p>
      </div>
      <div id="subsBody"></div>
    </section>

    <section class="screen" id="s-apps">
      <div class="banner-ad-wrap banner-ad-tight" data-ad-key="apps-top"><iframe src="https://uplcm.com/4/11998765" loading="lazy" scrolling="no" frameborder="0"></iframe></div>
      <div class="page-title" style="padding-top:8px">Apps</div>
      <div class="pad" style="margin-top:8px">
        <div class="searchbar" onclick="focusAppSearch()">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><circle cx="11" cy="11" r="7"/><path d="m20 20-3.2-3.2"/></svg>
          <input id="appSearch" placeholder="Search apps..." autocomplete="off">
        </div>
      </div>
      <div id="appsEmpty" style="display:none">
        <div class="empty" style="padding-top:60px">
          <div class="empty-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><rect x="3.4" y="3.4" width="7.2" height="7.2" rx="2.2"/><rect x="13.4" y="3.4" width="7.2" height="7.2" rx="2.2"/><rect x="3.4" y="13.4" width="7.2" height="7.2" rx="2.2"/><rect x="13.4" y="13.4" width="7.2" height="7.2" rx="2.2"/></svg></div>
          <h3>No apps available</h3>
          <p>Apps will appear here once they are published.</p>
        </div>
      </div>
      <div id="appsContent" style="display:none"><div class="sec" style="margin-top:14px"><div class="group" id="appsList"></div></div></div>
    </section>

    <section class="screen" id="s-appdetail"><div id="appDetailBody"></div></section>

    <section class="screen" id="s-ai">
      <header class="ai-top">
        <div class="ai-id">
          <div class="ai-mark"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3.2l1.9 5 5 1.9-5 1.9-1.9 5-1.9-5-5-1.9 5-1.9 1.9-5Z"/><path d="M18.8 16.4l.8 2.1 2.1.8-2.1.8-.8 2.1-.8-2.1-2.1-.8 2.1-.8.8-2.1Z"/></svg></div>
          <div><div class="ai-name">AI Assistant</div><div class="ai-status"><span style="background:#12A150;width:6px;height:6px;border-radius:50%;display:inline-block"></span> Nova 2.4 · Ready</div></div>
        </div>
        <div style="display:flex;gap:8px">
          <button class="icon-btn" onclick="go('aihistory')" aria-label="Chat history"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M3 12a9 9 0 1 0 3-6.7"/><path d="M3 4v5h5"/><path d="M12 8v4l3 2"/></svg></button>
          <button class="icon-btn" onclick="newChat()" aria-label="New chat"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M12 5v14M5 12h14"/></svg></button>
        </div>
      </header>
      <div class="chat" id="chatArea"></div>
      <div class="composer"><div class="composer-inner"><textarea id="chatInput" rows="1" placeholder="Ask anything..."></textarea><button class="send-btn" id="sendBtn" onclick="sendMessage()" aria-label="Send"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h13"/><path d="m12 5 7 7-7 7"/></svg></button></div></div>
    </section>

    <section class="screen" id="s-aihistory">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <div style="padding:64px 16px 0"><h2 style="font-size:22px;font-weight:800;letter-spacing:-.03em;margin-bottom:4px">Chat History</h2><p class="meta">Your recent AI conversations</p></div>
      <div class="sec"><div class="sec-head"><h2 class="sec-title">Recent</h2><button class="sec-link" onclick="confirmClearChats()">Clear all</button></div><div class="group" id="chatHistoryList"></div></div>
    </section>

    <section class="screen" id="s-profile">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <button class="float-back" style="left:auto;right:14px" onclick="go('settings')" aria-label="Settings"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.7 1.7 0 0 0 .3 1.9l.1.1a2 2 0 1 1-2.8 2.8l-.1-.1a1.7 1.7 0 0 0-2.9 1.2 2 2 0 1 1-4 0 1.7 1.7 0 0 0-2.9-1.2l-.1.1a2 2 0 1 1-2.8-2.8l.1-.1A1.7 1.7 0 0 0 3 15a2 2 0 1 1 0-4 1.7 1.7 0 0 0 1.2-2.9l-.1-.1a2 2 0 1 1 2.8-2.8l.1.1A1.7 1.7 0 0 0 10 4.6a2 2 0 1 1 4 0 1.7 1.7 0 0 0 2.9 1.2l.1-.1a2 2 0 1 1 2.8 2.8l-.1.1A1.7 1.7 0 0 0 21 11a2 2 0 1 1 0 4Z"/></svg></button>
      <div class="profile-hero">
        <div class="profile-av" id="profileAvatar">A<div class="edit-dot"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4Z"/></svg></div></div>
        <h1 id="profileName">Guest User</h1>
        <p id="profileEmail">Guest Mode</p>
        <button class="btn btn-secondary btn-sm" onclick="showToast('Profile locked in Guest Mode','info')">Edit Profile</button>
      </div>
      <div class="stat-row"><div class="stat-cell"><b>0h</b><span>Watched</span></div><div class="stat-cell"><b>0</b><span>Saved</span></div><div class="stat-cell"><b>0</b><span>Courses</span></div></div>
      <div class="section-label">Library</div>
      <div class="group">
        <div class="row-item" onclick="showToast('Opening your playlists','info')"><div class="ri-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M3 6h13M3 12h13M3 18h9"/><path d="m17 14 5 3-5 3v-6Z"/></svg></div><div class="ri-txt"><h4>My Playlists</h4><p>0 saved collections</p></div><div class="ri-chev"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg></div></div>
        <div class="row-item" onclick="go('premium')"><div class="ri-ico gold"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2l2.4 6.6L21 11l-6.6 2.4L12 20l-2.4-6.6L3 11l6.6-2.4L12 2Z"/></svg></div><div class="ri-txt"><h4>Premium</h4><p>Manage your subscription</p></div><div class="ri-chev"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg></div></div>
        <div class="row-item" onclick="go('aihistory')"><div class="ri-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12a8 8 0 0 1-8 8H7l-4 3v-6.5A8 8 0 0 1 3 12a8 8 0 0 1 8-8h2a8 8 0 0 1 8 8Z"/></svg></div><div class="ri-txt"><h4>AI History</h4><p>Recent conversations</p></div><div class="ri-chev"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg></div></div>
      </div>
      <div class="section-label">Account</div>
      <div class="group">
        <div class="row-item" onclick="go('settings')"><div class="ri-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="3"/><path d="M12 2v3M12 19v3M2 12h3M19 12h3M4.9 4.9l2.1 2.1M17 17l2.1 2.1M19.1 4.9 17 7M7 17l-2.1 2.1"/></svg></div><div class="ri-txt"><h4>Settings</h4><p>Playback, downloads, privacy</p></div><div class="ri-chev"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg></div></div>
      </div>
    </section>

    <section class="screen" id="s-settings">
      <button class="float-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
      <div style="padding:64px 16px 0"><h2 style="font-size:22px;font-weight:800;letter-spacing:-.03em">Settings</h2></div>
      <div class="section-label">Appearance</div>
      <div class="group">
        <div class="row-item" style="flex-direction:column;align-items:stretch;gap:10px;cursor:default">
          <div style="display:flex;align-items:center;gap:13px"><div class="ri-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="3"/><circle cx="8.5" cy="8.5" r="1.5"/><path d="m21 15-5-5L5 21"/></svg></div><div class="ri-txt"><h4>Background image</h4><p>Paste any image URL</p></div></div>
          <div class="bg-preview" id="bgPreview"><span>No background set</span></div>
          <div style="display:flex;gap:8px"><input class="input" id="bgUrlInput" type="url" placeholder="https://..." style="height:44px;font-size:13px;flex:1" autocomplete="off"><button class="btn btn-primary btn-sm" onclick="applyBgFromInput()" style="height:44px;padding:0 18px">Apply</button></div>
          <div style="display:flex;gap:8px"><button class="btn btn-secondary btn-sm" onclick="setAppBackground('')" style="flex:1">Reset</button><button class="btn btn-secondary btn-sm" onclick="setAppBackground('#F5F6FA')" style="flex:1">Default</button></div>
        </div>
      </div>
    </section>

  </div>

  <nav class="nav" id="bottomNav">
    <button class="nav-item active" data-tab="home" onclick="tab('home')"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.85" stroke-linecap="round" stroke-linejoin="round"><path d="M3 10.4 12 3.2l9 7.2"/><path d="M5.6 9.4V20a1 1 0 0 0 1 1h10.8a1 1 0 0 0 1-1V9.4"/><path d="M9.6 21v-5.6h4.8V21"/></svg><span>Home</span></button>
    <button class="nav-item" data-tab="search" onclick="tab('search')"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.85" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="7"/><path d="m20 20-3.4-3.4"/></svg><span>Search</span></button>
    <button class="nav-item" data-tab="premium" onclick="tab('premium')"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.85" stroke-linecap="round" stroke-linejoin="round"><path d="M3.5 8.2 7.8 11l4.2-6.6L16.2 11l4.3-2.8-1.7 11.2H5.2L3.5 8.2Z"/></svg><span>Premium</span></button>
    <button class="nav-item" data-tab="subs" onclick="tab('subscriptions')"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.85" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg><span>Subs</span></button>
    <button class="nav-item" data-tab="app" onclick="tab('apps')"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.85" stroke-linecap="round" stroke-linejoin="round"><rect x="3.4" y="3.4" width="7.2" height="7.2" rx="2.2"/><rect x="13.4" y="3.4" width="7.2" height="7.2" rx="2.2"/><rect x="3.4" y="13.4" width="7.2" height="7.2" rx="2.2"/><rect x="13.4" y="13.4" width="7.2" height="7.2" rx="2.2"/></svg><span>Apps</span></button>
  </nav>

  <div class="toast-wrap" id="toastWrap"></div>
  <div class="overlay" id="overlay" onclick="if(event.target===this)closeModal()"><div class="modal"><h3 id="modalTitle">Title</h3><p id="modalBody">Body</p><div class="modal-actions"><button class="btn btn-secondary" onclick="closeModal()">Cancel</button><button class="btn btn-primary" id="modalConfirm">Confirm</button></div></div></div>
  <div class="overlay" id="authOverlay" onclick="if(event.target===this)closeAuthModal()"><div class="modal" id="authModalBody" style="max-width:380px"></div></div>
  <div class="lightbox" id="lightbox" onclick="closeLightbox()"><button class="lb-close" aria-label="Close">✕</button><div id="lbInner"></div></div>
  <div class="short-reel-anim" id="likeAnim"><video id="likeAnimVideo" muted playsinline preload="auto" webkit-playsinline></video></div>
  <div class="sub-anim" id="subAnim"><div class="sub-bell">🔔</div><div class="sub-text">Subscribed</div></div>
  
  <!-- LANGUAGE BOTTOM SHEET -->
  <div id="langSheet" class="bottom-sheet-overlay" onclick="if(event.target===this)closeLanguageSheet()">
    <div class="bottom-sheet">
      <h3 style="font-size: 18px; font-weight: 800; margin-bottom: 16px;">Select Language</h3>
      <div class="lang-list" id="langList"></div>
    </div>
  </div>
</div>

<script>
const firebaseConfig = {
  apiKey: "AIzaSyCBTiRAMz3fkJelDDBUD7BcU12kzTwJJqo",
  authDomain: "satyam-aa701.firebaseapp.com",
  databaseURL: "https://satyam-aa701-default-rtdb.firebaseio.com",
  projectId: "satyam-aa701",
  storageBucket: "satyam-aa701.firebasestorage.app",
  messagingSenderId: "124086359001",
  appId: "1:124086359001:web:e360618a3631d913667fc8"
};
let firebaseApp = null, db = null, auth = null;
let firebaseReady = false, firebaseUser = null, firebaseAuthReady = false;
let firebaseInitPromise = null;
let firebaseInitError = null;
let pendingAfterAuth = null;
const FIREBASE_SDK = "https://www.gstatic.com/firebasejs/10.12.2";
async function loadFirebaseModules(){
  const [appMod, dbMod, authMod] = await Promise.all([
    import(FIREBASE_SDK + "/firebase-app.js"),
    import(FIREBASE_SDK + "/firebase-database.js"),
    import(FIREBASE_SDK + "/firebase-auth.js")
  ]);
  return { appMod, dbMod, authMod };
}
function initFirebaseOnce(){
  if(firebaseInitPromise) return firebaseInitPromise;
  firebaseInitPromise = (async () => {
    try{
      const { appMod, dbMod, authMod } = await loadFirebaseModules();
      firebaseApp = appMod.initializeApp(firebaseConfig);
      const rtdb = dbMod.getDatabase(firebaseApp);
      const authReal = authMod.getAuth(firebaseApp);
      db = {
        ref(path){
          const r = dbMod.ref(rtdb, path);
          return {
            on(eventType, cb, errCb){ return dbMod.onValue(r, snap => cb({ val: () => snap.val() }), errCb); },
            once(){ return dbMod.get(r).then(snap => ({ val: () => snap.val() })); },
            update(data){ return dbMod.update(r, data); },
            set(data){ return dbMod.set(r, data); },
            remove(){ return dbMod.remove(r); }
          };
        },
        ServerValue: { TIMESTAMP: dbMod.serverTimestamp() }
      };
      // Guest anonymous login
      const googleProvider = new authMod.GoogleAuthProvider();
      googleProvider.setCustomParameters({ prompt: 'select_account' });
      auth = {
        onAuthStateChanged(cb, errCb){ return authMod.onAuthStateChanged(authReal, cb, errCb); },
        createUserWithEmailAndPassword(email, pw){ return authMod.createUserWithEmailAndPassword(authReal, email, pw); },
        signInWithEmailAndPassword(email, pw){ return authMod.signInWithEmailAndPassword(authReal, email, pw); },
        signOut(){ return authMod.signOut(authReal); },
        signInWithPopup(){ return authMod.signInWithPopup(authReal, googleProvider); },
        signInWithRedirect(){ return authMod.signInWithRedirect(authReal, googleProvider); },
        getRedirectResult(){ return authMod.getRedirectResult(authReal); },
        signInAnonymously(){ return authMod.signInAnonymously(authReal); }, // Added for guest
        get currentUser(){ return authReal.currentUser; }
      };
      firebaseReady = true;
      firebaseInitError = null;
      console.log("✅ Firebase initialized successfully");
      
      // Auto anonymous sign in for guest mode
      if(!auth.currentUser) {
        try { await auth.signInAnonymously(); } catch(e) { console.warn("Anon auth failed", e); }
      }

      const finishAuth = u => {
        firebaseUser = u || null;
        firebaseAuthReady = true;
        if(firebaseUser){
          try{
            const existing = localStorage.getItem('learnifyUser');
            const parsed = existing ? JSON.parse(existing) : null;
            if(!parsed || parsed.uid !== u.uid){
              const profile = { uid: u.uid, email: u.email || '', name: u.displayName || (u.email ? displayNameFromEmail(u.email) : 'Guest User'), photoURL: u.photoURL || '', signedIn: true, provider: 'guest', updatedAt: Date.now() };
              saveLocalUser(profile);
              applyLocalProfile(profile);
            } else { applyLocalProfile(parsed); }
          }catch(e){}
          loadFirebaseUserProfile();
          syncUserDataFromFirebase(u.uid);
        }
        listenFirebaseData();
        if(typeof pendingAfterAuth === "function"){ try{ pendingAfterAuth(firebaseUser); }catch(e){} pendingAfterAuth = null; }
      };
      auth.onAuthStateChanged(finishAuth, () => { firebaseUser = null; firebaseAuthReady = true; listenFirebaseData(); });
      return firebaseUser;
    }catch(e){ 
      console.error("❌ Firebase init failed:", e); 
      firebaseInitError = e;
      firebaseReady = false; 
      firebaseAuthReady = true; 
      return null; 
    }
  })();
  return firebaseInitPromise;
}
(function startFirebaseLazy(){
  const boot = () => {
    if(window.__firebaseStarted) return;
    window.__firebaseStarted = true;
    initFirebaseOnce().then(() => { if(db) listenFirebaseData(); });
  };
  if('requestIdleCallback' in window){ requestIdleCallback(boot, {timeout: 1800}); }
  else if(document.readyState === 'complete'){ setTimeout(boot, 400); }
  else { window.addEventListener('load', () => setTimeout(boot, 250), {once:true}); }
})();
</script>

<script>
let VIDEOS = [], PLAYLISTS = [], APPS = [], PREMIUM = [], HERO_SLIDES = [], SHORTS = [];
let PREMIUM_PHOTOS = [];
let ADS = [];
let SHORT_ADS = [];
let SCHEDULED_VIDEOS = [];

let SOUND_ON = false;
try{ SOUND_ON = localStorage.getItem('learnifySound') === '1'; }catch(e){}

let APP_OVERRIDES = {};
let GLOBAL_THEME = 'light';
let GLOBAL_HEADER_BANNERS = [];

const LIGHT_THEME = {
  bg: '#F5F6FA', surface: '#FFFFFF', surface2: '#EFF1F7',
  ink: '#0E1016', ink2: '#3A3F4B', muted: '#7A8194', line: '#E7E9F0',
  brand: '#5B4CF0', brand2: '#7C6BFF', brandSoft: '#EEECFE',
  navBg: 'rgba(255,255,255,.70)', navBorder: 'rgba(255,255,255,.75)',
  navText: '#8A90A2', navActive: '#5B4CF0',
  glassBg: 'rgba(255,255,255,.72)', glassBorder: 'rgba(255,255,255,.55)',
  softWhite: 'rgba(255,255,255,.92)', softWhite2: 'rgba(255,255,255,.85)',
  floatBg: 'rgba(255,255,255,.92)', floatBorder: 'rgba(255,255,255,.75)',
  searchBg: '#FFFFFF', searchBorder: '#E7E9F0', searchText: '#0E1016', searchPlaceholder: '#A6ACBD',
  shortsChipBg: 'rgba(255,255,255,.92)', shortsChipText: '#0E1016',
  shortsPlayBg: 'rgba(255,255,255,.85)', thumbPlayBg: 'rgba(255,255,255,.92)'
};
const DARK_THEME = {
  bg: '#0A0B10', surface: '#141724', surface2: '#1D2130',
  ink: '#F5F6FA', ink2: '#A9AFC0', muted: '#7A8194', line: '#2A2F42',
  brand: '#7C6BFF', brand2: '#9B5BF0', brandSoft: '#2A2550',
  navBg: 'rgba(20,23,36,.70)', navBorder: 'rgba(255,255,255,.10)',
  navText: '#7A8194', navActive: '#7C6BFF',
  glassBg: 'rgba(20,23,36,.72)', glassBorder: 'rgba(255,255,255,.1)',
  softWhite: '#1D2130', softWhite2: '#2A2F42',
  floatBg: '#1D2130', floatBorder: '#2A2F42',
  searchBg: '#141724', searchBorder: '#2A2F42', searchText: '#F5F6FA', searchPlaceholder: '#A9AFC0',
  shortsChipBg: '#141724', shortsChipText: '#F5F6FA',
  shortsPlayBg: '#1D2130', thumbPlayBg: 'rgba(255,255,255,.85)'
};

const DEFAULT_AD_URL = 'https://uplcm.com/4/11998765';
let GLOBAL_AD_URLS = {};

function getAdUrl(key){
  if(!key) return DEFAULT_AD_URL;
  return GLOBAL_AD_URLS[key] || DEFAULT_AD_URL;
}
function saveAdUrl(key, url){
  if(!key) return;
  const clean = url && url.trim() ? url.trim() : DEFAULT_AD_URL;
  if(clean === DEFAULT_AD_URL) delete GLOBAL_AD_URLS[key];
  else GLOBAL_AD_URLS[key] = clean;
  try{ localStorage.setItem('learnifyAdUrls', JSON.stringify(GLOBAL_AD_URLS)); }catch(e){}
  if(db){
    try{ db.ref('learnify/adUrls').set(GLOBAL_AD_URLS); }catch(e){ console.warn('adUrls push failed:', e); }
  }
  refreshAllAds();
}
function refreshAllAds(){
  document.querySelectorAll('[data-ad-key]').forEach(wrap => {
    const key = wrap.dataset.adKey;
    const iframe = wrap.querySelector('iframe');
    if(!iframe) return;
    const url = getAdUrl(key);
    try{
      const current = iframe.getAttribute('src') || '';
      if(current !== url) iframe.setAttribute('src', url);
    }catch(e){}
  });
  setTimeout(() => { if(window.__setupAdTripleTap) window.__setupAdTripleTap(); }, 100);
}
window.__refreshAllAds = refreshAllAds;

function getPlaylistLikedSet(){ return readSetCache('learnifyPlaylistLikes'); }
function savePlaylistLikedSet(set){ writeSetCache('learnifyPlaylistLikes', set); }
function isPlaylistLiked(id){ if(!id) return false; return getPlaylistLikedSet().has(String(id)); }
async function togglePlaylistLike(id){
  if(!id) return false;
  const k = String(id);
  const set = getPlaylistLikedSet();
  let nowLiked;
  if(set.has(k)){ set.delete(k); nowLiked = false; }
  else { set.add(k); nowLiked = true; }
  savePlaylistLikedSet(set);
  const uid = currentUid();
  if(uid && db){
    try{
      const update = {};
      update[k] = nowLiked ? true : null;
      await db.ref('learnify/users/' + uid + '/playlistLikes').update(update);
    }catch(e){ console.warn('playlist like sync failed:', e); }
  }
  return nowLiked;
}
function getPlaylistLikeCount(p){
  if(!p) return 0;
  const base = Number(p.likes || 0);
  return base + (isPlaylistLiked(p.id) ? 1 : 0);
}

function getPlaylistChannel(p){
  if(!p) return '';
  return String(p.channel || p.creator || p.cat || 'general').toLowerCase().trim();
}
function getPlaylistChannelDisplay(p){
  if(!p) return 'General';
  const raw = String(p.channel || p.creator || p.cat || 'General').trim();
  const disp = getChannelDisplay(raw.toLowerCase(), raw);
  return disp.name || raw;
}

function loadAdminLocalFallback(){
  try{
    const raw = localStorage.getItem('cp_data_v1');
    if(!raw) return false;
    const d = JSON.parse(raw);
    if(!d || typeof d !== 'object') return false;
    if(Array.isArray(d.playlists) && d.playlists.length){ PLAYLISTS = d.playlists.map((v,i)=>makePlaylist(v, v.id || ('p'+i), i)).filter(Boolean); PREMIUM = PLAYLISTS.filter(p => p.premium); }
    if(Array.isArray(d.apps) && d.apps.length){ APPS = d.apps.map((v,i)=>makeApp(v, v.id || ('a'+i), i)).filter(Boolean); }
    if(Array.isArray(d.sliders) && d.sliders.length){ HERO_SLIDES = d.sliders.filter(x => x && x.active !== false).map((v,i)=>makeSlider(v,i)).filter(Boolean); }
    if(Array.isArray(d.shorts) && d.shorts.length){
      SHORTS = d.shorts.map((v,i)=>{
        const videoUrl = v.videoUrl || v.videoURL || v.video || v.link || v.url || v.src || v.videoLink || v.embed || '';
        let thumb = v.thumbnail || v.thumbnailUrl || v.image || v.imageUrl || v.thumb || v.photo || '';
        if (!thumb && videoUrl) { const info = normalizeVideoUrl(videoUrl); thumb = info.thumbnail || ''; }
        return { id: v.id || ('sh'+(i+1)), t: v.title || v.t || v.name || 'Short', thumb: thumb, dur: v.dur || v.duration || '', tag: v.tag || v.category || v.cat || 'Short', videoUrl: videoUrl, d: v.d || v.description || v.desc || '', views: Number(v.views || v.viewCount || v.view || 0) || 0 };
      }).filter(s=>s.videoUrl);
    }
    if(Array.isArray(d.videos) && d.videos.length){ VIDEOS = d.videos.map((v,i)=>makeVideo(v, v.id || ('v'+i), i)).filter(Boolean); }
    if(Array.isArray(d.shortAds) && d.shortAds.length){
      SHORT_ADS = d.shortAds.filter(a => a && a.videoUrl).map(a => ({
        id: String(a.id || ''),
        title: a.title || 'Sponsored',
        videoUrl: a.videoUrl || '',
        clickLink: a.clickLink || '',
        active: a.active !== false
      }));
    }
    if(Array.isArray(d.scheduledPlaylistVideos) && d.scheduledPlaylistVideos.length){
      SCHEDULED_VIDEOS = d.scheduledPlaylistVideos.filter(v => v && v.videoUrl).map(v => ({
        id: String(v.id || ''),
        title: v.title || 'Advertisement',
        videoUrl: v.videoUrl || '',
        thumbnail: v.thumbnail || ''
      }));
    }
    if(Array.isArray(d.premiumPhotos) && d.premiumPhotos.length){
      PREMIUM_PHOTOS = d.premiumPhotos.filter(p => p && p.image).map((v,i) => ({ id: String(v.id || ('ph'+i)), image: String(v.image || ''), link: String(v.link || v.url2 || ''), title: String(v.title || ''), badge: String(v.badge || ''), order: Number(v.order || i), active: v.active !== false }));
    }
    if(Array.isArray(d.ads) && d.ads.length){ ADS = d.ads.filter(a => a && a.image).map((v,i) => ({ id: String(v.id || ('ad'+i)), image: String(v.image || ''), link: String(v.link || v.url2 || ''), title: String(v.title || ''), active: v.active !== false })); }
    if(d.appSettings && typeof d.appSettings === 'object'){ applyAppSettings(d.appSettings); }
    window.VIDEOS=VIDEOS; window.PLAYLISTS=PLAYLISTS; window.APPS=APPS; window.SHORTS=SHORTS; window.PREMIUM_PHOTOS=PREMIUM_PHOTOS;
    return true;
  }catch(e){ console.warn('Admin local fallback failed:', e); return false; }
}

let CHAT_HISTORY = [];
let AI_REPLIES = [
  "Here's a clean way to approach it: start with the smallest version that still proves the idea, then layer polish only once the structure holds.",
  "Great question. I'd break it into three parts — the goal, the constraint, and the trade-off you're willing to accept. Which one matters most right now?",
  "Based on your library, I'd start with the first item in your saved videos — it covers exactly the foundation you're describing.",
  "I can turn that into a step-by-step checklist for the week. Want me to also pull the two most relevant videos from your saved playlists?"
];
const $  = (s, r=document) => r.querySelector(s);
const $$ = (s, r=document) => Array.from(r.querySelectorAll(s));
const esc = s => String(s==null?'':s).replace(/[&<>"']/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
const __memCache = new Map();

let GLOBAL_HOME_BRAND = null;
let GLOBAL_CHANNEL_BRANDS = {};
let GLOBAL_SUBS_BRAND = null;
let GLOBAL_SUBS_BG = null;
let GLOBAL_PLAYLIST_BG = null;
let GLOBAL_SEARCH_TITLE = 'Search';
let GLOBAL_PREMIUM_TITLE = 'Premium';
let GLOBAL_PREMIUM_SUBTITLE = 'Courses & masterclasses';

(function preloadBrandCache(){
  try{ const h = localStorage.getItem('learnifyBrand'); if(h) GLOBAL_HOME_BRAND = JSON.parse(h); }catch(e){}
  try{ const c = localStorage.getItem('learnifyChannelBrand'); if(c) GLOBAL_CHANNEL_BRANDS = JSON.parse(c) || {}; }catch(e){}
  try{ const s = localStorage.getItem('learnifySubsBrand'); if(s) GLOBAL_SUBS_BRAND = JSON.parse(s); }catch(e){}
  try{ const sb = localStorage.getItem('learnifySubsBg'); if(sb) GLOBAL_SUBS_BG = JSON.parse(sb); }catch(e){}
  try{ const pb = localStorage.getItem('learnifyPlaylistBg'); if(pb) GLOBAL_PLAYLIST_BG = JSON.parse(pb); }catch(e){}
  try{ const t = localStorage.getItem('learnifyTheme'); if(t) GLOBAL_THEME = t; }catch(e){}
  try{ const st = localStorage.getItem('learnifySearchTitle'); if(st) GLOBAL_SEARCH_TITLE = st; }catch(e){}
  try{ const pt = localStorage.getItem('learnifyPremiumTitle'); if(pt) GLOBAL_PREMIUM_TITLE = pt; }catch(e){}
  try{ const ps = localStorage.getItem('learnifyPremiumSubtitle'); if(ps) GLOBAL_PREMIUM_SUBTITLE = ps; }catch(e){}
  try{ const au = localStorage.getItem('learnifyAdUrls'); if(au) GLOBAL_AD_URLS = JSON.parse(au) || {}; }catch(e){}
  try{ const hb = localStorage.getItem('learnifyHeaderBanners'); if(hb) GLOBAL_HEADER_BANNERS = JSON.parse(hb) || []; }catch(e){}
})();

function getChannelBrandData(base){
  if(!base) return null;
  const k = String(base).toLowerCase().trim();
  return GLOBAL_CHANNEL_BRANDS[k] || null;
}
function getChannelDisplay(base, fallbackName){
  const b = getChannelBrandData(base);
  const nm = (b && b.name && String(b.name).trim()) ? String(b.name).trim() : (fallbackName || base || 'Channel');
  const ic = (b && b.icon) ? safeUrl(b.icon) : '';
  return { name: nm, icon: ic };
}

function pushHomeBrandToFirebase(){
  if(!db) return;
  try{
    if(GLOBAL_HOME_BRAND && (GLOBAL_HOME_BRAND.name || GLOBAL_HOME_BRAND.icon || GLOBAL_HOME_BRAND.welcome)){
      db.ref('learnify/brand').set(GLOBAL_HOME_BRAND);
    } else {
      db.ref('learnify/brand').remove();
    }
  }catch(e){ console.warn('brand push failed:', e); }
}
function pushChannelBrandToFirebase(base, data){
  if(!db || !base) return;
  const k = String(base).toLowerCase().trim();
  try{
    const upd = {};
    if(data && (data.name || data.icon)){
      upd[k] = data;
      db.ref('learnify/channelBrands').update(upd);
    } else {
      upd[k] = null;
      db.ref('learnify/channelBrands').update(upd);
    }
  }catch(e){ console.warn('channel brand push failed:', e); }
}

function refreshAllChannelBrands(){
  try{ if(typeof currentChannelTag !== 'undefined' && currentChannelTag){ applyChannelBrand(currentChannelTag); } }catch(e){}
  const reels = document.querySelectorAll('#shortPlayerBody .short-reel');
  reels.forEach(reel => {
    const sid = reel.dataset.shortId;
    if(!sid) return;
    const s = SHORTS.find(x => String(x.id) === String(sid));
    if(!s) return;
    const base = getBaseTag(s.tag);
    const disp = getChannelDisplay(base, s.tag);
    const iconUrl = disp.icon;
    const displayName = disp.name;
    const initial = (displayName.charAt(0)||'S').toUpperCase();
    const av   = reel.querySelector('.short-reel-channel-avatar');
    const nmEl = reel.querySelector('.short-reel-channel > span');
    const catEl = reel.querySelector('.short-reel-cat');
    if(av){
      if(iconUrl){ av.innerHTML = `<img src="${esc(iconUrl)}" alt="" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${initial}'">`; }
      else { av.textContent = initial; }
    }
    if(nmEl) nmEl.textContent = displayName;
    if(catEl){
      const cur = catEl.textContent || '';
      const suffixMatch = cur.match(/(\s*·\s*\d+\/\d+)$/);
      const suffix = suffixMatch ? suffixMatch[1] : '';
      catEl.textContent = displayName + suffix;
    }
  });
  try{ renderHomeThrottled(); }catch(e){}
}

function readJSONCache(key, fallback){ if(__memCache.has(key)) return __memCache.get(key); let val = fallback; try{ const raw = localStorage.getItem(key); if(raw != null) val = JSON.parse(raw); }catch(e){ val = fallback; } __memCache.set(key, val); return val; }
function writeJSONCache(key, val){ __memCache.set(key, val); try{ localStorage.setItem(key, JSON.stringify(val)); }catch(e){} }
function dropJSONCache(key){ __memCache.delete(key); try{ localStorage.removeItem(key); }catch(e){} }
function readSetCache(key){ const cached = __memCache.get(key); if(cached instanceof Set) return cached; let arr = []; try{ const raw = localStorage.getItem(key); if(raw) arr = JSON.parse(raw); }catch(e){ arr = []; } const s = new Set(Array.isArray(arr) ? arr.map(String) : []); __memCache.set(key, s); return s; }
function writeSetCache(key, set){ __memCache.set(key, set); try{ localStorage.setItem(key, JSON.stringify([...set])); }catch(e){} }

const NAVMAP = { home:'home', search:'search', results:'search', premium:'premium', playlist:'home', player:'home', apps:'app', appdetail:'app', ai:'ai', aihistory:'ai', shortplayer:'home', channel:'home', subscriptions:'subs', 'user-settings':'home' };
let navStack = [];
let lastTab = 'home';
function show(id){
  const target = document.getElementById('s-' + id);
  if(!target) return;
  if(id !== 'playlist'){ try{ stopPlaylistTimer(); }catch(e){} }
  $$('.screen').forEach(s => s.classList.toggle('active', s === target));
  target.scrollTop = 0;
  const bottomNav = $('#bottomNav');
  if (bottomNav) {
    const hideNav = (id === 'shortplayer' || id === 'mobile-login');
    bottomNav.style.display = hideNav ? 'none' : 'grid';
  }
  const mapped = NAVMAP[id];
  if(mapped){
    lastTab = mapped;
    $$('.nav-item').forEach(n => { const on = n.dataset.tab === mapped; n.classList.toggle('active', on); if(on){ n.classList.remove('pulse'); void n.offsetWidth; n.classList.add('pulse'); } });
  }
  if(id === 'ai') scrollChat();
  if(id === 'premium'){ try{ renderPremium(); }catch(e){} }
  if(id === 'apps'){ try{ renderApps(); }catch(e){} }
  if(id === 'subscriptions'){ try{ renderSubscriptions(); }catch(e){} }
  if(id === 'search') setTimeout(() => { const el = $('#searchInput'); if(el) el.focus(); }, 100);
  if(id === 'playlist' || id === 'premium' || id === 'subscriptions' || id === 'apps' || id === 'search'){
    setTimeout(() => { if(window.__refreshAllAds) window.__refreshAllAds(); }, 50);
  }
}
function go(id){ const cur = $('.screen.active'); if(cur && cur.id !== 's-' + id) navStack.push(cur.id.slice(2)); show(id); }
function back(){ try{ cleanupShortsReels(); }catch(e){} const prev = navStack.pop() || lastTab; show(prev); }
function tab(id){ try{ cleanupShortsReels(); }catch(e){} navStack = []; lastTab = id; if(id === 'search') resetSearchScreen(); if(id === 'ai') scrollChat(); show(id); }

function cleanVideoInput(value){
  let s = String(value == null ? '' : value).trim();
  if(!s) return '';
  const iframeMatch = s.match(/<iframe[^>]+(?:src|data-src)=[\"']([^\"']+)[\"'][^>]*>/i);
  if(iframeMatch && iframeMatch[1]) s = iframeMatch[1].trim();
  s = s.replace(/^[a-z]{1,4}(?=https?:\/\/)/i, '');
  s = s.replace(/^(?:url|link)\s*[:=]\s*/i, '');
  s = s.replace(/^['\"`\s]+|['\"`\s]+$/g, '');
  return s.trim();
}
function youtubeId(url){
  const u = String(url||'').trim(); if(!u) return '';
  if(/^[A-Za-z0-9_-]{11}$/.test(u)) return u;
  try{ const parsed = new URL(u, location.href); const host = parsed.hostname.toLowerCase().replace(/^www\./,'').replace(/^m\./,'').replace(/^music\./,''); if(host === 'youtu.be') return (parsed.pathname.split('/').filter(Boolean)[0] || '').split(/[?#]/)[0]; if(host === 'youtube.com' || host === 'youtube-nocookie.com'){ const v = parsed.searchParams.get('v'); if(v && /^[A-Za-z0-9_-]{11}$/.test(v)) return v; const parts = parsed.pathname.split('/').filter(Boolean); if(['embed','shorts','live','v','e'].includes(parts[0])){ const id = (parts[1]||'').split(/[?#]/)[0]; if(/^[A-Za-z0-9_-]{11}$/.test(id)) return id; } } }catch(e){}
  const m = u.match(/(?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:watch\?(?:.*&)?v=|embed\/|shorts\/|live\/|v\/|e\/))([A-Za-z0-9_-]{11})/i);
  return m ? m[1] : '';
}
function vimeoId(url){ const u = String(url||'').trim(); if(!u) return ''; const m = u.match(/vimeo\.com\/(?:video\/)?(\d+)/i); return m ? m[1] : ''; }
function instagramId(url){ const u = String(url||'').trim(); if(!u) return ''; const m = u.match(/instagram\.com\/(?:reel|reels|p|tv)\/([A-Za-z0-9_-]+)/i); return m ? m[1] : ''; }
function instagramType(url){ const u = String(url||'').trim(); if(/instagram\.com\/reels?\//i.test(u)) return 'reel'; if(/instagram\.com\/tv\//i.test(u)) return 'tv'; if(/instagram\.com\/p\//i.test(u)) return 'p'; return 'reel'; }
function isDirectVideoUrl(url){ return /\.(mp4|webm|ogg|ogv|m4v|mov)(?:[?#].*)?$/i.test(String(url||'').trim()); }
function isInstagramUrl(url){ return /instagram\.com\/(?:reel|reels|p|tv)\//i.test(String(url||'').trim()); }
function isProbablyUrl(url){ return /^https?:\/\//i.test(String(url||'').trim()); }
function safeUrl(url){ const u = cleanVideoInput(url); if(!u) return ''; if(/^(javascript|data|vbscript):/i.test(u)) return ''; if(!/^https?:\/\//i.test(u) && !u.startsWith('//')) return ''; return u.startsWith('//') ? 'https:' + u : u; }
function thumbnailFromEmbed(url){ try{ const parsed = new URL(String(url||''), location.href); const cand = parsed.searchParams.get('source')||parsed.searchParams.get('src')||parsed.searchParams.get('url')||parsed.searchParams.get('video'); if(!cand) return ''; const dec = decodeURIComponent(cand); const yid = youtubeId(dec); return yid ? `https://i.ytimg.com/vi/${encodeURIComponent(yid)}/mqdefault.jpg` : ''; }catch(e){ return ''; } }
const __webpSupported = (() => { try{ const c = document.createElement('canvas'); return c.toDataURL('image/webp').indexOf('data:image/webp') === 0; }catch(e){ return false; } })();
function youtubeThumb(videoId, quality = 'mq'){
  if(!videoId) return '';
  const q = quality === 'max' ? 'maxresdefault' : (quality === 'hq' ? 'hqdefault' : 'mqdefault');
  if(__webpSupported) return `https://i.ytimg.com/vi_webp/${encodeURIComponent(videoId)}/${q}.webp`;
  return `https://i.ytimg.com/vi/${encodeURIComponent(videoId)}/${q}.jpg`;
}
const __nvuCache = new Map();
function normalizeVideoUrl(input){
  let raw;
  if(input && typeof input === 'object'){ raw = firstValue(input, ['url','link','videoUrl','videoURL','videoLink','videoUri','src','video','embed','embedUrl','iframeUrl','source','sourceUrl','ytUrl','ytLink','youtubeUrl','youtubeLink'], ''); }
  else{ raw = input || ''; }
  const key = String(raw == null ? '' : raw);
  const hit = __nvuCache.get(key); if(hit) return hit;
  const result = __normalizeVideoUrlRaw(key);
  if(__nvuCache.size > 1200) __nvuCache.clear();
  __nvuCache.set(key, result);
  return result;
}
function __normalizeVideoUrlRaw(rawIn){
  let raw = cleanVideoInput(rawIn);
  if(!raw) return {src:'', type:'none', youtubeId:'', vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail:''};
  if(/^[A-Za-z0-9_-]{11}$/.test(raw)){ return {src:'https://www.youtube.com/watch?v='+raw, type:'youtube', youtubeId: raw, vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail: youtubeThumb(raw)}; }
  const src = safeUrl(raw); if(!src) return {src:'', type:'none', youtubeId:'', vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail:''};
  const yid = youtubeId(src); if(yid) return {src, type:'youtube', youtubeId:yid, vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail: youtubeThumb(yid)};
  const vid = vimeoId(src); if(vid) return {src, type:'vimeo', youtubeId:'', vimeoId:vid, instagramId:'', instagramKind:'', embedUrl:'', thumbnail:''};
  const igId = instagramId(src); if(igId) return {src, type:'instagram', youtubeId:'', vimeoId:'', instagramId:igId, instagramKind: instagramType(src), embedUrl:'', thumbnail:''};
  if(isDirectVideoUrl(src)) return {src, type:'direct', youtubeId:'', vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail:''};
  if(isProbablyUrl(src)) return {src, type:'iframe', youtubeId:'', vimeoId:'', instagramId:'', instagramKind:'', embedUrl:src, thumbnail: thumbnailFromEmbed(src)};
  return {src:'', type:'none', youtubeId:'', vimeoId:'', instagramId:'', instagramKind:'', embedUrl:'', thumbnail:''};
}
function youtubeEmbedUrl(url, opts={}){
  const info = normalizeVideoUrl(url);
  if(info.type !== 'youtube' || !info.youtubeId) return '';
  const params = new URLSearchParams({ playsinline:'1', rel:'0', autoplay: opts.autoplay ? '1' : '0', mute: opts.muted ? '1' : '0', controls: String(opts.controls===false ? 0 : 1), enablejsapi:'1' });
  try{ const proto = location.protocol; if((proto === 'http:' || proto === 'https:') && location.origin && location.origin !== 'null'){ params.set('origin', location.origin); } }catch(e){}
  if(opts.loop){ params.set('loop','1'); params.set('playlist', info.youtubeId); }
  return 'https://www.youtube-nocookie.com/embed/' + encodeURIComponent(info.youtubeId) + '?' + params.toString();
}
function vimeoEmbedUrl(url, opts={}){
  const info = normalizeVideoUrl(url);
  if(info.type !== 'vimeo' || !info.vimeoId) return '';
  const params = new URLSearchParams({ byline:'0', portrait:'0', title:'0', badge:'0', autopause:'0', autoplay: opts.autoplay ? '1' : '0', muted: opts.muted ? '1' : '0', controls: String(opts.controls===false ? 0 : 1), dnt:'1' });
  if(opts.loop) params.set('loop','1');
  return 'https://player.vimeo.com/video/' + encodeURIComponent(info.vimeoId) + '?' + params.toString();
}
function instagramEmbedUrl(url){
  const info = normalizeVideoUrl(url);
  if(info.type !== 'instagram' || !info.instagramId) return '';
  const kind = info.instagramKind === 'p' ? 'p' : 'reel';
  return 'https://www.instagram.com/' + kind + '/' + encodeURIComponent(info.instagramId) + '/embed/captioned/';
}
function createPlayerMedia(src, opts={}){
  const info = normalizeVideoUrl(src);
  if(info.type === 'none') return null;
  let el;
  if(info.type === 'youtube' || info.type === 'vimeo'){
    el = document.createElement('iframe');
    el.src = info.type === 'youtube' ? youtubeEmbedUrl(info.src, opts) : vimeoEmbedUrl(info.src, opts);
    el.title = opts.title || 'Learnify video';
    el.loading = opts.eager ? 'eager' : 'lazy';
    el.referrerPolicy = 'strict-origin-when-cross-origin';
    el.allow = 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share; fullscreen';
    el.allowFullscreen = true;
    el.setAttribute('allowfullscreen',''); el.setAttribute('playsinline','1'); el.setAttribute('webkit-playsinline','1'); el.setAttribute('frameborder','0');
    el.dataset.mediaType = info.type;
    el.style.cssText = 'width:100%;height:100%;border:0;display:block;background:#000';
    return el;
  }
  if(info.type === 'instagram'){
    el = document.createElement('iframe');
    el.src = instagramEmbedUrl(info.src);
    el.title = opts.title || 'Instagram Reel';
    el.loading = opts.eager ? 'eager' : 'lazy';
    el.referrerPolicy = 'strict-origin-when-cross-origin';
    el.allow = 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share; fullscreen';
    el.allowFullscreen = true;
    el.setAttribute('allowfullscreen',''); el.setAttribute('frameborder','0'); el.setAttribute('scrolling','no');
    el.dataset.mediaType = 'instagram';
    el.style.cssText = 'width:100%;height:100%;border:0;display:block;background:#000;overflow:hidden';
    return el;
  }
  if(info.type === 'direct'){
    el = document.createElement('video');
    el.src = info.src;
    el.controls = opts.controls !== false;
    el.playsInline = true;
    el.autoplay = !!opts.autoplay;
    el.muted = !!(opts.muted || opts.autoplay);
    el.loop = !!opts.loop;
    el.preload = opts.autoplay ? 'auto' : (opts.aggressive ? 'auto' : 'metadata');
    el.setAttribute('playsinline',''); el.setAttribute('webkit-playsinline','');
    if(el.muted) el.setAttribute('muted','');
    if(opts.autoplay) el.setAttribute('autoplay','');
    el.dataset.mediaType = 'direct';
    el.style.cssText = 'width:100%;height:100%;object-fit:'+(opts.objectFit||'cover')+';background:#000';
    if(opts.onEnded) el.addEventListener('ended', opts.onEnded, {once:true});
    el.addEventListener('error', () => { if(el.dataset.retried === '1') return; el.dataset.retried = '1'; setTimeout(() => { try{ el.load(); const p = el.play(); if(p && p.catch) p.catch(()=>{}); }catch(_){} }, 700); }, { once:false });
    if(opts.autoplay){
      const targetMuted = !SOUND_ON;
      el.muted = targetMuted;
      const start = () => {
        el.volume = 1;
        const p = el.play();
        if(p && p.catch) p.catch(() => {
          el.muted = true;
          const p2 = el.play();
          if(p2 && p2.catch) p2.catch(()=>{});
          const resume = () => {
            el.muted = !SOUND_ON;
            el.volume = 1;
            const p3 = el.play();
            if(p3 && p3.catch) p3.catch(()=>{});
            document.removeEventListener('touchstart', resume);
            document.removeEventListener('click', resume);
          };
          document.addEventListener('touchstart', resume, {once:true, passive:true});
          document.addEventListener('click', resume, {once:true});
        });
      };
      el.addEventListener('loadedmetadata', start, {once:true});
      el.addEventListener('canplay', start, {once:true});
      setTimeout(start, 100);
      if(SOUND_ON) scheduleSoundApply(el, 300);
    }
    return el;
  }
  el = document.createElement('iframe');
  el.src = info.embedUrl || info.src;
  el.title = opts.title || 'Embedded video';
  el.loading = opts.eager ? 'eager' : 'lazy';
  el.referrerPolicy = 'strict-origin-when-cross-origin';
  el.allow = 'accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share; fullscreen';
  el.allowFullscreen = true;
  el.setAttribute('allowfullscreen',''); el.setAttribute('playsinline','1'); el.setAttribute('webkit-playsinline','1'); el.setAttribute('frameborder','0');
  el.dataset.mediaType = 'iframe';
  el.style.cssText = 'width:100%;height:100%;border:0;display:block;background:#000';
  return el;
}
function attachIframeEndedHandler(iframe, type, onEnded){
  let fired = false;
  const handler = event => {
    if(fired) return;
    if(event.source !== iframe.contentWindow) return;
    try{ const raw = event.data; let data = raw; if(typeof raw === 'string'){ try { data = JSON.parse(raw); } catch(_) { return; } } if(!data || typeof data !== 'object') return; if(type === 'youtube' && data.event === 'onStateChange' && data.info === 0){ fired = true; window.removeEventListener('message', handler); try{ onEnded(); }catch(_){} } if(type === 'vimeo' && (data.event === 'finish' || data.method === 'finish')){ fired = true; window.removeEventListener('message', handler); try{ onEnded(); }catch(_){} } }catch(_){}
  };
  window.addEventListener('message', handler);
  iframe.__endedHandler = handler;
  return handler;
}
function mountPlayerMedia(container, src, opts={}){
  if(!container) return null;
  container.innerHTML='';
  const media = createPlayerMedia(src, opts);
  if(!media){ const empty=document.createElement('div'); empty.className='pd-empty'; empty.textContent=opts.emptyText || 'Video unavailable'; container.appendChild(empty); return null; }
  container.appendChild(media);
  const info = normalizeVideoUrl(src);
  if(info.type === 'youtube' || info.type === 'vimeo' || info.type === 'instagram'){
    if(opts.shield !== false && info.type !== 'instagram'){ const shield = document.createElement('div'); shield.className = 'yt-shield'; container.appendChild(shield); }
    if(opts.autoplay && info.type !== 'instagram'){
      const tryPlay = () => {
        applySoundToMedia(media, SOUND_ON);
        try{
          if(info.type === 'youtube'){ media.contentWindow.postMessage(JSON.stringify({event:'command', func:'playVideo', args:[]}), '*'); }
          else if(info.type === 'vimeo'){ media.contentWindow.postMessage(JSON.stringify({method:'play'}), '*'); }
        }catch(e){}
      };
      media.addEventListener('load', () => {
        tryPlay();
        if(SOUND_ON){ scheduleSoundApply(media, 400); }
      });
      tryPlay();
      if(SOUND_ON) scheduleSoundApply(media, 500);
    }
    if(opts.onEnded && info.type !== 'instagram'){ attachIframeEndedHandler(media, info.type, opts.onEnded); }
  }
  if(opts.soundToggle !== false){
    const sBtn = document.createElement('button');
    sBtn.type = 'button';
    sBtn.className = 'sound-toggle' + (SOUND_ON ? ' on' : '');
    sBtn.setAttribute('aria-label','Toggle sound');
    sBtn.innerHTML = soundIconHtml(SOUND_ON);
    sBtn.addEventListener('click', (ev) => { ev.stopPropagation(); toggleSound(); });
    container.appendChild(sBtn);
  }
  return media;
}
function thumbFor(v){
  if(!v) return '';
  const direct = safeUrl(v.thumbnail) || safeUrl(v.thumb) || safeUrl(v.image);
  if(direct) return direct;
  if(Array.isArray(v.links) && v.links.length){
    const first = v.links[0];
    let t = '';
    if(typeof first === 'string') t = normalizeVideoUrl(first).thumbnail || '';
    else if(first && typeof first === 'object'){ const custom = safeUrl(first.thumbnail) || safeUrl(first.thumb) || safeUrl(first.image); if(custom) t = custom; else t = normalizeVideoUrl(first.url || first.link || first.src || '').thumbnail || ''; }
    if(t) return t;
  }
  const info = normalizeVideoUrl(videoSource(v));
  return info.thumbnail || '';
}
function thumbForLink(link){
  if(link == null) return '';
  if(typeof link === 'string') return normalizeVideoUrl(link).thumbnail || '';
  const custom = safeUrl(link.thumbnail) || safeUrl(link.thumb) || safeUrl(link.image);
  if(custom) return custom;
  return normalizeVideoUrl(linkSrc(link)).thumbnail || '';
}
function linkSrc(link){ return normalizeVideoUrl(link).src; }
function linkTitle(link, idx){ if(link == null) return 'Video ' + ((idx||0)+1); if(typeof link === 'string') return 'Video ' + ((idx||0)+1); return link.title || link.t || link.name || ('Video ' + ((idx||0)+1)); }
function linkDuration(link){ if(link == null || typeof link === 'string') return ''; return link.dur || link.duration || ''; }
function linkCreator(link){ if(link == null || typeof link === 'string') return ''; return link.creator || link.channel || link.author || ''; }
function imageBlockHtml(url, alt, className){ const u = safeUrl(url); if(u) return `<img class="art-img ${className||''}" src="${esc(u)}" alt="${esc(alt||'')}" loading="lazy" decoding="async" onerror="this.onerror=null;this.style.display='none';">`; return ''; }

// FORCE GUEST MODE
function isSignedIn(){ 
  const mobile = localStorage.getItem('learnifyMobileUser');
  return !!mobile;
}
function currentUser(){ 
  let u = readJSONCache('learnifyUser', null);
  if(!u) {
    u = { name: 'Guest User', email: '', uid: 'guest_123', signedIn: true };
    writeJSONCache('learnifyUser', u);
  }
  return u;
}
function currentUid(){ const u = currentUser(); if(u && u.uid) return u.uid; return 'guest_123'; }
function saveLocalUser(user){ writeJSONCache('learnifyUser', user); }
function clearLocalUser(){ dropJSONCache('learnifyUser'); }
function displayNameFromEmail(email){ if(!email) return 'Guest User'; const local = String(email).split('@')[0] || 'user'; return local.charAt(0).toUpperCase() + local.slice(1); }
function isValidEmail(e){ return /^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.test(String(e||'').trim()); }

function authErrorMessage(code){ return 'Invalid login'; }
async function firebaseEmailAuth(){ return null; }
async function performAuth(){ return null; }
async function googleSignIn(){ return null; }
async function handleGoogleRedirect(){ return; }
async function syncUserDataFromFirebase(uid){
  if(!db || !uid) return;
  try{
    const snap = await db.ref('learnify/users/' + uid).once('value');
    const data = snap.val() || {};
    if(data.likes && typeof data.likes === 'object'){ const likedKeys = Object.keys(data.likes).filter(k => data.likes[k]); saveLikedSet(new Set(likedKeys)); }
    if(data.subs && typeof data.subs === 'object'){ const subKeys = Object.keys(data.subs).filter(k => data.subs[k]); saveSubscribedSet(new Set(subKeys)); }
    if(data.playlistLikes && typeof data.playlistLikes === 'object'){ const plKeys = Object.keys(data.playlistLikes).filter(k => data.playlistLikes[k]); savePlaylistLikedSet(new Set(plKeys)); }
    try{
      if(currentShortList && currentShortList.length && shortsReelsRoot){
        const slides = shortsReelsRoot.querySelectorAll('.short-reel');
        slides.forEach(slide => {
          const sid = slide.dataset.shortId;
          const likeBtn = slide.querySelector('.short-reel-action-btn');
          if(likeBtn && sid){ likeBtn.classList.toggle('liked', isLiked(sid)); }
          const subBtn = slide.querySelector('.short-reel-subscribe');
          if(subBtn){ const base = subBtn.dataset.baseTag || ''; const s = isSubscribed(base); subBtn.classList.toggle('subscribed', s); subBtn.textContent = s ? 'Subscribed' : 'Subscribe'; }
        });
      }
      if(currentChannelTag){ const chBtn = document.querySelector('#channelBody .channel-subscribe-btn'); if(chBtn){ const s = isSubscribed(currentChannelTag); chBtn.classList.toggle('subscribed', s); chBtn.textContent = s ? 'Subscribed' : 'Subscribe'; } }
      if(currentPlaylist){ try{ renderPlaylistActionsBar(); }catch(e){} }
    }catch(e){ console.warn('UI sync error:', e); }
  }catch(e){ console.warn('syncUserDataFromFirebase error:', e); }
}
function getUnlockedSet(){ return readSetCache('learnifyUnlocked'); }
function saveUnlockedSet(set){ writeSetCache('learnifyUnlocked', set); }
function isUnlocked(id){ if(!id) return false; return getUnlockedSet().has(String(id)); }
function markUnlocked(id){ const s = getUnlockedSet(); s.add(String(id)); saveUnlockedSet(s); }
function unlockPremium(id, type, title, onUnlocked){
  if(!id) return;
  const sid = String(id);
  if(isUnlocked(sid)){ showToast('Already unlocked', 'info'); if(typeof onUnlocked === 'function'){ try{ onUnlocked(); }catch(e){} } else { openPlaylist(sid); } return; }
  
  // Auto unlock since isSignedIn() is true
  markUnlocked(sid); 
  showToast('Unlocked: ' + (title||'Premium content'), 'success'); 
  refreshPremiumUI(); 
  if(typeof onUnlocked === 'function'){ try{ onUnlocked(); }catch(e){} } else { openPlaylist(sid); }
}
function getLikedSet(){ return readSetCache('learnifyLikes'); }
function saveLikedSet(set){ writeSetCache('learnifyLikes', set); }
function isLiked(id){ if(!id) return false; return getLikedSet().has(String(id)); }
async function toggleLike(id){
  if(!id) return false;
  const k = String(id);
  const set = getLikedSet();
  let nowLiked;
  if(set.has(k)){ set.delete(k); nowLiked = false; } else { set.add(k); nowLiked = true; }
  saveLikedSet(set);
  const uid = currentUid();
  if(uid && db){ try{ const path = 'learnify/users/' + uid + '/likes'; const update = {}; update[k] = nowLiked ? true : null; await db.ref(path).update(update); }catch(e){ console.warn('like sync failed:', e); } }
  return nowLiked;
}
function getSubscribedSet(){ return readSetCache('learnifySubs'); }
function saveSubscribedSet(set){ writeSetCache('learnifySubs', set); }
function isSubscribed(baseTag){ if(!baseTag) return false; return getSubscribedSet().has(String(baseTag).toLowerCase().trim()); }
async function toggleSubscribeCategory(baseTag){
  const k = String(baseTag||'').toLowerCase().trim();
  if(!k) return false;
  const set = getSubscribedSet();
  if(set.has(k)) { return true; }
  set.add(k);
  saveSubscribedSet(set);
  const uid = currentUid();
  if(uid && db){ try{ const path = 'learnify/users/' + uid + '/subs'; const update = {}; update[k] = true; await db.ref(path).update(update); }catch(e){ console.warn('sub sync failed:', e); } }
  return true;
}
function getViewsMap(){ return readJSONCache('learnifyViews', {}); }
function saveViewsMap(m){ writeJSONCache('learnifyViews', m); }
function getItemViews(id, baseViews){ if(!id) return 0; const m = getViewsMap(); const local = Number(m[String(id)] || 0); const base  = Number(baseViews || 0); return base + local; }
function incrementView(id){ if(!id) return; const m = getViewsMap(); const k = String(id); m[k] = Number(m[k] || 0) + 1; saveViewsMap(m); invalidateIndex(); }
function parseCount(str){
  if(str == null) return 0;
  if(typeof str === 'number') return str;
  const s = String(str).trim().toUpperCase().replace(/,/g,'');
  if(!s) return 0;
  const m = s.match(/^([\d.]+)\s*([KMB]?)/);
  if(!m) return 0;
  const num = parseFloat(m[1]) || 0;
  const mult = m[2] === 'K' ? 1000 : m[2] === 'M' ? 1000000 : m[2] === 'B' ? 1000000000 : 1;
  return Math.round(num * mult);
}
function formatCount(n){
  n = Number(n) || 0;
  if(n >= 1000000000) return (n/1000000000).toFixed(1).replace('.0','') + 'B';
  if(n >= 1000000) return (n/1000000).toFixed(1).replace('.0','') + 'M';
  if(n >= 1000) return (n/1000).toFixed(n >= 100000 ? 0 : 1).replace('.0','') + 'K';
  return String(n);
}
function getAppInstallsMap(){ return readJSONCache('learnifyAppInstalls', {}); }
function saveAppInstallsMap(m){ writeJSONCache('learnifyAppInstalls', m); }
function getAppInstalls(id, base){ if(!id) return Number(base||0); const m = getAppInstallsMap(); const local = Number(m[String(id)] || 0); const b = Number(base || 0); return b + local; }
function incrementAppInstall(id){ if(!id) return; const m = getAppInstallsMap(); const k = String(id); m[k] = Number(m[k] || 0) + 1; saveAppInstallsMap(m); }
function parseAge(val){ if(val == null || val === '') return 0; const n = parseInt(String(val).replace(/[^0-9]/g,''), 10); return isNaN(n) ? 0 : n; }
function computeAppAge(adminAge, createdAt){ const base = parseAge(adminAge); const t = Number(createdAt) || 0; if(!t) return base; const yearsPassed = Math.floor((Date.now() - t) / (365.25 * 24 * 60 * 60 * 1000)); return base + Math.max(0, yearsPassed); }

// Disable auth modals
function showAuthModal(ctx={}){ if(typeof ctx.onSuccess === 'function'){ try{ ctx.onSuccess(); }catch(e){} } }
function closeAuthModal(){}
function openAuthModal(){ showToast('Guest Mode active', 'info'); }
function refreshPremiumUI(){
  try{ renderHome(); }catch(e){}
  try{ renderPremium(); }catch(e){}
  try{ renderApps(); }catch(e){}
  invalidateIndex();
  INDEX = buildIndex();
  if(currentPlaylist && currentPlaylist.premium){ renderPlaylistDetail(); }
}
function isValidBgUrl(url){ const u = String(url||'').trim(); if(!u) return false; if(/^(javascript|data|vbscript):/i.test(u)) return false; return /^https?:\/\//i.test(u); }
function isBgColor(val){ return /^(#[0-9a-f]{3,8}|rgb\(|rgba\(|hsl\(|hsla\(|[a-z]+)$/i.test(String(val||'').trim()); }
function setAppBackground(value){
  const app = $('#app'); if(!app) return;
  const v = String(value||'').trim();
  if(!v){ try{ localStorage.removeItem('learnifyBg'); }catch(e){} app.style.removeProperty('background-image'); app.style.removeProperty('background-size'); app.style.removeProperty('background-position'); app.style.removeProperty('background-repeat'); app.style.backgroundImage = 'none'; app.style.backgroundColor = ''; document.documentElement.style.removeProperty('--bg'); document.body.style.backgroundColor = ''; updateBgPreview(); showToast('Background reset', 'success'); return; }
  if(!isValidBgUrl(v) && isBgColor(v)){ try{ localStorage.setItem('learnifyBg', JSON.stringify({type:'color', value:v})); }catch(e){} app.style.removeProperty('background-image'); app.style.backgroundImage = 'none'; app.style.backgroundColor = v; document.documentElement.style.setProperty('--bg', v); document.body.style.backgroundColor = v; updateBgPreview(); showToast('Background color applied', 'success'); return; }
  if(isValidBgUrl(v)){ try{ localStorage.setItem('learnifyBg', JSON.stringify({type:'image', value:v})); }catch(e){} const safe = v.replace(/"/g,'&quot;'); app.style.setProperty('background-image', `url("${safe}")`, ''); app.style.setProperty('background-size','cover',''); app.style.setProperty('background-position','center center',''); app.style.setProperty('background-repeat','no-repeat',''); app.style.setProperty('background-attachment','scroll',''); updateBgPreview(); showToast('Background image applied', 'success'); return; }
  showToast('Invalid URL or color', 'error');
}
function applyBgFromInput(){ const el = $('#bgUrlInput'); if(!el) return; const v = el.value.trim(); if(!v){ showToast('Kuch paste karo pehle', 'info'); return; } setAppBackground(v); el.value = ''; }
function updateBgPreview(){
  const preview = $('#bgPreview'); if(!preview) return;
  const app = $('#app');
  const bgImg = app ? app.style.backgroundImage : '';
  const bgCol = app ? app.style.backgroundColor : '';
  if(bgImg && bgImg !== 'none'){ const url = bgImg.replace(/^url\(["']?/, '').replace(/["']?\)$/, ''); preview.style.backgroundImage = `url("${url}")`; preview.style.backgroundColor = ''; preview.innerHTML = `<span>Current background</span>`; }
  else if(bgCol){ preview.style.backgroundImage = 'none'; preview.style.backgroundColor = bgCol; preview.innerHTML = `<span>Solid color</span>`; }
  else { preview.style.backgroundImage = 'none'; preview.style.backgroundColor = ''; preview.innerHTML = `<span>No background set</span>`; }
}
function loadStoredBackground(){
  try{
    const params = new URLSearchParams(location.search);
    const urlBg = params.get('bg');
    if(urlBg){ setAppBackground(decodeURIComponent(urlBg)); setTimeout(updateBgPreview, 100); return; }
    const raw = localStorage.getItem('learnifyBg');
    if(!raw){ setTimeout(updateBgPreview, 100); return; }
    const obj = JSON.parse(raw);
    if(!obj || !obj.value){ setTimeout(updateBgPreview, 100); return; }
    const app = $('#app'); if(!app){ setTimeout(updateBgPreview, 100); return; }
    if(obj.type === 'image' && isValidBgUrl(obj.value)){ const safe = obj.value.replace(/"/g,'&quot;'); app.style.setProperty('background-image', `url("${safe}")`, ''); app.style.setProperty('background-size','cover',''); app.style.setProperty('background-position','center center',''); app.style.setProperty('background-repeat','no-repeat',''); }
    else if(obj.type === 'color'){ app.style.backgroundColor = obj.value; document.documentElement.style.setProperty('--bg', obj.value); }
  }catch(e){}
  setTimeout(updateBgPreview, 100);
}
function applyTheme(theme){
  if(!theme || typeof theme !== 'object') return;
  const root = document.documentElement;
  const set = (varName, val) => { if(val != null && val !== '') root.style.setProperty(varName, String(val)); };
  set('--bg', theme.bg); set('--surface', theme.surface); set('--surface-2', theme.surface2);
  set('--ink', theme.ink); set('--ink-2', theme.ink2); set('--muted', theme.muted); set('--line', theme.line);
  set('--brand', theme.brand); set('--brand-2', theme.brand2); set('--brand-soft', theme.brandSoft);
  set('--nav-bg', theme.navBg); set('--nav-border', theme.navBorder); set('--nav-text', theme.navText); set('--nav-active', theme.navActive);
  set('--glass-bg', theme.glassBg); set('--glass-border', theme.glassBorder);
  set('--soft-white', theme.softWhite); set('--soft-white-2', theme.softWhite2);
  set('--float-bg', theme.floatBg); set('--float-border', theme.floatBorder);
  set('--search-bg', theme.searchBg); set('--search-border', theme.searchBorder); set('--search-text', theme.searchText); set('--search-placeholder', theme.searchPlaceholder);
  set('--shorts-chip-bg', theme.shortsChipBg); set('--shorts-chip-text', theme.shortsChipText);
  set('--shorts-play-bg', theme.shortsPlayBg); set('--thumb-play-bg', theme.thumbPlayBg);
}
function applyAppTheme(themeName){
  GLOBAL_THEME = themeName;
  if(themeName === 'dark'){
    document.body.classList.add('dark-theme');
    document.querySelector('meta[name="theme-color"]').setAttribute('content', '#0A0B10');
    applyTheme(DARK_THEME);
  } else {
    document.body.classList.remove('dark-theme');
    document.querySelector('meta[name="theme-color"]').setAttribute('content', '#F5F6FA');
    applyTheme(LIGHT_THEME);
  }
}

/* ============ SPLASH MEDIA ============ */
const SPLASH_SHOW_MS = 3000;
const SPLASH_FADE_MS = 600;
const SPLASH_VIDEO_MAX_MS = 15 * 60 * 1000;
const SPLASH_VIDEO_NO_START_MS = 20000;
let __splashShown = false;

(function injectSplashCSS(){
  if(document.getElementById('splashNoControlsCSS')) return;
  const style = document.createElement('style');
  style.id = 'splashNoControlsCSS';
  style.textContent = `
    #appSplashScreen video,
    #appSplashScreen iframe,
    #appSplashScreen img {
      pointer-events: none !important;
      -webkit-user-select: none !important;
      user-select: none !important;
      -webkit-touch-callout: none !important;
      -webkit-tap-highlight-color: transparent !important;
    }
    #appSplashScreen video::-webkit-media-controls,
    #appSplashScreen video::-webkit-media-controls-enclosure,
    #appSplashScreen video::-webkit-media-controls-panel,
    #appSplashScreen video::-webkit-media-controls-play-button,
    #appSplashScreen video::-webkit-media-controls-start-playback-button,
    #appSplashScreen video::-webkit-media-controls-overlay-play-button,
    #appSplashScreen video::-webkit-media-controls-picture-in-picture-button,
    #appSplashScreen video::-webkit-media-controls-fullscreen-button,
    #appSplashScreen video::-webkit-media-controls-volume-slider,
    #appSplashScreen video::-webkit-media-controls-mute-button,
    #appSplashScreen video::-webkit-media-controls-timeline,
    #appSplashScreen video::-webkit-media-controls-current-time-display,
    #appSplashScreen video::-webkit-media-controls-time-remaining-display,
    #appSplashScreen video::-internal-media-controls-overlay-cast-button,
    #appSplashScreen video::-internal-media-controls-download-button {
      display: none !important;
      -webkit-appearance: none !important;
      opacity: 0 !important;
      pointer-events: none !important;
      width: 0 !important;
      height: 0 !important;
    }
  `;
  document.head.appendChild(style);
})();

function getCachedSplash(){
  try{
    const raw = localStorage.getItem('learnifySplashMedia');
    if(!raw){
      const old = localStorage.getItem('learnifyFlashImage');
      if(old){
        const obj = JSON.parse(old);
        if(obj && obj.url) return { type:'image', url: String(obj.url) };
      }
      return null;
    }
    const obj = JSON.parse(raw);
    if(!obj || !obj.url) return null;
    return { type: obj.type || 'image', url: String(obj.url) };
  }catch(e){ return null; }
}

function cacheSplash(media){
  try{
    if(media && media.url && String(media.url).trim()){
      localStorage.setItem('learnifySplashMedia', JSON.stringify({
        type: media.type || 'image',
        url: String(media.url).trim(),
        at: Date.now()
      }));
    } else {
      localStorage.removeItem('learnifySplashMedia');
      localStorage.removeItem('learnifyFlashImage');
    }
  }catch(e){}
}

function showSplashScreen(media){
  if(!media || !media.url) return;
  if(__splashShown) return;
  if(document.getElementById('appSplashScreen')) return;
  const app = document.getElementById('app');
  if(!app) return;
  __splashShown = true;

  const splash = document.createElement('div');
  splash.id = 'appSplashScreen';
  splash.style.cssText = `
    position: absolute; inset: 0; z-index: 99999;
    background: #000;
    overflow: hidden;
    display: flex; align-items: center; justify-content: center;
    transition: opacity ${SPLASH_FADE_MS}ms ease;
    opacity: 1;
    border-radius: inherit;
    pointer-events: auto;
    -webkit-user-select: none;
    -moz-user-select: none;
    user-select: none;
    -webkit-touch-callout: none;
    -webkit-tap-highlight-color: transparent;
  `;

  splash.addEventListener('contextmenu', e => e.preventDefault());
  splash.addEventListener('selectstart', e => e.preventDefault());

  let closed = false;
  const closeSplash = () => {
    if(closed) return;
    closed = true;
    splash.style.opacity = '0';
    setTimeout(() => { try{ splash.remove(); }catch(e){} }, SPLASH_FADE_MS);
  };

  const splashStartTime = Date.now();
  splash.addEventListener('click', () => {
    if(Date.now() - splashStartTime > 3000) closeSplash();
  });
  splash.addEventListener('touchend', () => {
    if(Date.now() - splashStartTime > 3000) closeSplash();
  }, { passive: true });

  if(media.type === 'video'){
    let mediaEl = null;
    try{
      mediaEl = createPlayerMedia(media.url, {
        title: 'Splash',
        autoplay: true,
        muted: false,
        controls: false,
        loop: false,
        objectFit: 'contain',
        eager: true,
        shield: false,
        soundToggle: false
      });
    }catch(e){}

    if(!mediaEl){
      closeSplash();
      return;
    }

    mediaEl.style.cssText = 'width:100%;height:100%;object-fit:contain;display:block;border:0;background:#000;pointer-events:none;';
    mediaEl.setAttribute('controlsList', 'nodownload nofullscreen noremoteplayback noplaybackrate');
    mediaEl.setAttribute('disablePictureInPicture', '');
    mediaEl.setAttribute('disableRemotePlayback', '');
    try{ mediaEl.disablePictureInPicture = true; }catch(e){}
    try{ mediaEl.disableRemotePlayback = true; }catch(e){}

    if(mediaEl.tagName === 'VIDEO'){
      mediaEl.controls = false;
      mediaEl.removeAttribute('controls');
      mediaEl.muted = false;

      let hasStarted = false;
      let ended = false;
      const safeClose = () => {
        if(ended) return;
        ended = true;
        closeSplash();
      };

      const tryPlay = () => {
        const p = mediaEl.play();
        if(p && p.catch){
          p.catch(() => {
            mediaEl.muted = true;
            const p2 = mediaEl.play();
            if(p2 && p2.catch) p2.catch(()=>{});
          });
        }
      };

      mediaEl.addEventListener('playing', () => {
        hasStarted = true;
        clearTimeout(noPlayTimer);
      }, { once: true });

      mediaEl.addEventListener('ended', safeClose, { once: true });

      mediaEl.addEventListener('timeupdate', () => {
        if(ended) return;
        const dur = mediaEl.duration;
        const cur = mediaEl.currentTime;
        if(dur && isFinite(dur) && dur > 0 && cur > 0 && cur >= dur - 0.6){
          safeClose();
        }
      });

      mediaEl.addEventListener('loadedmetadata', () => {
        if(ended) return;
        const dur = mediaEl.duration;
        if(dur && isFinite(dur) && dur > 0){
          const waitMs = (dur * 1000) + 3000;
          setTimeout(safeClose, waitMs);
        }
      }, { once: true });

      mediaEl.addEventListener('error', () => setTimeout(safeClose, 1500), { once: true });

      const noPlayTimer = setTimeout(() => {
        if(!hasStarted) safeClose();
      }, SPLASH_VIDEO_NO_START_MS);

      setTimeout(safeClose, SPLASH_VIDEO_MAX_MS);

      mediaEl.addEventListener('loadedmetadata', tryPlay, { once: true });
      mediaEl.addEventListener('canplay', tryPlay, { once: true });
      setTimeout(tryPlay, 100);

    } else {
      const info = normalizeVideoUrl(media.url);
      let ended = false;
      let hasPlayed = false;

      const safeClose = () => {
        if(ended) return;
        ended = true;
        try { window.removeEventListener('message', iframeMsgHandler); } catch(e) {}
        try { clearInterval(pollInterval); } catch(e) {}
        closeSplash();
      };

      const iframeMsgHandler = (event) => {
        if(event.source !== mediaEl.contentWindow) return;
        try {
          let data = event.data;
          if(typeof data === 'string'){
            try { data = JSON.parse(data); } catch(_) { return; }
          }
          if(!data || typeof data !== 'object') return;

          if(data.event === 'onStateChange' && data.info === 0){
            safeClose();
            return;
          }

          if(data.event === 'infoDelivery' && data.info){
            const ci = data.info;
            if(typeof ci.playerState === 'number'){
              if(ci.playerState === 0){ safeClose(); return; }
              if(ci.playerState === 1) hasPlayed = true;
            }
            if(hasPlayed && typeof ci.currentTime === 'number' && typeof ci.duration === 'number' && ci.duration > 0){
              if(ci.currentTime >= ci.duration - 0.5){
                safeClose();
                return;
              }
            }
          }

          if(data.event === 'finish' || data.method === 'finish'){
            safeClose();
            return;
          }

          if(data.event === 'timeupdate' && data.data && typeof data.data.seconds === 'number' && typeof data.data.duration === 'number'){
            hasPlayed = true;
            if(data.data.duration > 0 && data.data.seconds >= data.data.duration - 0.5){
              safeClose();
            }
          }
        } catch(e) {}
      };

      window.addEventListener('message', iframeMsgHandler);

      const sendListening = () => {
        if(ended) return;
        try {
          mediaEl.contentWindow.postMessage(JSON.stringify({
            event: 'listening',
            id: 'splash',
            channel: 'widget'
          }), '*');
        } catch(e) {}
      };

      const pollInterval = setInterval(() => {
        if(ended) return;
        try {
          mediaEl.contentWindow.postMessage(JSON.stringify({
            event: 'command',
            func: 'getCurrentTime',
            args: []
          }), '*');
        } catch(e) {}
        try {
          mediaEl.contentWindow.postMessage(JSON.stringify({
            method: 'getCurrentTime'
          }), '*');
        } catch(e) {}
      }, 3000);

      mediaEl.addEventListener('load', () => {
        sendListening();
        setTimeout(sendListening, 300);
        setTimeout(sendListening, 1000);
        setTimeout(sendListening, 2000);
      });

      mediaEl.addEventListener('error', () => setTimeout(safeClose, 1500), { once: true });

      setTimeout(safeClose, 90000);
    }

    splash.appendChild(mediaEl);

  } else {
    const img = document.createElement('img');
    img.src = media.url;
    img.style.cssText = 'width:100%;height:100%;object-fit:cover;display:block;pointer-events:none;';
    img.alt = '';
    img.decoding = 'async';
    img.setAttribute('draggable','false');
    splash.appendChild(img);

    const maxTimer = setTimeout(closeSplash, SPLASH_SHOW_MS + 3000);
    const onLoaded = () => {
      clearTimeout(maxTimer);
      setTimeout(closeSplash, SPLASH_SHOW_MS);
    };
    if(img.complete && img.naturalWidth > 0){
      onLoaded();
    } else {
      img.addEventListener('load', onLoaded, { once: true });
      img.addEventListener('error', () => {
        clearTimeout(maxTimer);
        setTimeout(closeSplash, 400);
      }, { once: true });
    }
  }

  app.appendChild(splash);
}
/* ============ END SPLASH MEDIA ============ */

function applySearchTitle(){
  const el = document.getElementById('searchTitle');
  if(el) el.textContent = GLOBAL_SEARCH_TITLE || 'Search';
}
function applyPremiumTitle(){
  const tEl = document.getElementById('premiumTitle');
  const sEl = document.getElementById('premiumSubtitle');
  if(tEl) tEl.textContent = GLOBAL_PREMIUM_TITLE || 'Premium';
  if(sEl) sEl.textContent = GLOBAL_PREMIUM_SUBTITLE || 'Courses & masterclasses';
}
window.__applySearchTitle = applySearchTitle;
window.__applyPremiumTitle = applyPremiumTitle;

let headerBannerTimer = null;

function renderHeaderBanners() {
  const track = document.getElementById('homeBannerTrack');
  const wrapper = document.getElementById('homeBannerWrapper');
  if(!track || !wrapper) return;

  if(headerBannerTimer) clearInterval(headerBannerTimer);
  track.style.transform = 'translateY(0)';
  track.innerHTML = '';

  if(!GLOBAL_HEADER_BANNERS.length) {
    track.innerHTML = `<div style="height:38px; display:grid; place-items:center; font-size:11px; color:var(--muted); font-weight:600;">No Banner</div>`;
    return;
  }

  let html = GLOBAL_HEADER_BANNERS.map(url => `<img src="${esc(url)}" class="home-banner-img" alt="Banner" loading="lazy" decoding="async" onerror="this.style.display='none'">`).join('');
  
  if(GLOBAL_HEADER_BANNERS.length > 1) {
    html += `<img src="${esc(GLOBAL_HEADER_BANNERS[0])}" class="home-banner-img" alt="Banner" loading="lazy" decoding="async" onerror="this.style.display='none'">`;
  }
  
  track.innerHTML = html;

  if(GLOBAL_HEADER_BANNERS.length > 1) {
    let currentIndex = 0;
    headerBannerTimer = setInterval(() => {
      currentIndex++;
      track.style.transition = 'transform 0.6s ease-in-out';
      track.style.transform = `translateY(-${currentIndex * 38}px)`;

      if(currentIndex >= GLOBAL_HEADER_BANNERS.length) {
        setTimeout(() => {
          track.style.transition = 'none';
          track.style.transform = 'translateY(0)';
          currentIndex = 0;
        }, 600); 
      }
    }, 2000); 
  }
}

function openHeaderBannerEditor() {
  const overlay = document.createElement('div');
  overlay.className = 'overlay on';
  overlay.style.zIndex = '600';
  overlay.innerHTML = `
    <div class="modal" style="max-width:380px">
      <div style="text-align:center;margin-bottom:14px">
        <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">🖼️</div>
        <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Edit Header Banners</h3>
        <p style="font-size:12.5px;color:var(--muted);margin:0">Add up to 5 image URLs.</p>
      </div>
      <div id="headerBannerInputs"></div>
      <div style="display:flex;gap:9px;margin-bottom:10px;margin-top:14px;">
        <button class="btn btn-secondary" id="hdrBannerCancel" style="flex:1">Cancel</button>
        <button class="btn btn-primary" id="hdrBannerSave" style="flex:2">Save</button>
      </div>
    </div>`;
  document.body.appendChild(overlay);

  const inputsContainer = overlay.querySelector('#headerBannerInputs');
  for(let i = 0; i < 5; i++) {
    const val = GLOBAL_HEADER_BANNERS[i] || '';
    inputsContainer.innerHTML += `
      <div class="field" style="margin-bottom:8px">
        <input class="input" id="hdrBannerInp${i}" type="url" placeholder="Image URL ${i+1}" value="${esc(val)}" autocomplete="off" style="height:40px; font-size:13px;">
      </div>
    `;
  }

  const close = () => overlay.remove();
  
  overlay.querySelector('#hdrBannerCancel').addEventListener('click', close);
  overlay.querySelector('#hdrBannerSave').addEventListener('click', () => {
    const urls = [];
    for(let i = 0; i < 5; i++) {
      const v = overlay.querySelector(`#hdrBannerInp${i}`).value.trim();
      if(v) urls.push(v);
    }
    
    if(db) {
      db.ref('learnify/headerBanners').set(urls).then(() => {
        showToast('Header banners updated!', 'success');
        close();
      }).catch(e => {
        showToast('Failed to save', 'error');
      });
    } else {
      applyHeaderBanners(urls);
      localStorage.setItem('learnifyHeaderBanners', JSON.stringify(urls));
      showToast('Header banners updated locally!', 'success');
      close();
    }
  });
  
  overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
}

let headerBannerTapCount = 0;
let headerBannerTapTimer = null;

function attachHeaderBannerTap() {
  const wrapper = document.getElementById('homeBannerWrapper');
  if(!wrapper || wrapper.dataset.ready === '1') return;
  wrapper.dataset.ready = '1';
  
  wrapper.addEventListener('click', (e) => {
    e.preventDefault();
    e.stopPropagation();
    headerBannerTapCount++;
    clearTimeout(headerBannerTapTimer);
    
    if(headerBannerTapCount >= 5) {
      headerBannerTapCount = 0;
      promptPassword(openHeaderBannerEditor, 'Banner Access', 'Enter password to change header banners.');
    } else {
      headerBannerTapTimer = setTimeout(() => { headerBannerTapCount = 0; }, 600);
    }
  });
}

function playlistCard(p){
  const thumb = thumbFor(p);
  return `<div class="playlist-large" onclick="openPlaylist('${esc(p.id)}')"><div class="art ar-169">${imageBlockHtml(thumb, p.t)}<div class="playlist-overlay"><div class="playlist-title">${esc(p.t)}</div></div></div></div>`;
}
function premiumCard(p){
  const thumb = thumbFor(p);
  const price = (p.price != null && p.price !== '') ? Number(p.price) : null;
  const old = (p.old != null && p.old !== '') ? Number(p.old) : null;
  const count = p.n || (p.links ? p.links.length : 0);
  const unlocked = isUnlocked(p.id);
  const badgeHtml = unlocked ? `<span class="badge unlocked on-art">✓ Unlocked</span>` : `<span class="badge premium on-art">Premium</span>`;
  const btnHtml = unlocked ? `<button class="btn btn-primary btn-sm" onclick="event.stopPropagation();openPlaylist('${esc(p.id)}')">Play</button>` : `<button class="btn btn-primary btn-sm" onclick="event.stopPropagation();unlockPremium('${esc(p.id)}','playlist','${esc(p.t)}')">Unlock</button>`;
  return `<article class="pcard" onclick="openPlaylist('${esc(p.id)}')"><div class="art ar-169">${imageBlockHtml(thumb, p.t)}${badgeHtml}${count ? `<span class="chip-dur">${count} lessons</span>` : ''}</div><div class="pcard-body"><h4>${esc(p.t)}</h4><p class="meta">${esc(p.dur||'')}${p.cat ? (p.dur?' · ':'') + esc(p.cat) : ''}</p><div class="pcard-foot"><span class="price">${unlocked ? '' : (price !== null ? '$'+price : '')}${old !== null && !unlocked ? `<s>$${old}</s>` : ''}</span>${btnHtml}</div></div></article>`;
}

function appIconHtml(a, size){
  const sz = size || '';
  const img = safeUrl(a.image || a.icon || a.logo);
  if(img) return `<div class="app-ico ${sz}" style="background:transparent;"><img src="${esc(img)}" alt="${esc(a.n)}" loading="lazy" decoding="async" onerror="this.onerror=null;this.style.display='none';this.parentElement.classList.add('fallback');this.parentElement.textContent='${esc((a.n||'?').charAt(0).toUpperCase())}'"></div>`;
  const letter = (a.n||'?').trim().charAt(0).toUpperCase() || '?';
  return `<div class="app-ico fallback ${sz}">${esc(letter)}</div>`;
}

function appCardV(a){ return `<article class="acard-v" onclick="openApp('${esc(a.id)}')">${appIconHtml(a,'')}<h4>${esc(a.n)}</h4><p class="meta">${a.rating ? '<span class="star">★</span> '+esc(a.rating) : ''}${a.dl ? (a.rating?' · ':'')+esc(a.dl) : ''}</p></article>`; }
function appRow(a){
  const installs = getAppInstalls(a.id, parseCount(a.dl));
  return `<div class="app-row" onclick="openApp('${esc(a.id)}')">${appIconHtml(a,'sm')}<div class="app-row-txt"><h4>${esc(a.n)}</h4><p class="meta">${a.rating ? '<span class="star">★</span> '+esc(a.rating) : ''}${a.rating && installs ? ' · ' : ''}${installs ? formatCount(installs)+' downloads' : ''}</p></div><button class="btn btn-secondary btn-sm" onclick="event.stopPropagation();quickInstall(this)">Install</button></div>`;
}
const HERO_AUTO_ADVANCE_MS = 6000;
let __heroAutoTimer = null;
function heroSlideThumb(slide){ if(!slide) return ''; const custom = safeUrl(slide.image) || safeUrl(slide.thumbnail) || safeUrl(slide.thumb) || safeUrl(slide.photo) || safeUrl(slide.backgroundImage); if(custom) return custom; return normalizeVideoUrl(videoSource(slide)).thumbnail || ''; }
function heroSlideLink(slide){ if(!slide) return ''; return safeUrl(slide.openUrl || slide.openLink || slide.clickUrl || slide.link || slide.url || ''); }
function heroSlideLabel(slide){ return slide ? String(slide.t || slide.title || slide.name || '') : ''; }
function heroSlideDesc(slide){ return slide ? String(slide.d || slide.description || slide.desc || '') : ''; }
function heroSlideClick(i){ const slide = HERO_SLIDES[i]; if(!slide) return; const url = heroSlideLink(slide); if(!url){ showToast('Link not available', 'info'); return; } try{ window.open(url, '_blank', 'noopener,noreferrer'); } catch(e){ location.href = url; } }
function renderHero(){
  const track = $('#heroTrack'), dots = $('#heroDots'), heroEl = $('#homeHero');
  if(!track || !dots || !heroEl) return;
  if(__heroAutoTimer){ clearInterval(__heroAutoTimer); __heroAutoTimer = null; }
  const slides = HERO_SLIDES.filter(s => heroSlideThumb(s));
  if(!slides.length){ heroEl.style.display = 'none'; track.innerHTML = ''; dots.innerHTML = ''; return; }
  heroEl.style.display = '';
  track.innerHTML = slides.map((slide, i)=>{
    const thumb = heroSlideThumb(slide);
    const title = heroSlideLabel(slide), desc = heroSlideDesc(slide);
    const hasText = !!(title || desc);
    return `<div class="hero-slide"><div class="hero-card" onclick="heroSlideClick(${i})"><div class="hero-media"><img src="${esc(thumb)}" alt="${esc(title||'Slide')}" loading="${i===0?'eager':'lazy'}" decoding="async" fetchpriority="${i===0?'high':'low'}" onerror="this.style.display='none';"></div>${hasText ? `<div class="hero-scrim"></div><div class="hero-body">${title?`<div class="hero-title">${esc(title)}</div>`:''}${desc?`<div class="hero-desc">${esc(desc)}</div>`:''}</div>` : ''}</div></div>`;
  }).join('');
  dots.innerHTML = slides.map((_, i) => `<button class="dot ${i===0?'on':''}" onclick="event.stopPropagation();heroGo(${i})"></button>`).join('');
  let idx = 0;
  const updateDots = () => Array.from(dots.children).forEach((d, i) => d.classList.toggle('on', i === idx));
  const goTo = (i, smooth) => { const n = Math.max(0, Math.min(slides.length - 1, Number(i) || 0)); idx = n; updateDots(); try{ track.scrollTo({ left: track.clientWidth * n, behavior: smooth ? 'smooth' : 'auto' }); }catch(e){ track.scrollLeft = track.clientWidth * n; } };
  window.heroGo = i => { goTo(i, true); restartAuto(); };
  window.heroNext = () => { idx = (idx + 1) % slides.length; goTo(idx, true); };
  track.addEventListener('scroll', () => { const i = Math.round(track.scrollLeft / Math.max(1, track.clientWidth)); if(i !== idx && i >= 0 && i < slides.length){ idx = i; updateDots(); } }, { passive: true });
  function restartAuto(){ if(__heroAutoTimer){ clearInterval(__heroAutoTimer); __heroAutoTimer = null; } if(slides.length > 1 && HERO_AUTO_ADVANCE_MS > 0) __heroAutoTimer = setInterval(() => window.heroNext(), HERO_AUTO_ADVANCE_MS); }
  goTo(0, false); restartAuto();
}

function shortsCard(s){
  const thumb = safeUrl(s.thumb) || '';
  const title = esc(s.t || 'Short');
  const tag = esc(s.tag || 'Short');
  const views = getItemViews(s.id, s.views);
  const imgHtml = thumb ? `<img src="${thumb}" alt="${title}" loading="lazy" decoding="async" onerror="this.style.display='none';this.parentElement.classList.add('fallback')">` : `<div class="thumb-fallback">📱</div>`;
  return `<div class="shorts-item" onclick="openShort('${esc(s.id)}')">${imgHtml}<div class="short-tag">${tag}</div><div class="short-overlay"><div class="short-label">${title}</div>${views ? `<div class="short-views">${views} views</div>` : ''}</div></div>`;
}
const LIKE_ANIM_URL = "https://cdnl.iconscout.com/lottie/premium/thumb/like-animation-gif-download-8476914.mp4";
function playLikeAnimation(){
  const wrap = document.getElementById('likeAnim');
  const vid  = document.getElementById('likeAnimVideo');
  if(!wrap || !vid) return;
  wrap.classList.remove('show');
  try{ vid.pause(); }catch(e){}
  void wrap.offsetWidth;
  if(vid.dataset.loaded !== '1'){ vid.src = LIKE_ANIM_URL; vid.dataset.loaded = '1'; try{ vid.load(); }catch(e){} }
  try{ vid.currentTime = 0; }catch(e){}
  wrap.classList.add('show');
  try{ vid.play().catch(()=>{}); }catch(e){}
  clearTimeout(wrap._hideTimer);
  wrap._hideTimer = setTimeout(() => wrap.classList.remove('show'), 1400);
}
function playSubscribeAnimation(){
  const wrap = document.getElementById('subAnim');
  if(!wrap) return;
  wrap.classList.remove('show');
  void wrap.offsetWidth;
  wrap.classList.add('show');
  clearTimeout(wrap._hideTimer);
  wrap._hideTimer = setTimeout(() => wrap.classList.remove('show'), 1400);
}

async function handleReelLike(btn){
  if(!btn) return;
  const slide = btn.closest('.short-reel');
  const sid = slide ? slide.dataset.shortId : '';
  if(!sid) return;
  const nowLiked = await toggleLike(sid);
  btn.classList.toggle('liked', nowLiked);
  if(nowLiked) playLikeAnimation();
  else showToast('Like removed', 'info');
}
async function handleReelSubscribe(btn){
  if(!btn) return;
  const base = btn.dataset.baseTag || '';
  if(!base) return;
  if(isSubscribed(base)) { showToast('Already subscribed', 'info'); return; }
  const nowSubbed = await toggleSubscribeCategory(base);
  document.querySelectorAll('.short-reel-subscribe').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  document.querySelectorAll('.channel-subscribe-btn').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  document.querySelectorAll('.pd-action-btn[data-base-tag]').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.classList.toggle('primary', !nowSubbed); const sp = b.querySelector('span'); if(sp) sp.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  if(nowSubbed){ playSubscribeAnimation(); showToast('Subscribed to ' + base, 'success'); }
}

function renderPlaylistAd(){
  const slot = $('#pdAdSlot');
  if(!slot) return;
  const activeAds = ADS.filter(a => a && a.active !== false && a.image);
  if(!activeAds.length){ slot.classList.remove('on'); slot.innerHTML = ''; return; }
  const seed = currentPlaylist ? String(currentPlaylist.id) : '';
  let h = 0; for(let i=0;i<seed.length;i++) h = ((h<<5)-h+seed.charCodeAt(i))|0;
  const pick = activeAds[Math.abs(h) % activeAds.length];
  const img = safeUrl(pick.image);
  if(!img){ slot.classList.remove('on'); slot.innerHTML=''; return; }
  const link = safeUrl(pick.link);
  const title = esc(pick.title || 'Sponsored');
  const onclick = link ? `onclick="event.stopPropagation();openAdLink('${esc(link)}')"` : '';
  slot.classList.add('on');
  slot.innerHTML = `<div class="pd-ad-card" ${onclick}>
    <span class="ad-label">AD</span>
    <img src="${esc(img)}" alt="" loading="lazy" decoding="async" onerror="this.parentElement.parentElement.classList.remove('on')">
    <span class="ad-title">${title}</span>
    ${link?'<span class="ad-cta">Open ›</span>':''}
  </div>`;
}
function openAdLink(url){
  const u = safeUrl(url);
  if(!u) return;
  try{ window.open(u, '_blank', 'noopener,noreferrer'); }catch(e){ location.href = u; }
}
function renderPlaylistActionsBar(){
  const bar = $('#pdActionsBar');
  if(!bar) return;
  const p = currentPlaylist;
  if(!p){ bar.innerHTML = ''; return; }
  const liked = isPlaylistLiked(p.id);
  const likeCount = getPlaylistLikeCount(p);
  const channelTag = getPlaylistChannel(p);
  const channelName = getPlaylistChannelDisplay(p);
  const subbed = channelTag ? isSubscribed(channelTag) : false;
  const likeLabel = likeCount >= 1000 ? (likeCount/1000).toFixed(1).replace('.0','')+'K' : String(likeCount);
  bar.innerHTML = `
    <button class="pd-action-btn ${liked?'liked':''}" onclick="handlePlaylistLike(this)">
      <svg viewBox="0 0 24 24" fill="${liked?'currentColor':'none'}" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 9V5a3 3 0 0 0-3-3l-4 9v11h11.28a2 2 0 0 0 2-1.7l1.38-9a2 2 0 0 0-2-2.3zM7 22H4a2 2 0 0 1-2-2v-7a2 2 0 0 1 2-2h3"/></svg>
      <span>Like</span>
      <span class="pd-action-count">${likeLabel}</span>
    </button>
    <button class="pd-action-btn ${subbed?'subscribed':'primary'}" data-base-tag="${esc(channelTag)}" onclick="handlePlaylistSubscribe(this)">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
      <span>${subbed ? 'Subscribed' : 'Subscribe'}</span>
    </button>
    <div class="pd-actions-spacer"></div>
    <span class="meta" style="font-size:11px;font-weight:600">${esc(channelName)}</span>
  `;
}
async function handlePlaylistLike(btn){
  if(!btn || !currentPlaylist) return;
  const nowLiked = await togglePlaylistLike(currentPlaylist.id);
  btn.classList.toggle('liked', nowLiked);
  const svg = btn.querySelector('svg');
  if(svg) svg.setAttribute('fill', nowLiked ? 'currentColor' : 'none');
  const countEl = btn.querySelector('.pd-action-count');
  if(countEl){
    const c = getPlaylistLikeCount(currentPlaylist);
    countEl.textContent = c >= 1000 ? (c/1000).toFixed(1).replace('.0','')+'K' : String(c);
  }
  if(nowLiked){ playLikeAnimation(); showToast('Liked!', 'success'); }
}

async function handlePlaylistSubscribe(btn){
  if(!btn) return;
  const base = btn.dataset.baseTag || '';
  if(!base) return;
  if(isSubscribed(base)) { showToast('Already subscribed', 'info'); return; }
  const nowSubbed = await toggleSubscribeCategory(base);
  document.querySelectorAll('.pd-action-btn[data-base-tag]').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.classList.toggle('primary', !nowSubbed); const sp = b.querySelector('span'); if(sp) sp.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  document.querySelectorAll('.short-reel-subscribe').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  document.querySelectorAll('.channel-subscribe-btn').forEach(b => { if((b.dataset.baseTag||'') === base){ b.classList.toggle('subscribed', nowSubbed); b.textContent = nowSubbed ? 'Subscribed' : 'Subscribe'; } });
  if(nowSubbed){ playSubscribeAnimation(); showToast('Subscribed to ' + base, 'success'); }
}

let __currentSubsChannel = null;
function renderSubscriptions(){
  const body = $('#subsBody');
  if(!body) return;
  const subs = [...getSubscribedSet()];
  if(!subs.length){
    body.innerHTML = `<div class="empty" style="padding-top:38px"><div class="empty-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg></div><h3>No subscriptions yet</h3><p>Subscribe to channels from shorts or playlists to see them here.</p></div>`;
    return;
  }
  if(!__currentSubsChannel || !subs.includes(__currentSubsChannel)) __currentSubsChannel = subs[0];
  const chips = subs.map(base => {
    const disp = getChannelDisplay(base, base.replace(/\b\w/g, c => c.toUpperCase()));
    const initials = (disp.name.charAt(0) || 'C').toUpperCase();
    const avatarInner = disp.icon ? `<img src="${esc(disp.icon)}" alt="" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${esc(initials)}'">` : esc(initials);
    const active = base === __currentSubsChannel;
    return `<button class="chip ${active?'active':''}" data-base="${esc(base)}"><span class="chip-av">${avatarInner}</span><span>${esc(disp.name)}</span></button>`;
  }).join('');
  const sel = __currentSubsChannel;
  const chShorts = SHORTS.filter(s => getBaseTag(s.tag) === sel);
  const chPlaylists = PLAYLISTS.filter(p => getPlaylistChannel(p) === sel);
  chShorts.sort((a,b) => { const na = getTagNumber(a.tag), nb = getTagNumber(b.tag); if(na !== nb) return na - nb; return String(a.id).localeCompare(String(b.id)); });
  const chDisp = getChannelDisplay(sel, sel.replace(/\b\w/g, c => c.toUpperCase()));
  let contentHtml = '';
  if(chPlaylists.length){
    contentHtml += `<div class="sec"><div class="sec-head"><h2 class="sec-title">Playlists</h2><span class="meta">${chPlaylists.length}</span></div><div style="padding:0 16px 8px;">${chPlaylists.map(playlistCard).join('')}</div></div>`;
  }
  if(chShorts.length){
    contentHtml += `<div class="sec"><div class="sec-head"><h2 class="sec-title">Shorts</h2><span class="meta">${chShorts.length}</span></div><div style="display:grid;grid-template-columns:repeat(2,1fr);gap:10px;padding:2px 16px 6px;">${chShorts.slice(0,12).map(shortsCard).join('')}</div></div>`;
  }
  if(!chPlaylists.length && !chShorts.length){
    contentHtml = `<div class="empty" style="padding:34px 20px"><h3>No content yet</h3><p>Nothing published by ${esc(chDisp.name)} yet.</p></div>`;
  }
  body.innerHTML = `<div class="section-label" style="margin-top:4px">Subscribed channels</div><div class="chip-row">${chips}</div>${contentHtml}<div style="height:20px"></div>`;
}
function selectSubsChannel(base){
  if(Date.now() - Number(window.__lastChipLongPressAt || 0) < 500) return;
  __currentSubsChannel = String(base || '').toLowerCase().trim();
  renderSubscriptions();
}

let currentChannelTag = null;
function openChannel(tagOrBase){
  const base = getBaseTag(tagOrBase);
  if(!base){ showToast('Channel not available', 'info'); return; }
  currentChannelTag = base;
  renderChannelPage(base);
  go('channel');
}
function renderChannelPage(base){
  const body = $('#channelBody'); if(!body) return;
  const shorts = SHORTS.filter(s => getBaseTag(s.tag) === base).sort((a,b) => { const na = getTagNumber(a.tag), nb = getTagNumber(b.tag); if(na !== nb) return na - nb; return String(a.id).localeCompare(String(b.id)); });
  const subbed = isSubscribed(base);
  const disp = getChannelDisplay(base, base.replace(/\b\w/g, c => c.toUpperCase()));
  const channelName = disp.name;
  const avatarInner = disp.icon
    ? `<img src="${esc(disp.icon)}" alt="" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${esc((channelName.charAt(0)||'S').toUpperCase())}'">`
    : esc((channelName.charAt(0) || 'S').toUpperCase());
  body.innerHTML = `<div class="channel-hero"><div class="channel-avatar">${avatarInner}</div><h1 class="channel-name">${esc(channelName)}</h1><p class="channel-meta">${shorts.length} short${shorts.length > 1 ? 's' : ''}</p><button class="btn ${subbed ? 'channel-subscribe-btn subscribed' : 'btn-primary channel-subscribe-btn'}" data-base-tag="${esc(base)}" onclick="handleReelSubscribe(this)">${subbed ? 'Subscribed' : 'Subscribe'}</button></div><div class="channel-section-label">All Videos</div>${shorts.length ? `<div class="channel-grid">${shorts.map(s => `<div class="channel-short" onclick="openShort('${esc(s.id)}')"><div class="channel-short-thumb">${s.thumb ? `<img src="${esc(s.thumb)}" alt="" loading="lazy" decoding="async" onerror="this.style.display='none';this.parentElement.innerHTML='<div class=&quot;channel-short-fallback&quot;>📱</div>'">` : `<div class="channel-short-fallback">📱</div>`}</div><div class="channel-short-info"><div class="channel-short-title">${esc(s.t || 'Short')}</div><div class="channel-short-views">${getItemViews(s.id, s.views)} views</div></div></div>`).join('')}</div>` : `<div class="empty" style="padding-top:30px"><h3>No videos yet</h3><p>This channel doesn't have any videos.</p></div>`}`;
}
let currentShortId = null;
let currentShortList = [];
let shortsReelsRoot = null;
let shortsActiveIdx = -1;
let shortsScrollListener = null;
let shortsTouchStartY = 0, shortsTouchStartX = 0;
let shortsTouchLastY = 0, shortsTouchLastTime = 0;
let shortsTouchStartTime = 0;
let shortsTouchListeners = null;
let shortsDesktopNav = null;
let shortsAutoplayTimers = [];
const __reelReleaseTimers = new Map();
const REEL_RELEASE_DELAY = 900;
let __scrollActivateTimer = null;
let __pendingActivateIdx = -1;
const SCROLL_DEBOUNCE = 90;
let __reelObserver = null;
let __thumbPreloader = null;
let __idlePrefetchHandle = null;
const VIRTUAL_RANGE = 2;
const __lqipCache = new Map();
function getLQIP(seed){
  if(!seed) seed = 'x';
  if(__lqipCache.has(seed)) return __lqipCache.get(seed);
  let h = 0;
  for(let i=0; i<seed.length; i++) h = ((h<<5) - h + seed.charCodeAt(i)) | 0;
  const hue1 = Math.abs(h) % 360;
  const hue2 = (hue1 + 40) % 360;
  const c1 = `hsl(${hue1},45%,12%)`;
  const c2 = `hsl(${hue2},50%,20%)`;
  const svg = `<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 178'><defs><linearGradient id='g' x1='0' y1='0' x2='0' y2='1'><stop offset='0' stop-color='${c1}'/><stop offset='1' stop-color='${c2}'/></linearGradient></defs><rect width='100' height='178' fill='url(%23g)'/></svg>`;
  const data = 'data:image/svg+xml;utf8,' + svg.replace(/#/g,'%23');
  __lqipCache.set(seed, data);
  return data;
}
function setupReelObserver(root){
  teardownReelObserver();
  if(!('IntersectionObserver' in window)) return;
  __reelObserver = new IntersectionObserver((entries) => {
    let best = null, bestRatio = 0;
    entries.forEach(en => { if(en.intersectionRatio > bestRatio){ bestRatio = en.intersectionRatio; best = en.target; } });
    if(best && bestRatio > 0.55){
      const idx = parseInt(best.dataset.idx, 10);
      if(!isNaN(idx) && idx !== shortsActiveIdx){ clearTimeout(__scrollActivateTimer); __scrollActivateTimer = setTimeout(() => { shortsActiveIdx = idx; activateReel(idx); }, 60); }
    }
  }, { root, threshold: [0, 0.25, 0.55, 0.75, 1.0], rootMargin: '0px' });
  root.querySelectorAll('.short-reel').forEach(el => __reelObserver.observe(el));
}
function teardownReelObserver(){ if(__reelObserver){ __reelObserver.disconnect(); __reelObserver = null; } }
function preloadThumbsAround(idx){
  if(!currentShortList || !currentShortList.length) return;
  if(__thumbPreloader) { __thumbPreloader.innerHTML = ''; }
  else { __thumbPreloader = document.createElement('div'); __thumbPreloader.style.cssText = 'position:absolute;width:0;height:0;overflow:hidden;pointer-events:none'; document.body.appendChild(__thumbPreloader); }
  for(let i = idx + 1; i <= idx + 3 && i < currentShortList.length; i++){
    const s = currentShortList[i];
    const thumb = safeUrl(s && s.thumb);
    if(!thumb) continue;
    const img = document.createElement('img');
    img.src = thumb; img.loading = 'eager'; img.decoding = 'async'; img.width = 1; img.height = 1;
    __thumbPreloader.appendChild(img);
  }
}
function scheduleIdlePrefetch(centerIdx){
  if(__idlePrefetchHandle && 'cancelIdleCallback' in window){ try{ cancelIdleCallback(__idlePrefetchHandle); }catch(e){} __idlePrefetchHandle = null; }
  const run = () => {
    __idlePrefetchHandle = null;
    if(!currentShortList || !currentShortList.length) return;
    for(let i = centerIdx + 4; i <= centerIdx + 8 && i < currentShortList.length; i++){
      const s = currentShortList[i];
      if(!s || !s.thumb) continue;
      const img = new Image();
      img.decoding = 'async'; img.loading = 'eager';
      img.src = safeUrl(s.thumb);
    }
  };
  if('requestIdleCallback' in window){ __idlePrefetchHandle = requestIdleCallback(run, { timeout: 2000 }); }
  else { setTimeout(run, 500); }
}
function preloadDirectional(fromIdx, dir, count){
  if(!__thumbPreloader) { __thumbPreloader = document.createElement('div'); __thumbPreloader.style.cssText = 'position:absolute;width:0;height:0;overflow:hidden;pointer-events:none'; document.body.appendChild(__thumbPreloader); }
  for(let i = 1; i <= count; i++){
    const idx = fromIdx + (dir * i);
    if(idx < 0 || idx >= currentShortList.length) continue;
    const s = currentShortList[idx];
    const thumb = safeUrl(s && s.thumb);
    if(!thumb) continue;
    if(__thumbPreloader.querySelector(`img[data-idx="${idx}"]`)) continue;
    const img = document.createElement('img');
    img.dataset.idx = idx;
    img.src = thumb; img.loading = 'eager'; img.decoding = 'async'; img.width = 1; img.height = 1;
    __thumbPreloader.appendChild(img);
  }
}
function scheduleReleaseReel(idx, delay = REEL_RELEASE_DELAY){
  if(!shortsReelsRoot) return;
  if(__reelReleaseTimers.has(idx)) clearTimeout(__reelReleaseTimers.get(idx));
  const t = setTimeout(() => { __reelReleaseTimers.delete(idx); releaseReelMedia(idx); }, delay);
  __reelReleaseTimers.set(idx, t);
}
function cancelScheduledRelease(idx){ if(__reelReleaseTimers.has(idx)){ clearTimeout(__reelReleaseTimers.get(idx)); __reelReleaseTimers.delete(idx); } }
function cancelAllScheduledReleases(){ __reelReleaseTimers.forEach(t => clearTimeout(t)); __reelReleaseTimers.clear(); }
function getBaseTag(tag){ return String(tag || '').replace(/\s*\d+\s*$/, '').trim().toLowerCase(); }
function getTagNumber(tag){ const m = String(tag || '').match(/(\d+)\s*$/); return m ? parseInt(m[1], 10) : 0; }
function getRelatedShorts(currentShort){
  const base = getBaseTag(currentShort.tag);
  return SHORTS.filter(s => getBaseTag(s.tag) === base).sort((a, b) => { const na = getTagNumber(a.tag), nb = getTagNumber(b.tag); if(na !== nb) return na - nb; return String(a.id).localeCompare(String(b.id)); });
}

function buildShortsPlaylistWithAds(currentShort){
  const list = getRelatedShorts(currentShort);
  if(!SHORT_ADS || !SHORT_ADS.length) return list;
  const activeAds = SHORT_ADS.filter(a => a && a.active !== false && a.videoUrl);
  if(!activeAds.length) return list;

  const startIdx = list.findIndex(s => String(s.id) === String(currentShort.id));
  if(startIdx < 0) return list;

  const before = list.slice(0, startIdx);
  const forward = list.slice(startIdx);

  const result = [];
  let adIdx = 0;
  let counter = 0;
  for(let i = 0; i < forward.length; i++){
    result.push(forward[i]);
    counter++;
    if(counter >= 4 && i < forward.length - 1){
      const ad = activeAds[adIdx % activeAds.length];
      adIdx++;
      result.push({
        id: 'shortad_' + (ad.id || adIdx) + '_' + i,
        isAd: true,
        t: ad.title || 'Sponsored',
        title: ad.title || 'Sponsored',
        videoUrl: ad.videoUrl,
        thumb: normalizeVideoUrl(ad.videoUrl).thumbnail || '',
        clickLink: ad.clickLink || '',
        tag: 'Ad',
        views: 0
      });
      counter = 0;
    }
  }
  return [...before, ...result];
}

function openShort(id){
  const s = SHORTS.find(x => String(x.id) === String(id));
  if(!s){ showToast('Short video not found','error'); return; }
  currentShortList = buildShortsPlaylistWithAds(s);
  currentShortId = s.id;
  go('shortplayer');
  renderShortsReels(currentShortList, s.id);
  setTimeout(() => { try{ renderHomeThrottled(); }catch(e){} }, 300);
}
function renderShortsReels(list, startId){
  const mount = $('#shortPlayerBody');
  if(!mount) return;
  const startIdx = Math.max(0, list.findIndex(x => String(x.id) === String(startId)));
  shortsActiveIdx = startIdx;
  try{
    const firstSrc = list[startIdx] && list[startIdx].videoUrl;
    if(firstSrc){ const inf = normalizeVideoUrl(firstSrc); if(inf.type === 'youtube') preconnectOnce('https://www.youtube-nocookie.com'); if(inf.type === 'vimeo') preconnectOnce('https://player.vimeo.com'); }
  }catch(e){}
  const placeholders = list.map((s, i) => `<div class="short-reel short-reel-placeholder" data-idx="${i}" data-short-id="${esc(s.id)}" data-src="${esc(s.videoUrl || '')}" data-filled="false"></div>`).join('');
  mount.innerHTML = `<div class="shorts-reels" id="shortsReels">${placeholders}</div><div class="shorts-progress"><i id="shortsProgressBar"></i></div><button class="shorts-global-back" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button><button class="shorts-sound-toggle ${SOUND_ON?'on':''}" onclick="toggleShortsSound()" aria-label="Toggle sound">${soundIconHtml(SOUND_ON)}</button>`;
  const root = document.getElementById('shortsReels');
  shortsReelsRoot = root;
  if(!root) return;
  let tries = 0;
  const boot = () => { tries++; const h = root.clientHeight; if((!h || h < 10) && tries < 30){ requestAnimationFrame(boot); return; } fillVirtualReels(startIdx, h); root.scrollTop = startIdx * h; activateReel(startIdx); attachShortsScroll(root); setupReelObserver(root); attachShortsGestures(root); attachShortsDesktopNav(root); };
  requestAnimationFrame(boot);
}
function fillVirtualReels(centerIdx, height){
  if(!shortsReelsRoot || !currentShortList) return;
  const slides = shortsReelsRoot.querySelectorAll('.short-reel');
  const total = slides.length;
  const lo = Math.max(0, centerIdx - VIRTUAL_RANGE);
  const hi = Math.min(total - 1, centerIdx + VIRTUAL_RANGE);
  const h = height || shortsReelsRoot.clientHeight || 1;
  for(let i = 0; i < total; i++){
    const el = slides[i];
    const isInRange = i >= lo && i <= hi;
    const hasContent = el.dataset.filled === 'true';
    if(isInRange && !hasContent){ el.dataset.filled = 'true'; const s = currentShortList[i]; el.innerHTML = renderReelSlideInner(s, i, total); }
    else if(!isInRange && hasContent){ el.dataset.filled = 'false'; el.innerHTML = ''; try{ releaseReelMedia(i); }catch(e){} }
    el.style.height = h + 'px';
  }
}

function renderAdReelSlide(s, i, total){
  const thumb = safeUrl(s.thumb) || '';
  const lqip  = getLQIP(s.id);
  const clickAttr = s.clickLink ? `onclick="event.stopPropagation();openAdLink('${esc(s.clickLink)}')"` : '';
  return `
    <div class="short-reel-media" data-loaded="false">
      <img class="short-reel-lqip" src="${lqip}" alt="" aria-hidden="true">
      ${thumb ? `<img class="short-reel-thumb" src="${esc(thumb)}" alt="" loading="eager" decoding="async" onerror="this.style.display='none'">` : ''}
      <div class="short-reel-spinner"></div>
    </div>
    <div class="short-reel-cat" style="background:rgba(229,72,77,.88);border-color:rgba(255,255,255,.25)">Sponsored · ${i+1}/${total}</div>
    <div class="short-reel-ui">
      <div class="short-reel-actions">
        <button class="short-reel-action-btn" ${clickAttr}>
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>
          <span>Visit</span>
        </button>
      </div>
      <div class="short-reel-info">
        <div class="short-reel-channel">
          <div class="short-reel-channel-avatar" style="background:#E5484D;color:#fff;font-weight:900;font-size:11px">AD</div>
          <span>Sponsored</span>
        </div>
        <h3>${esc(s.title || s.t || 'Advertisement')}</h3>
      </div>
    </div>
  `;
}

function renderReelSlideInner(s, i, total){
  if(s && s.isAd) return renderAdReelSlide(s, i, total);
  const tag = s.tag || 'Short';
  const base = getBaseTag(tag);
  const subbed = isSubscribed(base);
  const liked = isLiked(s.id);
  const disp = getChannelDisplay(base, tag);
  const displayName = disp.name;
  const displayIcon = disp.icon;
  const channelName = esc(displayName);
  const channelInitial = esc((displayName.charAt(0) || 'S').toUpperCase());
  const avatarInner = displayIcon
    ? `<img src="${esc(displayIcon)}" alt="" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${channelInitial}'">`
    : channelInitial;
  const likes = esc(s.likes || '1.3k');
  const thumb = safeUrl(s.thumb) || '';
  const lqip = getLQIP(s.id);
  return `
    <div class="short-reel-media" data-loaded="false">
      <img class="short-reel-lqip" src="${lqip}" alt="" aria-hidden="true">
      ${thumb ? `<img class="short-reel-thumb" src="${esc(thumb)}" alt="" loading="eager" decoding="async" fetchpriority="high" onerror="this.style.display='none'">` : ''}
      <div class="short-reel-spinner"></div>
    </div>
    <div class="short-reel-cat">${channelName}${total > 1 ? ` · ${i+1}/${total}` : ''}</div>
    <div class="short-reel-ui">
      <div class="short-reel-actions">
        <button class="short-reel-action-btn ${liked?'liked':''}" onclick="handleReelLike(this)">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 9V5a3 3 0 0 0-3-3l-4 9v11h11.28a2 2 0 0 0 2-1.7l1.38-9a2 2 0 0 0-2-2.3zM7 22H4a2 2 0 0 1-2-2v-7a2 2 0 0 1 2-2h3"/></svg>
          <span>${likes}</span>
        </button>
        <button class="short-reel-action-btn" onclick="copyLink('${esc(s.videoUrl || '')}')">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"/><polyline points="16 6 12 2 8 6"/><line x1="12" y1="2" x2="12" y2="15"/></svg>
          <span>Share</span>
        </button>
      </div>
      <div class="short-reel-info">
        <div class="short-reel-channel">
          <div class="short-reel-channel-avatar" onclick="event.stopPropagation();openChannel('${esc(base)}')">${avatarInner}</div>
          <span onclick="event.stopPropagation();openChannel('${esc(base)}')">${channelName}</span>
          <button class="short-reel-subscribe ${subbed?'subscribed':''}" data-base-tag="${esc(base)}" onclick="handleReelSubscribe(this)">${subbed?'Subscribed':'Subscribe'}</button>
        </div>
      </div>
    </div>
  `;
}

function ensureReelMedia(idx, autoplay){
  if(!shortsReelsRoot) return;
  const slide = shortsReelsRoot.querySelectorAll('.short-reel')[idx];
  if(!slide) return;
  const media = slide.querySelector('.short-reel-media');
  if(!media) return;
  const src = slide.dataset.src;
  if(!src) return;
  if(media.dataset.loaded === 'true'){ if(autoplay) playReelMedia(media); return; }
  media.dataset.loaded = 'true';
  const opts = { title:'', autoplay: !!autoplay, muted: !SOUND_ON, controls:false, loop:true, eager:true, shield:true, objectFit:'cover', aggressive: !autoplay, emptyText:'Video unavailable' };
  const el = createPlayerMedia(src, opts);
  if(!el){ media.classList.add('playing'); return; }
  if(el.tagName === 'VIDEO'){
    el.controls = false;
    el.removeAttribute('controls');
    el.muted = true; 
    el.setAttribute('muted', '');
    el.setAttribute('playsinline', '');
    el.setAttribute('webkit-playsinline', '');
    if(SOUND_ON) {
      setTimeout(() => applySoundToMedia(el, true), 100);
    }
  }
  const markPlaying = () => { media.classList.add('playing'); };
  el.addEventListener('load', markPlaying);
  el.addEventListener('loadeddata', markPlaying);
  el.addEventListener('canplay', markPlaying);
  setTimeout(markPlaying, 3000);
  media.appendChild(el);
  const info = normalizeVideoUrl(src);
  if(el.tagName === 'IFRAME' && opts.shield !== false && info.type !== 'instagram'){
    const shield = document.createElement('div'); shield.className = 'yt-shield'; media.appendChild(shield);
  }
  if(autoplay){
    scheduleSoundApply(el, 350);
    if(SOUND_ON) scheduleSoundApply(el, 900);
  }
}
function releaseReelMedia(idx){
  if(!shortsReelsRoot) return;
  const slide = shortsReelsRoot.querySelectorAll('.short-reel')[idx];
  if(!slide) return;
  const media = slide.querySelector('.short-reel-media');
  if(!media || media.dataset.loaded !== 'true') return;
  pauseReelMedia(media);
  try{
    media.querySelectorAll('video').forEach(v => { try{ v.pause(); v.removeAttribute('src'); v.innerHTML = ''; v.load(); }catch(e){} });
    media.querySelectorAll('iframe').forEach(f => {
      try{ const t = f.dataset.mediaType;
        if(t === 'youtube'){ f.contentWindow.postMessage(JSON.stringify({event:'command', func:'stopVideo', args:[]}), '*'); }
        else if(t === 'vimeo'){ f.contentWindow.postMessage(JSON.stringify({method:'pause'}), '*'); }
        f.src = 'about:blank';
      }catch(e){}
    });
  }catch(e){}
  media.dataset.loaded = 'false';
  media.classList.remove('playing');
  media.querySelectorAll('iframe,video').forEach(el => el.remove());
  slide.dataset.viewCounted = 'false';
}
const __preconnectedHosts = new Set();
function preconnectOnce(host){
  if(!host || __preconnectedHosts.has(host)) return;
  __preconnectedHosts.add(host);
  const link = document.createElement('link');
  link.rel = 'preconnect'; link.href = host; link.crossOrigin = '';
  document.head.appendChild(link);
}
function activateReel(idx){
  if(!shortsReelsRoot) return;
  preloadThumbsAround(idx); scheduleIdlePrefetch(idx); fillVirtualReels(idx);
  const slides = shortsReelsRoot.querySelectorAll('.short-reel');
  const total = slides.length;
  for(let i = 0; i < total; i++){
    const slide = slides[i];
    const media = slide.querySelector('.short-reel-media');
    slide.classList.toggle('is-active', i === idx);
    if(i === idx){
      cancelScheduledRelease(i); ensureReelMedia(i, true);
      if(SOUND_ON){
        setTimeout(() => {
          const mm = slide.querySelector('.short-reel-media video, .short-reel-media iframe');
          if(mm) applySoundToMedia(mm, true);
        }, 500);
      }
      const sid = slide.dataset.shortId;
      if(sid && slide.dataset.viewCounted !== 'true'){
        slide.dataset.viewCounted = 'true';
        const cur = currentShortList[idx];
        if(cur && !cur.isAd) incrementView(cur.id || sid);
      }
      const nextS = currentShortList[idx]; if(nextS && nextS.videoUrl){ const info = normalizeVideoUrl(nextS.videoUrl); if(info.youtubeId) preconnectOnce('https://www.youtube-nocookie.com'); }
      const nn = currentShortList[idx + 1]; if(nn && nn.videoUrl){ const info = normalizeVideoUrl(nn.videoUrl); if(info.youtubeId) preconnectOnce('https://www.youtube-nocookie.com'); }
    } else if(i === idx + 1){
      cancelScheduledRelease(i);
      if(i < total - 1){ const ns = slides[i+1]; if(ns){ const st = ns.dataset.src; if(st){ const inf = normalizeVideoUrl(st); if(inf.type === 'youtube') preconnectOnce('https://www.youtube-nocookie.com'); } } }
      ensureReelMedia(i, false);
      pauseReelMedia(media);
    }
    else { pauseReelMedia(media); scheduleReleaseReel(i, REEL_RELEASE_DELAY); }
  }
}
function playReelMedia(mediaEl){
  if(!mediaEl) return;
  const v = mediaEl.querySelector('video');
  if(v){ try{ v.muted = !SOUND_ON; const p = v.play(); if(p && p.catch) p.catch(()=>{}); }catch(e){} return; }
  const iframe = mediaEl.querySelector('iframe'); if(!iframe) return;
  const type = iframe.dataset.mediaType;
  if(type === 'instagram') return;
  const doPlay = () => { try{ if(type === 'youtube'){ iframe.contentWindow.postMessage(JSON.stringify({event:'command', func:'playVideo', args:[]}), '*'); } else if(type === 'vimeo'){ iframe.contentWindow.postMessage(JSON.stringify({method:'play'}), '*'); } }catch(e){} };
  doPlay(); setTimeout(doPlay, 250); setTimeout(doPlay, 700); setTimeout(doPlay, 1400);
}
function pauseReelMedia(mediaEl){
  if(!mediaEl) return;
  const v = mediaEl.querySelector('video'); if(v){ try{ v.pause(); }catch(e){} return; }
  const iframe = mediaEl.querySelector('iframe'); if(!iframe) return;
  const type = iframe.dataset.mediaType; if(type === 'instagram') return;
  try{ if(type === 'youtube'){ iframe.contentWindow.postMessage(JSON.stringify({event:'command', func:'pauseVideo', args:[]}), '*'); } else if(type === 'vimeo'){ iframe.contentWindow.postMessage(JSON.stringify({method:'pause'}), '*'); } }catch(e){}
}
function attachShortsScroll(root){
  detachShortsScroll();
  let rafPending = false; let lastScrollTop = root.scrollTop; let lastTime = performance.now(); let scrollDir = 0; let __scrollEndTimer = null;
  const onScroll = () => {
    root.classList.add('scrolling'); clearTimeout(__scrollEndTimer);
    __scrollEndTimer = setTimeout(() => root.classList.remove('scrolling'), 150);
    if(rafPending) return; rafPending = true;
    requestAnimationFrame(() => {
      rafPending = false;
      const h = root.clientHeight || 1;
      const now = performance.now();
      const dy = root.scrollTop - lastScrollTop; const dt = Math.max(1, now - lastTime);
      const velocity = Math.abs(dy) / dt;
      scrollDir = dy > 0 ? 1 : (dy < 0 ? -1 : scrollDir);
      lastScrollTop = root.scrollTop; lastTime = now;
      const idx = Math.max(0, Math.min(currentShortList.length - 1, Math.round(root.scrollTop / h)));
      const bar = document.getElementById('shortsProgressBar');
      if(bar){ const pct = Math.min(100, Math.max(0, (root.scrollTop / Math.max(1, root.scrollHeight - h)) * 100)); bar.style.width = pct + '%'; }
      if(velocity > 1.5){ preloadDirectional(idx, scrollDir, 4); } else if(velocity > 0.3){ preloadDirectional(idx, scrollDir, 2); }
      if(!__reelObserver){ if(idx !== __pendingActivateIdx){ __pendingActivateIdx = idx; clearTimeout(__scrollActivateTimer); __scrollActivateTimer = setTimeout(() => { if(idx !== shortsActiveIdx){ shortsActiveIdx = idx; activateReel(idx); } __pendingActivateIdx = -1; }, SCROLL_DEBOUNCE); } }
    });
  };
  root.addEventListener('scroll', onScroll, { passive: true });
  shortsScrollListener = { root, onScroll };
}
function detachShortsScroll(){ if(shortsScrollListener){ try{ shortsScrollListener.root.removeEventListener('scroll', shortsScrollListener.onScroll); }catch(e){} shortsScrollListener = null; } }
function attachShortsGestures(root){
  detachShortsGestures();
  const onTouchStart = (e) => { if(!e.touches[0]) return; shortsTouchStartY = e.touches[0].clientY; shortsTouchStartX = e.touches[0].clientX; shortsTouchLastY = shortsTouchStartY; shortsTouchStartTime = performance.now(); shortsTouchLastTime = shortsTouchStartTime; };
  const onTouchMove = (e) => { if(!e.touches[0]) return; shortsTouchLastY = e.touches[0].clientY; shortsTouchLastTime = performance.now(); };
  const onTouchEnd = () => {};
  root.addEventListener('touchstart', onTouchStart, { passive: true });
  root.addEventListener('touchmove', onTouchMove, { passive: true });
  root.addEventListener('touchend', onTouchEnd, { passive: true });
  shortsTouchListeners = { root, onTouchStart, onTouchMove, onTouchEnd };
}
function detachShortsGestures(){
  if(shortsTouchListeners){ try{ shortsTouchListeners.root.removeEventListener('touchstart', shortsTouchListeners.onTouchStart); shortsTouchListeners.root.removeEventListener('touchmove', shortsTouchListeners.onTouchMove); shortsTouchListeners.root.removeEventListener('touchend', shortsTouchListeners.onTouchEnd); }catch(e){} shortsTouchListeners = null; }
}
function attachShortsDesktopNav(root){
  detachShortsDesktopNav();
  const onKey = (e) => { if(!shortsReelsRoot) return; const h = shortsReelsRoot.clientHeight || 1; if(e.key === 'ArrowDown' || e.key === 'PageDown'){ e.preventDefault(); shortsReelsRoot.scrollBy({ top: h, behavior: 'smooth' }); } else if(e.key === 'ArrowUp' || e.key === 'PageUp'){ e.preventDefault(); shortsReelsRoot.scrollBy({ top: -h, behavior: 'smooth' }); } };
  window.addEventListener('keydown', onKey);
  shortsDesktopNav = { root, onKey };
}
function detachShortsDesktopNav(){ if(shortsDesktopNav){ try{ window.removeEventListener('keydown', shortsDesktopNav.onKey); }catch(e){} shortsDesktopNav = null; } }
function cleanupShortsReels(){
  teardownReelObserver();
  if(__thumbPreloader){ try{ __thumbPreloader.innerHTML = ''; }catch(e){} }
  detachShortsScroll(); detachShortsGestures(); detachShortsDesktopNav();
  cancelAllScheduledReleases(); clearTimeout(__scrollActivateTimer); __pendingActivateIdx = -1;
  if(__idlePrefetchHandle && 'cancelIdleCallback' in window){ try{ cancelIdleCallback(__idlePrefetchHandle); }catch(e){} __idlePrefetchHandle = null; }
  shortsAutoplayTimers.forEach(t => clearTimeout(t)); shortsAutoplayTimers = [];
  shortsReelsRoot = null; shortsActiveIdx = -1;
  try{
    document.querySelectorAll('#shortPlayerBody video').forEach(v => { try{ v.pause(); v.src=''; v.load(); }catch(e){} });
    document.querySelectorAll('#shortPlayerBody iframe').forEach(f => { try{ if(f.dataset.mediaType === 'youtube') f.contentWindow.postMessage(JSON.stringify({event:'command', func:'pauseVideo', args:[]}), '*'); if(f.dataset.mediaType === 'vimeo') f.contentWindow.postMessage(JSON.stringify({method:'pause'}), '*'); }catch(e){} });
  }catch(e){}
}
function renderPremiumPhotos(){
  const grid = $('#premiumPhotoGrid'); const wrap = $('#secPhotoGrid');
  if(!grid || !wrap) return;
  const active = PREMIUM_PHOTOS.filter(p => p && p.active !== false && p.image);
  if(!active.length){ wrap.style.display = 'none'; grid.innerHTML = ''; return; }
  wrap.style.display = '';

  const cells = active.map((p) => {
    const img = safeUrl(p.image); if(!img) return '';
    const idx = PREMIUM_PHOTOS.indexOf(p);
    const title = esc(p.title || ''); const badge = p.badge ? esc(p.badge) : '';
    return `<div class="premium-photo-item" onclick="openPremiumPhoto(${idx})"><img src="${img}" alt="${title}" loading="lazy" decoding="async" onerror="this.onerror=null;this.style.opacity='0';">${badge ? `<span class="pp-badge">${badge}</span>` : ''}${title ? `<div class="pp-title">${title}</div>` : ''}</div>`;
  }).filter(Boolean);

  let gridHtml = '';
  cells.forEach((cell, i) => {
    gridHtml += cell;
    const isSecond = (i % 2 === 1);
    const isLast = (i === cells.length - 1);
    if(isSecond && !isLast){
      const adKey = 'premium-photo-' + i;
      gridHtml += `<div class="premium-banner-ad" data-ad-key="${esc(adKey)}"><iframe src="${esc(getAdUrl(adKey))}" loading="lazy" scrolling="no" frameborder="0"></iframe></div>`;
    }
  });
  grid.innerHTML = gridHtml;
  setTimeout(() => { if(window.__setupAdTripleTap) window.__setupAdTripleTap(); }, 100);
}
function openPremiumPhoto(i){
  const p = PREMIUM_PHOTOS[i]; if(!p) return;
  const link = safeUrl(p.link);
  if(!link){ showToast('Link not available', 'info'); return; }
  try{ window.open(link, '_blank', 'noopener,noreferrer'); } catch(e){ try{ location.href = link; }catch(e2){} }
}

function renderHome(){
  const feed = $('#homeFeed'); if(!feed) return;
  const sortByViews = arr => arr.map(x => ({ x, v: getItemViews(x.id, x.views) })).sort((a, b) => b.v - a.v).map(o => o.x);
  const sortedPlaylists = sortByViews(PLAYLISTS); const sortedShorts = sortByViews(SHORTS);
  const usedPlaylists = new Set(), usedShorts = new Set();
  let pIdx = 0, sIdx = 0; const MAX_BLOCKS = 12; const blocksHtml = [];
  for(let b = 0; b < MAX_BLOCKS; b++){
    let blockHtml = '', anyAdded = false;
    while(pIdx < sortedPlaylists.length && usedPlaylists.has(sortedPlaylists[pIdx].id)) pIdx++;
    if(pIdx < sortedPlaylists.length){ const p = sortedPlaylists[pIdx++]; usedPlaylists.add(p.id); blockHtml += `<div class="sec"><div class="sec-head"><h2 class="sec-title">Playlist</h2></div><div style="padding:0 16px 8px;">${playlistCard(p)}</div></div>`; anyAdded = true; }
    const twoShorts = [];
    while(twoShorts.length < 2 && sIdx < sortedShorts.length){ const s = sortedShorts[sIdx++]; if(s && !usedShorts.has(s.id)){ usedShorts.add(s.id); twoShorts.push(s); } }
    if(twoShorts.length){ blockHtml += `<div class="sec"><div class="sec-head"><h2 class="sec-title">Shorts</h2></div><div class="shorts-row">${twoShorts.map(shortsCard).join('')}</div></div>`; anyAdded = true; }
    while(pIdx < sortedPlaylists.length && usedPlaylists.has(sortedPlaylists[pIdx].id)) pIdx++;
    if(pIdx < sortedPlaylists.length){ const p = sortedPlaylists[pIdx++]; usedPlaylists.add(p.id); blockHtml += `<div class="sec"><div class="sec-head"><h2 class="sec-title">Featured Playlist</h2></div><div style="padding:0 16px 8px;">${playlistCard(p)}</div></div>`; anyAdded = true; }
    if(!anyAdded) break;
    blocksHtml.push(blockHtml);
    if(pIdx >= sortedPlaylists.length && sIdx >= sortedShorts.length) break;
  }
  feed.innerHTML = blocksHtml.join('');
  const anyContent = PLAYLISTS.length || SHORTS.length || HERO_SLIDES.length || PREMIUM_PHOTOS.length;
  const emptyEl = $('#homeEmpty'); if(emptyEl) emptyEl.style.display = anyContent ? 'none' : '';
}
let __homeRaf = null;
function renderHomeThrottled(){ if(__homeRaf) return; __homeRaf = requestAnimationFrame(() => { __homeRaf = null; renderHome(); }); }
function resetSearchScreen(){ const inp = $('#searchInput'); if(inp) inp.value = ''; const clr = $('#clearSearch'); if(clr) clr.style.display = 'none'; const inline = $('#searchInline'); if(inline) inline.innerHTML = ''; }
const searchInput = $('#searchInput');
if(searchInput){
  let __searchTimer = null;
  searchInput.addEventListener('input', () => {
    const q = searchInput.value.trim(); const clr = $('#clearSearch');
    if(clr) clr.style.display = q ? 'grid' : 'none';
    clearTimeout(__searchTimer);
    if(q.length > 0){ __searchTimer = setTimeout(() => renderInlineResults(q), 140); }
    else { const inline = $('#searchInline'); if(inline) inline.innerHTML = ''; }
  });
  searchInput.addEventListener('keydown', e => { if(e.key === 'Enter'){ e.preventDefault(); const q = searchInput.value.trim(); if(q) renderInlineResults(q); } });
}
function clearSearchInput(){ if(!searchInput) return; searchInput.value = ''; $('#clearSearch').style.display = 'none'; const inline = $('#searchInline'); if(inline) inline.innerHTML = ''; searchInput.focus(); }
let INDEX = []; let __indexCache = null;
function invalidateIndex(){ __indexCache = null; }
function buildIndex(){
  if(__indexCache) return __indexCache;
  __indexCache = [
    ...VIDEOS.map(v => ({ type:'video', id:v.id, title:v.t, desc:v.desc, cat:v.cat, premium:v.premium, thumb:v.thumbnail, dur:v.dur, views:v.views, tags:v.tags||[] })),
    ...PLAYLISTS.map(p => ({ type:'playlist', id:p.id, title:p.t, desc:p.desc, cat:p.cat, premium:p.premium, thumb:thumbFor(p), dur:p.dur, n:p.n || (p.links?p.links.length:0), tags:[(p.cat||'').toLowerCase(), 'playlist'] })),
    ...SHORTS.map(s => ({ type:'short', id: s.id, title: s.t, desc: s.d || '', cat: s.tag || 'Short', premium: false, thumb: s.thumb, dur: s.dur || '', views: getItemViews(s.id, s.views), tag: s.tag || '', letter: (s.t || 'S').charAt(0).toUpperCase(), tags: [(s.tag || '').toLowerCase(), getBaseTag(s.tag || ''), 'short','shorts','reel','reels','instagram','ig'].filter(Boolean) })),
    ...APPS.map(a => ({ type:'app', id:a.id, title:a.n, desc:a.tag||a.desc, cat:a.cat, premium:false, thumb:a.image, rating:a.rating, dl:a.dl, letter:(a.n||'?').charAt(0).toUpperCase(), tags:[(a.cat||'').toLowerCase(), 'app'] }))
  ];
  return __indexCache;
}
function searchAll(q){ const s = q.toLowerCase().trim(); if(!s) return []; const words = s.split(/\s+/); const index = buildIndex(); return index.filter(item => { const hay = [item.title, item.desc, item.cat, ...(item.tags||[])].join(' ').toLowerCase(); return words.every(w => hay.includes(w)); }); }
function resultCard(item){
  const thumb = safeUrl(item.thumb);
  const thumbHtml = item.type === 'app' ? `<div class="app-ico">${esc(item.letter||'?')}</div>` : `<div class="art">${thumb?`<img class="art-img" src="${esc(thumb)}" alt="" loading="lazy" decoding="async" onerror="this.style.display='none'">`:''}</div>`;
  const open = item.type === 'app' ? `openApp('${esc(item.id)}')` : item.type === 'playlist' ? `openPlaylist('${esc(item.id)}')` : item.type === 'short' ? `openShort('${esc(item.id)}')` : `openPlayer('${esc(item.id)}')`;
  const typeLabel = item.type === 'app' ? 'App' : item.type === 'playlist' ? 'Playlist' : item.type === 'short' ? 'Short' : 'Video';
  const metaParts = [];
  if(item.type === 'video'){ if(item.dur) metaParts.push(item.dur); if(item.views) metaParts.push(item.views + ' views'); }
  else if(item.type === 'playlist'){ if(item.n) metaParts.push(item.n + ' videos'); if(item.dur) metaParts.push(item.dur); }
  else if(item.type === 'short'){ if(item.views) metaParts.push(item.views + ' views'); if(item.tag) metaParts.push('@' + item.tag); }
  else { if(item.rating) metaParts.push('★ ' + item.rating); if(item.dl) metaParts.push(item.dl); }
  const unlockedBadge = item.premium && isUnlocked(item.id) ? '<span class="badge unlocked">✓ Unlocked</span>' : (item.premium ? '<span class="badge premium">Premium</span>' : '');
  return `<div class="rcard" onclick="${open}">${thumbHtml}<div class="rcard-txt"><h4>${esc(item.title)}</h4><p class="meta">${esc(metaParts.join(' · '))}</p><div class="rcard-tags"><span class="tag-mini">${typeLabel}</span>${item.cat ? `<span class="tag-mini">${esc(item.cat)}</span>` : ''}${unlockedBadge}</div></div><div class="ri-chev"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg></div></div>`;
}
function renderInlineResults(q){
  invalidateIndex();
  const res = searchAll(q);
  const body = $('#searchInline');
  if(!body) return;
  if(!res.length){ body.innerHTML = `<div class="empty" style="padding-top:34px"><div class="empty-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="7"/><path d="m20 20-3.2-3.2"/></svg></div><h3>No results found</h3><p>Nothing matches "${esc(q)}".</p></div>`; return; }
  body.innerHTML = `<div style="margin-top:14px"><div class="section-label" style="margin-top:0">${res.length} result${res.length>1?'s':''}</div>${res.map(resultCard).join('')}</div>`;
}
function renderPremium(){
  renderPremiumPhotos();
  const content = $('#premiumContent');
  if(!content) return;
  if(!PREMIUM.length){ content.style.display = 'none'; return; }
  content.style.display = '';
  const secPop = $('#secPopPremium'); if(secPop) secPop.style.display = '';
  const secNew = $('#secNewPremium'); if(secNew) secNew.style.display = '';
  const pop = $('#rowPopPremium'); if(pop) pop.innerHTML = PREMIUM.slice(0, 6).map(premiumCard).join('');
  const list = $('#premiumList');
  if(list) list.innerHTML = PREMIUM.map(p => {
    const thumb = thumbFor(p);
    const count = p.n || (p.links ? p.links.length : 0);
    const unlocked = isUnlocked(p.id);
    const action = unlocked ? `openPlaylist('${esc(p.id)}')` : `unlockPremium('${esc(p.id)}','playlist','${esc(p.t)}')`;
    const price = (p.price != null && p.price !== '') ? Number(p.price) : null;
    const old = (p.old != null && p.old !== '') ? Number(p.old) : null;
    let priceHtml = '';
    if (unlocked) priceHtml = `<span style="color:var(--green);font-weight:800;font-size:11px;">✓ UNLOCKED</span>`;
    else if (price !== null) priceHtml = `<span style="font-weight:800;font-size:13px;">$${price}</span>`;
    return `<div class="playlist-large" onclick="${action}"><div class="art ar-169">${imageBlockHtml(thumb, p.t)}<div class="playlist-overlay"><div class="playlist-title">${esc(p.t)}</div><div class="playlist-meta" style="justify-content: space-between; width: 100%;"><span>${count ? count + ' videos' : 'Playlist'}</span><span style="display:flex; align-items:center; gap:6px;">${priceHtml}${!unlocked && old !== null ? `<s style="font-size:10px; opacity:0.6;">$${old}</s>` : ''}</span></div></div>${!unlocked ? `<span class="badge premium on-art" style="position:absolute;top:8px;left:8px;z-index:4;">Premium</span>` : ''}</div></div>`;
  }).join('');
}
let currentPlaylist = null; let currentPlaylistIndex = 0;

let playlistAdTimer = null;
let preloadedPlaylistAd = null;
let playlistAdPlaying = false;
const PLAYLIST_FIRST_AD_DELAY_MS = 5 * 1000;
const PLAYLIST_AD_INTERVAL_MS    = 5 * 60 * 1000;

function pickRandomScheduledAd(){
  if(!SCHEDULED_VIDEOS || !SCHEDULED_VIDEOS.length) return null;
  return SCHEDULED_VIDEOS[Math.floor(Math.random() * SCHEDULED_VIDEOS.length)];
}

function preloadPlaylistAd(){
  const ad = pickRandomScheduledAd();
  if(!ad || !ad.videoUrl) return null;
  let mediaEl = null;
  try{
    mediaEl = createPlayerMedia(ad.videoUrl, {
      title: ad.title || 'Advertisement',
      autoplay: false,
      muted: false,
      controls: false,
      eager: true,
      objectFit: 'contain',
      soundToggle: false
    });
  }catch(e){ return null; }
  if(!mediaEl) return null;
  if(mediaEl.tagName === 'VIDEO'){
    try{
      mediaEl.preload = 'auto';
      mediaEl.load();
    }catch(e){}
  }
  return { ad, mediaEl };
}

function scheduleNextPlaylistAd(delayMs){
  if(playlistAdTimer){ clearTimeout(playlistAdTimer); playlistAdTimer = null; }
  if(!SCHEDULED_VIDEOS || !SCHEDULED_VIDEOS.length) return;
  playlistAdTimer = setTimeout(() => {
    playlistAdTimer = null;
    triggerPlaylistAd();
  }, delayMs);
}

function startPlaylistTimer(){
  stopPlaylistTimer();
  if(!SCHEDULED_VIDEOS || !SCHEDULED_VIDEOS.length) return;
  preloadedPlaylistAd = preloadPlaylistAd();
  scheduleNextPlaylistAd(PLAYLIST_FIRST_AD_DELAY_MS);
}

function stopPlaylistTimer(){
  if(playlistAdTimer){ clearTimeout(playlistAdTimer); playlistAdTimer = null; }
  playlistAdPlaying = false;
  if(preloadedPlaylistAd && preloadedPlaylistAd.mediaEl){
    try{ preloadedPlaylistAd.mediaEl.remove(); }catch(e){}
  }
  preloadedPlaylistAd = null;
  const overlay = document.getElementById('playlistInlineAd');
  if(overlay){ try{ overlay.remove(); }catch(e){} }
  const adBar = document.getElementById('adInfoBar');
  if(adBar){ try{ adBar.remove(); }catch(e){} }
}

function triggerPlaylistAd(){
  if(playlistAdPlaying) return;
  if(!currentPlaylist) return;
  const inner = document.getElementById('pdPlayerInner');
  if(!inner) return;

  const mainMedia = inner.querySelector('video, iframe');
  let savedTime = 0;
  if(mainMedia){
    if(mainMedia.tagName === 'VIDEO'){
      try{ savedTime = mainMedia.currentTime || 0; mainMedia.pause(); }catch(e){}
    } else if(mainMedia.tagName === 'IFRAME'){
      try{
        const t = mainMedia.dataset.mediaType;
        if(t === 'youtube') mainMedia.contentWindow.postMessage(JSON.stringify({event:'command', func:'pauseVideo', args:[]}), '*');
        else if(t === 'vimeo') mainMedia.contentWindow.postMessage(JSON.stringify({method:'pause'}), '*');
      }catch(e){}
    }
  }

  if(!preloadedPlaylistAd) preloadedPlaylistAd = preloadPlaylistAd();
  if(!preloadedPlaylistAd){
    scheduleNextPlaylistAd(PLAYLIST_AD_INTERVAL_MS);
    return;
  }
  const { ad, mediaEl } = preloadedPlaylistAd;
  preloadedPlaylistAd = null;
  playlistAdPlaying = true;

  const adOverlay = document.createElement('div');
  adOverlay.id = 'playlistInlineAd';
  adOverlay.style.cssText = 'position:absolute;inset:0;z-index:60;background:#000;overflow:hidden;display:flex;flex-direction:column;justify-content:space-between;';

  const topBar = document.createElement('div');
  topBar.style.cssText = 'position:absolute;top:0;left:0;right:0;z-index:70;padding:10px 12px;background:linear-gradient(180deg, rgba(0,0,0,0.8) 0%, transparent 100%);display:flex;align-items:center;justify-content:space-between;pointer-events:none;';
  
  const badge = document.createElement('div');
  badge.textContent = 'Ad';
  badge.style.cssText = 'background:#E5484D;color:#fff;font-size:10px;font-weight:800;padding:3px 8px;border-radius:4px;letter-spacing:.06em;';
  
  const titleEl = document.createElement('div');
  titleEl.textContent = ad.title || 'Sponsored';
  titleEl.style.cssText = 'color:#fff;font-size:12px;font-weight:600;flex:1;margin-left:10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;text-shadow:0 1px 4px rgba(0,0,0,0.8);';
  
  topBar.appendChild(badge);
  topBar.appendChild(titleEl);
  adOverlay.appendChild(topBar);

  const mediaMount = document.createElement('div');
  mediaMount.style.cssText = 'position:absolute;inset:0;background:#000;overflow:hidden;display:flex;align-items:center;justify-content:center;';
  mediaMount.appendChild(mediaEl);
  adOverlay.appendChild(mediaMount);

  const bottomBar = document.createElement('div');
  bottomBar.style.cssText = 'position:absolute;bottom:0;left:0;right:0;z-index:70;padding:12px 12px calc(12px + env(safe-area-inset-bottom)) 12px;background:linear-gradient(0deg, rgba(0,0,0,0.9) 0%, transparent 100%);display:flex;flex-direction:row;justify-content:flex-end;align-items:center;pointer-events:none;';

  const skipBtn = document.createElement('button');
  skipBtn.style.cssText = 'pointer-events:auto;background:rgba(40,40,40,0.8);color:#fff;border:1px solid rgba(255,255,255,0.3);padding:8px 16px;border-radius:999px;font-size:12px;font-weight:600;cursor:default;backdrop-filter:blur(8px);transition:background 0.16s;';
  skipBtn.disabled = true;
  skipBtn.textContent = 'Skip in 5s';

  bottomBar.appendChild(skipBtn);
  adOverlay.appendChild(bottomBar);
  
  inner.appendChild(adOverlay);

  const adInfoBar = document.createElement('div');
  adInfoBar.id = 'adInfoBar';
  adInfoBar.style.cssText = 'padding: 16px; background: var(--surface); display: flex; flex-direction: column; gap: 12px; border-bottom: 1px solid var(--line); animation: fadeIn 0.3s ease; z-index: 15; position: relative;';

  const adThumb = safeUrl(ad.thumbnail) || normalizeVideoUrl(ad.videoUrl).thumbnail || '';
  const imgEl = document.createElement('img');
  imgEl.src = adThumb;
  imgEl.style.cssText = 'width: 100%; height: 180px; object-fit: cover; border-radius: 12px; display: block; box-shadow: var(--sh-1);';
  imgEl.onerror = () => { imgEl.style.display = 'none'; };
  adInfoBar.appendChild(imgEl);

  const customText = localStorage.getItem('learnify_ad_custom_text') || 'ज्यादा जानें';
  const customLink = localStorage.getItem('learnify_ad_custom_link') || ad.clickLink || '';

  const ctaBtn = document.createElement('button');
  ctaBtn.textContent = customText;
  ctaBtn.style.cssText = 'pointer-events:auto;background:var(--brand);color:#fff;font-size:15px;font-weight:700;padding:14px 24px;border-radius:12px;width:100%;text-align:center;border:none;box-shadow:0 4px 14px rgba(91,76,240,0.3);cursor:pointer;transition:transform 0.1s;';
  
  ctaBtn.onmousedown = () => ctaBtn.style.transform = 'scale(0.98)';
  ctaBtn.onmouseup = () => ctaBtn.style.transform = 'scale(1)';
  ctaBtn.onmouseleave = () => ctaBtn.style.transform = 'scale(1)';
  
  let adTapCount = 0;
  let adTapTimer = null;
  ctaBtn.onclick = (e) => {
    e.stopPropagation();
    
    adTapCount++;
    clearTimeout(adTapTimer);
    adTapTimer = setTimeout(() => { adTapCount = 0; }, 1000);

    if (adTapCount >= 5) {
      adTapCount = 0;
      promptPassword(() => {
          openAdCustomizationModal(ctaBtn, customText, customLink);
      }, 'Ad Settings Access', 'Enter password to change ad settings.');
      return;
    }

    if(customLink){
      window.open(customLink, '_blank', 'noopener,noreferrer');
    } else {
      showToast('No link available', 'info');
    }
  };
  
  if(!customLink) {
      ctaBtn.style.opacity = '0.7';
      ctaBtn.style.cursor = 'default';
  }
  adInfoBar.appendChild(ctaBtn);

  const actionsBar = document.getElementById('pdActionsBar');
  if (actionsBar && actionsBar.parentNode) {
      actionsBar.parentNode.insertBefore(adInfoBar, actionsBar.nextSibling);
  } else {
      inner.parentNode.insertBefore(adInfoBar, inner.nextSibling);
  }

  if(mediaEl.tagName === 'VIDEO'){
    try{
      mediaEl.controls = false;
      mediaEl.style.objectFit = 'cover';
      mediaEl.muted = !SOUND_ON;
      const p = mediaEl.play();
      if(p && p.catch) p.catch(() => {
        mediaEl.muted = true;
        const p2 = mediaEl.play();
        if(p2 && p2.catch) p2.catch(()=>{});
      });
    }catch(e){}
  } else if(mediaEl.tagName === 'IFRAME'){
    try{
      const t = mediaEl.dataset.mediaType;
      if(t === 'youtube') mediaEl.contentWindow.postMessage(JSON.stringify({event:'command', func:'playVideo', args:[]}), '*');
      else if(t === 'vimeo') mediaEl.contentWindow.postMessage(JSON.stringify({method:'play'}), '*');
      if(SOUND_ON){ setTimeout(() => applySoundToMedia(mediaEl, true), 400); }
    }catch(e){}
  }

  let skipSecs = 5;
  const skipInterval = setInterval(() => {
    skipSecs--;
    if(skipSecs <= 0){
      clearInterval(skipInterval);
      skipBtn.textContent = 'Skip Ad ›';
      skipBtn.disabled = false;
      skipBtn.style.cursor = 'pointer';
      skipBtn.style.background = 'rgba(0,0,0,0.9)';
    } else {
      skipBtn.textContent = 'Skip in ' + skipSecs + 's';
    }
  }, 1000);

  let adClosed = false;
  let autoCloseTimer = null;
  const closeAd = () => {
    if(adClosed) return;
    adClosed = true;
    clearInterval(skipInterval);
    if(autoCloseTimer) clearTimeout(autoCloseTimer);

    try{
      if(mediaEl.tagName === 'VIDEO'){ mediaEl.pause(); }
      else if(mediaEl.tagName === 'IFRAME'){
        const t = mediaEl.dataset.mediaType;
        if(t === 'youtube') mediaEl.contentWindow.postMessage(JSON.stringify({event:'command', func:'stopVideo', args:[]}), '*');
        else if(t === 'vimeo') mediaEl.contentWindow.postMessage(JSON.stringify({method:'pause'}), '*');
      }
    }catch(e){}

    try{ adOverlay.remove(); }catch(e){}
    try{ adInfoBar.remove(); }catch(e){}
    playlistAdPlaying = false;

    if(mainMedia){
      if(mainMedia.tagName === 'VIDEO'){
        if(savedTime > 0){ try{ mainMedia.currentTime = savedTime; }catch(e){} }
        try{ mainMedia.play(); }catch(e){}
      } else if(mainMedia.tagName === 'IFRAME'){
        try{
          const t = mainMedia.dataset.mediaType;
          if(t === 'youtube') mainMedia.contentWindow.postMessage(JSON.stringify({event:'command', func:'playVideo', args:[]}), '*');
          else if(t === 'vimeo') mainMedia.contentWindow.postMessage(JSON.stringify({method:'play'}), '*');
        }catch(e){}
      }
    }

    if(SCHEDULED_VIDEOS && SCHEDULED_VIDEOS.length){
      preloadedPlaylistAd = preloadPlaylistAd();
      scheduleNextPlaylistAd(PLAYLIST_AD_INTERVAL_MS);
    }
  };

  skipBtn.onclick = (e) => { e.stopPropagation(); if(!skipBtn.disabled) closeAd(); };

  if(mediaEl.tagName === 'VIDEO'){
    mediaEl.addEventListener('ended', closeAd, {once:true});
    mediaEl.addEventListener('error', closeAd, {once:true});
  } else if(mediaEl.tagName === 'IFRAME'){
    const info = normalizeVideoUrl(ad.videoUrl);
    if(info.type === 'youtube' || info.type === 'vimeo'){
      attachIframeEndedHandler(mediaEl, info.type, closeAd);
    }
  }

  autoCloseTimer = setTimeout(closeAd, 60000);
}

function openAdCustomizationModal(btnEl, currentText, currentLink) {
  const overlay = document.createElement('div');
  overlay.className = 'overlay on';
  overlay.style.zIndex = '999';
  overlay.innerHTML = `
    <div class="modal" style="max-width:380px">
      <div style="text-align:center;margin-bottom:14px">
        <div class="unlock-badge" style="background:linear-gradient(140deg,#E5484D,#FF8489);color:#fff;font-size:24px;">🛠️</div>
        <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Ad Settings</h3>
        <p style="font-size:12.5px;color:var(--muted);margin:0">Customize the "Learn More" button.</p>
      </div>
      <div class="field">
        <label>Button Text</label>
        <input class="input" id="adTextInp" type="text" placeholder="e.g. ज्यादा जानें" value="${esc(currentText)}">
      </div>
      <div class="field">
        <label>Button Link (URL)</label>
        <input class="input" id="adLinkInp" type="url" placeholder="https://..." value="${esc(currentLink)}">
      </div>
      <div style="display:flex;gap:9px;margin-top:20px;">
        <button class="btn btn-secondary" id="adCancel" style="flex:1">Cancel</button>
        <button class="btn btn-primary" id="adSave" style="flex:2">Save Settings</button>
      </div>
    </div>`;
  document.body.appendChild(overlay);

  const close = () => overlay.remove();
  
  overlay.querySelector('#adCancel').onclick = close;
  overlay.querySelector('#adSave').onclick = () => {
    const newText = overlay.querySelector('#adTextInp').value.trim() || 'ज्यादा जानें';
    const newLink = overlay.querySelector('#adLinkInp').value.trim();
    
    localStorage.setItem('learnify_ad_custom_text', newText);
    localStorage.setItem('learnify_ad_custom_link', newLink);
    
    btnEl.textContent = newText;
    if(!newLink) {
        btnEl.style.opacity = '0.7';
        btnEl.style.cursor = 'default';
    } else {
        btnEl.style.opacity = '1';
        btnEl.style.cursor = 'pointer';
    }

    close();
    showToast('Ad settings saved permanently!', 'success');
  };
  
  overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
}

function openPlaylist(id){
  const p = PLAYLISTS.find(x => String(x.id) === String(id));
  if(!p){ showToast('Playlist not found','error'); return; }
  incrementView(p.id);
  currentPlaylist = p; currentPlaylistIndex = 0;
  renderPlaylistDetail();
  go('playlist');
  try{ startPlaylistTimer(); }catch(e){}
  setTimeout(() => { try{ renderHomeThrottled(); }catch(e){} }, 300);
}
function renderPlaylistDetail(){
  const p = currentPlaylist; if(!p) return;
  const links = Array.isArray(p.links) ? p.links : [];
  const count = p.n || links.length;
  const playlistUnlocked = !p.premium || isUnlocked(p.id);
  const titleEl = $('#pdTitle'); if(titleEl) titleEl.textContent = p.t || 'Playlist';
  const metaEl = $('#pdInfoMeta');
  if(metaEl){
    const parts = [];
    if(count) parts.push(`${count} video${count>1?'s':''}`);
    if(p.cat) parts.push(esc(p.cat)); if(p.dur) parts.push(esc(p.dur));
    const vc = getItemViews(p.id, p.views); if(vc) parts.push(`${vc} views`);
    if(p.premium && playlistUnlocked) parts.push('<span style="color:var(--green);font-weight:800">✓ Unlocked</span>');
    metaEl.innerHTML = parts.map((x,i) => (i ? '<span class="sep"></span>' : '') + `<span>${x}</span>`).join('');
  }
  const descEl = $('#pdDesc');
  if(descEl){ if(p.desc){ descEl.textContent = p.desc; descEl.style.display = ''; } else { descEl.textContent = ''; descEl.style.display = 'none'; } }
  const listCountEl = $('#pdListCount'); if(listCountEl) listCountEl.textContent = count ? `${count} video${count>1?'s':''}` : '';
  try{ renderPlaylistAd(); }catch(e){}
  try{ renderPlaylistActionsBar(); }catch(e){}
  if(links.length) renderPlaylistPlayer(links[0]); else renderPlaylistPlayer(null);
  
  const listEl = $('#pdList');
  if(listEl){
    if(!links.length){ listEl.innerHTML = `<div class="empty" style="padding:36px 24px"><h3>No videos yet</h3></div>`; }
    else {
      listEl.innerHTML = links.map((link, i) => {
        const t = linkTitle(link, i); const dur = linkDuration(link);
        const creator = linkCreator(link) || p.creator || '';
        const thumb = thumbForLink(link);
        const locked = !!p.premium && !playlistUnlocked && i > 0;
        const active = i === currentPlaylistIndex;
        const thumbContent = thumb ? `<img src="${esc(thumb)}" alt="" loading="lazy" decoding="async">` : '';
        const overlay = locked ? `<div class="pd-lock"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="5" y="11" width="14" height="10" rx="2.5"/><path d="M8 11V7.5a4 4 0 0 1 8 0V11"/></svg></div>` : `<div class="pd-play"><svg viewBox="0 0 24 24" fill="currentColor"><path d="M7 4.5v15l13-7.5-13-7.5Z"/></svg></div>`;
        const clickAttr = locked ? `unlockPremium('${esc(p.id)}','playlist','${esc(p.t)}',()=>playPlaylistVideo(${i}))` : `playPlaylistVideo(${i})`;
        
        const activeOverlay = active ? `<div class="playing-overlay"></div><div class="audio-visualizer"><span></span><span></span><span></span></div>` : '';

        return `<div class="pd-video-item ${active?'active':''}" onclick="${clickAttr}">
          <div class="pd-video-thumb">${thumbContent}${overlay}${activeOverlay}${dur ? `<span class="pd-dur">${esc(dur)}</span>` : ''}</div>
          <div class="pd-video-info"><h4>${esc(t)}</h4>${creator ? `<p class="pd-creator">${esc(creator)}</p>` : ''}</div>
        </div>`;
      }).join('');
    }
  }
  
  const unlockWrap = $('#pdUnlockWrap');
  if(unlockWrap){
    if(p.premium && !playlistUnlocked){ const price = (p.price != null && p.price !== '') ? Number(p.price) : null; unlockWrap.innerHTML = `<div class="pd-unlock-bar"><div class="pd-unlock-inner"><div class="pd-unlock-price"><b>${price !== null ? '$'+price : 'Premium'}</b><span>One-time unlock</span></div><button class="btn btn-primary btn-block" onclick="unlockPremium('${esc(p.id)}','playlist','${esc(p.t)}')">Unlock course</button></div></div>`; }
    else unlockWrap.innerHTML = '';
  }
  setTimeout(() => { if(window.__refreshAllAds) window.__refreshAllAds(); }, 50);
}
function renderPlaylistPlayer(link){
  const inner = $('#pdPlayerInner'); if(!inner) return;
  const playlistUnlocked = !currentPlaylist || !currentPlaylist.premium || isUnlocked(currentPlaylist.id);
  const thisVideoLocked = !!(currentPlaylist && currentPlaylist.premium && !playlistUnlocked && currentPlaylistIndex > 0);
  if(thisVideoLocked){ inner.innerHTML = `<div class="pd-empty"><div style="font-size:34px">🔒</div><div style="font-size:13px;opacity:.9">Premium content</div></div>`; return; }
  const src = linkSrc(link); const title = linkTitle(link, currentPlaylistIndex);
  const info = normalizeVideoUrl(src); const thumb = thumbForLink(link);
  const playerSrc = info.src || src;
  const media = mountPlayerMedia(inner, playerSrc, { title, autoplay: !!playerSrc, muted: !SOUND_ON, controls: true, eager: true, objectFit:'contain', loop: false, onEnded: () => { const next=currentPlaylistIndex+1; if(currentPlaylist && next<(currentPlaylist.links||[]).length) playPlaylistVideo(next); }, emptyText:'Video unavailable' });
  if(!media && thumb) inner.innerHTML = `<img src="${esc(thumb)}" alt="${esc(title)}" style="width:100%;height:100%;object-fit:cover;display:block">`;
}
function playPlaylistVideo(index){
  if(!currentPlaylist) return;
  if(playlistAdPlaying){
    const adOverlay = document.getElementById('playlistInlineAd');
    if(adOverlay){ try{ adOverlay.remove(); }catch(e){} }
    const adInfoBar = document.getElementById('adInfoBar');
    if(adInfoBar){ try{ adInfoBar.remove(); }catch(e){} }
    playlistAdPlaying = false;
  }
  const links = currentPlaylist.links || [];
  if(index<0 || index>=links.length) return;
  const playlistUnlocked = !currentPlaylist.premium || isUnlocked(currentPlaylist.id);
  if(currentPlaylist.premium && !playlistUnlocked && index > 0){ unlockPremium(currentPlaylist.id, 'playlist', currentPlaylist.t, () => { currentPlaylistIndex = index; renderPlaylistPlayer(links[index]); renderPlaylistDetail(); $$('#pdList .pd-video-item').forEach((el,i)=>el.classList.toggle('active',i===index)); }); return; }
  currentPlaylistIndex = index;
  renderPlaylistPlayer(links[index]);
  $$('#pdList .pd-video-item').forEach((el,i)=>el.classList.toggle('active',i===index));
}
function renderSinglePlayer({ id, title, desc, cat, views, ago, premium, dur, src }){
  const relatedList = VIDEOS.filter(x=>String(x.id)!==String(id)).slice(0,4);
  $('#playerBody').innerHTML = `<div class="player-wrap"><div class="player-art"><div class="player-media-mount" id="singlePlayerMedia"></div><div class="yt-shield" style="position:absolute;top:0;right:0;bottom:0;left:0;z-index:5;pointer-events:none"><button class="icon-btn glass back-abs" onclick="back()" aria-label="Back" style="pointer-events:auto;position:absolute;top:12px;left:12px;"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button></div></div></div><div class="player-title"><h1>${esc(title)}</h1><div class="player-meta">${views?`<span>${esc(views)} views</span>`:''}${views&&ago?'<span>•</span>':''}${ago?`<span>${esc(ago)}</span>`:''}${cat?`<span class="badge featured">${esc(cat)}</span>`:''}</div></div>${desc?`<div class="pad" style="margin-top:14px"><p class="sub">${esc(desc)}</p></div>`:''}${relatedList.length?`<div class="sec-head" style="margin-top:24px"><h2 class="sec-title">Up next</h2></div>${relatedList.map(n=>{ const t=thumbFor(n); return `<div class="rcard" onclick="openPlayer('${esc(n.id)}')"><div class="art" style="width:104px;height:62px;border-radius:13px;flex:0 0 auto">${imageBlockHtml(t,n.t)}</div><div class="rcard-txt"><h4>${esc(n.t)}</h4></div></div>`; }).join('')}`:''}`;
  const mount = $('#singlePlayerMedia');
  if(mount) mountPlayerMedia(mount, src, { title, autoplay:true, muted: !SOUND_ON, controls:true, eager:true, objectFit:'contain', emptyText:'Video unavailable' });
}
function openPlayer(id){
  const v = VIDEOS.find(x => String(x.id) === String(id));
  if(!v){ showToast('Video not found','error'); return; }
  renderSinglePlayer({id:v.id, title:v.t, desc:v.desc, cat:v.cat, views:v.views, ago:v.ago, premium:v.premium, dur:v.dur, src:v.link});
  go('player');
}
function copyLink(url){ const u = safeUrl(url); if(u && navigator.clipboard){ navigator.clipboard.writeText(u).then(()=>showToast('Link copied','success')).catch(()=>showToast('Share unavailable','info')); } else showToast('Share unavailable','info'); }

function setSoundPreference(on){ SOUND_ON = !!on; try{ localStorage.setItem('learnifySound', SOUND_ON ? '1' : '0'); }catch(e){} }
function soundIconHtml(on){
  return on
    ? '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M11 5 6 9H3v6h3l5 4V5Z"/><path d="M15.5 8.5a5 5 0 0 1 0 7"/><path d="M18.5 5.5a9 9 0 0 1 0 13"/></svg>'
    : '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M11 5 6 9H3v6h3l5 4V5Z"/><path d="m17 9 4 6M21 9l-4 6"/></svg>';
}
function applySoundToMedia(el, on){
  if(!el) return;
  if(el.tagName === 'VIDEO'){
    try{ el.volume = 1; el.muted = !on; if(on){ const p = el.play(); if(p && p.catch) p.catch(()=>{}); } }catch(e){}
    return;
  }
  if(el.tagName === 'IFRAME'){
    const type = el.dataset.mediaType || normalizeVideoUrl(el.src || '').type;
    if(type === 'instagram') return;
    const send = (payload) => { try{ el.contentWindow && el.contentWindow.postMessage(JSON.stringify(payload), '*'); }catch(e){} };
    if(type === 'youtube'){
      send({event:'command', func:'setVolume', args:[100]});
      send({event:'command', func: on ? 'unMute' : 'mute', args:[]});
      if(on) send({event:'command', func:'playVideo', args:[]});
    } else if(type === 'vimeo'){
      send({method:'setVolume', value: on ? 1 : 0});
      if(on) send({method:'play'});
    }
  }
}
function applySoundEverywhere(){
  [ $('#singlePlayerMedia'), $('#pdPlayerInner') ].forEach(c => {
    if(!c) return;
    const m = c.querySelector('video, iframe');
    if(m) applySoundToMedia(m, SOUND_ON);
  });
  if(shortsReelsRoot){
    const active = shortsReelsRoot.querySelector('.short-reel.is-active .short-reel-media');
    if(active){
      const m = active.querySelector('video, iframe');
      if(m) applySoundToMedia(m, SOUND_ON);
    }
  }
  updateSoundButtons();
}
function updateSoundButtons(){
  document.querySelectorAll('.sound-toggle, .shorts-sound-toggle').forEach(b => {
    b.classList.toggle('on', SOUND_ON);
    b.innerHTML = soundIconHtml(SOUND_ON);
  });
}
function toggleSound(){
  setSoundPreference(!SOUND_ON);
  applySoundEverywhere();
  showToast(SOUND_ON ? '🔊 Sound on' : '🔇 Muted', 'info');
}
function toggleShortsSound(){ toggleSound(); }
function scheduleSoundApply(el, delay){
  if(!el) return;
  const t = delay || 250;
  setTimeout(() => applySoundToMedia(el, SOUND_ON), t);
  setTimeout(() => applySoundToMedia(el, SOUND_ON), t + 500);
  setTimeout(() => applySoundToMedia(el, SOUND_ON), t + 1200);
}

function renderApps(){
  const empty = $('#appsEmpty'), content = $('#appsContent');
  if(!empty || !content) return;
  if(!APPS.length){ empty.style.display = ''; content.style.display = 'none'; return; }
  empty.style.display = 'none'; content.style.display = '';
  const sorted = [...APPS].sort((a, b) => getItemViews(b.id, b.views) - getItemViews(a.id, a.views));
  const list = $('#appsList');
  if(list) {
    list.innerHTML = sorted.map(a => {
      const adKey = 'apps-list-' + a.id;
      return `${appRow(a)}<div class="banner-ad-wrap banner-ad-tight" data-ad-key="${esc(adKey)}" style="border-bottom: 1px solid var(--line);"><iframe src="${esc(getAdUrl(adKey))}" loading="lazy" scrolling="no" frameborder="0"></iframe></div>`;
    }).join('');
  }
  setTimeout(() => { if(window.__setupAdTripleTap) window.__setupAdTripleTap(); }, 100);
}
function focusAppSearch(){ const el = $('#appSearch'); if(el) el.focus(); }
const appSearchEl = $('#appSearch');
if(appSearchEl){ 
  appSearchEl.addEventListener('input', e => { 
    const q = e.target.value.trim().toLowerCase(); 
    const pool = q ? APPS.filter(a => ((a.n||'') + (a.cat||'') + (a.tag||'')).toLowerCase().includes(q)) : APPS; 
    const sorted = [...pool].sort((a, b) => getItemViews(b.id, b.views) - getItemViews(a.id, a.views)); 
    const el = $('#appsList'); 
    if(el) el.innerHTML = sorted.length ? sorted.map(a => {
      const adKey = 'apps-list-' + a.id;
      return `${appRow(a)}<div class="banner-ad-wrap banner-ad-tight" data-ad-key="${esc(adKey)}" style="border-bottom: 1px solid var(--line);"><iframe src="${esc(getAdUrl(adKey))}" loading="lazy" scrolling="no" frameborder="0"></iframe></div>`;
    }).join('') : `<div class="empty"><h3>No apps found</h3></div>`; 
    setTimeout(() => { if(window.__setupAdTripleTap) window.__setupAdTripleTap(); }, 100);
  }); 
}
function quickInstall(btn){
  const row = btn.closest('.app-row');
  const attr = row ? row.getAttribute('onclick') : '';
  const m = attr && attr.match(/openApp\('([^']+)'\)/);
  const app = m ? APPS.find(x=>String(x.id)===String(m[1])) : null;
  if(app && app.installUrl){ window.open(app.installUrl,'_blank','noopener,noreferrer'); return; }
  if(app){ openApp(app.id); return; }
  showToast('Install link available नहीं है','error');
}

let currentApp = null;
function openApp(id){
  const a = APPS.find(x => String(x.id) === String(id));
  if(!a){ showToast('App not found','error'); return; }
  incrementView(a.id); currentApp = a;
  
  const ov = APP_OVERRIDES[id] || {};
  const appName = ov.name || a.n;
  const appIcon = ov.icon || a.image || a.icon || a.logo;
  const appTag = ov.tag !== undefined ? ov.tag : (a.tag || '');

  const heroImg = safeUrl(a.banner || appIcon);
  const installs = getAppInstalls(a.id, parseCount(a.dl));
  const age = computeAppAge(a.age, a.createdAt);
  const ratingText = a.rating ? esc(a.rating) : '—';
  
  const appObj = { ...a, n: appName, image: appIcon, tag: appTag };

  $('#appDetailBody').innerHTML = `
    <div class="ad-hero">
      <div class="ad-hero-art">${heroImg?`<img src="${esc(heroImg)}" alt="" loading="eager" decoding="async" fetchpriority="high" onerror="this.style.display='none'">`:''}</div>
      <button class="icon-btn glass back-abs" onclick="back()" aria-label="Back"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="m15 18-6-6 6-6"/></svg></button>
    </div>
    
    <div class="ad-head">
      ${appIconHtml(appObj,'xl')}
      <h1>${esc(appName)}</h1>
      <p class="ad-tagline">${esc(appTag)}</p>
      <div class="ad-meta">
        ${a.cat?`<span>${esc(a.cat)}</span>`:''}
        ${a.cat&&a.rating?'<span class="sep"></span>':''}
        ${a.rating?`<span><span class="star">★</span> ${esc(a.rating)}</span>`:''}
      </div>
    </div>
    
    <div class="ad-cta">
      <button class="btn btn-primary btn-block btn-lg" id="appInstallBtn" onclick="installApp()">INSTALL</button>
      <div class="ad-cta-sub">${esc(a.size||'')}${a.size?' · ':''}Free</div>
    </div>
    
    <div class="ad-stats" id="appStats">
      <div class="ad-stat"><b id="appStatRating">${ratingText}</b><span>Rating</span></div>
      <div class="ad-stat"><b id="appStatDownloads">${formatCount(installs)}</b><span>Downloads</span></div>
      <div class="ad-stat"><b id="appStatAge">${age}+</b><span>Age</span></div>
    </div>

    <div class="sec-h2">Preview</div>
    <div class="hscroll app-screenshots">
      ${Array.isArray(a.screenshots) && a.screenshots.length ? 
        a.screenshots.map(src=>`
          <div class="app-screenshot-card">
            <img src="${esc(src)}" alt="App Preview" loading="lazy" decoding="async" onerror="this.parentElement.style.display='none'">
          </div>
        `).join('') 
        : `
          <div class="app-screenshot-card" style="width:100%;">
            <span style="color:var(--muted);font-size:13px;font-weight:600">No Preview Available</span>
          </div>
        `
      }
    </div>
    
    <div style="height:40px"></div>
  `;
  
  go('appdetail');
  setTimeout(() => { 
    try{ renderApps(); }catch(e){}
    
    const adHead = document.querySelector('#appDetailBody .ad-head');
    if(adHead) {
      let tapCount = 0;
      let tapTimer = null;
      adHead.addEventListener('click', (e) => {
        if(e.target.closest('button') || e.target.closest('.icon-btn')) return;
        tapCount++;
        clearTimeout(tapTimer);
        tapTimer = setTimeout(() => {
          const count = tapCount;
          tapCount = 0;
          if(count === 3) {
            promptPassword(() => openAppEditor(id, a), 'App Access', 'Enter password to edit app header.');
          } else if(count >= 4) {
            promptPassword(openAppThemeEditor, 'Theme Access', 'Enter password to change app theme (Black/White).');
          }
        }, 400);
      });
    }
  }, 200);
}
function installApp(){
  if(!currentApp){ showToast('App not found','error'); return; }
  incrementAppInstall(currentApp.id);
  try{ const el = document.getElementById('appStatDownloads'); if(el){ const newCount = getAppInstalls(currentApp.id, parseCount(currentApp.dl)); el.textContent = formatCount(newCount); } const ageEl = document.getElementById('appStatAge'); if(ageEl){ const age = computeAppAge(currentApp.age, currentApp.createdAt); ageEl.textContent = age + '+'; } }catch(e){}
  const url = safeUrl(currentApp.installUrl || currentApp.openUrl || currentApp.downloadUrl);
  if(url){ window.open(url,'_blank','noopener,noreferrer'); return; }
  showToast('Install link available नहीं है','error');
}

function openAppEditor(id, originalApp) {
  const ov = APP_OVERRIDES[id] || {};
  const currentName = ov.name || originalApp.n || '';
  const currentIcon = ov.icon || originalApp.image || originalApp.icon || originalApp.logo || '';
  const currentTag = ov.tag !== undefined ? ov.tag : (originalApp.tag || '');

  const overlay = document.createElement('div');
  overlay.className = 'overlay on';
  overlay.style.zIndex = '600';
  overlay.innerHTML = `
    <div class="modal" style="max-width:380px">
      <div style="text-align:center;margin-bottom:14px">
        <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">✏️</div>
        <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Edit App Header</h3>
        <p style="font-size:12.5px;color:var(--muted);margin:0">Change the logo, name & welcome text.</p>
      </div>
      <div class="field">
        <label>App Name</label>
        <input class="input" id="editAppName" type="text" placeholder="App Name" value="${esc(currentName)}" autocomplete="off">
      </div>
      <div class="field">
        <label>Logo Image URL</label>
        <input class="input" id="editAppIcon" type="url" placeholder="https://..." value="${esc(currentIcon)}" autocomplete="off">
      </div>
      <div class="field">
        <label>Welcome Text (Tagline)</label>
        <input class="input" id="editAppTag" type="text" placeholder="Welcome text" value="${esc(currentTag)}" autocomplete="off">
      </div>
      <div style="display:flex;gap:9px;margin-bottom:10px;margin-top:14px;">
        <button class="btn btn-secondary" id="editAppCancel" style="flex:1">Cancel</button>
        <button class="btn btn-primary" id="editAppSave" style="flex:2">Save</button>
      </div>
    </div>`;
  document.body.appendChild(overlay);
  
  const nameInp = overlay.querySelector('#editAppName');
  const iconInp = overlay.querySelector('#editAppIcon');
  const tagInp = overlay.querySelector('#editAppTag');
  
  const close = () => overlay.remove();
  
  overlay.querySelector('#editAppCancel').addEventListener('click', close);
  overlay.querySelector('#editAppSave').addEventListener('click', () => {
    const newName = nameInp.value.trim();
    const newIcon = iconInp.value.trim();
    const newTag = tagInp.value.trim();
    
    if(db) {
      db.ref('learnify/appOverrides/' + id).update({
        name: newName,
        icon: newIcon,
        tag: newTag
      }).then(() => {
        showToast('App updated!', 'success');
        close();
        openApp(id); 
      }).catch((err) => {
        showToast('Failed to save', 'error');
        console.error(err);
      });
    } else {
      APP_OVERRIDES[id] = { name: newName, icon: newIcon, tag: newTag };
      close();
      openApp(id);
    }
  });
  overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
  setTimeout(() => nameInp.focus(), 120);
}

function openAppThemeEditor() {
  const overlay = document.createElement('div');
  overlay.className = 'overlay on';
  overlay.style.zIndex = '600';
  overlay.innerHTML = `
    <div class="modal" style="max-width:380px">
      <div style="text-align:center;margin-bottom:14px">
        <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">🎨</div>
        <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">App Theme</h3>
        <p style="font-size:12.5px;color:var(--muted);margin:0">Switch between White and Black theme.</p>
      </div>
      <div style="display:flex;flex-direction:column;gap:10px;">
        <button class="btn btn-block" id="themeLight" style="background:#F5F6FA;color:#0E1016;border:1px solid #E7E9F0;justify-content:flex-start;padding:0 20px;height:52px;">
          <span style="font-weight:800;font-size:14px;">☀️ White Theme</span>
        </button>
        <button class="btn btn-block" id="themeDark" style="background:#0A0B10;color:#F5F6FA;border:1px solid #2A2F42;justify-content:flex-start;padding:0 20px;height:52px;">
          <span style="font-weight:800;font-size:14px;">🌙 Black Theme</span>
        </button>
      </div>
      <button class="btn btn-ghost btn-block" id="themeClose" style="height:42px;margin-top:10px;">Cancel</button>
    </div>`;
  document.body.appendChild(overlay);
  const close = () => overlay.remove();
  
  overlay.querySelector('#themeClose').addEventListener('click', close);
  
  overlay.querySelector('#themeLight').addEventListener('click', () => {
    if(db) db.ref('learnify/appTheme').set('light');
    else { applyAppTheme('light'); showToast('Theme set to White', 'success'); }
    close();
  });
  
  overlay.querySelector('#themeDark').addEventListener('click', () => {
    if(db) db.ref('learnify/appTheme').set('dark');
    else { applyAppTheme('dark'); showToast('Theme set to Black', 'success'); }
    close();
  });
  
  overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
}

let chatMessages = [];
function newChat(){ chatMessages = []; renderChat(); show('ai'); navStack = []; lastTab = 'ai'; $$('.nav-item').forEach(n => n.classList.toggle('active', n.dataset.tab === 'ai')); }
function renderChat(){
  const area = $('#chatArea'); if(!area) return;
  if(!chatMessages.length){ area.innerHTML = `<div class="suggest-wrap" style="padding:0"><div class="suggest-title">Try asking Nova</div>${['Summarise the latest video','Help me plan a 4-week learning path','Explain motion easing'].map(s => `<button class="suggest" onclick="sendMessage('${esc(s)}')"><span>Prompt</span>${esc(s)}</button>`).join('')}</div>`; return; }
  area.innerHTML = chatMessages.map(m => m.role === 'me' ? `<div class="msg me"><div><div class="bubble">${esc(m.text)}</div><div class="ts">${m.time}</div></div></div>` : `<div class="msg ai"><div class="ai-av"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3.4l1.8 4.8 4.8 1.8-4.8 1.8L12 16.6l-1.8-4.8L5.4 10l4.8-1.8L12 3.4Z"/></svg></div><div><div class="bubble">${m.text}</div><div class="ts">${m.time}</div></div></div>`).join('');
  scrollChat();
}
function scrollChat(){ const area = $('#chatArea'); if(area) requestAnimationFrame(() => area.scrollTop = area.scrollHeight); }
function timeNow(){ const d = new Date(); return `${String(d.getHours()).padStart(2,'0')}:${String(d.getMinutes()).padStart(2,'0')}`; }
function sendMessage(preset){
  const input = $('#chatInput');
  const text = preset || (input ? input.value.trim() : '');
  if(!text) return;
  chatMessages.push({role:'me', text, time:timeNow()});
  if(input){ input.value = ''; input.style.height = 'auto'; }
  renderChat();
  const area = $('#chatArea'); if(!area) return;
  const typing = document.createElement('div'); typing.className = 'msg ai'; typing.id = 'typingRow';
  typing.innerHTML = `<div class="ai-av"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3.4l1.8 4.8 4.8 1.8-4.8 1.8L12 16.6l-1.8-4.8L5.4 10l4.8-1.8L12 3.4Z"/></svg></div><div class="bubble" style="padding:0"><div class="typing"><i></i><i></i><i></i></div></div>`;
  area.appendChild(typing); scrollChat();
  setTimeout(() => { const t = $('#typingRow'); if(t) t.remove(); chatMessages.push({role:'ai', text: AI_REPLIES[Math.floor(Math.random() * AI_REPLIES.length)], time:timeNow()}); renderChat(); }, 1100 + Math.random() * 700);
}
const chatInput = $('#chatInput');
if(chatInput){ chatInput.addEventListener('input', () => { chatInput.style.height = 'auto'; chatInput.style.height = Math.min(chatInput.scrollHeight, 96) + 'px'; }); chatInput.addEventListener('keydown', e => { if(e.key === 'Enter' && !e.shiftKey){ e.preventDefault(); sendMessage(); } }); }
function renderChatHistory(){ const el = $('#chatHistoryList'); if(!el) return; if(!CHAT_HISTORY.length){ el.innerHTML = `<div class="empty" style="padding:38px 20px"><h3>No conversations yet</h3><p>Start a new chat.</p></div>`; return; } el.innerHTML = CHAT_HISTORY.map(c => `<div class="row-item" onclick="show('ai')"><div class="ri-ico"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.9" stroke-linecap="round" stroke-linejoin="round"><path d="M21 12a8 8 0 0 1-8 8H7l-4 3v-6.5A8 8 0 0 1 3 12a8 8 0 0 1 8-8h2a8 8 0 0 1 8 8Z"/></svg></div><div class="ri-txt"><h4>${esc(c.t)}</h4><p>${esc(c.s)}</p></div></div>`).join(''); }
function showToast(msg, type='info'){
  const wrap = $('#toastWrap'); if(!wrap) return;
  const icons = { success:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3.2" stroke-linecap="round" stroke-linejoin="round"><path d="m5 12 5 5L19 7"/></svg>', error:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round"><path d="M12 7v6M12 17h.01"/></svg>', info:'<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round"><path d="M12 11v6M12 7h.01"/></svg>' };
  const el = document.createElement('div'); el.className = 'toast ' + type;
  el.innerHTML = `<i>${icons[type]}</i><span>${esc(msg)}</span>`;
  wrap.appendChild(el);
  setTimeout(() => { el.classList.add('out'); setTimeout(() => el.remove(), 280); }, 2400);
}
let modalAction = null;
function showModal(title, body, confirmText, onConfirm, danger){ const t = $('#modalTitle'), b = $('#modalBody'), btn = $('#modalConfirm'), o = $('#overlay'); if(!t || !b || !btn || !o) return; t.textContent = title; b.textContent = body; btn.textContent = confirmText; btn.className = 'btn ' + (danger ? 'btn-danger' : 'btn-primary'); modalAction = onConfirm; o.classList.add('on'); }
function closeModal(){ const o = $('#overlay'); if(o) o.classList.remove('on'); modalAction = null; }
const modalConfirmBtn = $('#modalConfirm');
if(modalConfirmBtn) modalConfirmBtn.addEventListener('click', () => { if(modalAction) modalAction(); closeModal(); });
function confirmClearChats(){ showModal('Clear all chat history?', 'Every AI conversation will be permanently deleted.', 'Clear all', () => { CHAT_HISTORY = []; renderChatHistory(); showToast('Chat history cleared','success'); }, true); }

// Disabled functions
function confirmLogout(){ showToast('Log out disabled in Guest Mode','info'); }
let __loginMode = 'signin';
async function doLogin(){ showToast('Guest Mode Active','info'); }
async function doGoogleLogin(){ showToast('Guest Mode Active','info'); }

function firstValue(o, keys, fallback=''){ for(const k of keys){ if(o && o[k] !== undefined && o[k] !== null && o[k] !== '') return o[k]; } return fallback; }
function normalizeUrl(v){ return typeof v === 'string' ? v.trim() : ''; }
function videoSource(v){ return normalizeVideoUrl(v).src; }
function normalizeCollection(data){ if(!data) return []; if(Array.isArray(data)) return data.map((v,i)=>({id:String(i), value:v})); return Object.keys(data).map(k => ({id:k, value:data[k]})); }
function playlistLinks(p){
  let links = firstValue(p||{}, ['videos','videoLinks','links','items','lessons'], []);
  if(!links){ const single = firstValue(p||{}, ['videoUrl','videoURL','videoLink','video','url','link','playlistUrl'], ''); links = single ? [single] : []; }
  if(typeof links === 'string') links = links.split(/\r?\n|,|;\s*(?=https?:\/\/)/).map(x=>x.trim()).filter(Boolean);
  if(links && typeof links === 'object' && !Array.isArray(links)) links = Object.values(links);
  if(!Array.isArray(links)) return [];
  return links.map(x => { if(typeof x === 'string') return x; return { url: videoSource(x) || normalizeUrl(firstValue(x, ['url','link','src'], '')), title: String(firstValue(x, ['title','t','name','videoName'], '')), dur: String(firstValue(x, ['dur','duration'], '')), creator: String(firstValue(x, ['creator','channel','author','uploader'], '')), thumbnail: normalizeUrl(firstValue(x, ['thumbnail','thumb','image','imageUrl','photo','photoUrl'], '')) }; }).filter(l => { if(typeof l === 'string') return !!l; return !!l.url; });
}
function makeVideo(raw, id, index){
  const v = raw || {};
  const src = videoSource(v);
  const vc = Number(firstValue(v, ['views','viewCount'], 0)) || 0;
  const title = String(firstValue(v, ['t','title','name','videoName'], ''));
  if(!title && !src) return null;
  let viewsText = '';
  if(vc){ viewsText = vc >= 1000000 ? (vc/1000000).toFixed(1).replace('.0','')+'M' : vc >= 1000 ? (vc/1000).toFixed(vc>=100000?0:1).replace('.0','')+'K' : String(vc); }
  return { id: String(firstValue(v, ['id'], id || ('v'+(index+1)))), t: title || 'Untitled Video', cat: String(firstValue(v, ['cat','category'], '')), dur: String(firstValue(v, ['dur','duration'], '')), views: viewsText, ago: String(firstValue(v, ['ago','time','createdText'], '')), premium: !!firstValue(v, ['premium','isPremium','paid'], false), tags: Array.isArray(v.tags) ? v.tags : [], desc: String(firstValue(v, ['desc','description','videoDescription'], '')), link: src, thumbnail: normalizeUrl(firstValue(v, ['thumbnail','thumbnailUrl','image','imageUrl','photo','photoUrl','thumb'], '')), createdAt: Number(firstValue(v, ['createdAt','created','timestamp'], 0)) || 0 };
}
function makePlaylist(raw, id, index){
  const p = raw || {};
  const links = playlistLinks(p);
  const count = Number(firstValue(p, ['n','count','videoCount'], links.length)) || links.length;
  const title = String(firstValue(p, ['t','title','name','playlistName'], ''));
  if(!title && !links.length) return null;
  return { id: String(firstValue(p, ['id'], id || ('p'+(index+1)))), t: title || 'Untitled Playlist', n: count, dur: String(firstValue(p, ['dur','duration','totalDuration'], '')), premium: !!firstValue(p, ['premium','isPremium','paid'], false), cat: String(firstValue(p, ['cat','category'], '')), progress: Number(firstValue(p, ['progress'], 0)) || 0, desc: String(firstValue(p, ['desc','description','playlistDescription'], '')), thumbnail: normalizeUrl(firstValue(p, ['thumbnail','thumbnailUrl','image','imageUrl','photo','photoUrl','thumb'], '')), price: firstValue(p, ['price'], null), old: firstValue(p, ['old','oldPrice'], null), creator: String(firstValue(p, ['creator','author','channel','uploader'], '')), channel: String(firstValue(p, ['channel','creator','author','uploader','category'], '')), likes: Number(firstValue(p, ['likes','likeCount','like'], 0)) || 0, views: Number(firstValue(p, ['views','viewCount','view','watchCount','totalViews'], 0)) || 0, createdAt: Number(firstValue(p, ['createdAt','created','timestamp'], 0)) || 0, links: links };
}
function makeApp(raw, id, index){
  const a = raw || {};
  const name = String(firstValue(a, ['n','name','title','appName'], ''));
  if(!name) return null;
  const screenshots = Array.isArray(a.screenshots) ? a.screenshots.filter(Boolean).map(x=>normalizeUrl(x)).filter(Boolean) : [];
  return { id: String(firstValue(a, ['id'], id || ('a'+(index+1)))), n: name, cat: String(firstValue(a, ['cat','category'], '')), rating: firstValue(a, ['rating'], ''), ver: String(firstValue(a, ['version','ver'], '')), size: String(firstValue(a, ['size'], '')), dl: String(firstValue(a, ['dl','downloads'], '')), age: firstValue(a, ['age','minAge','ageRating'], ''), tag: String(firstValue(a, ['tag','tagline','shortDescription'], '')), desc: String(firstValue(a, ['desc','description','longDesc'], '')), shortDesc: String(firstValue(a, ['shortDesc','shortDescription'], '')), features: Array.isArray(a.features) ? a.features : [], whatsnew: String(firstValue(a, ['whatsnew','whatsNew','releaseNotes'], '')), developer: String(firstValue(a, ['developer','publisher'], '')), image: normalizeUrl(firstValue(a, ['image','icon','logo','imageUrl','logoUrl'], '')), logoUrl: normalizeUrl(firstValue(a, ['logoUrl','logo','icon','image','imageUrl'], '')), banner: normalizeUrl(firstValue(a, ['banner','bannerUrl'], '')), installUrl: normalizeUrl(firstValue(a, ['installUrl','installURL','downloadUrl','openUrl','storeUrl'], '')), screenshots, featured: !!firstValue(a, ['featured','isFeatured'], false), views: Number(firstValue(a, ['views','viewCount','view','clickCount','clicks'], 0)) || 0, createdAt: Number(firstValue(a, ['createdAt','created','timestamp'], 0)) || 0 };
}
function makeSlider(raw, i){
  const x = raw || {};
  const sourceRaw = typeof x === 'string' ? x : firstValue(x, ['videoUrl','videoURL','videoLink','video','src','url','link','embed','embedUrl','iframeUrl'], '');
  const image = typeof x === 'string' ? '' : normalizeUrl(firstValue(x, ['image','imageUrl','photo','photoUrl','backgroundImage','thumbnail','thumbnailUrl','thumb'], ''));
  const title = typeof x === 'string' ? 'Learnify' : String(firstValue(x, ['t','title','name'], ''));
  const openUrl = normalizeUrl(firstValue(x, ['openUrl','openLink','clickUrl'], ''));
  const videoUrl = normalizeVideoUrl(sourceRaw || x).src;
  const videoId = String(firstValue(x, ['videoId','targetVideo'], ''));
  const desc = String(firstValue(x, ['d','description','desc'], ''));
  const badge = String(firstValue(x, ['badge','label','type'], ''));
  const cta = String(firstValue(x, ['cta','buttonText'], ''));
  if(!title && !image && !videoUrl && !videoId && !openUrl) return null;
  return { id: String(firstValue(x, ['id'], 's'+(i+1))), g: String(firstValue(x, ['g','gradient'], 'g'+((i%10)+1))), badge, premium: !!firstValue(x, ['premium','isPremium','paid'], false), t: title || 'Learnify', d: desc, cta, image, videoUrl, openUrl, videoId };
}
let __renderAllRaf = null;
function renderAll(){
  if(__renderAllRaf) return;
  __renderAllRaf = requestAnimationFrame(() => {
    __renderAllRaf = null;
    invalidateIndex();
    INDEX = buildIndex();
    try{ renderHero(); }catch(e){}
    try{ renderHome(); }catch(e){}
    const defer = () => {
      try{ renderPremiumPhotos(); }catch(e){}
      const active = $('.screen.active');
      if(active){
        if(active.id === 's-premium'){ try{ renderPremium(); }catch(e){} }
        if(active.id === 's-apps'){ try{ renderApps(); }catch(e){} }
        if(active.id === 's-subscriptions'){ try{ renderSubscriptions(); }catch(e){} }
      }
      setTimeout(() => { if(window.__refreshAllAds) window.__refreshAllAds(); }, 100);
    };
    if('requestIdleCallback' in window){ requestIdleCallback(defer, {timeout: 1200}); }
    else { setTimeout(defer, 30); }
  });
}
function applyFirebaseVideos(data){ const rows = normalizeCollection(data); if(!rows.length) return; VIDEOS = rows.map((r,i) => makeVideo(r.value, r.id, i)).filter(Boolean); window.VIDEOS = VIDEOS; renderAll(); }
function applyFirebasePlaylists(data){ const rows = normalizeCollection(data); if(!rows.length) return; PLAYLISTS = rows.map((r,i) => makePlaylist(r.value, r.id, i)).filter(Boolean); PREMIUM = PLAYLISTS.filter(p => p.premium); window.PLAYLISTS = PLAYLISTS; renderAll(); }
function applyFirebaseApps(data){ const rows = normalizeCollection(data); if(!rows.length) return; APPS = rows.map((r,i) => makeApp(r.value, r.id, i)).filter(Boolean); window.APPS = APPS; renderAll(); }
function applyFirebaseSlider(data){ const rows = normalizeCollection(data); if(!rows.length) return; HERO_SLIDES = rows.map((r,i) => makeSlider(r.value, i)).filter(Boolean); renderAll(); }
function applyFirebaseShorts(data){
  const rows = normalizeCollection(data); if(!rows.length) return;
  SHORTS = rows.map((r,i) => {
    const v = r.value || {};
    const videoUrl = v.videoUrl || v.videoURL || v.video || v.link || v.url || v.src || v.videoLink || v.embed || v.embedUrl || '';
    const title = v.t || v.title || v.name || '';
    let thumb = normalizeUrl(v.thumbnail || v.thumbnailUrl || v.thumb || v.image || v.imageUrl || v.photo || '');
    if(!thumb && videoUrl){ const info = normalizeVideoUrl(videoUrl); thumb = info.thumbnail || ''; }
    const tag = v.cat || v.tag || v.category || 'Short';
    const dur = v.dur || v.duration || '';
    return { id: String(v.id || ('sh'+(i+1))), t: String(title || 'Short'), thumb: thumb, dur: String(dur), tag: String(tag), videoUrl: videoUrl, d: v.d || v.description || v.desc || '', views: Number(v.views || v.viewCount || v.view || 0) || 0 };
  }).filter(s => s.videoUrl);
  window.SHORTS = SHORTS; renderAll();
}
function applyFirebasePremiumPhotos(data){
  const rows = normalizeCollection(data);
  if(!rows.length){ PREMIUM_PHOTOS = []; renderPremiumPhotos(); return; }
  PREMIUM_PHOTOS = rows.filter(r => r.value && r.value.active !== false).map((r, i) => {
    const v = r.value || {};
    return { id: String(v.id || r.id), image: normalizeUrl(firstValue(v, ['image','img','photo','photoUrl','src','url','thumbnail','thumb'], '')), link: normalizeUrl(firstValue(v, ['link','href','openUrl','openLink','clickUrl','target','url2'], '')), title: String(firstValue(v, ['title','t','name'], '')), badge: String(firstValue(v, ['badge','tag','label'], '')), order: Number(firstValue(v, ['order','sort','index'], i)) || i, active: v.active !== false };
  }).filter(p => p.image);
  PREMIUM_PHOTOS.sort((a, b) => (a.order || 0) - (b.order || 0));
  window.PREMIUM_PHOTOS = PREMIUM_PHOTOS; renderPremiumPhotos();
}
function applyFirebaseAds(data){
  const rows = normalizeCollection(data);
  if(!rows.length){ ADS = []; return; }
  ADS = rows.map((r, i) => {
    const v = r.value || {};
    return {
      id: String(v.id || r.id || ('ad'+i)),
      image: normalizeUrl(firstValue(v, ['image','img','photo','photoUrl','src','url','banner'], '')),
      link: normalizeUrl(firstValue(v, ['link','href','openUrl','openLink','clickUrl','target'], '')),
      title: String(firstValue(v, ['title','t','name'], '')),
      active: v.active !== false
    };
  }).filter(a => a.image);
  try{ if(currentPlaylist) renderPlaylistAd(); }catch(e){}
}
function applyFirebaseGames(data){ window.LEARNIFY_GAMES_DATA = data || {}; }
function applyAppSettings(settings){
  if(!settings) return;
  try{
    const bg = firstValue(settings, ['backgroundColor','background','bg','appBackground'], '');
    const img = firstValue(settings, ['backgroundImage','backgroundPhoto','backgroundUrl','bgImage','imageUrl','photoUrl'], '');
    const mode = String(firstValue(settings, ['backgroundMode','bgMode'], img ? 'image' : 'color') || '').toLowerCase();
    const app = $('#app');
    const validColor = /^(#[0-9a-f]{3,8}|rgb\(|rgba\(|hsl\(|hsla\()/i.test(String(bg));
    if(validColor){ document.documentElement.style.setProperty('--bg', String(bg)); if(app) app.style.backgroundColor = String(bg); document.body.style.backgroundColor = String(bg); }
    if(app && img && mode !== 'color'){ const safeImg = String(img).replace(/"/g,'&quot;'); app.style.setProperty('background-image', `url("${safeImg}")`, ''); app.style.setProperty('background-size','cover',''); app.style.setProperty('background-position','center center',''); app.style.setProperty('background-repeat','no-repeat',''); }
    if(settings.theme && typeof settings.theme === 'object'){ applyTheme(settings.theme); }

    const rawFlashImg = settings.flashImageUrl;
    const rawFlashVid = settings.flashVideoUrl;
    const flashType = String(settings.flashType || '').toLowerCase();
    const flashImgUrl = (rawFlashImg != null) ? String(rawFlashImg).trim() : '';
    const flashVidUrl = (rawFlashVid != null) ? String(rawFlashVid).trim() : '';

    let splashMedia = null;
    if(flashType === 'video' && flashVidUrl) splashMedia = { type:'video', url: flashVidUrl };
    else if(flashType === 'image' && flashImgUrl) splashMedia = { type:'image', url: flashImgUrl };
    else if(flashVidUrl) splashMedia = { type:'video', url: flashVidUrl };
    else if(flashImgUrl) splashMedia = { type:'image', url: flashImgUrl };

    if(splashMedia){
      cacheSplash(splashMedia);
      showSplashScreen(splashMedia);
    } else {
      cacheSplash(null);
    }

    setTimeout(updateBgPreview, 100);
  }catch(e){ console.error('Settings apply failed:',e); }
}
let firebaseListenersAttached = false;
function listenFirebaseData(){
  if(!db || firebaseListenersAttached) return;
  firebaseListenersAttached = true;
  db.ref('learnify/videos').on('value', s => applyFirebaseVideos(s.val()), err => console.error(err));
  db.ref('learnify/playlists').on('value', s => applyFirebasePlaylists(s.val()), err => console.error(err));
  db.ref('learnify/apps').on('value', s => applyFirebaseApps(s.val()), err => console.error(err));
  db.ref('learnify/slider').on('value', s => applyFirebaseSlider(s.val()), err => console.error(err));
  db.ref('learnify/shorts').on('value', s => applyFirebaseShorts(s.val()), err => console.error(err));
  db.ref('learnify/premiumPhotos').on('value', s => applyFirebasePremiumPhotos(s.val()), err => console.error(err));
  db.ref('learnify/ads').on('value', s => applyFirebaseAds(s.val()), err => console.error(err));
  db.ref('learnify/games').on('value', s => applyFirebaseGames(s.val()), err => console.error(err));

  db.ref('learnify/shortAds').on('value', s => {
    const data = s.val() || {};
    SHORT_ADS = Object.values(data)
      .filter(a => a && a.active !== false && a.videoUrl)
      .map(a => ({
        id: String(a.id || ''),
        title: a.title || 'Sponsored',
        videoUrl: a.videoUrl || '',
        clickLink: a.clickLink || '',
        active: a.active !== false
      }));
    window.SHORT_ADS = SHORT_ADS;
  }, err => console.warn('shortAds listener err', err));

  db.ref('learnify/scheduledPlaylistVideos').on('value', s => {
    const data = s.val() || {};
    SCHEDULED_VIDEOS = Object.values(data)
      .filter(v => v && v.videoUrl)
      .map(v => ({
        id: String(v.id || ''),
        title: v.title || 'Advertisement',
        videoUrl: v.videoUrl || '',
        thumbnail: v.thumbnail || ''
      }));
    window.SCHEDULED_VIDEOS = SCHEDULED_VIDEOS;
  }, err => console.warn('scheduledPlaylistVideos listener err', err));

  db.ref('learnify/appSettings').on('value', s => applyAppSettings(s.val()), err => console.error(err));

  db.ref('learnify/appOverrides').on('value', s => {
    APP_OVERRIDES = s.val() || {};
    if(currentApp) openApp(currentApp.id); 
  }, err => console.warn('appOverrides listener err', err));

  db.ref('learnify/appTheme').on('value', s => {
    const theme = s.val() || 'light';
    applyAppTheme(theme);
  }, err => console.warn('appTheme listener err', err));

  db.ref('learnify/brand').on('value', s => {
    const v = s.val();
    GLOBAL_HOME_BRAND = v || null;
    try{
      if(v) localStorage.setItem('learnifyBrand', JSON.stringify(v));
      else localStorage.removeItem('learnifyBrand');
    }catch(e){}
    if(window.__applyBrand){ try{ window.__applyBrand(); }catch(e){} }
  }, err => console.warn('brand listener err', err));

  db.ref('learnify/channelBrands').on('value', s => {
    const v = s.val() || {};
    GLOBAL_CHANNEL_BRANDS = v;
    try{ localStorage.setItem('learnifyChannelBrand', JSON.stringify(v)); }catch(e){}
    refreshAllChannelBrands();
  }, err => console.warn('channelBrands listener err', err));

  db.ref('learnify/subsBrand').on('value', s => {
    const v = s.val();
    GLOBAL_SUBS_BRAND = v || null;
    try{
      if(v) localStorage.setItem('learnifySubsBrand', JSON.stringify(v));
      else localStorage.removeItem('learnifySubsBrand');
    }catch(e){}
    try{ if(window.__applySubsBrand) window.__applySubsBrand(); }catch(e){}
  }, err => console.warn('subsBrand listener err', err));

  db.ref('learnify/subsBg').on('value', s => {
    const v = s.val();
    GLOBAL_SUBS_BG = v || null;
    try{
      if(v) localStorage.setItem('learnifySubsBg', JSON.stringify(v));
      else localStorage.removeItem('learnifySubsBg');
    }catch(e){}
    try{ if(window.__applySubsBg) window.__applySubsBg(); }catch(e){}
  }, err => console.warn('subsBg listener err', err));

  db.ref('learnify/playlistBg').on('value', s => {
    const v = s.val();
    GLOBAL_PLAYLIST_BG = v || null;
    try{
      if(v) localStorage.setItem('learnifyPlaylistBg', JSON.stringify(v));
      else localStorage.removeItem('learnifyPlaylistBg');
    }catch(e){}
    try{ if(window.__applyPlaylistBg) window.__applyPlaylistBg(); }catch(e){}
  }, err => console.warn('playlistBg listener err', err));

  db.ref('learnify/searchTitle').on('value', s => {
    const v = s.val();
    GLOBAL_SEARCH_TITLE = v || 'Search';
    try{
      if(v) localStorage.setItem('learnifySearchTitle', v);
      else localStorage.removeItem('learnifySearchTitle');
    }catch(e){}
    try{ if(window.__applySearchTitle) window.__applySearchTitle(); }catch(e){}
  }, err => console.warn('searchTitle listener err', err));

  db.ref('learnify/premiumTitles').on('value', s => {
    const v = s.val() || {};
    GLOBAL_PREMIUM_TITLE = v.title || 'Premium';
    GLOBAL_PREMIUM_SUBTITLE = v.subtitle || 'Courses & masterclasses';
    try{
      if(v.title) localStorage.setItem('learnifyPremiumTitle', v.title);
      else localStorage.removeItem('learnifyPremiumTitle');
      if(v.subtitle) localStorage.setItem('learnifyPremiumSubtitle', v.subtitle);
      else localStorage.removeItem('learnifyPremiumSubtitle');
    }catch(e){}
    try{ if(window.__applyPremiumTitle) window.__applyPremiumTitle(); }catch(e){}
  }, err => console.warn('premiumTitles listener err', err));

  db.ref('learnify/adUrls').on('value', s => {
    const v = s.val() || {};
    GLOBAL_AD_URLS = v;
    try{ localStorage.setItem('learnifyAdUrls', JSON.stringify(v)); }catch(e){}
    try{ if(window.__refreshAllAds) window.__refreshAllAds(); }catch(e){}
  }, err => console.warn('adUrls listener err', err));

  db.ref('learnify/headerBanners').on('value', s => {
    const v = s.val() || [];
    const banners = Array.isArray(v) ? v : Object.values(v);
    GLOBAL_HEADER_BANNERS = banners.filter(Boolean);
    try{ localStorage.setItem('learnifyHeaderBanners', JSON.stringify(GLOBAL_HEADER_BANNERS)); }catch(e){}
    renderHeaderBanners();
  }, err => console.warn('headerBanners listener err', err));

  db.ref('learnify/loginConfig').on('value', s => {
    const v = s.val() || {};
    if(v.videoUrl !== undefined) {
      localStorage.setItem('learnifyLoginVideo', v.videoUrl);
      const loginScreen = document.getElementById('s-mobile-login');
      if(loginScreen && loginScreen.classList.contains('active')) {
        loadLoginVideo();
      }
    }
    if(v.goText !== undefined) {
      localStorage.setItem('learnifyGoText', v.goText);
      const goBtn = document.getElementById('goBtn');
      if(goBtn) goBtn.textContent = v.goText || 'GO';
    }
  }, err => console.warn('loginConfig listener err', err));
}
function loadFirebaseUserProfile(){ if(!db || !firebaseReady || !firebaseUser || !firebaseUser.uid) return; db.ref('learnify/users/' + firebaseUser.uid).once('value').then(s => { const profile = s.val(); if(!profile || !profile.email) return; const localProfile = { uid: firebaseUser.uid, email: profile.email, name: profile.name || displayNameFromEmail(profile.email), photoURL: profile.photoURL || firebaseUser.photoURL || '', signedIn: true, provider: profile.provider || 'password', updatedAt: Date.now() }; saveLocalUser(localProfile); applyLocalProfile(localProfile); }).catch(() => {}); }
function loadStoredProfile(){ try { const raw = localStorage.getItem('learnifyUser'); if(raw) applyLocalProfile(JSON.parse(raw)); } catch(e){} }
function applyLocalProfile(profile){
  if(!profile) return;
  const name = profile.name || 'Guest User';
  $$('.brand-hello').forEach(el => el.textContent = 'Welcome, ' + name);
  const pn = $('#profileName'); if(pn) pn.textContent = name;
  const pd = $('#profileEmail'); if(pd) pd.textContent = profile.email || 'Guest Mode';
  const pa = $('#profileAvatar');
  if(pa){
    if(profile.photoURL){ pa.innerHTML = `<img src="${esc(profile.photoURL)}" alt="" onerror="this.remove()"><div class="edit-dot"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4Z"/></svg></div>`; }
    else { pa.innerHTML = `${esc((name[0]||'L').toUpperCase())}<div class="edit-dot"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4Z"/></svg></div>`; }
  }
}

// NEW LOGIN LOGIC
function attemptMobileLogin() {
  const nameInp = document.getElementById('userNameInput');
  const inp = document.getElementById('mobileNumberInput');
  const nameVal = nameInp ? nameInp.value.trim() : '';
  const val = inp ? inp.value.trim() : '';
  
  if (!nameVal) {
    showToast('Please enter your name', 'error');
    if(nameInp) {
      nameInp.style.borderColor = '#E5484D';
      setTimeout(() => { nameInp.style.borderColor = '#333'; }, 1000);
    }
    return;
  }

  // Offline Validation for 10 digit Indian Mobile
  const isValid = /^[6-9]\d{9}$/.test(val);
  
  if (!isValid) {
    showToast('Please enter a valid 10-digit mobile number', 'error');
    if(inp) {
      inp.style.borderColor = '#E5484D';
      setTimeout(() => { inp.style.borderColor = '#333'; }, 1000);
    }
    return;
  }
  
  // Save to local storage
  localStorage.setItem('learnifyMobileUser', val);
  
  // Update User State
  saveLocalUser({ name: nameVal, email: val + '@mobile.com', uid: 'user_' + val, signedIn: true });
  
  // Go to Home
  show('home');
  applyLocalProfile(currentUser());
  showToast('Logged in successfully!', 'success');
  
  // Trigger Language Selection if not set
  if(!localStorage.getItem('learnifyLanguage')){
      setTimeout(showLanguageSheet, 800);
  }
}

// 5-Tap Video Secret
let loginVideoTapCount = 0;
let loginVideoTapTimer = null;

function attachLoginVideoTap() {
  const container = document.getElementById('loginVideoContainer');
  if(!container) return;
  
  container.addEventListener('click', (e) => {
    e.preventDefault();
    
    // --- FIX: Video ko play karne ke liye ---
    const media = container.querySelector('video, iframe');
    if (media) {
      if (media.tagName === 'VIDEO') {
        if (media.paused) {
          media.play().catch(()=>{});
        }
      } else if (media.tagName === 'IFRAME') {
        try {
          media.contentWindow.postMessage(JSON.stringify({event:'command', func:'playVideo', args:[]}), '*');
        } catch(err){}
      }
    }
    // ----------------------------------------

    loginVideoTapCount++;
    clearTimeout(loginVideoTapTimer);
    
    if(loginVideoTapCount >= 5) {
      loginVideoTapCount = 0;
      promptPassword(() => {
        const url = prompt("Enter Login Video URL (YouTube, MP4, etc.):", localStorage.getItem('learnifyLoginVideo') || '');
        if(url !== null) {
          localStorage.setItem('learnifyLoginVideo', url.trim());
          loadLoginVideo();
          if(db) {
            db.ref('learnify/loginConfig/videoUrl').set(url.trim())
              .then(() => showToast('Video updated permanently for everyone!', 'success'))
              .catch(() => showToast('Failed to update globally. Check DB rules.', 'error'));
          } else {
            showToast('Saved locally. Firebase not ready.', 'info');
          }
        }
      }, 'Video Access', 'Enter password to change login video.');
    } else {
      loginVideoTapTimer = setTimeout(() => { loginVideoTapCount = 0; }, 600);
    }
  });
}

function loadLoginVideo() {
  const container = document.getElementById('loginVideoContainer');
  if(!container) return;
  const url = localStorage.getItem('learnifyLoginVideo') || 'https://www.w3schools.com/html/mov_bbb.mp4'; // Default video
  
  container.innerHTML = '';
  if(url) {
    const media = createPlayerMedia(url, { autoplay:true, muted:true, controls:false, loop:true, objectFit:'cover' });
    if(media) {
      media.style.pointerEvents = 'none';
      container.appendChild(media);
    }
  }
}

// 5-Tap GO Secret
let goBtnTapCount = 0;
let goBtnTapTimer = null;

function attachGoBtnTap() {
  const btn = document.getElementById('goBtn');
  if(!btn) return;
  
  btn.addEventListener('click', (e) => {
    // If user typed valid number, we proceed with login
    const inp = document.getElementById('mobileNumberInput');
    const val = inp ? inp.value.trim() : '';
    
    if (/^[6-9]\d{9}$/.test(val)) {
      return; // Let normal login happen
    }

    // Secret 5-tap logic if number is not valid
    e.preventDefault();
    goBtnTapCount++;
    clearTimeout(goBtnTapTimer);
    
    if(goBtnTapCount >= 5) {
      goBtnTapCount = 0;
      promptPassword(() => {
        const text = prompt("Enter new GO button text:", localStorage.getItem('learnifyGoText') || 'GO');
        if(text !== null && text.trim()) {
          localStorage.setItem('learnifyGoText', text.trim());
          btn.textContent = text.trim();
          if(db) {
            db.ref('learnify/loginConfig/goText').set(text.trim())
              .then(() => showToast('Button text updated permanently for everyone!', 'success'))
              .catch(() => showToast('Failed to update globally. Check DB rules.', 'error'));
          } else {
            showToast('Saved locally. Firebase not ready.', 'info');
          }
        }
      }, 'Button Access', 'Enter password to change button text.');
    } else {
      goBtnTapTimer = setTimeout(() => { goBtnTapCount = 0; }, 600);
    }
  });
}

// Language Sheet Logic
function showLanguageSheet() {
    const list = document.getElementById('langList');
    const currentLang = localStorage.getItem('learnifyLanguage') || '';
    const langs = [
        { name: 'English', val: 'English' },
        { name: 'हिंदी (Hindi)', val: 'हिंदी (Hindi)' },
        { name: 'বাংলা (Bengali)', val: 'বাংলা (Bengali)' },
        { name: 'தமிழ் (Tamil)', val: 'தமிழ் (Tamil)' },
        { name: 'తెలుగు (Telugu)', val: 'తెలుగు (Telugu)' },
        { name: 'मराठी (Marathi)', val: 'मराठी (Marathi)' }
    ];
    list.innerHTML = langs.map(l => `<div class="lang-option ${currentLang === l.val ? 'active' : ''}" onclick="selectLanguage('${l.val}')">${l.name}</div>`).join('');
    document.getElementById('langSheet').classList.add('on');
}
function closeLanguageSheet() {
    document.getElementById('langSheet').classList.remove('on');
}
function selectLanguage(lang) {
    localStorage.setItem('learnifyLanguage', lang);
    const btn = document.getElementById('usrLangBtn');
    if(btn) btn.innerHTML = lang + ' <span>›</span>';
    closeLanguageSheet();
    showToast(lang + ' selected', 'success');
}

// User Settings Logic
function openUserSettings() {
    const u = currentUser();
    document.getElementById('usrName').value = u.name || '';
    document.getElementById('usrPhone').value = u.email ? u.email.replace('@mobile.com','') : '';
    const lang = localStorage.getItem('learnifyLanguage') || 'Select Language';
    document.getElementById('usrLangBtn').innerHTML = lang + ' <span>›</span>';
    
    const toggle = document.getElementById('usrThemeToggle');
    if(localStorage.getItem('learnifyTheme') === 'dark') toggle.classList.add('on');
    else toggle.classList.remove('on');
    
    go('user-settings');
}

function toggleTheme() {
    const toggle = document.getElementById('usrThemeToggle');
    toggle.classList.toggle('on');
}

function saveUserSettings() {
    const name = document.getElementById('usrName').value.trim();
    const phone = document.getElementById('usrPhone').value.trim();
    const isDark = document.getElementById('usrThemeToggle').classList.contains('on');
    
    if(!name) { showToast('Name cannot be empty', 'error'); return; }
    if(phone && !/^[6-9]\d{9}$/.test(phone)) { showToast('Enter valid 10-digit mobile number', 'error'); return; }

    const u = currentUser();
    u.name = name;
    if(phone) {
        u.email = phone + '@mobile.com';
        u.uid = 'user_' + phone;
        localStorage.setItem('learnifyMobileUser', phone);
    }
    saveLocalUser(u);
    applyLocalProfile(u);

    applyAppTheme(isDark ? 'dark' : 'light');
    localStorage.setItem('learnifyTheme', isDark ? 'dark' : 'light');

    showToast('Settings saved!', 'success');
    back();
}


function init(){
  // Check login state
  const hasLogin = localStorage.getItem('learnifyMobileUser');
  
  // Apply saved theme
  const savedTheme = localStorage.getItem('learnifyTheme');
  if(savedTheme) applyAppTheme(savedTheme);

  // Apply saved GO text
  const savedGoText = localStorage.getItem('learnifyGoText');
  if(savedGoText) {
    const goBtn = document.getElementById('goBtn');
    if(goBtn) goBtn.textContent = savedGoText;
  }

  if(hasLogin){
    show('home');
    if(!localStorage.getItem('learnifyLanguage')){
        setTimeout(showLanguageSheet, 1000);
    }
  } else {
    show('mobile-login');
    loadLoginVideo();
    attachLoginVideoTap();
    attachGoBtnTap();
  }

  try{
    const cachedSplash = getCachedSplash();
    if(cachedSplash) showSplashScreen(cachedSplash);
  }catch(e){}

  const work = () => {
    try{ invalidateIndex(); INDEX = buildIndex(); }catch(e){}
    try{ renderHero(); }catch(e){}
    try{ renderHome(); }catch(e){}
    try{ renderHeaderBanners(); }catch(e){}
    try{ renderChat(); renderChatHistory(); }catch(e){}
    try{ loadStoredProfile(); }catch(e){}
    try{ loadStoredBackground(); }catch(e){}
    try{ if(window.__applyBrand) window.__applyBrand(); }catch(e){}
    try{ if(window.__applySubsBrand) window.__applySubsBrand(); }catch(e){}
    try{ if(window.__applySubsBg) window.__applySubsBg(); }catch(e){}
    try{ if(window.__applyPlaylistBg) window.__applyPlaylistBg(); }catch(e){}
    try{ applyAppTheme(GLOBAL_THEME); }catch(e){}
    try{ if(window.__applySearchTitle) window.__applySearchTitle(); }catch(e){}
    try{ if(window.__applyPremiumTitle) window.__applyPremiumTitle(); }catch(e){}
    try{ if(window.__refreshAllAds) window.__refreshAllAds(); }catch(e){}
  };
  if('requestIdleCallback' in window){ requestIdleCallback(work, {timeout: 300}); }
  else { setTimeout(work, 16); }
  setTimeout(() => { try{ listenFirebaseData(); }catch(e){} }, 2000);
}
loadAdminLocalFallback();
init();

(function setupBrandCustomization(){
  const BRAND_PWD = '7080354035';
  const HOME_KEY = 'learnifyBrand';
  const CHANNEL_KEY = 'learnifyChannelBrand';

  function loadHomeBrand(){
    if(GLOBAL_HOME_BRAND) return GLOBAL_HOME_BRAND;
    try{ const raw = localStorage.getItem(HOME_KEY); if(!raw) return null; const d = JSON.parse(raw); return (d && typeof d === 'object') ? d : null; }catch(e){ return null; }
  }
  function saveHomeBrand(data){
    const clean = (data && (data.name || data.icon || data.welcome)) ? { 
      name: String(data.name||'').trim(), 
      icon: String(data.icon||'').trim(),
      welcome: String(data.welcome||'').trim()
    } : null;
    GLOBAL_HOME_BRAND = clean;
    try{
      if(clean) localStorage.setItem(HOME_KEY, JSON.stringify(clean));
      else localStorage.removeItem(HOME_KEY);
    }catch(e){}
    pushHomeBrandToFirebase();
  }
  function applyHomeBrand(){
    const b = loadHomeBrand();
    const mark = document.getElementById('homeBrandMark');
    const nameEl = document.getElementById('homeBrandName');
    if(!mark || !nameEl) return;
    const hasName = b && b.name && String(b.name).trim();
    const iconUrl = b && b.icon ? safeUrl(b.icon) : '';
    const name = hasName ? String(b.name).trim() : 'LEARNIFY';
    const customWelcome = b && b.welcome ? String(b.welcome).trim() : '';
    
    nameEl.textContent = name;
    
    let welcomeText = customWelcome;
    if(!welcomeText){
      const profile = currentUser();
      if(profile && profile.name) welcomeText = 'Welcome, ' + profile.name;
      else welcomeText = 'Welcome to Learnify';
    }
    $$('.brand-hello').forEach(el => el.textContent = welcomeText);
    
    if(iconUrl){
      mark.innerHTML = `<img src="${esc(iconUrl)}" alt="${esc(name)}" style="width:100%;height:100%;object-fit:cover;border-radius:inherit;display:block;position:relative;z-index:2" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${esc((name.charAt(0)||'N').toUpperCase())}'">`;
    } else {
      mark.textContent = (name.charAt(0) || 'N').toUpperCase();
    }
  }
  function loadChannelMap(){
    try{ const raw = localStorage.getItem(CHANNEL_KEY); if(!raw) return {}; const d = JSON.parse(raw); return (d && typeof d === 'object') ? d : {}; }catch(e){ return {}; }
  }
  function saveChannelMap(map){ try{ localStorage.setItem(CHANNEL_KEY, JSON.stringify(map || {})); }catch(e){} }
  function getChannelBrand(base){
    if(!base) return null;
    const k = String(base).toLowerCase().trim();
    if(GLOBAL_CHANNEL_BRANDS && GLOBAL_CHANNEL_BRANDS[k]) return GLOBAL_CHANNEL_BRANDS[k];
    const map = loadChannelMap();
    return map[k] || null;
  }
  function setChannelBrand(base, data){
    if(!base) return;
    const k = String(base).toLowerCase().trim();
    const clean = (!data || (!data.name && !data.icon)) ? null
                 : { name: String(data.name||'').trim(), icon: String(data.icon||'').trim() };
    if(clean) GLOBAL_CHANNEL_BRANDS[k] = clean;
    else delete GLOBAL_CHANNEL_BRANDS[k];
    saveChannelMap(GLOBAL_CHANNEL_BRANDS);
    pushChannelBrandToFirebase(k, clean);
  }
  function applyChannelBrand(base){
    if(!base) return;
    const base_lc = String(base).toLowerCase().trim();
    const data = getChannelBrand(base);
    const displayName = (data && data.name) ? String(data.name).trim() : '';
    const iconUrl = (data && data.icon) ? safeUrl(data.icon) : '';

    const root = document.getElementById('channelBody');
    if(root){
      const avatar = root.querySelector('.channel-avatar');
      const nameEl = root.querySelector('.channel-name');
      if(avatar && nameEl){
        const nm = displayName || nameEl.textContent || '';
        if(displayName) nameEl.textContent = displayName;
        if(iconUrl){
          avatar.innerHTML = `<img src="${esc(iconUrl)}" alt="${esc(nm)}" onerror="this.onerror=null;this.remove();this.parentElement.textContent='${esc((nm.charAt(0)||'C').toUpperCase())}'">`;
        } else if(displayName){
          avatar.textContent = (displayName.charAt(0) || 'C').toUpperCase();
        }
      }
    }

    const reels = document.querySelectorAll('#shortPlayerBody .short-reel');
    reels.forEach(reel => {
      const sid = reel.dataset.shortId;
      if(!sid) return;
      const s = SHORTS.find(x => String(x.id) === String(sid));
      if(!s) return;
      if(getBaseTag(s.tag) !== base_lc) return;

      const av   = reel.querySelector('.short-reel-channel-avatar');
      const nmEl = reel.querySelector('.short-reel-channel > span');
      const catEl = reel.querySelector('.short-reel-cat');

      if(av){
        if(iconUrl){ av.innerHTML = `<img src="${esc(iconUrl)}" alt="" onerror="this.onerror=null;this.remove()">`; }
        else if(displayName){ av.textContent = (displayName.charAt(0) || 'S').toUpperCase(); }
      }
      if(nmEl && displayName) nmEl.textContent = displayName;
      if(catEl){
        const cur = catEl.textContent || '';
        const suffixMatch = cur.match(/(\s*·\s*\d+\/\d+)$/);
        const suffix = suffixMatch ? suffixMatch[1] : '';
        if(displayName) catEl.textContent = displayName + suffix;
      }
    });
  }

  function promptPassword(onSuccess, titleText, subtitle){
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:340px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="width:56px;height:56px;font-size:24px">🔐</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">${esc(titleText||'Brand Access')}</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">${esc(subtitle||'Enter password to continue.')}</p>
        </div>
        <div class="field">
          <label>Password</label>
          <input class="input" id="brandPwdInput" type="password" inputmode="numeric" placeholder="Enter password" autocomplete="off">
          <div class="err-msg" id="brandPwdErr" style="display:none"></div>
        </div>
        <div class="modal-actions">
          <button class="btn btn-secondary" id="brandPwdCancel">Cancel</button>
          <button class="btn btn-primary" id="brandPwdOk">Unlock</button>
        </div>
      </div>`;
    document.body.appendChild(overlay);

    const pwdInp = overlay.querySelector('#brandPwdInput');
    const errEl  = overlay.querySelector('#brandPwdErr');
    const close  = () => overlay.remove();

    const tryUnlock = () => {
      const v = (pwdInp.value || '').trim();
      if(v === BRAND_PWD){ close(); if(typeof onSuccess === 'function'){ try{ onSuccess(); }catch(e){} } }
      else {
        errEl.textContent = 'Wrong password. Try again.';
        errEl.style.display = 'flex';
        pwdInp.classList.add('error');
        pwdInp.value = '';
        pwdInp.focus();
      }
    };
    overlay.querySelector('#brandPwdCancel').addEventListener('click', close);
    overlay.querySelector('#brandPwdOk').addEventListener('click', tryUnlock);
    pwdInp.addEventListener('keydown', (e) => { if(e.key === 'Enter'){ e.preventDefault(); tryUnlock(); } });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => pwdInp.focus(), 120);
  }
  window.promptPassword = promptPassword;

  function openHomeEditor(){
    const b = loadHomeBrand() || {};
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">✏️</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Customize App Brand</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Change app name & icon (URL).</p>
        </div>
        <div class="field">
          <label>Welcome Text</label>
          <input class="input" id="brandWelcomeInp" type="text" placeholder="Welcome to Learnify" value="${esc(b.welcome||'')}" autocomplete="off">
        </div>
        <div class="field">
          <label>App Name</label>
          <input class="input" id="brandNameInp" type="text" placeholder="Learnify" value="${esc(b.name||'')}" autocomplete="off">
        </div>
        <div class="field">
          <label>Icon Image URL</label>
          <input class="input" id="brandIconInp" type="url" placeholder="https://... (empty = first letter)" value="${esc(b.icon||'')}" autocomplete="off">
        </div>
        <div style="margin-bottom:14px">
          <div class="bg-preview" id="brandPreview" style="height:70px;background-color:var(--surface-2)"></div>
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="brandReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="brandSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="brandClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);

    const welcomeInp = overlay.querySelector('#brandWelcomeInp');
    const nameInp = overlay.querySelector('#brandNameInp');
    const iconInp = overlay.querySelector('#brandIconInp');
    const prev    = overlay.querySelector('#brandPreview');

    const updatePreview = () => {
      const img = safeUrl(iconInp.value);
      const nm  = (nameInp.value || 'Learnify').trim() || 'Learnify';
      if(img){
        const safeImg = img.replace(/"/g,'&quot;');
        prev.style.backgroundImage = `url("${safeImg}")`;
        prev.style.backgroundSize = 'cover';
        prev.style.backgroundPosition = 'center';
        prev.innerHTML = `<span>${esc(nm)}</span>`;
      } else {
        prev.style.backgroundImage = 'none';
        prev.style.backgroundColor = '';
        const letter = (nm.charAt(0) || 'N').toUpperCase();
        prev.innerHTML = `<span>${esc(letter)} — ${esc(nm)}</span>`;
      }
    };
    nameInp.addEventListener('input', updatePreview);
    iconInp.addEventListener('input', updatePreview);
    updatePreview();

    const close = () => { overlay.remove(); applyHomeBrand(); };

    overlay.querySelector('#brandClose').addEventListener('click', close);
    overlay.querySelector('#brandSave').addEventListener('click', () => {
      const welcome = (welcomeInp.value || '').trim();
      const name = (nameInp.value || '').trim();
      const icon = (iconInp.value || '').trim();
      saveHomeBrand({ name, icon, welcome });
      close();
      showToast('App brand updated!', 'success');
    });
    overlay.querySelector('#brandReset').addEventListener('click', () => {
      saveHomeBrand(null);
      close();
      showToast('App brand reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => welcomeInp.focus(), 120);
  }

  function openChannelEditor(base){
    if(!base) return;
    const b = getChannelBrand(base) || {};
    const prettyName = String(base).replace(/\b\w/g, c => c.toUpperCase());
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">✏️</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Customize Channel</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Channel: <b style="color:var(--ink)">${esc(prettyName)}</b></p>
        </div>
        <div class="field">
          <label>Channel Name</label>
          <input class="input" id="chNameInp" type="text" placeholder="${esc(prettyName)}" value="${esc(b.name||'')}" autocomplete="off">
        </div>
        <div class="field">
          <label>Channel Icon URL</label>
          <input class="input" id="chIconInp" type="url" placeholder="https://... (empty = first letter)" value="${esc(b.icon||'')}" autocomplete="off">
        </div>
        <div style="margin-bottom:14px">
          <div class="bg-preview" id="chPreview" style="height:70px;background-color:var(--surface-2);border-radius:50%"></div>
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="chReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="chSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="chClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);

    const nameInp = overlay.querySelector('#chNameInp');
    const iconInp = overlay.querySelector('#chIconInp');
    const prev    = overlay.querySelector('#chPreview');

    const updatePreview = () => {
      const img = safeUrl(iconInp.value);
      const nm  = (nameInp.value || prettyName).trim() || prettyName;
      if(img){
        const safeImg = img.replace(/"/g,'&quot;');
        prev.style.backgroundImage = `url("${safeImg}")`;
        prev.style.backgroundSize = 'cover';
        prev.style.backgroundPosition = 'center';
        prev.innerHTML = '';
      } else {
        prev.style.backgroundImage = 'none';
        prev.style.backgroundColor = '';
        const letter = (nm.charAt(0) || 'C').toUpperCase();
        prev.innerHTML = `<span>${esc(letter)} — ${esc(nm)}</span>`;
      }
    };
    nameInp.addEventListener('input', updatePreview);
    iconInp.addEventListener('input', updatePreview);
    updatePreview();

    const close = () => { overlay.remove(); applyChannelBrand(base); };

    overlay.querySelector('#chClose').addEventListener('click', close);
    overlay.querySelector('#chSave').addEventListener('click', () => {
      const name = (nameInp.value || '').trim();
      const icon = (iconInp.value || '').trim();
      setChannelBrand(base, { name, icon });
      close();
      showToast('Channel updated!', 'success');
    });
    overlay.querySelector('#chReset').addEventListener('click', () => {
      setChannelBrand(base, null);
      close();
      showToast('Channel reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => nameInp.focus(), 120);
  }
  window.openChannelEditor = openChannelEditor;

  const SUBS_KEY = 'learnifySubsBrand';
  function loadSubsBrand(){
    if(GLOBAL_SUBS_BRAND) return GLOBAL_SUBS_BRAND;
    try{ const raw = localStorage.getItem(SUBS_KEY); if(!raw) return null; const d = JSON.parse(raw); return (d && typeof d === 'object') ? d : null; }catch(e){ return null; }
  }
  function saveSubsBrand(data){
    const clean = (data && (data.name || data.icon)) ? { name: String(data.name||'').trim(), icon: String(data.icon||'').trim() } : null;
    GLOBAL_SUBS_BRAND = clean;
    try{
      if(clean) localStorage.setItem(SUBS_KEY, JSON.stringify(clean));
      else localStorage.removeItem(SUBS_KEY);
    }catch(e){}
    if(!db) return;
    try{
      if(clean) db.ref('learnify/subsBrand').set(clean);
      else db.ref('learnify/subsBrand').remove();
    }catch(e){ console.warn('subs brand push failed:', e); }
  }
  function applySubsBrand(){
    const b = loadSubsBrand();
    const iconWrap = document.querySelector('#s-subscriptions .subs-icon');
    const titleEl = document.querySelector('#s-subscriptions .subs-hero h1');
    if(!iconWrap) return;
    const iconUrl = b && b.icon ? safeUrl(b.icon) : '';
    const name = b && b.name ? String(b.name).trim() : 'Subscriptions';
    if(iconUrl){
      iconWrap.innerHTML = `<img src="${esc(iconUrl)}" alt="${esc(name)}" style="width:100%;height:100%;object-fit:cover;border-radius:inherit;display:block;position:relative;z-index:2" onerror="this.onerror=null;this.remove()">`;
    }
    if(titleEl) titleEl.textContent = name;
  }
  function openSubsEditor(){
    const b = loadSubsBrand() || {};
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">✏️</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Customize Subscriptions</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Change subscription icon & title (URL).</p>
        </div>
        <div class="field">
          <label>Title</label>
          <input class="input" id="subsNameInp" type="text" placeholder="Subscriptions" value="${esc(b.name||'')}" autocomplete="off">
        </div>
        <div class="field">
          <label>Icon Image URL</label>
          <input class="input" id="subsIconInp" type="url" placeholder="https://... (empty = default icon)" value="${esc(b.icon||'')}" autocomplete="off">
        </div>
        <div style="margin-bottom:14px">
          <div class="bg-preview" id="subsPreview" style="height:70px;background-color:var(--surface-2);border-radius:22px"></div>
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="subsReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="subsSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="subsClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const nameInp = overlay.querySelector('#subsNameInp');
    const iconInp = overlay.querySelector('#subsIconInp');
    const prev = overlay.querySelector('#subsPreview');
    const updatePreview = () => {
      const img = safeUrl(iconInp.value);
      const nm = (nameInp.value || 'Subscriptions').trim() || 'Subscriptions';
      if(img){
        const safeImg = img.replace(/"/g,'&quot;');
        prev.style.backgroundImage = `url("${safeImg}")`;
        prev.style.backgroundSize = 'cover';
        prev.style.backgroundPosition = 'center';
        prev.innerHTML = `<span style="position:relative;z-index:2">${esc(nm)}</span>`;
      } else {
        prev.style.backgroundImage = 'none';
        prev.innerHTML = `<span>${esc(nm)}</span>`;
      }
    };
    nameInp.addEventListener('input', updatePreview);
    iconInp.addEventListener('input', updatePreview);
    updatePreview();
    const close = () => { overlay.remove(); applySubsBrand(); };
    overlay.querySelector('#subsClose').addEventListener('click', close);
    overlay.querySelector('#subsSave').addEventListener('click', () => {
      saveSubsBrand({ name: nameInp.value, icon: iconInp.value });
      close();
      showToast('Subscriptions updated!', 'success');
    });
    overlay.querySelector('#subsReset').addEventListener('click', () => {
      saveSubsBrand(null);
      close();
      showToast('Subscriptions reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => nameInp.focus(), 120);
  }

  let subsTapCount = 0, subsTapTimer = null;
  function attachSubsTripleTap(){
    const icon = document.querySelector('#s-subscriptions .subs-icon');
    if(!icon || icon.dataset.tripleReady === '1') return;
    icon.dataset.tripleReady = '1';
    icon.style.cursor = 'pointer';
    icon.style.userSelect = 'none';
    icon.addEventListener('click', (e) => {
      e.preventDefault();
      e.stopPropagation();
      subsTapCount++;
      clearTimeout(subsTapTimer);
      if(subsTapCount >= 3){
        subsTapCount = 0;
        promptPassword(openSubsEditor, 'Subscriptions Access', 'Enter password to change subscription icon & title.');
      } else {
        subsTapTimer = setTimeout(() => { subsTapCount = 0; }, 400);
      }
    }, { passive: false });
  }

  const SUBS_BG_KEY = 'learnifySubsBg';
  function loadSubsBg(){
    if(GLOBAL_SUBS_BG) return GLOBAL_SUBS_BG;
    try{ const raw = localStorage.getItem(SUBS_BG_KEY); if(!raw) return null; return JSON.parse(raw); }catch(e){ return null; }
  }
  function saveSubsBg(url){
    const clean = url ? String(url).trim() : null;
    GLOBAL_SUBS_BG = clean;
    try{
      if(clean) localStorage.setItem(SUBS_BG_KEY, JSON.stringify(clean));
      else localStorage.removeItem(SUBS_BG_KEY);
    }catch(e){}
    if(!db) return;
    try{
      if(clean) db.ref('learnify/subsBg').set(clean);
      else db.ref('learnify/subsBg').remove();
    }catch(e){ console.warn('subs bg push failed:', e); }
  }
  function applySubsBg(){
    const url = loadSubsBg();
    const hero = document.getElementById('subsHero');
    if(!hero) return;
    if(url && safeUrl(url)){
      hero.style.backgroundImage = `url("${safeUrl(url)}")`;
      hero.style.backgroundSize = 'cover';
      hero.style.backgroundPosition = 'center';
    } else {
      hero.style.backgroundImage = 'linear-gradient(170deg,var(--brand-soft) 0%,transparent 100%)';
    }
  }
  function openSubsBgEditor(){
    const current = loadSubsBg() || '';
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">🖼️</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Subscriptions Background</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Paste an image URL to change the header background.</p>
        </div>
        <div class="field">
          <label>Background Image URL</label>
          <input class="input" id="subsBgInp" type="url" placeholder="https://..." value="${esc(current)}" autocomplete="off">
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="subsBgReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="subsBgSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="subsBgClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const inp = overlay.querySelector('#subsBgInp');
    const close = () => { overlay.remove(); applySubsBg(); };
    overlay.querySelector('#subsBgClose').addEventListener('click', close);
    overlay.querySelector('#subsBgSave').addEventListener('click', () => {
      saveSubsBg(inp.value);
      close();
      showToast('Subscriptions background updated!', 'success');
    });
    overlay.querySelector('#subsBgReset').addEventListener('click', () => {
      saveSubsBg(null);
      close();
      showToast('Subscriptions background reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => inp.focus(), 120);
  }

  let subsBgTapCount = 0, subsBgTapTimer = null;
  function attachSubsBgTripleTap(){
    const hero = document.getElementById('subsHero');
    if(!hero || hero.dataset.tripleReady === '1') return;
    hero.dataset.tripleReady = '1';
    hero.style.cursor = 'pointer';
    hero.addEventListener('click', (e) => {
      if(e.target.closest('.subs-icon')) return;
      subsBgTapCount++;
      clearTimeout(subsBgTapTimer);
      if(subsBgTapCount >= 3){
        subsBgTapCount = 0;
        promptPassword(openSubsBgEditor, 'Background Access', 'Enter password to change the subscriptions background.');
      } else {
        subsBgTapTimer = setTimeout(() => { subsBgTapCount = 0; }, 400);
      }
    }, { passive: false });
  }

  const PLAYLIST_BG_KEY = 'learnifyPlaylistBg';
  function loadPlaylistBg(){
    if(GLOBAL_PLAYLIST_BG) return GLOBAL_PLAYLIST_BG;
    try{ const raw = localStorage.getItem(PLAYLIST_BG_KEY); if(!raw) return null; return JSON.parse(raw); }catch(e){ return null; }
  }
  function savePlaylistBg(color){
    const clean = color ? String(color).trim() : null;
    GLOBAL_PLAYLIST_BG = clean;
    try{
      if(clean) localStorage.setItem(PLAYLIST_BG_KEY, JSON.stringify(clean));
      else localStorage.removeItem(PLAYLIST_BG_KEY);
    }catch(e){}
    if(!db) return;
    try{
      if(clean) db.ref('learnify/playlistBg').set(clean);
      else db.ref('learnify/playlistBg').remove();
    }catch(e){ console.warn('playlist bg push failed:', e); }
  }
  function applyPlaylistBg(){
    const color = loadPlaylistBg();
    const app = document.getElementById('app');
    if(!app) return;
    if(color){
      app.style.setProperty('--pd-actions-bg', color);
    } else {
      app.style.removeProperty('--pd-actions-bg');
    }
  }
  function openPlaylistBgEditor(){
    const current = loadPlaylistBg() || '';
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">🎨</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Playlist Strip Color</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Change the background color of the actions bar.</p>
        </div>
        <div class="field">
          <label>Color (Hex / Name)</label>
          <input class="input" id="playlistBgInp" type="text" placeholder="#FFFFFF or transparent" value="${esc(current)}" autocomplete="off">
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="playlistBgReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="playlistBgSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="playlistBgClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const inp = overlay.querySelector('#playlistBgInp');
    const close = () => { overlay.remove(); applyPlaylistBg(); };
    overlay.querySelector('#playlistBgClose').addEventListener('click', close);
    overlay.querySelector('#playlistBgSave').addEventListener('click', () => {
      savePlaylistBg(inp.value);
      close();
      showToast('Playlist color updated!', 'success');
    });
    overlay.querySelector('#playlistBgReset').addEventListener('click', () => {
      savePlaylistBg(null);
      close();
      showToast('Playlist color reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => inp.focus(), 120);
  }

  let playlistBgTapCount = 0, playlistBgTapTimer = null;
  function attachPlaylistBgTripleTap(){
    const bar = document.getElementById('pdActionsBar');
    if(!bar || bar.dataset.tripleReady === '1') return;
    bar.dataset.tripleReady = '1';
    bar.addEventListener('click', (e) => {
      if(e.target.closest('.pd-action-btn')) return;
      playlistBgTapCount++;
      clearTimeout(playlistBgTapTimer);
      if(playlistBgTapCount >= 3){
        playlistBgTapCount = 0;
        promptPassword(openPlaylistBgEditor, 'Color Access', 'Enter password to change the playlist background color.');
      } else {
        playlistBgTapTimer = setTimeout(() => { playlistBgTapCount = 0; }, 400);
      }
    }, { passive: false });
  }

  let chipTapCount = {}, chipTapTimer = {};
  function attachSubsChipTripleTap(){
    if(window.__subsChipTripleReady) return;
    window.__subsChipTripleReady = true;
    document.addEventListener('click', (e) => {
      const chip = e.target.closest('#subsBody .chip');
      if(!chip) return;
      const base = chip.dataset.base;
      if(!base) return;
      
      e.preventDefault();
      e.stopPropagation();
      
      chipTapCount[base] = (chipTapCount[base] || 0) + 1;
      clearTimeout(chipTapTimer[base]);
      
      if(chipTapCount[base] >= 3){
        chipTapCount[base] = 0;
        promptPassword(
          () => openChannelEditor(base),
          'Channel Access',
          'Enter password to change channel name & icon.'
        );
      } else {
        chipTapTimer[base] = setTimeout(() => { 
          if(chipTapCount[base] === 1) {
            selectSubsChannel(base);
          }
          chipTapCount[base] = 0; 
        }, 400);
      }
    }, true); 
  }

  function saveSearchTitle(title){
    GLOBAL_SEARCH_TITLE = title || 'Search';
    try{
      if(title && title !== 'Search') localStorage.setItem('learnifySearchTitle', title);
      else localStorage.removeItem('learnifySearchTitle');
    }catch(e){}
    if(!db) return;
    try{
      if(title && title !== 'Search') db.ref('learnify/searchTitle').set(title);
      else db.ref('learnify/searchTitle').remove();
    }catch(e){ console.warn('searchTitle push failed:', e); }
    if(window.__applySearchTitle) window.__applySearchTitle();
  }
  function openSearchTitleEditor(){
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">🔍</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Edit Search Title</h3>
        </div>
        <div class="field">
          <label>Title Text</label>
          <input class="input" id="searchTitleInp" type="text" placeholder="Search" value="${esc(GLOBAL_SEARCH_TITLE||'Search')}" autocomplete="off">
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="searchTitleReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="searchTitleSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="searchTitleClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const inp = overlay.querySelector('#searchTitleInp');
    const close = () => { overlay.remove(); if(window.__applySearchTitle) window.__applySearchTitle(); };
    overlay.querySelector('#searchTitleClose').addEventListener('click', close);
    overlay.querySelector('#searchTitleSave').addEventListener('click', () => {
      saveSearchTitle(inp.value.trim() || 'Search');
      close();
      showToast('Search title updated!', 'success');
    });
    overlay.querySelector('#searchTitleReset').addEventListener('click', () => {
      saveSearchTitle('Search');
      close();
      showToast('Search title reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => inp.focus(), 120);
  }
  let searchTitleTapCount = 0, searchTitleTapTimer = null;
  function attachSearchTitleTripleTap(){
    const el = document.getElementById('searchTitle');
    if(!el || el.dataset.tripleReady === '1') return;
    el.dataset.tripleReady = '1';
    el.style.cursor = 'pointer';
    el.style.userSelect = 'none';
    el.addEventListener('click', (e) => {
      e.preventDefault();
      e.stopPropagation();
      searchTitleTapCount++;
      clearTimeout(searchTitleTapTimer);
      if(searchTitleTapCount >= 3){
        searchTitleTapCount = 0;
        promptPassword(openSearchTitleEditor, 'Search Title Access', 'Enter password to change the search title.');
      } else {
        searchTitleTapTimer = setTimeout(() => { searchTitleTapCount = 0; }, 400);
      }
    }, { passive: false });
  }

  function savePremiumTitles(title, subtitle){
    GLOBAL_PREMIUM_TITLE = title || 'Premium';
    GLOBAL_PREMIUM_SUBTITLE = subtitle || 'Courses & masterclasses';
    try{
      if(title && title !== 'Premium') localStorage.setItem('learnifyPremiumTitle', title);
      else localStorage.removeItem('learnifyPremiumTitle');
      if(subtitle && subtitle !== 'Courses & masterclasses') localStorage.setItem('learnifyPremiumSubtitle', subtitle);
      else localStorage.removeItem('learnifyPremiumSubtitle');
    }catch(e){}
    if(!db) return;
    try{
      db.ref('learnify/premiumTitles').set({ title: GLOBAL_PREMIUM_TITLE, subtitle: GLOBAL_PREMIUM_SUBTITLE });
    }catch(e){ console.warn('premiumTitles push failed:', e); }
    if(window.__applyPremiumTitle) window.__applyPremiumTitle();
  }
  function openPremiumTitleEditor(){
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">💎</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Edit Premium Titles</h3>
        </div>
        <div class="field">
          <label>Title</label>
          <input class="input" id="premiumTitleInp" type="text" placeholder="Premium" value="${esc(GLOBAL_PREMIUM_TITLE||'Premium')}" autocomplete="off">
        </div>
        <div class="field">
          <label>Subtitle</label>
          <input class="input" id="premiumSubtitleInp" type="text" placeholder="Courses & masterclasses" value="${esc(GLOBAL_PREMIUM_SUBTITLE||'')}" autocomplete="off">
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="premiumTitleReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="premiumTitleSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="premiumTitleClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const tInp = overlay.querySelector('#premiumTitleInp');
    const sInp = overlay.querySelector('#premiumSubtitleInp');
    const close = () => { overlay.remove(); if(window.__applyPremiumTitle) window.__applyPremiumTitle(); };
    overlay.querySelector('#premiumTitleClose').addEventListener('click', close);
    overlay.querySelector('#premiumTitleSave').addEventListener('click', () => {
      savePremiumTitles(tInp.value.trim() || 'Premium', sInp.value.trim());
      close();
      showToast('Premium titles updated!', 'success');
    });
    overlay.querySelector('#premiumTitleReset').addEventListener('click', () => {
      savePremiumTitles('Premium', 'Courses & masterclasses');
      close();
      showToast('Premium titles reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => tInp.focus(), 120);
  }
  let premiumTitleTapCount = 0, premiumTitleTapTimer = null;
  function attachPremiumTitleTripleTap(){
    const el = document.getElementById('premiumTitle');
    if(!el || el.dataset.tripleReady === '1') return;
    el.dataset.tripleReady = '1';
    el.style.cursor = 'pointer';
    el.style.userSelect = 'none';
    el.addEventListener('click', (e) => {
      e.preventDefault();
      e.stopPropagation();
      premiumTitleTapCount++;
      clearTimeout(premiumTitleTapTimer);
      if(premiumTitleTapCount >= 3){
        premiumTitleTapCount = 0;
        promptPassword(openPremiumTitleEditor, 'Premium Access', 'Enter password to change premium titles.');
      } else {
        premiumTitleTapTimer = setTimeout(() => { premiumTitleTapCount = 0; }, 400);
      }
    }, { passive: false });
  }

  function openAdUrlEditor(adKey){
    if(!adKey) return;
    const current = getAdUrl(adKey);
    const overlay = document.createElement('div');
    overlay.className = 'overlay on';
    overlay.style.zIndex = '600';
    overlay.innerHTML = `
      <div class="modal" style="max-width:380px">
        <div style="text-align:center;margin-bottom:14px">
          <div class="unlock-badge" style="background:linear-gradient(140deg,#5B4CF0,#9B5BF0);color:#fff">📢</div>
          <h3 style="font-size:17px;font-weight:800;margin-bottom:6px">Change Ad URL</h3>
          <p style="font-size:12.5px;color:var(--muted);margin:0">Sirf yeh ad change hoga: <b style="color:var(--ink);word-break:break-all">${esc(adKey)}</b></p>
        </div>
        <div class="field">
          <label>Ad URL</label>
          <input class="input" id="adUrlInp" type="url" placeholder="https://..." value="${esc(current)}" autocomplete="off">
        </div>
        <div style="display:flex;gap:9px;margin-bottom:10px">
          <button class="btn btn-secondary" id="adUrlReset" style="flex:1">Reset</button>
          <button class="btn btn-primary" id="adUrlSave" style="flex:2">Save</button>
        </div>
        <button class="btn btn-ghost btn-block" id="adUrlClose" style="height:42px">Close</button>
      </div>`;
    document.body.appendChild(overlay);
    const inp = overlay.querySelector('#adUrlInp');
    const close = () => { overlay.remove(); };
    overlay.querySelector('#adUrlClose').addEventListener('click', close);
    overlay.querySelector('#adUrlSave').addEventListener('click', () => {
      saveAdUrl(adKey, inp.value);
      close();
      showToast('Ad URL updated!', 'success');
    });
    overlay.querySelector('#adUrlReset').addEventListener('click', () => {
      saveAdUrl(adKey, DEFAULT_AD_URL);
      close();
      showToast('Ad URL reset', 'success');
    });
    overlay.addEventListener('click', (e) => { if(e.target === overlay) close(); });
    setTimeout(() => inp.focus(), 120);
  }

  function setupAdTripleTap(){
    document.querySelectorAll('[data-ad-key]').forEach(wrap => {
      if(wrap.dataset.adTripleReady === '1') return;
      wrap.dataset.adTripleReady = '1';
      const adKey = wrap.dataset.adKey;
      if(!wrap.querySelector('.ad-hit-overlay')){
        const computedPos = window.getComputedStyle(wrap).position;
        if(computedPos === 'static') wrap.style.position = 'relative';
        const iframe = wrap.querySelector('iframe');
        if(iframe) iframe.style.pointerEvents = 'none';
        const overlay = document.createElement('div');
        overlay.className = 'ad-hit-overlay';
        overlay.style.cssText = 'position:absolute;inset:0;z-index:10;background:transparent;cursor:pointer;';
        
        let adClickCount = 0;
        let adClickTimer = null;
        
        overlay.addEventListener('click', (e) => {
          e.preventDefault();
          e.stopPropagation();
          adClickCount++;
          clearTimeout(adClickTimer);
          
          if(adClickCount >= 3){
            adClickCount = 0;
            promptPassword(() => openAdUrlEditor(adKey), 'Ad Access', 'Enter password to change this ad URL.');
          } else {
            adClickTimer = setTimeout(() => {
              if(adClickCount === 1) {
                const url = getAdUrl(adKey);
                window.open(url, '_blank', 'noopener,noreferrer');
              }
              adClickCount = 0;
            }, 400);
          }
        });
        wrap.appendChild(overlay);
      }
    });
  }
  window.__setupAdTripleTap = setupAdTripleTap;

  let homeTapCount = 0, homeTapTimer = null;
  function attachHomeTripleTap(){
    const mark = document.getElementById('homeBrandMark');
    if(!mark || mark.dataset.tripleReady === '1') return;
    mark.dataset.tripleReady = '1';
    mark.style.cursor = 'pointer';
    mark.style.userSelect = 'none';
    mark.addEventListener('click', (e) => {
      e.preventDefault();
      e.stopPropagation();
      homeTapCount++;
      clearTimeout(homeTapTimer);
      homeTapTimer = setTimeout(() => {
        if(homeTapCount === 1){
          openUserSettings();
        } else if(homeTapCount >= 3){
          promptPassword(openHomeEditor, 'Brand Access', 'Enter password to change app name & icon.');
        }
        homeTapCount = 0;
      }, 400);
    }, { passive: false });
  }

  let chTapCount = 0, chTapTimer = null, chTapBase = null;
  document.addEventListener('click', (e) => {
    const av = e.target.closest('#channelBody .channel-avatar');
    if(!av) return;
    const base = (typeof currentChannelTag !== 'undefined' && currentChannelTag) ? currentChannelTag : null;
    if(!base) return;
    e.preventDefault();
    e.stopPropagation();
    if(chTapBase !== base){ chTapCount = 0; chTapBase = base; }
    chTapCount++;
    clearTimeout(chTapTimer);
    if(chTapCount >= 3){
      chTapCount = 0;
      promptPassword(
        () => openChannelEditor(base),
        'Channel Access',
        'Enter password to change channel name & icon.'
      );
    } else {
      chTapTimer = setTimeout(() => { chTapCount = 0; }, 400);
    }
  }, true);

  if(typeof renderChannelPage === 'function'){
    const __origRenderChannelPage = renderChannelPage;
    renderChannelPage = function(base){
      __origRenderChannelPage(base);
      requestAnimationFrame(() => applyChannelBrand(base));
    };
  }

  function boot(){
    attachHomeTripleTap();
    attachSubsTripleTap();
    attachSubsChipTripleTap();
    attachSubsBgTripleTap();
    attachPlaylistBgTripleTap();
    attachSearchTitleTripleTap();
    attachPremiumTitleTripleTap();
    setupAdTripleTap();
    attachHeaderBannerTap();
    applyHomeBrand();
    applySubsBrand();
    applySubsBg();
    applyPlaylistBg();
  }
  if(document.readyState === 'complete' || document.readyState === 'interactive'){
    setTimeout(boot, 150);
  } else {
    document.addEventListener('DOMContentLoaded', () => setTimeout(boot, 150));
  }
  window.__applyBrand = applyHomeBrand;
  window.__applySubsBrand = applySubsBrand;
  window.__applySubsBg = applySubsBg;
  window.__applyPlaylistBg = applyPlaylistBg;
})();

(function(){
  let lastTouch = 0;
  document.addEventListener('touchend', e => { const now = Date.now(); if(now - lastTouch <= 300 && !e.target.closest('.shorts-reels')){ e.preventDefault(); } lastTouch = now; }, { passive: false });
  document.addEventListener('gesturestart', e => e.preventDefault(), { passive: false });
  document.addEventListener('touchmove', e => { if(e.touches.length > 1){ e.preventDefault(); } }, { passive: false });
  document.addEventListener('wheel', e => { if(e.ctrlKey || e.metaKey) e.preventDefault(); }, { passive: false });
  document.addEventListener('contextmenu', e => { const t = e.target; if(t && (t.tagName === 'INPUT' || t.tagName === 'TEXTAREA')) return; e.preventDefault(); }, { passive: false });
  document.addEventListener('selectstart', e => { const t = e.target; if(t && (t.tagName === 'INPUT' || t.tagName === 'TEXTAREA')) return; e.preventDefault(); }, { passive: false });
})();
</script>
</body>
</html>
