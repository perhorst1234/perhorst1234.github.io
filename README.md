<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Self-Hosted Apps voor Familie</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
  <style>
    body {
      background: linear-gradient(45deg, #fffacd, #ffefd5, #ffdab9);
      background-size: 600% 600%;
      animation: gradientAnimation 15s ease infinite;
    }

    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .app-container {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
      margin-top: 20px;
    }

    .app {
      text-align: center;
      flex: 1 1 calc(25% - 40px);
      max-width: calc(25% - 40px);
      min-width: 200px;
    }

    .app img {
      max-width: 100%;
      height: auto;
    }

    .app h3 {
      margin: 10px 0;
    }

    .app a {
      display: block;
      margin-top: 10px;
    }

    .modal {
      display: none;
      position: fixed;
      z-index: 1;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0,0,0,0.4);
    }

    .modal-content {
      background-color: #fefefe;
      margin: 15% auto;
      padding: 20px;
      border: 1px solid #888;
      width: 80%;
      max-width: 500px;
    }

    .close {
      color: #aaa;
      float: right;
      font-size: 28px;
      font-weight: bold;
    }

    .close:hover,
    .close:focus {
      color: black;
      text-decoration: none;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <nav class="container-fluid">
    <ul>
      <li><strong>Familie Apps</strong></li>
    </ul>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Contact</a></li>
      <li><a href="#" role="button" id="helpLink">Help</a></li>
    </ul>
  </nav>

  <main class="container">
    <div class="grid">
      <section>
        <hgroup>
          <h2>Overzicht van Self-Hosted Apps</h2>
          <h3>Klik op een app voor meer informatie</h3>
        </hgroup>
        <div class="app-container">
          <div class="app">
            <img src="jellyfin.png" alt="Jellyfin">
            <h3>Jellyfin</h3>
            <a href="https://jellyfin.org" target="_blank">Open Jellyfin</a>
            <p>Username: user12 <br> Password: pass123</p>
          </div>
          <div class="app">
            <img src="jellyseerr.png" alt="Jellyseerr">
            <h3>Jellyseerr</h3>
            <a href="https://github.com/Fallenbagel/jellyseerr" target="_blank">Open Jellyseerr</a>
            <p>Username: user456 <br> Password: pass456</p>
          </div>
          <div class="app">
            <img src="immich.png" alt="Immich">
            <h3>Immich</h3>
            <a href="https://immich.app" target="_blank">Open Immich</a>
            <p>Username: user789 <br> Password: pass789</p>
          </div>
          <div class="app">
            <img src="https://cdn-icons-png.flaticon.com/512/4943/4943821.png" alt="NAS Schermer42">
            <h3>NAS Schermer42</h3>
            <a href="#" target="_blank">Instructies voor NAS</a>
            <p>Username: nasuser <br> Password: naspass</p>
          </div>
        </div>
      </section>
    </div>
  </main>

  <div id="myModal" class="modal">
    <div class="modal-content">
      <span class="close">&times;</span>
      <p id="helpText">Help text goes here. You can edit this later.</p>
    </div>
  </div>

  <script>
    document.getElementById('helpLink').onclick = function() {
      document.getElementById('myModal').style.display = 'block';
    }

    document.getElementsByClassName('close')[0].onclick = function() {
      document.getElementById('myModal').style.display = 'none';
    }

    window.onclick = function(event) {
      if (event.target == document.getElementById('myModal')) {
        document.getElementById('myModal').style.display = 'none';
      }
    }
  </script>
</body>
</html>
