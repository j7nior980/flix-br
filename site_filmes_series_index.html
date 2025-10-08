<!--
  Projeto: Site de Filmes & Séries (index.html)
  Descrição: Página única com tema Dark/Light, layout responsivo estilo "Netflix",
  menu com navegação suave, login/cadastro (com opção convidado) e player sobreposto.
  Fonte: Poppins (Light e Bold)
  Paleta: #040D12 (escuro), #f3f3f3 (claro), #C63C51 (accent)

  Comentários em português explicam cada trecho do código para facilitar alterações.
-->

<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>StreamPlay — Filmes & Séries</title>

  <!-- Importa Poppins (300 = Light, 700 = Bold) -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;700&display=swap" rel="stylesheet">

  <!-- Meta theme colors -->
  <meta name="theme-color" content="#040D12" />

  <style>
    /* ----- Variáveis de tema e paleta ----- */
    :root{
      --bg-dark: #040D12;      /* cor primária escura */
      --bg-light: #f3f3f3;     /* cor primária clara */
      --accent: #C63C51;      /* cor de destaque */
      --muted: rgba(255,255,255,0.08);

      --pad: 18px;
      --radius: 12px;
      --max-width: 1200px;

      --ff: 'Poppins', system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }

    /* Tema escuro por padrão */
    html,body{
      height:100%;
      margin:0;
      font-family: var(--ff);
      background: var(--bg-dark);
      color: #fff;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      scroll-behavior: smooth; /* fallback para rolagem suave */
    }

    /* Tema claro (adiciona a classe .light no body para ativar) */
    body.light{
      background: var(--bg-light);
      color: #111;
    }

    /* ----- Header e Navegação ----- */
    header{
      position:sticky;
      top:0;
      backdrop-filter: blur(6px);
      z-index:1000;
      padding:10px 20px;
      box-shadow: 0 1px 0 rgba(0,0,0,0.2);
    }

    .nav{
      max-width: var(--max-width);
      margin: 0 auto;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:12px;
      cursor:pointer;
    }

    .logo{
      width:42px;
      height:42px;
      border-radius:8px;
      background: linear-gradient(135deg,var(--accent),#7a1b2a);
      display:flex;align-items:center;justify-content:center;font-weight:700;
      font-size:18px;color:#fff;
    }

    nav ul{
      list-style:none;padding:0;margin:0;display:flex;gap:18px;align-items:center;
    }

    nav a{
      text-decoration:none;color:inherit;font-weight:700;font-size:14px;opacity:0.95;
      padding:8px 10px;border-radius:8px;transition:background .18s, transform .12s;
    }
    nav a:hover{ transform:translateY(-2px); background:var(--muted); }

    .controls{display:flex;gap:8px;align-items:center}

    .btn{
      background:var(--accent);color:#fff;padding:8px 12px;border-radius:8px;border:0;cursor:pointer;font-weight:700;
    }
    .btn.ghost{ background:transparent;border:1px solid rgba(255,255,255,0.08); }

    /* Toggle de tema */
    .theme-toggle{ background:transparent;border:0;color:inherit;cursor:pointer;padding:6px;border-radius:8px; }

    /* ----- Hero / Carrossel simples ----- */
    .container{ max-width:var(--max-width);margin:24px auto;padding:0 16px; }

    .hero{
      display:grid;grid-template-columns:1fr;gap:16px;align-items:end;padding:18px;border-radius:16px;overflow:hidden;
      background: linear-gradient(90deg, rgba(0,0,0,0.45), transparent);
      min-height:260px;position:relative;
    }

    .hero .cover{ position:absolute; inset:0;background-image:url('https://images.unsplash.com/photo-1524985069026-dd778a71c7b4'); background-size:cover;background-position:center; filter:brightness(.45); }
    .hero .content{ position:relative; z-index:2; }
    .hero h1{ margin:0;font-size:28px;font-weight:700;letter-spacing:0.3px; }
    .hero p{ margin:8px 0 0 0; max-width:70%; line-height:1.4; }

    /* ----- Grades de filmes e cards ----- */
    .section{ margin:28px 0; }
    .section h2{ margin:0 0 14px 0; font-size:18px; font-weight:700; }

    .grid{
      display:grid;grid-template-columns: repeat(auto-fill,minmax(140px,1fr));gap:12px;
    }

    .card{
      border-radius:10px;overflow:hidden; cursor:pointer; position:relative; background:linear-gradient(180deg, rgba(0,0,0,0.16), rgba(0,0,0,0.35));
      transition: transform .18s, box-shadow .18s;
    }
    .card img{ width:100%; height:210px; object-fit:cover; display:block; }
    .card .meta{ padding:8px; font-size:13px; }
    .card:hover{ transform:translateY(-6px); box-shadow:0 10px 30px rgba(0,0,0,0.45); }

    /* Badge de play */
    .play-badge{ position:absolute;right:10px;bottom:8px;background:var(--accent);padding:6px 8px;border-radius:999px;font-weight:700;font-size:12px; }

    /* ----- Player overlay ----- */
    .overlay{ position:fixed; inset:0; display:none;align-items:center;justify-content:center;background:rgba(0,0,0,0.75); z-index:2000;padding:20px; }
    .overlay.open{ display:flex; }
    .player{
      width:100%; max-width:1000px; background: #000; border-radius:12px; overflow:hidden; position:relative;
    }
    .player video{ width:100%; height:auto; display:block; background:#000; }
    .player .close{ position:absolute; right:10px; top:10px; z-index:10; background:rgba(0,0,0,0.6); border:0;color:#fff;padding:8px 10px;border-radius:8px; cursor:pointer; }

    /* ----- Login / Cadastro modal ----- */
    .modal{ position:fixed; inset:0; display:none; align-items:center; justify-content:center; z-index:2100; background:rgba(0,0,0,0.6); }
    .modal.open{ display:flex; }
    .modal-card{ width:100%; max-width:420px; border-radius:12px; padding:18px; background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(0,0,0,0.35)); }

    .form-group{ margin-bottom:12px; }
    input[type="text"], input[type="email"], input[type="password"]{ width:100%; padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.08); background:transparent;color:inherit; }

    .small{ font-size:13px; opacity:0.85; }

    /* ----- Footer ----- */
    footer{ padding:28px 0; text-align:center; opacity:0.8; }

    /* ----- Responsividade ----- */
    @media (min-width:720px){
      .hero{ grid-template-columns: 2fr 1fr; min-height:340px; }
      .card img{ height:170px; }
    }

    @media (min-width:1000px){
      nav a{ font-size:15px; }
      .card img{ height:200px; }
    }

    /* Ajustes tema claro para elementos específicos */
    body.light .card{ background:linear-gradient(180deg, rgba(0,0,0,0.03), rgba(0,0,0,0.06)); }
    body.light .hero{ background: linear-gradient(90deg, rgba(255,255,255,0.02), transparent); }
    body.light nav a:hover{ background: rgba(0,0,0,0.04); }

  </style>
</head>
<body>

  <!-- Header com menu -->
  <header>
    <div class="nav">
      <div class="brand" onclick="scrollToSection('home')">
        <div class="logo">SP</div>
        <div>
          <div style="font-weight:700;">StreamPlay</div>
          <div style="font-size:12px;margin-top:2px;opacity:0.8;">Filmes • Séries</div>
        </div>
      </div>

      <nav>
        <ul>
          <li><a href="#home" data-target="home">Home</a></li>
          <li><a href="#filmes" data-target="filmes">Filmes</a></li>
          <li><a href="#series" data-target="series">Séries</a></li>
          <li><a href="#contato" data-target="contato">Contato</a></li>
          <li><a href="#discord" data-target="discord">Discord</a></li>
        </ul>
      </nav>

      <div class="controls">
        <button class="theme-toggle" id="themeBtn" title="Mudar tema">🌓</button>
        <button class="btn" id="openLogin">Entrar / Cadastrar</button>
      </div>
    </div>
  </header>

  <!-- Conteúdo principal -->
  <main class="container">

    <!-- HERO / DESTAQUE -->
    <section id="home" class="hero">
      <div class="cover" aria-hidden="true"></div>
      <div class="content">
        <h1>Bem-vindo ao StreamPlay</h1>
        <p>Encontre os melhores filmes e séries com interface moderna, modos Dark e Light, e um player sobreposto para assistir sem sair da página.</p>
        <div style="margin-top:12px;display:flex;gap:8px;">
          <button class="btn" onclick="document.getElementById('filmes').scrollIntoView({behavior:'smooth'})">Ver Filmes</button>
          <button class="btn ghost" onclick="document.getElementById('series').scrollIntoView({behavior:'smooth'})">Ver Séries</button>
        </div>
      </div>
    </section>

    <!-- Seção de filmes -->
    <section id="filmes" class="section">
      <h2>Filmes em Destaque</h2>
      <div class="grid" id="grid-filmes">
        <!-- Cards gerados via JavaScript. Cada card ao clicar abrirá o player sobreposto. -->
      </div>
    </section>

    <!-- Seção de séries -->
    <section id="series" class="section">
      <h2>Séries Populares</h2>
      <div class="grid" id="grid-series">
        <!-- Cards gerados via JavaScript -->
      </div>
    </section>

    <!-- Contato -->
    <section id="contato" class="section">
      <h2>Contato</h2>
      <p class="small">Envie sugestões, reportes de erros ou pedidos de títulos. Email: contato@streamplay.exemplo (placeholder)</p>
    </section>

    <!-- Discord -->
    <section id="discord" class="section">
      <h2>Discord</h2>
      <p class="small">Junte-se ao nosso servidor para discutir lançamentos e recomendações.</p>
      <a class="small" href="#" onclick="alert('Link do Discord placeholder')">Entrar no Discord</a>
    </section>

  </main>

  <footer>
    <div class="container">© <span id="ano"></span> StreamPlay. Todos os direitos reservados.</div>
  </footer>

  <!-- Player Overlay (aberto quando o usuário clica num card) -->
  <div id="overlay" class="overlay" role="dialog" aria-hidden="true">
    <div class="player" role="document">
      <button class="close" id="closePlayer">Fechar ✕</button>
      <!-- Vídeo: trocar src para o arquivo real; controls ativados para poder pausar/volume/etc -->
      <video id="videoPlayer" controls preload="metadata">
        <source id="videoSource" src="" type="video/mp4">
        Seu navegador não suporta vídeo HTML5.
      </video>
    </div>
  </div>

  <!-- Modal de Login/Cadastro -->
  <div id="modalLogin" class="modal" aria-hidden="true">
    <div class="modal-card">
      <h3 style="margin-top:0;">Entrar / Cadastrar</h3>
      <p class="small">Entre com sua conta ou use o modo convidado para navegar sem cadastro.</p>

      <div class="form-group">
        <input id="inputEmail" type="email" placeholder="Email (ex: voce@exemplo.com)">
      </div>
      <div class="form-group">
        <input id="inputPassword" type="password" placeholder="Senha">
      </div>

      <div style="display:flex;gap:8px;">
        <button class="btn" id="btnLogin">Entrar</button>
        <button class="btn ghost" id="btnGuest">Entrar como Convidado</button>
      </div>

      <div style="margin-top:12px;display:flex;justify-content:space-between;align-items:center;">
        <small class="small">Ainda não tem conta? <a href="#" onclick="alert('Fluxo de cadastro placeholder')">Cadastrar</a></small>
        <button class="btn" id="closeModal">Fechar</button>
      </div>
    </div>
  </div>

  <script>
    // ----- Dados de exemplo (substituir por API/back-end) -----
    // Cada item tem: id, title, thumb (imagem), src (vídeo placeholder)
    const filmes = [
      {id:1, title:'Aventura Noturna', thumb:'https://images.unsplash.com/photo-1502139214984-2d0c9d7891f3', src:'https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm'},
      {id:2, title:'Mistério Profundo', thumb:'https://images.unsplash.com/photo-1524985069026-dd778a71c7b4', src:'https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm'},
      {id:3, title:'Comédia Urbana', thumb:'https://images.unsplash.com/photo-1517604931442-7fefb1a58d16', src:'https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm'}
    ];

    const series = [
      {id:11, title:'Série: Alto Risco', thumb:'https://images.unsplash.com/photo-1542204165-1e2f2e6f8caa', src:'https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm'},
      {id:12, title:'Série: Laços', thumb:'https://images.unsplash.com/photo-1517607640852-1f1a0b1b4b5b', src:'https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.webm'}
    ];

    // ----- Funções utilitárias -----
    function $(sel){ return document.querySelector(sel); }
    function $$(sel){ return Array.from(document.querySelectorAll(sel)); }

    // Preenche os grids com cards
    function renderCards(){
      const gridF = $('#grid-filmes');
      const gridS = $('#grid-series');

      filmes.forEach(f => {
        const card = document.createElement('div'); card.className='card';
        card.innerHTML = `
          <img src="${f.thumb}" alt="${f.title}">
          <div class="meta"><strong>${f.title}</strong></div>
          <div class="play-badge">ASSISTIR</div>
        `;
        card.addEventListener('click', ()=> openPlayer(f));
        gridF.appendChild(card);
      });

      series.forEach(s => {
        const card = document.createElement('div'); card.className='card';
        card.innerHTML = `
          <img src="${s.thumb}" alt="${s.title}">
          <div class="meta"><strong>${s.title}</strong></div>
          <div class="play-badge">ASSISTIR</div>
        `;
        card.addEventListener('click', ()=> openPlayer(s));
        gridS.appendChild(card);
      });
    }

    // Abre o overlay do player e carrega o src do vídeo
    function openPlayer(item){
      const overlay = $('#overlay');
      const video = $('#videoPlayer');
      const source = $('#videoSource');

      // Mostra overlay
      overlay.classList.add('open');
      overlay.setAttribute('aria-hidden','false');

      // Ajusta fonte do vídeo (trocar src para vídeo real)
      source.src = item.src || '';
      video.load();
      video.play().catch(()=>{ /* autoplay pode falhar em alguns navegadores */ });
    }

    // Fecha o player
    function closePlayer(){
      const overlay = $('#overlay');
      const video = $('#videoPlayer');

      video.pause();
      video.currentTime = 0;
      overlay.classList.remove('open');
      overlay.setAttribute('aria-hidden','true');
    }

    // Navegação suave quando clicar nos links do menu
    document.querySelectorAll('nav a[data-target]').forEach(a => {
      a.addEventListener('click', (e)=>{
        e.preventDefault();
        const target = a.dataset.target;
        const el = document.getElementById(target);
        if(el) el.scrollIntoView({behavior:'smooth'});
      });
    });

    // ----- Login / Convidado (placeholder sem back-end) -----
    const modal = $('#modalLogin');
    $('#openLogin').addEventListener('click', ()=>{ modal.classList.add('open'); modal.setAttribute('aria-hidden','false'); });
    $('#closeModal').addEventListener('click', ()=>{ modal.classList.remove('open'); modal.setAttribute('aria-hidden','true'); });

    // Entrar (simulação simples) - aqui você conectaria ao back-end
    $('#btnLogin').addEventListener('click', ()=>{
      const email = $('#inputEmail').value.trim();
      if(!email){ alert('Digite um email válido (placeholder)'); return; }
      localStorage.setItem('streamplay_user', email);
      alert('Login simulado: ' + email);
      modal.classList.remove('open'); modal.setAttribute('aria-hidden','true');
    });

    // Convidado: salva flag no localStorage e fecha modal
    $('#btnGuest').addEventListener('click', ()=>{
      localStorage.setItem('streamplay_user','convidado');
      alert('Entrou como convidado');
      modal.classList.remove('open'); modal.setAttribute('aria-hidden','true');
    });

    // Fecha player quando clicar fora do player
    $('#overlay').addEventListener('click', (e)=>{ if(e.target.id === 'overlay') closePlayer(); });
    $('#closePlayer').addEventListener('click', closePlayer);

    // ----- Tema Dark/Light: salva preferência no localStorage -----
    const themeBtn = $('#themeBtn');
    function setTheme(light){
      if(light){ document.body.classList.add('light'); localStorage.setItem('streamplay_theme','light'); document.querySelector('meta[name=theme-color]').content = '#f3f3f3'; }
      else { document.body.classList.remove('light'); localStorage.setItem('streamplay_theme','dark'); document.querySelector('meta[name=theme-color]').content = '#040D12'; }
    }
    // Inicializa tema salvo
    (function(){
      const t = localStorage.getItem('streamplay_theme') || 'dark';
      setTheme(t==='light');
    })();

    themeBtn.addEventListener('click', ()=>{
      const isLight = document.body.classList.contains('light');
      setTheme(!isLight);
    });

    // ----- Utilitários adicionais -----
    // Preenche grids, atualiza ano do footer
    renderCards();
    document.getElementById('ano').textContent = new Date().getFullYear();

    // Função usada no clique da marca para rolar ao topo
    function scrollToSection(id){ document.getElementById(id).scrollIntoView({behavior:'smooth'}); }

    // Ajustes e dicas:
    // - Para integrar com um back-end, substitua os arrays `filmes` e `series` por uma chamada fetch() à API.
    // - Para adicionar legendas, forneça <track kind="subtitles" ...> no elemento <video>.
    // - Substitua os src dos vídeos por URLs reais ou por blobs streaming (HLS/DASH requer player adicional como hls.js).
    // - Os comentários no CSS e HTML ajudam a localizar onde alterar a paleta, fontes e comportamento.

  </script>

<!-- Painel Admin (visível apenas para o email autorizado) -->
<section id="painel-admin" class="section" style="display:none;">
  <h2>Painel Admin</h2>
  <p class="small">Gerencie filmes e séries disponíveis no site.</p>

  <form id="adminForm" style="max-width:500px;">
    <div class="form-group">
      <label>Nome do Filme/Série:</label>
      <input type="text" id="adminTitulo" placeholder="Ex: Vingadores: Ultimato" required />
    </div>

    <div class="form-group">
      <label>Descrição:</label>
      <textarea id="adminDescricao" placeholder="Breve descrição do filme ou série" rows="4"
        style="width:100%;border-radius:8px;border:1px solid rgba(255,255,255,0.08);background:transparent;color:inherit;padding:10px;"></textarea>
    </div>

    <div class="form-group">
      <label>Upload do Arquivo:</label>
      <input type="file" id="adminArquivo" accept="video/*" required />
    </div>

    <div class="form-group">
      <label>Categoria:</label>
      <select id="adminCategoria"
        style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.08);background:transparent;color:inherit;">
        <option value="filme">Filme</option>
        <option value="serie">Série</option>
      </select>
    </div>

    <button type="submit" class="btn">Enviar</button>
  </form>

  <div id="listaUploads" style="margin-top:20px;">
    <h3>Uploads Recentes</h3>
    <ul id="uploadsList" style="list-style:none;padding:0;margin:0;"></ul>
  </div>
