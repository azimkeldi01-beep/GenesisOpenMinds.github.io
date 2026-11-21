<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ArtTech Genesis</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root {
  --bg:#f3f5f7;
  --surface:#ffffff;
  --surface2:#e9eef2;
  --primary:#29465f;
  --primary2:#426d8e;
  --text:#192b3b;
  --muted:#73808d;
  --border:#dce3e9;
  --success:#477c68;
  --radius:12px;
}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:var(--bg);color:var(--text);font-family:Inter,Arial,sans-serif;line-height:1.6}
button,input,textarea,select{font:inherit}
button{cursor:pointer}
a{text-decoration:none;color:inherit}
.topbar{height:76px;background:rgba(255,255,255,.96);border-bottom:1px solid var(--border);display:flex;align-items:center;padding:0 6%;gap:35px;position:sticky;top:0;z-index:10}
.logo{font-size:21px;font-weight:800;letter-spacing:-1px}
.logo span{color:var(--primary2)}
nav{display:flex;gap:28px}
nav a{font-size:13px;color:var(--muted);font-weight:600}
nav a:hover{color:var(--primary)}
#userBox{margin-left:auto;font-size:13px}
.btn{border:1px solid var(--border);background:#fff;color:var(--text);padding:11px 19px;border-radius:8px;font-size:13px;font-weight:600;transition:.2s}
.btn:hover{background:var(--surface2)}
.btn.primary{background:var(--primary);color:white;border-color:var(--primary)}
.btn.primary:hover{background:var(--primary2)}
.btn.danger{color:#a34c4c}
.btn.small{padding:8px 13px;font-size:12px}
.btn.full{width:100%;margin-top:14px}
section{padding:90px 6%}
.container{max-width:1200px;margin:auto}
.hero{background:#e8edf1;min-height:620px;display:flex;align-items:center}
.hero-inner{max-width:1200px;margin:auto;width:100%;display:grid;grid-template-columns:1.1fr .9fr;gap:65px;align-items:center}
.eyebrow{font-size:11px;letter-spacing:3px;text-transform:uppercase;color:var(--primary2);font-weight:700}
h1,h2,h3,h4,p{margin-top:0}
h1{font-size:clamp(42px,7vw,82px);line-height:1.02;letter-spacing:-5px;margin:22px 0}
h1 span{color:var(--primary2)}
.hero-description{max-width:550px;color:#596a79;font-size:16px;line-height:1.9}
.hero-buttons{display:flex;gap:12px;margin-top:30px;flex-wrap:wrap}
.hero-visual{display:grid;grid-template-columns:1fr 1fr;gap:15px;transform:rotate(-2deg)}
.visual-card{height:210px;border-radius:8px;background-size:cover;background-position:center;box-shadow:0 15px 35px #263d5020}
.visual-card:nth-child(1){background:linear-gradient(145deg,#526e7e,#a7b9c3)}
.visual-card:nth-child(2){background:linear-gradient(145deg,#263a4c,#718798);margin-top:35px}
.visual-card:nth-child(3){background:linear-gradient(145deg,#8c9ba4,#d4d9db);margin-top:-25px}
.visual-card:nth-child(4){background:linear-gradient(145deg,#526778,#c1cbd0)}
.visual-caption{background:#fff;padding:15px;border-radius:7px;font-size:12px;font-weight:600;grid-column:1/3}
.section-heading{margin-bottom:38px}
.section-heading h2{font-size:clamp(32px,4vw,48px);letter-spacing:-2px;margin-bottom:8px}
.section-heading p{color:var(--muted);font-size:14px}
.studio{background:var(--bg)}
.studio-grid{display:grid;grid-template-columns:310px 1fr;gap:24px;align-items:start}
.card{background:var(--surface);border:1px solid var(--border);border-radius:var(--radius);padding:25px;box-shadow:0 5px 20px #1c344308}
.card h3{font-size:19px;letter-spacing:-.5px;margin-bottom:17px}
label{display:block;font-size:12px;font-weight:600;margin:15px 0 7px}
input,textarea,select{width:100%;padding:12px 13px;border:1px solid var(--border);border-radius:7px;background:#fff;color:var(--text);font-size:13px;outline:none}
input:focus,textarea:focus,select:focus{border-color:var(--primary2);box-shadow:0 0 0 3px #426d8e18}
textarea{resize:vertical}
.palette{display:flex;gap:10px;flex-wrap:wrap;margin:13px 0}
.color{width:29px;height:29px;border-radius:50%;border:3px solid white;outline:1px solid var(--border)}
.color.active{outline:2px solid var(--primary)}
.folder-list{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:16px}
.folder-item{border:1px solid var(--border);border-radius:8px;padding:13px 9px;background:#fff;text-align:center;cursor:pointer;transition:.2s}
.folder-item:hover,.folder-item.active{border-color:var(--primary2);background:#edf2f6}
.folder-icon{height:35px;width:48px;margin:0 auto 8px;border-radius:5px 5px 7px 7px;position:relative;background:var(--folder-color,#29465f)}
.folder-icon:before{content:"";position:absolute;top:-5px;left:0;width:20px;height:8px;border-radius:4px 4px 0 0;background:inherit}
.folder-item strong{display:block;font-size:11px;overflow-wrap:anywhere}
.folder-item small{font-size:10px;color:var(--muted)}
.empty{text-align:center;padding:90px 15px;color:var(--muted)}
.empty-icon{font-size:42px;color:#9aaab7;margin-bottom:12px}
.workspace-head{display:flex;align-items:center;gap:15px;border-bottom:1px solid var(--border);padding-bottom:18px;margin-bottom:20px}
.workspace-head h3{margin:0}
.workspace-head p{margin:3px 0 0;font-size:12px;color:var(--muted)}
.drop{border:1px dashed #9eafbd;border-radius:9px;background:#f7f9fa;text-align:center;padding:28px;margin-top:18px;color:var(--muted);font-size:13px}
.drop.drag{background:#e7eef3;border-color:var(--primary)}
.drop input{display:none}
.file-list{display:flex;gap:10px;flex-wrap:wrap;margin-top:15px}
.file-item{width:90px;height:90px;border-radius:7px;position:relative;overflow:hidden;background:#e8edf1}
.file-item img,.file-item video{width:100%;height:100%;object-fit:cover}
.file-item .remove{position:absolute;top:4px;right:4px;background:#fff;border:0;border-radius:50%;width:22px;height:22px}
.row{display:grid;grid-template-columns:1fr 1fr;gap:15px}
.actions{display:flex;justify-content:flex-end;gap:10px;margin-top:22px;flex-wrap:wrap}
.archive{background:#e8edf1}
.archive-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(235px,1fr));gap:18px}
.day-card{background:#fff;border:1px solid var(--border);border-radius:10px;overflow:hidden;cursor:pointer;transition:.2s}
.day-card:hover{transform:translateY(-4px);box-shadow:0 12px 25px #20384b16}
.day-cover{height:155px;background:#526d82;display:flex;align-items:center;justify-content:center;color:white;font-size:38px;background-size:cover;background-position:center}
.day-info{padding:17px}
.day-info h3{font-size:17px;margin:0 0 5px}
.day-info p{font-size:11px;color:var(--muted);margin:0}
.day-info .day-preview{font-size:12px;margin-top:10px;color:#536474}
footer{padding:28px 6%;text-align:center;background:#fff;color:var(--muted);font-size:11px;border-top:1px solid var(--border)}
.modal{position:fixed;inset:0;background:#102234a8;z-index:20;display:none;align-items:center;justify-content:center;padding:20px}
.modal.open{display:flex}
.modal-box{background:white;border-radius:12px;width:100%;max-width:440px;padding:30px;max-height:90vh;overflow:auto;position:relative}
.modal-box.wide{max-width:900px;padding:0}
.close{position:absolute;right:15px;top:12px;border:0;background:#edf1f4;border-radius:6px;width:32px;height:32px;font-size:20px}
.modal-box h2{font-size:26px;letter-spacing:-1px}
.tabs{display:flex;gap:5px;background:#edf1f4;padding:4px;border-radius:7px;margin:20px 0}
.tabs button{flex:1;border:0;background:transparent;padding:9px;border-radius:5px;font-size:12px;font-weight:600}
.tabs button.active{background:#fff;color:var(--primary)}
.memory-layout{display:grid;grid-template-columns:1.1fr .9fr;min-height:480px}
.memory-photo{background:#344f64;min-height:350px;display:flex;align-items:center;justify-content:center;color:white;background-size:cover;background-position:center}
.memory-content{padding:30px;background:#f5f7f8}
.memory-content h2{font-size:30px}
.memory-content p{font-size:13px;white-space:pre-wrap}
.memory-meta{color:var(--muted);font-size:11px;margin-bottom:20px}
.ai-button{position:fixed;right:25px;bottom:25px;z-index:12;background:var(--primary);color:white;border:0;border-radius:8px;padding:14px 20px;font-weight:600;font-size:12px;box-shadow:0 5px 20px #1c344330}
.ai-panel{position:fixed;right:25px;bottom:85px;width:340px;max-width:calc(100vw - 30px);background:white;border:1px solid var(--border);border-radius:12px;box-shadow:0 10px 40px #10223430;z-index:12;display:none;overflow:hidden}
.ai-panel.open{display:block}
.ai-head{padding:15px;background:#e8edf1;font-weight:700;font-size:13px;display:flex;justify-content:space-between}
.ai-messages{height:250px;overflow:auto;padding:15px;display:flex;flex-direction:column;gap:10px}
.message{font-size:12px;padding:10px 13px;border-radius:8px;max-width:90%}
.message.bot{background:#edf1f4;align-self:flex-start}
.message.user{background:#dce6ed;align-self:flex-end}
.ai-form{display:flex;gap:7px;padding:12px;border-top:1px solid var(--border)}
.ai-form input{flex:1;min-width:0}
.toast{position:fixed;bottom:25px;left:50%;transform:translate(-50%,20px);background:#192f41;color:white;padding:12px 20px;border-radius:7px;font-size:12px;opacity:0;transition:.2s;z-index:40;pointer-events:none}
.toast.show{opacity:1;transform:translate(-50%,0)}
@media(max-width:800px){
 .hero-inner{grid-template-columns:1fr;gap:35px}
 .hero{padding-top:65px;padding-bottom:65px}
 .hero-visual{max-width:500px}
 .studio-grid{grid-template-columns:1fr}
 .topbar{padding:0 18px}
 nav{gap:12px}
 section{padding:65px 5%}
}
@media(max-width:520px){
 .topbar{height:65px;gap:12px}
 .logo{font-size:17px}
 nav{display:none}
 h1{letter-spacing:-3px}
 .row{grid-template-columns:1fr;gap:0}
 .memory-layout{grid-template-columns:1fr}
 .memory-photo{min-height:240px}
 .modal-box{padding:23px}
 .folder-list{grid-template-columns:repeat(2,1fr)}
}
</style>
</head>
<body>

<header class="topbar">
 <a href="#home" class="logo">ArtTech <span>Genesis</span></a>
 <nav>
  <a href="#studio">Рабочее пространство</a>
  <a href="#archive">Дневник</a>
 </nav>
 <div id="userBox"><button class="btn small" onclick="openAuth()">Войти</button></div>
</header>

<section class="hero" id="home">
 <div class="hero-inner">
  <div>
   <div class="eyebrow">GENESIS OPEN MINDS · DIGITAL DIARY</div>
   <h1>ArtTech<br><span>Genesis.</span></h1>
   <p class="hero-description">Личное цифровое пространство для сохранения воспоминаний. Текст, фотографии и музыка объединяются в единую историю, отражающую настроение и атмосферу каждого дня.</p>
   <div class="hero-buttons">
    <button class="btn primary" onclick="document.querySelector('#studio').scrollIntoView()">Создать воспоминание</button>
    <button class="btn" onclick="openAuth()">Войти в аккаунт</button>
   </div>
  </div>
  <div class="hero-visual">
   <div class="visual-card"></div>
   <div class="visual-card"></div>
   <div class="visual-card"></div>
   <div class="visual-card"></div>
   <div class="visual-caption">Каждый день — отдельная история. Каждая история — часть вашей жизни.</div>
  </div>
 </div>
</section>

<section class="studio" id="studio">
 <div class="container">
  <div class="section-heading">
   <div class="eyebrow">01 / WORKSPACE</div>
   <h2>Рабочее пространство</h2>
   <p>Создавайте папки, добавляйте материалы и сохраняйте свои воспоминания.</p>
  </div>
  <div class="studio-grid">
   <div class="card">
    <h3>Создать папку</h3>
    <form id="folderForm">
     <label for="folderName">Название папки</label>
     <input id="folderName" maxlength="60" placeholder="Например, Незабываемый день" required>
     <label>Цвет папки</label>
     <div class="palette" id="palette"></div>
     <button class="btn primary full" type="submit">Создать папку</button>
    </form>
    <h3 style="margin-top:30px">Мои папки</h3>
    <div class="folder-list" id="folderList"></div>
   </div>

   <div class="card" id="workspace">
    <div class="empty" id="empty">
     <div class="empty-icon">▤</div>
     <h3>Рабочее пространство пусто</h3>
     <p>Создайте папку, чтобы начать работу с воспоминаниями.</p>
    </div>
    <div id="editor" hidden>
     <div class="workspace-head">
      <div class="folder-icon" id="editorIcon"></div>
      <div><h3 id="editorTitle"></h3><p id="editorDate"></p></div>
     </div>
     <label for="dayText">Описание дня</label>
     <textarea id="dayText" rows="6" placeholder="Опишите события, эмоции, места и людей, которые сделали этот день особенным..."></textarea>
     <div class="drop" id="drop">
      <p><strong>Добавить фотографии, видео или музыку</strong></p>
      <p>Перетащите файлы сюда или выберите их на устройстве.</p>
      <button class="btn small" type="button" id="chooseFiles">Выбрать файлы</button>
      <input type="file" id="fileInput" accept="image/*,video/*,audio/*" multiple>
     </div>
     <div class="file-list" id="fileList"></div>
     <div class="row">
      <div><label for="songUrl">Ссылка на песню</label><input id="songUrl" type="url" placeholder="Ссылка на музыку"></div>
      <div><label for="songInfo">Исполнитель и название</label><input id="songInfo" placeholder="Название композиции"></div>
     </div>
     <div class="row">
      <div><label for="mood">Настроение дня</label>
       <select id="mood"><option value="">Не выбрано</option><option>Спокойствие</option><option>Радость</option><option>Ностальгия</option><option>Вдохновение</option><option>Грусть</option><option>Приключение</option></select>
      </div>
      <div><label for="weather">Атмосфера</label>
       <select id="weather"><option value="">Не выбрано</option><option>Солнечно</option><option>Облачно</option><option>Дождливо</option><option>Снежно</option><option>Вечер</option><option>Ночь</option></select>
      </div>
     </div>
     <div class="actions">
      <button class="btn" type="button" onclick="deleteCurrent()">Удалить папку</button>
      <button class="btn primary" type="button" onclick="saveCurrent()">Сохранить воспоминание</button>
     </div>
    </div>
   </div>
  </div>
 </div>
</section>

<section class="archive" id="archive">
 <div class="container">
  <div class="section-heading">
   <div class="eyebrow">02 / PERSONAL ARCHIVE</div>
   <h2>Мой дневник</h2>
   <p>Все сохранённые воспоминания собраны в одном месте.</p>
  </div>
  <div class="archive-grid" id="archiveGrid">
   <p class="empty">Пока здесь нет сохранённых воспоминаний.</p>
  </div>
 </div>
</section>

<footer>ArtTech Genesis · Personal Digital Diary</footer>

<div class="modal" id="authModal">
 <div class="modal-box">
  <button class="close" onclick="closeModal('authModal')">×</button>
  <div class="eyebrow">PERSONAL ACCOUNT</div>
  <h2 id="authTitle">Вход в аккаунт</h2>
  <div class="tabs">
   <button id="loginTab" class="active" onclick="switchAuth('login')">Вход</button>
   <button id="registerTab" onclick="switchAuth('register')">Регистрация</button>
  </div>
  <form id="authForm">
   <label for="authName" id="nameLabel" hidden>Имя пользователя</label>
   <input id="authName" placeholder="Ваше имя" hidden>
   <label for="authEmail">Электронная почта</label>
   <input id="authEmail" type="email" placeholder="name@example.com" required>
   <label for="authPassword">Пароль</label>
   <input id="authPassword" type="password" minlength="6" placeholder="Минимум 6 символов" required>
   <button class="btn primary full" type="submit" id="authSubmit">Войти</button>
  </form>
  <p id="authMessage" style="font-size:12px;color:var(--muted);margin-top:14px"></p>
 </div>
</div>

<div class="modal" id="memoryModal">
 <div class="modal-box wide">
  <button class="close" onclick="closeModal('memoryModal')">×</button>
  <div class="memory-layout">
   <div class="memory-photo" id="memoryPhoto">ARTTECH GENESIS</div>
   <div class="memory-content">
    <div class="eyebrow">PERSONAL MEMORY</div>
    <h2 id="memoryTitle"></h2>
    <div class="memory-meta" id="memoryDate"></div>
    <p id="memoryText"></p>
    <p id="memoryMood"></p>
    <p id="memorySong"></p>
    <div id="memoryFiles"></div>
   </div>
  </div>
 </div>
</div>

<button class="ai-button" id="aiButton">ИИ-помощник</button>
<div class="ai-panel" id="aiPanel">
 <div class="ai-head"><span>ArtTech Assistant</span><button style="border:0;background:none" onclick="toggleAI()">✕</button></div>
 <div class="ai-messages" id="aiMessages">
  <div class="message bot">Здравствуйте! Я помогу подобрать название воспоминания, определить настроение текста и предложить цветовую палитру.</div>
 </div>
 <form class="ai-form" id="aiForm">
  <input id="aiInput" placeholder="Введите сообщение..." autocomplete="off">
  <button class="btn primary small">Отправить</button>
 </form>
</div>
<div class="toast" id="toast"></div>

<script>
const $=s=>document.querySelector(s);
const colors=["#29465f","#426d8e","#647b8b","#52645b","#766b61","#6c6d80","#384d58","#8a765f"];
let selectedColor=colors[0];
let folders=JSON.parse(localStorage.getItem("ag_folders")||"[]");
let currentId=null;
let currentFiles=[];
let authMode="login";
let currentUser=JSON.parse(localStorage.getItem("ag_user")||"null");

function saveData(){
 localStorage.setItem("ag_folders",JSON.stringify(folders));
}
function toast(message){
 const t=$("#toast");t.textContent=message;t.classList.add("show");
 setTimeout(()=>t.classList.remove("show"),2500);
}
function escapeHTML(s){
 return String(s||"").replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]));
}
function formatDate(date){
 return new Date(date).toLocaleDateString("ru-RU",{day:"numeric",month:"long",year:"numeric"});
}
function initPalette(){
 $("#palette").innerHTML=colors.map((c,i)=>`<button type="button" class="color ${i===0?"active":""}" style="background:${c}" data-color="${c}" aria-label="Цвет ${i+1}"></button>`).join("");
}
$("#palette").addEventListener("click",e=>{
 const b=e.target.closest("[data-color]");if(!b)return;
 selectedColor=b.dataset.color;
 document.querySelectorAll(".color").forEach(x=>x.classList.toggle("active",x===b));
});
function renderFolders(){
 $("#folderList").innerHTML=folders.length?folders.map(f=>`
 <div class="folder-item ${f.id===currentId?"active":""}" data-id="${f.id}">
  <div class="folder-icon" style="--folder-color:${f.color}"></div>
  <strong>${escapeHTML(f.name)}</strong>
  <small>${formatDate(f.date)}</small>
 </div>`).join(""):'<p style="font-size:12px;color:var(--muted)">Папок пока нет.</p>';
}
function renderArchive(){
 const saved=folders.filter(f=>f.saved);
 $("#archiveGrid").innerHTML=saved.length?saved.map(f=>{
  const photo=(f.files||[]).find(x=>x.type&&x.type.startsWith("image/"));
  return `<article class="day-card" data-memory="${f.id}">
   <div class="day-cover" style="${photo&&photo.data?`background-image:url('${photo.data}')`:"background-color:"+f.color}">${photo?"": "▤"}</div>
   <div class="day-info"><h3>${escapeHTML(f.name)}</h3>
   <p>${formatDate(f.date)}</p>
   <div class="day-preview">${escapeHTML((f.text||"Воспоминание").slice(0,100))}</div></div>
  </article>`;
 }).join(""):'<p class="empty">Пока здесь нет сохранённых воспоминаний.</p>';
}
function openFolder(id){
 currentId=id;
 const f=folders.find(x=>x.id===id);
 $("#empty").hidden=!!f;
 $("#editor").hidden=!f;
 if(!f){currentFiles=[];renderFolders();return;}
 $("#editorTitle").textContent=f.name;
 $("#editorDate").textContent=formatDate(f.date);
 $("#editorIcon").style.setProperty("--folder-color",f.color);
 $("#dayText").value=f.text||"";
 $("#songUrl").value=f.songUrl||"";
 $("#songInfo").value=f.songInfo||"";
 $("#mood").value=f.mood||"";
 $("#weather").value=f.weather||"";
 currentFiles=(f.files||[]).map(x=>({...x}));
 renderFiles();renderFolders();
}
function renderFiles(){
 $("#fileList").innerHTML=currentFiles.map((f,i)=>{
  let content=f.type.startsWith("image/")?`<img src="${f.data}">`:f.type.startsWith("video/")?`<video src="${f.data}"></video>`:`<div style="padding:28px 5px;text-align:center;font-size:11px">♫ AUDIO</div>`;
  return `<div class="file-item">${content}<button class="remove" data-remove="${i}">×</button></div>`;
 }).join("");
}
$("#folderList").addEventListener("click",e=>{
 const item=e.target.closest("[data-id]");if(item)openFolder(item.dataset.id);
});
$("#folderForm").addEventListener("submit",e=>{
 e.preventDefault();
 const name=$("#folderName").value.trim();if(!name)return;
 const f={id:Date.now().toString(36),name,color:selectedColor,date:new Date().toISOString(),text:"",files:[],saved:false};
 folders.unshift(f);saveData();$("#folderName").value="";openFolder(f.id);toast("Папка создана");
});
$("#chooseFiles").onclick=()=>$("#fileInput").click();
$("#fileInput").addEventListener("change",e=>addFiles(e.target.files));
async function addFiles(files){
 for(const file of files){
  if(file.size>8*1024*1024){toast("Файл больше 8 МБ");continue;}
  const data=await new Promise((resolve,reject)=>{
   const r=new FileReader();r.onload=()=>resolve(r.result);r.onerror=reject;r.readAsDataURL(file);
  });
  currentFiles.push({name:file.name,type:file.type||"application/octet-stream",data});
 }
 renderFiles();$("#fileInput").value="";
}
$("#fileList").addEventListener("click",e=>{
 const b=e.target.closest("[data-remove]");if(!b)return;
 currentFiles.splice(Number(b.dataset.remove),1);renderFiles();
});
const drop=$("#drop");
drop.addEventListener("dragover",e=>{e.preventDefault();drop.classList.add("drag")});
drop.addEventListener("dragleave",()=>drop.classList.remove("drag"));
drop.addEventListener("drop",e=>{e.preventDefault();drop.classList.remove("drag");addFiles(e.dataTransfer.files)});
function saveCurrent(){
 const f=folders.find(x=>x.id===currentId);if(!f)return;
 f.text=$("#dayText").value;
 f.songUrl=$("#songUrl").value;
 f.songInfo=$("#songInfo").value;
 f.mood=$("#mood").value;
 f.weather=$("#weather").value;
 f.files=currentFiles;
 f.saved=true;
 saveData();renderFolders();renderArchive();toast("Воспоминание сохранено");
}
function deleteCurrent(){
 if(!currentId||!confirm("Удалить эту папку и её содержимое?"))return;
 folders=folders.filter(f=>f.id!==currentId);
 currentId=null;saveData();openFolder(null);renderArchive();toast("Папка удалена");
}
$("#archiveGrid").addEventListener("click",e=>{
 const card=e.target.closest("[data-memory]");if(!card)return;
 const f=folders.find(x=>x.id===card.dataset.memory);if(!f)return;
 $("#memoryTitle").textContent=f.name;
 $("#memoryDate").textContent=formatDate(f.date);
 $("#memoryText").textContent=f.text||"Описание отсутствует.";
 $("#memoryMood").textContent=f.mood?"Настроение: "+f.mood:"";
 $("#memorySong").textContent=f.songInfo?"Музыка: "+f.songInfo:"";
 const photo=(f.files||[]).find(x=>x.type.startsWith("image/"));
 $("#memoryPhoto").style.backgroundImage=photo?`url("${photo.data}")`:"";
 $("#memoryPhoto").textContent=photo?"": "ARTTECH GENESIS";
 $("#memoryFiles").innerHTML=f.songUrl?`<a href="${escapeHTML(f.songUrl)}" target="_blank" rel="noopener" class="btn small">Открыть музыку</a>`:"";
 $("#memoryModal").classList.add("open");
});
function openAuth(){switchAuth("login");$("#authModal").classList.add("open")}
function closeModal(id){$("#"+id).classList.remove("open")}
function switchAuth(mode){
 authMode=mode;
 $("#loginTab").classList.toggle("active",mode==="login");
 $("#registerTab").classList.toggle("active",mode==="register");
 $("#authTitle").textContent=mode==="login"?"Вход в аккаунт":"Создание аккаунта";
 $("#nameLabel").hidden=mode!=="register";
 $("#authName").hidden=mode!=="register";
 $("#authName").required=mode==="register";
 $("#authSubmit").textContent=mode==="login"?"Войти":"Зарегистрироваться";
 $("#authMessage").textContent="";
}
$("#authForm").addEventListener("submit",e=>{
 e.preventDefault();
 const email=$("#authEmail").value.trim().toLowerCase();
 const password=$("#authPassword").value;
 const users=JSON.parse(localStorage.getItem("ag_users")||"{}");
 if(authMode==="register"){
  const name=$("#authName").value.trim();
  if(!name){toast("Введите имя");return}
  if(users[email]){toast("Аккаунт уже существует");return}
  users[email]={name,email,password};
  localStorage.setItem("ag_users",JSON.stringify(users));
  currentUser={name,email};
 }else{
  if(!users[email]||users[email].password!==password){$("#authMessage").textContent="Неверная почта или пароль";return}
  currentUser={name:users[email].name,email};
 }
 localStorage.setItem("ag_user",JSON.stringify(currentUser));
 updateUser();closeModal("authModal");toast("Вы вошли в аккаунт");
});
function updateUser(){
 $("#userBox").innerHTML=currentUser?`<span style="font-weight:600;margin-right:12px">${escapeHTML(currentUser.name)}</span><button class="btn small" onclick="logout()">Выйти</button>`:`<button class="btn small" onclick="openAuth()">Войти</button>`;
}
function logout(){
 currentUser=null;localStorage.removeItem("ag_user");updateUser();toast("Вы вышли из аккаунта");
}
function toggleAI(){$("#aiPanel").classList.toggle("open")}
$("#aiButton").onclick=toggleAI;
$("#aiForm").addEventListener("submit",e=>{
 e.preventDefault();
 const value=$("#aiInput").value.trim();if(!value)return;
 addMessage(value,"user");$("#aiInput").value="";
 setTimeout(()=>addMessage(aiResponse(value),"bot"),300);
});
function addMessage(text,type){
 const div=document.createElement("div");div.className="message "+type;div.textContent=text;
 $("#aiMessages").appendChild(div);$("#aiMessages").scrollTop=$("#aiMessages").scrollHeight;
}
function aiResponse(text){
 const t=text.toLowerCase();
 if(t.includes("назван"))return "Для названия воспоминания используйте короткую фразу, которая передаёт главное событие или чувство дня. Например: «Момент вне времени», «Новый этап», «Тихий вечер».";
 if(t.includes("цвет")||t.includes("палитр"))return "Для спокойного дня подойдут холодные серо-голубые оттенки. Для активного и насыщенного дня — более контрастные синие и графитовые тона.";
 if(t.includes("настроен")||t.includes("эмоц"))return "Попробуйте выделить три главные эмоции дня. Они помогут точнее передать его атмосферу в описании и визуальном оформлении.";
 if(t.includes("музык")||t.includes("песн"))return "Музыка может стать эмоциональным фоном воспоминания. Укажите композицию, исполнителя и то, с каким событием она у вас ассоциируется.";
 if(t.includes("привет"))return "Здравствуйте! Я помогу оформить воспоминания, подобрать название и определить настроение.";
 return "Попробуйте описать основные события дня, эмоции и детали окружающей обстановки. Я помогу превратить их в цельное воспоминание. Также могу предложить название и цветовую палитру.";
}
document.querySelectorAll(".modal").forEach(m=>m.addEventListener("click",e=>{if(e.target===m)m.classList.remove("open")}));
initPalette();renderFolders();renderArchive();updateUser();
</script>
</body>
</html>
