<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Selfhosted Apps</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
    <style>
        .app-icon {
            width: 100px;
            height: 100px;
        }
        .app-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            padding: 20px;
        }
        .app {
            text-align: center;
            margin: 20px;
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
            <li><strong>Selfhosted Apps</strong></li>
        </ul>
        <ul>
            <li><a href="#jellyfin">Jellyfin</a></li>
            <li><a href="#jellyseerr">Jellyseerr</a></li>
            <li><a href="#immich">Immich</a></li>
            <li><a href="#nas-schermer42">NAS Schermer42</a></li>
        </ul>
    </nav>
    <main class="container">
        <div class="app-container">
            <section id="jellyfin" class="app">
                <hgroup>
                    <h2>Jellyfin</h2>
                </hgroup>
                <figure>
                    <img src="https://iconduck.com/icons/14121/jellyfin" alt="Jellyfin Icon" class="app-icon">
                    <figcaption>
                        <a href="https://iconduck.com/icons/14121/jellyfin" target="_blank">Jellyfin</a>
                    </figcaption>
                </figure>
                <a href="https://jellyfin.org/" role="button">Go to Jellyfin</a>
            </section>

            <section id="jellyseerr" class="app">
                <hgroup>
                    <h2>Jellyseerr</h2>
                </hgroup>
                <figure>
                    <img src="https://iconduck.com/icons/252954/jellyseerr" alt="Jellyseerr Icon" class="app-icon">
                    <figcaption>
                        <a href="https://iconduck.com/icons/252954/jellyseerr" target="_blank">Jellyseerr</a>
                    </figcaption>
                </figure>
                <a href="https://jellyseerr.com/" role="button">Go to Jellyseerr</a>
            </section>

            <section id="immich" class="app">
                <hgroup>
                    <h2>Immich</h2>
                </hgroup>
                <figure>
                    <img src="https://play.google.com/store/apps/details?id=app.alextran.immich" alt="Immich Icon" class="app-icon">
                    <figcaption>
                        <a href="https://play.google.com/store/apps/details?id=app.alextran.immich" target="_blank">Immich</a>
                    </figcaption>
                </figure>
                <a href="https://immich.app/" role="button">Go to Immich</a>
            </section>

            <section id="nas-schermer42" class="app">
                <hgroup>
                    <h2>NAS Schermer42</h2>
                </hgroup>
                <figure>
                    <img src="https://www.flaticon.com/free-icon/nas_4943821" alt="NAS Icon" class="app-icon">
                    <figcaption>
                        <a href="https://www.flaticon.com/free-icon/nas_4943821" target="_blank">NAS Schermer42</a>
                    </figcaption>
                </figure>
                <a href="#" role="button" onclick="showInstructions()">Get Instructions</a>
            </section>
        </div>
    </main>
    <section aria-label="Subscribe example">
        <div class="container">
            <article>
                <hgroup>
                    <h2>Subscribe</h2>
                    <h3>Stay updated with our latest news</h3>
                </hgroup>
                <form class="grid">
                    <input type="text" id="firstname" name="firstname" placeholder="First Name" aria-label="First Name" required />
                    <input type="email" id="email" name="email" placeholder="Email" aria-label="Email" required />
                    <button type="submit" onclick="event.preventDefault()">Subscribe</button>
                </form>
            </article>
        </div>
    </section>
    <footer class="container">
        <small><a href="#">Privacy Policy</a> • <a href="#">Terms of Service</a></small>
    </footer>

    <script>
        function showInstructions() {
            alert("To access NAS Schermer42, follow these instructions:\n1. Connect to the network.\n2. Open your file explorer.\n3. Enter the address \\NAS-SCHERMER42.\n4. Use the provided username and password.");
        }
    </script>
</body>
</html>