</section>

<script>
  // ----- Configuração do admin -----
  const EMAIL_ADMIN = "j7niorp123@gmail.com"; // email autorizado
  const painel = document.getElementById('painel-admin');
  const form = document.getElementById('adminForm');
  const uploadsList = document.getElementById('uploadsList');

  // ----- Mostra botão "Painel Admin" no menu apenas para admin -----
  function showAdminButton() {
    const navList = document.querySelector('nav ul');
    if (!document.getElementById('btnAdmin')) {
      const li = document.createElement('li');
      li.innerHTML = '<a id="btnAdmin" href="#painel-admin" data-target="painel-admin">Painel Admin</a>';
      navList.appendChild(li);
    }
  }

  // ----- Verifica login salvo -----
  const usuarioAtual = localStorage.getItem('streamplay_user');

  if (usuarioAtual === EMAIL_ADMIN) {
    painel.style.display = 'block';
    showAdminButton();
  } else {
    console.log("Painel admin oculto (usuário comum ou convidado)");
  }

  // ----- Uploads locais -----
  const uploads = JSON.parse(localStorage.getItem('streamplay_uploads') || '[]');
  renderUploads();

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    const titulo = document.getElementById('adminTitulo').value.trim();
    const descricao = document.getElementById('adminDescricao').value.trim();
    const categoria = document.getElementById('adminCategoria').value;
    const arquivo = document.getElementById('adminArquivo').files[0];

    if (!arquivo) {
      alert('Selecione um arquivo de vídeo.');
      return;
    }

    const novoUpload = {
      id: Date.now(),
      titulo,
      descricao,
      categoria,
      arquivo: arquivo.name
    };

    uploads.push(novoUpload);
    localStorage.setItem('streamplay_uploads', JSON.stringify(uploads));
    renderUploads();
    form.reset();
    alert('Upload salvo localmente!');
  });

  function renderUploads() {
    uploadsList.innerHTML = '';
    uploads.forEach(item => {
      const li = document.createElement('li');
      li.innerHTML = `
        <div style="margin-bottom:8px;padding:10px;border-radius:8px;background:rgba(255,255,255,0.05);">
          <strong>${item.titulo}</strong> (${item.categoria})<br>
          <span style="opacity:0.8;">${item.descricao}</span><br>
          <small>Arquivo: ${item.arquivo}</small>
        </div>
      `;
      uploadsList.appendChild(li);
    });
  }
</script>

</body>
</html>
