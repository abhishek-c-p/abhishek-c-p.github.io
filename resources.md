---
layout: page
title: Resources
permalink: /resources/
---

<div class="resources-grid">
  <a class="resource-card" href="/resources/physics-equations/">
    <div class="resource-card-title">Physics Equations</div>
    <div class="resource-card-subtitle">
      PHY 2130 / 2140 equation sheets, derivations, examples
    </div>
  </a>
</div>

<hr>

/* ===== Resources page footer-style contact block ===== */
.resources-contact-footer {
  margin-top: 3rem;
  padding: 2.5rem 1.5rem;
  background: #0f141a; /* dark panel */
  border-top: 1px solid rgba(255,255,255,0.06);
}

.rcf-wrap {
  max-width: 1100px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1.4fr 0.9fr; /* form wider than info */
  gap: 2.2rem;
  align-items: start;
}

/* Left form */
.rcf-form h2 {
  margin: 0 0 0.4rem 0;
  font-size: 1.9rem;
  letter-spacing: 1px;
  color: #fff2a8 !important; /* your H1 light yellow */
}
.rcf-sub {
  margin-bottom: 1.2rem;
  color: #c9d1d9;
  font-size: 0.98rem;
}

.rcf-form form input,
.rcf-form form textarea {
  width: 100%;
  background: #0b0d10;
  color: #e6edf3;
  border: 1px solid rgba(255,255,255,0.12);
  border-radius: 6px;
  padding: 0.85rem 0.9rem;
  font-size: 1rem;
  margin-bottom: 0.85rem;
  outline: none;
}

.rcf-form form input:focus,
.rcf-form form textarea:focus {
  border-color: #ff4fd8;
  box-shadow: 0 0 0 2px rgba(255,79,216,0.2);
}

.rcf-form form button {
  background: #ff4fd8;
  color: #0b0d10;
  font-weight: 900;
  border: none;
  border-radius: 6px;
  padding: 0.75rem 1.7rem;
  cursor: pointer;
  letter-spacing: 1px;
  transition: transform 0.08s ease, box-shadow 0.2s ease;
}

.rcf-form form button:hover {
  transform: translateY(-1px);
  box-shadow: 0 0 14px rgba(255,79,216,0.55);
}

/* Right info */
.rcf-info {
  color: #e6edf3;
}
.rcf-info h3 {
  margin-top: 0.25rem;
  color: #a9d6ff !important; /* your H2 light blue */
  font-size: 1.3rem;
}
.rcf-info a {
  color: #e6edf3;
  text-decoration: none;
}
.rcf-info a:hover {
  color: #a5bfff;
}

/* Social icons */
.rcf-socials {
  margin-top: 1rem;
  display: flex;
  gap: 0.9rem;
  font-size: 2rem;
}
.rcf-socials a {
  color: #e6edf3;
  opacity: 0.9;
  transition: color 0.2s ease, transform 0.1s ease;
}
.rcf-socials a:hover {
  color: #ff4fd8;
  transform: translateY(-2px);
}

/* Mobile */
@media (max-width: 800px) {
  .rcf-wrap {
    grid-template-columns: 1fr;
  }
}

