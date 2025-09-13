# Welcome to The Project Docs

Highlights

<style>
/* grid base (targets mkdocs-material grid.cards structure) */
.grid.cards > ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  align-items: stretch;
}

/* each card container (li) */
.grid.cards > ul > li {
  border: 1px solid transparent;
  border-radius: 12px;
  padding: 1.25rem;
  display: flex;
  align-items: stretch;
  justify-content: center;
  text-align: center;
  transition: border-color .15s ease, box-shadow .15s ease, transform .08s ease;
  background: var(--md-surface-fill);
  min-height: 160px;
  overflow: hidden;
}

/* make the inner link fill the li so the whole box is clickable */
.grid.cards > ul > li > a.feature-link {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  width: 100%;
  height: 100%;
  color: inherit;
  text-decoration: none;
}

/* hover/focus on the li (or the link) */
.grid.cards > ul > li:hover,
.grid.cards > ul > li:focus-within {
  border-color: #0ea5e9;
  box-shadow: 0 8px 24px rgba(14,165,233,0.08);
  transform: translateY(-2px);
}

/* feature content */
.feature-card { display:flex; flex-direction:column; align-items:center; justify-content:center; gap:.4rem; width:100%; }

/* icon swap behavior (default show light, hide dark) */
.feature-icon .icon--dark { display: none; }
.feature-icon .icon--light { display: inline-block; }

/* swap when Material's theme is dark (slate) */
[data-md-color-scheme="slate"] .feature-icon .icon--dark { display:inline-block; }
[data-md-color-scheme="slate"] .feature-icon .icon--light { display:none; }

/* SVG sizing: ~70% of the card content width */
.feature-icon img {
  width: 70%;
  max-width: 260px;
  height: auto;
  display: block;
  margin: 0 auto;
  object-fit: contain;
}

/* title style under icon */
.feature-card strong {
  display: block;
  margin-top: 0.2rem;
  font-weight: 700;
  font-size: 1rem;
  color: var(--md-sys-typography-on-surface);
}

/* small-screen responsiveness */
@media (max-width: 520px) {
  .grid.cards > ul { grid-template-columns: 1fr; }
  .grid.cards > ul > li { min-height: 140px; }
  .feature-icon img { width: 60%; }
}
</style>

<div class="grid cards" markdown>
- <a class="feature-link" href="/zenOS/"><div class="feature-card">
    <span class="feature-icon">
      <img class="icon icon--light" src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12.svg" alt="zenOS (light)">
      <img class="icon icon--dark"  src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12-dark.svg"  alt="zenOS (dark)">
    </span>
    **zenOS**
  </div></a>
- <a class="feature-link" href="/AuthKit%20API/"><div class="feature-card">
    <span class="feature-icon">
      <!-- AuthKit: chỉ dùng 1 ảnh chung cho light & dark -->
      <img class="icon icon--light" src="https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/AuthKit.svg" alt="AuthKit">
    </span>
    **AuthKit API**
  </div></a>
</div>
