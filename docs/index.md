# Welcome to The Project Docs

Highlights

<style>
/* Grid: two equal columns on wide screens, one column on small screens */
.custom-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1rem;
  margin: 0;
  padding: 0;
}

/* Make sure ul/li (if any) have no bullets — we use plain divs, but keep safe rules */
.custom-grid * { box-sizing: border-box; }

/* Card (each box) */
.card {
  border: 1px solid transparent;
  border-radius: 12px;
  background: var(--md-surface-fill);
  min-height: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  transition: border-color .15s ease, box-shadow .15s ease, transform .08s ease;
  padding: 1.25rem;
}

/* Make entire card clickable: the link fills the card */
.card > a.card-link {
  display: flex;
  width: 100%;
  height: 100%;
  gap: 0.6rem;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: inherit !important; /* avoid blue link color */
}

/* Hover state: blue border */
.card:hover,
.card:focus-within {
  border-color: #0ea5e9;
  box-shadow: 0 8px 24px rgba(14,165,233,0.08);
  transform: translateY(-2px);
}

/* Icon sizing: scale to 70% of card inner width */
.card .icon {
  width: 70%;
  max-width: 320px; /* absolute cap if needed */
  height: auto;
  display: block;
  margin: 0 auto;
  object-fit: contain;
}

/* For icons we support light/dark by toggling which img is visible */
.icon--dark { display: none; }
.icon--light { display: block; }

/* When Material theme is dark (slate), show dark icons */
[data-md-color-scheme="slate"] .icon--dark { display: block; }
[data-md-color-scheme="slate"] .icon--light { display: none; }

/* Title */
.card .title {
  margin-top: 0.35rem;
  font-weight: 700;
  font-size: 1rem;
  color: var(--md-sys-typography-on-surface);
  line-height: 1;
}

/* Remove any default list markers if content accidentally rendered as list */
ul, li { list-style: none; margin: 0; padding: 0; }

/* Responsive: stack to single column on small screens */
@media (max-width: 720px) {
  .custom-grid { grid-template-columns: 1fr; }
  .card { min-height: 140px; }
  .card .icon { width: 60%; }
}
</style>

<div class="custom-grid">

  <!-- Card 1: zenOS -->
  <div class="card" role="group" aria-label="zenOS">
    <a class="card-link" href="/zenOS/" aria-label="Open zenOS docs">
      <span class="icon-wrap">
        <!-- light and dark versions (dark shows when data-md-color-scheme="slate") -->
        <img class="icon icon--light" src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12.svg" alt="zenOS">
        <img class="icon icon--dark"  src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12-dark.svg" alt="zenOS">
      </span>
      <span class="title">zenOS</span>
    </a>
  </div>

  <!-- Card 2: AuthKit (single image used for both themes) -->
  <div class="card" role="group" aria-label="AuthKit API">
    <a class="card-link" href="/AuthKit%20API/" aria-label="Open AuthKit API docs">
      <span class="icon-wrap">
        <!-- Only one image (used both for light & dark) -->
        <img class="icon" src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/AuthKit.svg" alt="AuthKit">
      </span>
      <span class="title">AuthKit API</span>
    </a>
  </div>

</div>
