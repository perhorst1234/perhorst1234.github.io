<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Self-Hosted Apps voor Familie</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
  <style>
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
      <li><a href="#" role="button">Help</a></li>
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
            <img src="https://iconduck.com/icons/14121/jellyfin" alt="Jellyfin">
            <h3>Jellyfin</h3>
            <a href="https://jellyfin.org" target="_blank">Open Jellyfin</a>
            <p>Username: user123 <br> Password: pass123</p>
          </div>
          <div class="app">
            <img src="https://iconduck.com/icons/252954/jellyseerr" alt="Jellyseerr">
            <h3>Jellyseerr</h3>
            <a href="https://github.com/Fallenbagel/jellyseerr" target="_blank">Open Jellyseerr</a>
            <p>Username: user456 <br> Password: pass456</p>
          </div>
          <div class="app">
            <img src="https://play-lh.googleusercontent.com/AlexTranImmichIcon=w240-h480-rw" alt="Immich">
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

  <footer class="container">
    <small><a href="#">Privacybeleid</a> • <a href="#">Contact</a></small>
  </footer>
</body>
</html>
