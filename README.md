<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Larokee Lights | Cinematic Nature Photography</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- SEO -->
<meta name="description" content="Larokee Lights – Cinematic nature & landscape photography capturing light, mood, and atmosphere.">
<meta name="keywords" content="Photography, Nature Photography, Landscape, Cinematic, Larokee Lights">

<!-- Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>
:root {
  --bg: #070707;
  --text: #f5f5f5;
  --accent: #d4af37;
  --muted: #9ca3af;
  --card: #111;
}

.light {
  --bg: #f9fafb;
  --text: #0a0a0a;
  --card: #ffffff;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: "Poppins", sans-serif;
  transition: background .4s, color .4s;
}

/* Header */
header {
  position: fixed;
  width: 100%;
  top: 0;
  background: rgba(0,0,0,.6);
  backdrop-filter: blur(12px);
  z-index: 1000;
}

nav {
  max-width: 1200px;
  margin: auto;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-family: "Playfair Display", serif;
  font-size: 1.6rem;
  color: var(--accent);
}

nav a {
  color: var(--text);
  text-decoration: none;
  margin-left: 2rem;
  font-size: .9rem;
}

nav a:hover {
  color: var(--accent);
}

.toggle {
  cursor: pointer;
  border: 1px solid var(--accent);
  padding: .3rem .8rem;
  border-radius: 20px;
  font-size: .8rem;
  color: var(--accent);
}

/* Sections */
section {
  padding: 7rem 2rem;
  max-width: 1200px;
  margin: auto;
}

/* Hero */
.hero {
  height: 100vh;
  background:
    linear-gradient(rgba(0,0,0,.75), rgba(0,0,0,.75)),
    url("https://images.unsplash.com/photo-1501785888041-af3ef285b470?q=80&w=1600")
    center/cover;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.hero h1 {
  font-family: "Playfair Display", serif;
  font-size: 4rem;
}

.hero p {
  color: var(--muted);
  max-width: 600px;
  margin: 1rem auto;
}

/* About */
.about p {
  max-width: 700px;
  margin: auto;
  text-align: center;
  color: var(--muted);
}

/* Gallery */
.gallery {
  columns: 3 280px;
  column-gap: 1.2rem;
}

.gallery img {
  width: 100%;
  margin-bottom: 1.2rem;
  border-radius: 12px;
  cursor: pointer;
  transition: transform .4s, filter .4s;
}

.gallery img:hover {
  transform: scale(1.03);
  filter: brightness(1.1);
}

/* Lightbox */
.lightbox {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,.95);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 3000;
}

.lightbox img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 12px;
}

.lightbox.active {
  display: flex;
}

/* Testimonials */
.testimonials {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
  gap: 1.5rem;
}

.quote {
  background: var(--card);
  padding: 1.5rem;
  border-radius: 14px;
  font-style: italic;
}

/* Pricing */
.pricing {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
  gap: 2rem;
}

.plan {
  background: var(--card);
  padding: 2rem;
  border-radius: 16px;
  text-align: center;
}

.plan h3 {
  font-family: "Playfair Display", serif;
}

.price {
  font-size: 2rem;
  color: var(--accent);
  margin: 1rem 0;
}

/* Contact */
form {
  max-width: 500px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

input, textarea {
  padding: .8rem;
  border-radius: 8px;
  border: none;
}

button {
  padding: .8rem;
  background: var(--accent);
  border: none;
  cursor: pointer;
  font-weight: 600;
}

footer {
  text-align: center;
  padding: 2rem;
  color: var(--muted);
}
</style>
</head>

<body>

<header>
<nav>
  <div class="logo">Larokee Lights</div>
  <div>
    <a href="#about">About</a>
    <a href="#gallery">Gallery</a>
    <a href="#pricing">Bookings</a>
    <a href="#contact">Contact</a>
    <span class="toggle" id="modeToggle">Light</span>
  </div>
</nav>
</header>

<section class="hero">
  <div>
    <h1>Larokee Lights</h1>
    <p>Cinematic nature photography — capturing atmosphere, silence, and light.</p>
  </div>
</section>

<section id="about" class="about">
  <h2 style="text-align:center;">About</h2>
  <p>
    Larokee Lights is a cinematic nature photography brand focused on landscapes,
    natural light, and atmospheric storytelling.
  </p>
</section>

<section id="gallery">
  <h2 style="text-align:center;margin-bottom:2rem;">Gallery</h2>
  <div class="gallery">
    <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?q=80&w=800">
    <img src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?q=80&w=800">
    <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?q=80&w=800">
    <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?q=80&w=800">
    <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?q=80&w=800">
    <img src="https://images.unsplash.com/photo-1426604966848-d7adac402bff?q=80&w=800">
  </div>
</section>

<section>
  <h2 style="text-align:center;margin-bottom:2rem;">Testimonials</h2>
  <div class="testimonials">
    <div class="quote">“The atmosphere in these images is unreal.”</div>
    <div class="quote">“Larokee Lights captures silence and scale perfectly.”</div>
    <div class="quote">“Every photo feels like a film still.”</div>
  </div>
</section>

<section id="pricing">
  <h2 style="text-align:center;margin-bottom:2rem;">Bookings</h2>
  <div class="pricing">
    <div class="plan">
      <h3>Print License</h3>
      <p class="price">$150</p>
      <p>High-resolution nature prints</p>
    </div>
    <div class="plan">
      <h3>Commercial Use</h3>
      <p class="price">$450</p>
      <p>Brand & publication licensing</p>
    </div>
    <div class="plan">
      <h3>Exclusive Rights</h3>
      <p class="price">$900</p>
      <p>Full ownership & exclusivity</p>
    </div>
  </div>
</section>

<section id="contact">
  <h2 style="text-align:center;">Contact</h2>
  <form id="contactForm">
    <input placeholder="Name" required>
    <input type="email" placeholder="Email" required>
    <textarea rows="4" placeholder="Message" required></textarea>
    <button>Send</button>
  </form>
</section>

<footer>
© 2026 Larokee Lights — Cinematic Nature Photography
</footer>

<div class="lightbox" id="lightbox"><img></div>

<script>
/* Lightbox */
const imgs = document.querySelectorAll(".gallery img");
const box = document.getElementById("lightbox");
const boxImg = box.querySelector("img");

imgs.forEach(img => {
  img.onclick = () => {
    boxImg.src = img.src;
    box.classList.add("active");
  };
});

box.onclick = () => box.classList.remove("active");

/* Dark / Light Mode */
const toggle = document.getElementById("modeToggle");
const body = document.body;

if(localStorage.mode === "light") {
  body.classList.add("light");
  toggle.textContent = "Dark";
}

toggle.onclick = () => {
  body.classList.toggle("light");
  const light = body.classList.contains("light");
  localStorage.mode = light ? "light" : "dark";
  toggle.textContent = light ? "Dark" : "Light";
};

/* Contact */
document.getElementById("contactForm").onsubmit = e => {
  e.preventDefault();
  alert("🌲 Message sent. We'll be in touch.");
  e.target.reset();
};
</script>

</body>
</html>
