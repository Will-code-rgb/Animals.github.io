<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Animal Friends</title>
  <link rel="stylesheet" href="assets/css/styles.css" />
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <h1 class="site-title">Animal Friends</h1>
      <nav class="nav">
        <a href="#gallery">Gallery</a>
        <a href="#about">About</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container">
        <h2>Find your new best friend</h2>
        <p>Browse adoptable animals, learn about them, and get connected.</p>

        <div class="controls">
          <input id="search" type="search" placeholder="Search by name or species..." />
          <select id="filterSpecies">
            <option value="">All species</option>
          </select>
        </div>
      </div>
    </section>

    <section id="gallery" class="container gallery-section">
      <h3>Adoptable Animals</h3>
      <div id="cards" class="cards-grid" aria-live="polite"></div>
      <div id="noResults" class="no-results" hidden>No animals found.</div>
    </section>

    <section id="about" class="container about">
      <h3>About</h3>
      <p>This demo shows a simple static site that loads animal data from a JSON file and renders a responsive gallery. It uses vanilla JavaScript, CSS Grid, and progressive enhancement.</p>
    </section>
  </main>

  <!-- Modal -->
  <div id="modal" class="modal" aria-hidden="true">
    <div class="modal-dialog" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
      <button id="closeModal" class="modal-close" aria-label="Close">&times;</button>
      <div class="modal-content">
        <img id="modalImage" src="" alt="" />
        <div class="modal-body">
          <h4 id="modalTitle"></h4>
          <p id="modalSpeciesAge"></p>
          <p id="modalDesc"></p>
          <a id="contactLink" class="btn" href="#">Contact to adopt</a>
        </div>
      </div>
    </div>
  </div>

  <footer class="site-footer">
    <div class="container">
      <p>Built with ❤️ — Animal Friends Demo</p>
    </div>
  </footer>

  <script src="assets/js/script.js"></script>
</body>
</html>
