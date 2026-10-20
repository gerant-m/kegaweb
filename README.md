
<!DOCTYPE html>
<html lang="rw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KUGALI VIBE | Youth Entertainment</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Mono&family=Playfair+Display:wght@700;800;900&display=swap');

:root {
  --bg:#0b101b; --orange:#ff5a00; --blue:#0788ff;
  --cream:#f4eddd; --muted:#aab0bd; --line:#293142;
}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--cream);font-family:Arial,sans-serif}
button,input,textarea,select{font:inherit}
button{cursor:pointer}
a{color:inherit;text-decoration:none}
header{display:flex;align-items:flex-start;gap:25px;padding:15px 3%;border-bottom:1px solid var(--line);position:sticky;top:0;background:#0b101bf5;z-index:5}
.logo{font-weight:900;font-size:30px;line-height:.85;min-width:100px;letter-spacing:-1px}
.logo span{display:block;color:var(--orange)}
.logo span+span{color:var(--blue)}
nav{display:flex;gap:20px;flex:1;flex-wrap:wrap}
nav a{font: bold 12px Georgia,serif;text-transform:uppercase;padding-top:5px}
nav a:hover{color:var(--orange)}
button{border:0;padding:12px 17px;font-weight:bold}
.primary{background:var(--orange);color:#111}
.secondary{border:2px solid var(--cream);background:transparent;color:var(--cream)}
.subnav{text-align:center;padding:15px;border-bottom:1px solid var(--line);font:bold 12px Georgia;letter-spacing:2px}
.hero{padding:45px 4%;display:grid;grid-template-columns:1.2fr .8fr;gap:5%;align-items:center}
.featured{position:relative;padding:10px}
.featured:before{content:"";position:absolute;inset:0;background:var(--orange);transform:rotate(-2deg);z-index:-1}
.picture{height:350px;background:linear-gradient(#0002,#0004),url('https://images.unsplash.com/photo-1531058020387-3be344556be6?auto=format&fit=crop&w=1200&q=85') center/cover;border:8px solid var(--cream);display:grid;place-items:center}
.play{border-radius:50%;width:85px;height:85px;background:var(--orange);font-size:28px}
.label{font:13px 'DM Mono',monospace;letter-spacing:3px;color:var(--orange);text-transform:uppercase}
h1{font:900 clamp(38px,5vw,65px)/.98 'Playfair Display',Georgia,serif;margin:20px 0}
h2{font:800 32px 'Playfair Display',Georgia,serif}
p{line-height:1.65}
.muted{color:var(--muted)}
.section{padding:28px 4% 45px;border-top:1px solid var(--line)}
.section-title{display:flex;justify-content:space-between;align-items:center}
.cards{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.card{background:#111827;border:1px solid #263144;cursor:pointer;min-width:0}
.card:hover{border-color:var(--orange);transform:translateY(-3px)}
.thumb{height:175px;background-size:cover;background-position:center;display:grid;place-items:center}
.thumb span{background:var(--orange);color:#111;border-radius:50%;padding:14px}
.card-body{padding:14px}
.card h3{font:700 20px 'Playfair Display',Georgia,serif}
.card p{font-size:13px;color:var(--muted)}
.card small{color:var(--orange)}
.news-layout{display:grid;grid-template-columns:1.2fr 1fr;gap:20px}
.news-feature{min-height:260px;padding:25px;display:flex;align-items:end;background:linear-gradient(transparent,#000d),url('https://images.unsplash.com/photo-1523580494863-6f3031224c94?auto=format&fit=crop&w=1000&q=80') center/cover}
.news-list{display:grid;gap:12px}
.news-item{padding:15px;border-bottom:1px solid var(--line);cursor:pointer}
footer{padding:30px 4%;border-top:1px solid var(--line);color:var(--muted);display:flex;justify-content:space-between;gap:15px;flex-wrap:wrap}
.modal{display:none;position:fixed;inset:0;background:#000c;z-index:10;align-items:center;justify-content:center;padding:15px}
.modal.show{display:flex}
.modalbox{background:#111827;border:1px solid #39445a;padding:25px;width:min(500px,100%);max-height:90vh;overflow:auto;position:relative}
.close{float:right;background:none;color:white;font-size:24px;padding:0}
.field{margin:14px 0}
.field label{display:block;font:12px 'DM Mono',monospace;margin-bottom:7px;color:var(--muted)}
.field input,.field textarea,.field select{width:100%;padding:12px;background:#080d16;border:1px solid #39445a;color:white}
.field textarea{min-height:85px}
.row{display:flex;justify-content:space-between;align-items:center;gap:10px;border-bottom:1px solid var(--line);padding:10px 0}
@media(max-width:850px){header{flex-wrap:wrap;gap:15px}nav{gap:12px}nav a{font-size:10px}.hero{grid-template-columns:1fr;gap:30px}.cards{grid-template-columns:repeat(2,1fr)}.news-layout{grid-template-columns:1fr}.picture{height:280px}}
@media(max-width:480px){header{padding:13px 4%}.logo{font-size:25px;min-width:75px}nav{gap:10px}.hero{padding:30px 5%}.picture{height:220px}.section{padding:25px 5%}.cards{gap:10px}.thumb{height:130px}.card-body{padding:10px}h2{font-size:27px}.card h3{font-size:16px}}
</style>
</head>
<body>
<header>
  <a href="#" class="logo"><span>KUGALI</span><span>VIBE</span></a>
  <nav>
    <a href="#trending">Trending</a>
    <a href="#videos">Videos</a>
    <a href="#news">News</a>
    <a href="#music">Music</a>
    <a href="#culture">Culture</a>
    <a href="#sports">Sports</a>
  </nav>
  <button class="secondary" onclick="show('login')">LOGIN</button>
  <button class="primary" onclick="show('register')">JOIN US</button>
</header>

<div class="subnav">KUGALI VIBE + &nbsp; CULTURE · STORIES · WHAT'S TRENDING</div>

<main>
<section class="hero" id="trending">
  <div class="featured">
    <div class="picture" id="heroPicture">
      <button class="play" onclick="openStory(featuredId)">▶</button>
    </div>
  </div>
  <div>
    <div class="label">Featured · Now Trending</div>
    <h1 id="heroTitle">THE NEW WAVE: YOUTH CULTURE IS HERE</h1>
    <p id="heroDesc">Amakuru agezweho, imyidagaduro, umuziki, sports n'ibindi byose urubyiruko rukunda.</p>
    <p class="muted">KUGALI VIBE ORIGINALS · TRENDING NOW</p>
    <button class="primary" onclick="openStory(featuredId)">▶ REBA INKURU</button>
  </div>
</section>

<section class="section" id="videos">
  <div class="section-title"><div><div class="label">Watch something good</div><h2>Trending Videos</h2></div></div>
  <div class="cards" id="videoCards"></div>
</section>

<section class="section" id="news">
  <div class="label">Stay in the know</div><h2>Latest News</h2>
  <div class="news-layout">
    <div class="news-feature"><div><div class="label">TOP STORY</div><h2>Inkuru zigezweho n'ibiganiro by'urubyiruko</h2></div></div>
    <div class="news-list" id="newsList"></div>
  </div>
</section>

<section class="section" id="music">
  <div class="label">Fresh sounds</div><h2>Music & Pop Culture</h2>
  <div class="cards" id="musicCards"></div>
</section>

<section class="section" id="culture">
  <div class="label">Join the conversation</div><h2>KUGALI VIBE Community</h2>
  <p class="muted">Fungura konti, ukunde inkuru, utange ibitekerezo kandi ukurikirane ibigezweho.</p>
  <button class="primary" onclick="show('register')">FUNGURA KONTE</button>
  <button class="secondary" onclick="show('admin')">ADMIN</button>
</section>
</main>

<footer>
  <div><b style="color:white;font-size:22px">KUGALI VIBE</b><p>Culture. Stories. Now.</p></div>
  <div>© <span id="year"></span> KUGALI VIBE</div>
</footer>

<div class="modal" id="login"><div class="modalbox">
  <button class="close" onclick="hide('login')">×</button><h2>Login</h2>
  <form onsubmit="loginUser(event)">
    <div class="field"><label>Email</label><input id="loginEmail" type="email" required></div>
    <div class="field"><label>Password</label><input id="loginPass" type="password" required></div>
    <button class="primary">LOGIN</button>
  </form>
</div></div>

<div class="modal" id="register"><div class="modalbox">
  <button class="close" onclick="hide('register')">×</button><h2>Create Account</h2>
  <form onsubmit="registerUser(event)">
    <div class="field"><label>Your name</label><input id="regName" required></div>
    <div class="field"><label>Email</label><input id="regEmail" type="email" required></div>
    <div class="field"><label>Password</label><input id="regPass" type="password" minlength="6" required></div>
    <button class="primary">REGISTER</button>
  </form>
</div></div>

<div class="modal" id="story"><div class="modalbox">
  <button class="close" onclick="hide('story')">×</button>
  <div class="label">KUGALI VIBE STORY</div><h2 id="storyTitle"></h2>
  <p id="storyDesc"></p><div id="storyVideo"></div>
  <button class="primary" onclick="likeStory()">♥ LIKE <span id="likeCount">0</span></button>
  <div class="field"><label>Comment</label><textarea id="commentText" placeholder="Andika igitekerezo..."></textarea></div>
  <button class="secondary" onclick="addComment()">POST COMMENT</button>
  <div id="comments"></div>
</div></div>

<div class="modal" id="admin"><div class="modalbox">
  <button class="close" onclick="hide('admin')">×</button><h2>Admin Dashboard</h2>
  <p class="muted">Demo password: vibeadmin2026</p>
  <div class="field"><label>Admin password</label><input id="adminPass" type="password"></div>
  <button class="primary" onclick="adminLogin()">OPEN ADMIN</button>
  <div id="adminTools" style="display:none">
    <h3>Publish content</h3>
    <form onsubmit="addContent(event)">
      <div class="field"><label>Category</label><select id="newType"><option value="video">Video</option><option value="news">News</option><option value="music">Music</option></select></div>
      <div class="field"><label>Title</label><input id="newTitle" required></div>
      <div class="field"><label>Description</label><textarea id="newDesc" required></textarea></div>
      <div class="field"><label>Image URL</label><input id="newImage" type="url" placeholder="https://..."></div>
      <div class="field"><label>Video URL (optional)</label><input id="newVideo" type="url" placeholder="https://..."></div>
      <button class="primary">PUBLISH</button>
    </form>
    <h3>Manage posts</h3><div id="adminList"></div>
  </div>
</div></div>

<script>
const starter = [
{id:1,type:'video',title:'Inside the Youth Creative Scene',desc:'Abasore n’inkumi bari guteza imbere impano zabo.',image:'https://images.unsplash.com/photo-1492684223066-81342ee5ff30?auto=format&fit=crop&w=900&q=80',video:'',likes:10,views:1200},
{id:2,type:'video',title:'Music Trends This Week',desc:'Indirimbo n’abahanzi bari kuvugwa cyane.',image:'https://images.unsplash.com/photo-1501389615356-6c9c6b5f4d7b?auto=format&fit=crop&w=900&q=80',video:'',likes:8,views:850},
{id:3,type:'video',title:'Fashion & Street Style',desc:'Imideri mishya n’imyambarire y’urubyiruko.',image:'https://images.unsplash.com/photo-1529139574466-a303027c1d8b?auto=format&fit=crop&w=900&q=80',video:'',likes:12,views:730},
{id:4,type:'video',title:'Sports Fans Talk',desc:'Ibyaranze imikino n’ibitekerezo by’abafana.',image:'https://images.unsplash.com/photo-1522778119026-d647f0596c20?auto=format&fit=crop&w=900&q=80',video:'',likes:5,views:600},
{id:5,type:'news',title:'Amakuru mashya y’urubyiruko',desc:'Inkuru n’ibikorwa bishya byo gukurikirana.',image:'https://images.unsplash.com/photo-1523580494863-6f3031224c94?auto=format&fit=crop&w=900&q=80',video:'',likes:3,views:0},
{id:6,type:'news',title:'Ibikorwa n’ibirori biri imbere',desc:'Menya ibirori n’ibikorwa bishya.',image:'https://images.unsplash.com/photo-1531058020387-3be344556be6?auto=format&fit=crop&w=900&q=80',video:'',likes:2,views:0},
{id:7,type:'music',title:'Fresh Music & New Sounds',desc:'Menya umuziki mushya uri kuvugwa.',image:'https://images.unsplash.com/photo-1516280440614-37939bbacd81?auto=format&fit=crop&w=900&q=80',video:'',likes:9,views:0},
{id:8,type:'music',title:'Behind The Music',desc:'Ibiganiro n’inkuru zijyanye n’umuziki.',image:'https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?auto=format&fit=crop&w=900&q=80',video:'',likes:4,views:0}
];
let posts=JSON.parse(localStorage.getItem('kvPosts')||'null')||starter;
let users=JSON.parse(localStorage.getItem('kvUsers')||'[]');
let current=JSON.parse(localStorage.getItem('kvCurrent')||'null');
let featuredId=1,activeId=null,admin=false;

function save(){localStorage.setItem('kvPosts',JSON.stringify(posts));localStorage.setItem('kvUsers',JSON.stringify(users));localStorage.setItem('kvCurrent',JSON.stringify(current))}
function safe(s){return String(s||'').replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]))}
function show(id){document.getElementById(id).classList.add('show')}
function hide(id){document.getElementById(id).classList.remove('show')}
function card(p){return `<article class="card" onclick="openStory(${p.id})"><div class="thumb" style="background-image:url('${safe(p.image)}')"><span>▶</span></div><div class="card-body"><small>${safe(p.type.toUpperCase())}</small><h3>${safe(p.title)}</h3><p>${safe(p.desc)}</p><small>♥ ${p.likes||0} · ${p.views||0} VIEWS</small></div></article>`}
function render(){
 document.getElementById('videoCards').innerHTML=posts.filter(p=>p.type==='video').map(card).join('');
 document.getElementById('musicCards').innerHTML=posts.filter(p=>p.type==='music').map(card).join('');
 document.getElementById('newsList').innerHTML=posts.filter(p=>p.type==='news').map(p=>`<div class="news-item" onclick="openStory(${p.id})"><small>${safe(p.type.toUpperCase())}</small><h3>${safe(p.title)}</h3><p class="muted">${safe(p.desc)}</p></div>`).join('');
 let f=posts.find(p=>p.id===featuredId)||posts.find(p=>p.type==='video');
 if(f){featuredId=f.id;document.getElementById('heroTitle').textContent=f.title;document.getElementById('heroDesc').textContent=f.desc;document.getElementById('heroPicture').style.backgroundImage=`url('${f.image}')`}
 if(admin)renderAdmin();
}
function openStory(id){
 let p=posts.find(x=>x.id===id);if(!p)return;activeId=id;p.views=(p.views||0)+1;save();
 document.getElementById('storyTitle').textContent=p.title;
 document.getElementById('storyDesc').textContent=p.desc;
 document.getElementById('likeCount').textContent=p.likes||0;
 document.getElementById('storyVideo').innerHTML=p.video?`<p><a target="_blank" rel="noopener" href="${safe(p.video)}">▶ Watch video</a></p>`:'';
 renderComments();render();show('story');
}
function likeStory(){if(!current){alert('Banza winjire muri konti yawe.');return}let p=posts.find(x=>x.id===activeId);p.likes=(p.likes||0)+1;save();document.getElementById('likeCount').textContent=p.likes;render()}
function addComment(){if(!current){alert('Banza winjire muri konti yawe.');return}let t=document.getElementById('commentText').value.trim();if(!t)return;let k='kvComments'+activeId;let arr=JSON.parse(localStorage.getItem(k)||'[]');arr.unshift({name:current.name,text:t});localStorage.setItem(k,JSON.stringify(arr));document.getElementById('commentText').value='';renderComments()}
function renderComments(){let arr=JSON.parse(localStorage.getItem('kvComments'+activeId)||'[]');document.getElementById('comments').innerHTML='<h3>Comments</h3>'+arr.map(c=>`<div class="row"><b>${safe(c.name)}</b><span>${safe(c.text)}</span></div>`).join('')}
function registerUser(e){e.preventDefault();let name=document.getElementById('regName').value.trim(),email=document.getElementById('regEmail').value.trim().toLowerCase(),pass=document.getElementById('regPass').value;if(users.some(u=>u.email===email)){alert('Iyi email isanzwe ifite konti.');return}users.push({name,email,pass});current={name,email};save();hide('register');e.target.reset();alert('Konti yafunguwe!');render()}
function loginUser(e){e.preventDefault();let email=document.getElementById('loginEmail').value.trim().toLowerCase(),pass=document.getElementById('loginPass').value;let u=users.find(x=>x.email===email&&x.pass===pass);if(!u){alert('Email cyangwa password si byo.');return}current={name:u.name,email:u.email};save();hide('login');e.target.reset();alert('Winjiye neza.');render()}
function adminLogin(){if(document.getElementById('adminPass').value!=='vibeadmin2026'){alert('Password si yo.');return}admin=true;document.getElementById('adminTools').style.display='block';renderAdmin()}
function addContent(e){e.preventDefault();if(!admin)return;let type=document.getElementById('newType').value;posts.unshift({id:Date.now(),type,title:document.getElementById('newTitle').value.trim(),desc:document.getElementById('newDesc').value.trim(),image:document.getElementById('newImage').value.trim()||'https://images.unsplash.com/photo-1492684223066-81342ee5ff30?auto=format&fit=crop&w=900&q=80',video:document.getElementById('newVideo').value.trim(),likes:0,views:0});save();e.target.reset();render();alert('Inkuru yashyizweho.')}
function renderAdmin(){document.getElementById('adminList').innerHTML=posts.map(p=>`<div class="row"><span>${safe(p.title)}</span><button onclick="deletePost(${p.id})">DELETE</button></div>`).join('')}
function deletePost(id){if(!admin)return;posts=posts.filter(p=>p.id!==id);save();render()}
document.querySelectorAll('.modal').forEach(m=>m.addEventListener('click',e=>{if(e.target===m)m.classList.remove('show')}));
document.getElementById('year').textContent=new Date().getFullYear();
render();
</script>
</body>
</html>
