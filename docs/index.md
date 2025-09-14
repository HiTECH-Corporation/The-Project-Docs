# Welcome to The Project Docs
<style>
.custom-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1rem;
  margin: 0;
  padding: 0;
}

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

.card > a.card-link {
  display: flex;
  width: 100%;
  height: 100%;
  gap: 0.6rem;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: inherit !important;
}

.card:hover,
.card:focus-within {
  border-color: #0ea5e9;
  box-shadow: 0 8px 24px rgba(14,165,233,0.08);
  transform: translateY(-2px);
}

.icon-bg {
  width: 70%;
  max-width: 320px;
  height: 6.5rem;
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
  display: block;
  margin: 0 auto;
}

.zen-icon {
  background-image: url("https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12.svg");
}
.auth-icon {
  background-image: url("https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/AuthKit.svg");
}

[data-md-color-scheme="slate"] .zen-icon {
  background-image: url("https://cdn.jsdelivr.net/gh/HiTECH-Corporation/The-Project-Docs@latest/assets/zenOS-Nature12-dark.svg");
}

.card .title {
  margin-top: 0.35rem;
  font-weight: 700;
  font-size: 1rem;
  color: var(--md-sys-typography-on-surface);
}

ul, li { list-style: none; margin: 0; padding: 0; }

@media (max-width: 720px) {
  .custom-grid { grid-template-columns: 1fr; }
  .card { min-height: 140px; }
  .icon-bg { width: 60%; height: 5.5rem; }
}
</style>

<div class="custom-grid">

  <div class="card" role="group" aria-label="zenOS">
    <a class="card-link" href="/zenOS/" aria-label="Open zenOS docs">
      <span class="icon-bg zen-icon" aria-hidden="true"></span>
      <span class="title">zenOS</span>
    </a>
  </div>

  <div class="card" role="group" aria-label="AuthKit API">
    <a class="card-link" href="/AuthKit%20API/" aria-label="Open AuthKit API docs">
      <span class="icon-bg auth-icon" aria-hidden="true"></span>
      <span class="title">AuthKit API</span>
    </a>
  </div>

</div>
