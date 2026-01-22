# Sparkn-Snack.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Spark N Snack is a subscription box experience designed to spark creativity and nourish faith. Each month, founders Gracie and Sabreana curate a joyful collection of DIY projects, journaling prompts, devotionals, and uplifting treats—helping users pause, create, and connect in a meaningful way. Perfect for anyone looking to combine fun, personal growth, and spiritual inspiration in their everyday life.">
<title>Spark N Snack | Spark Creativity. Nourish Faith.</title>

<!-- Google Fonts Handwritten -->
<link href="https://fonts.googleapis.com/css2?family=Amatic+SC:wght@700&family=Indie+Flower&display=swap" rel="stylesheet">

<style>
/* Base Styles */
* { margin:0; padding:0; box-sizing:border-box; font-family: 'Indie Flower', cursive; }
body { line-height:1.6; color:#333; background:#fff; }
a { text-decoration:none; color:inherit; }

/* Header / Hero */
header.hero {
  background: linear-gradient(135deg, #ff9933, #cc33ff);
  color:white;
  padding:2rem;
  text-align:center;
}
header .logo { font-family:'Amatic SC', cursive; font-size:3rem; margin-bottom:1rem; }
header h2 { font-size:2.5rem; margin-bottom:0.5rem; }
header p { font-size:1.2rem; margin-bottom:1rem; }
header .btn { background:white; color:#ff9933; padding:0.8rem 1.6rem; border-radius:30px; font-weight:bold; border:none; cursor:pointer; font-size:1rem; transition:0.3s; }
header .btn:hover { background:#ffcc66; }

/* Nav */
nav { display:flex; justify-content:center; gap:2rem; margin-bottom:1rem; }
nav a { color:white; font-weight:bold; }

/* Sections */
.section { padding:4rem 2rem; max-width:900px; margin:auto; }
.section h2 { text-align:center; font-family:'Amatic SC', cursive; font-size:2.2rem; margin-bottom:1.5rem; }
.section.alt { background:#f9f9f9; }

/* Boxes Cards */
.cards { display:grid; grid-template-columns:repeat(auto-fit, minmax(220px,1fr)); gap:1.5rem; }
.card { background:white; padding:1.5rem; border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1); text-align:center; }

/* Forms */
form { display:flex; flex-direction:column; gap:0.8rem; max-width:400px; margin:2rem auto; }
input, textarea { padding:0.6rem; border-radius:6px; border:1px solid #ccc; font-family:'Indie Flower', cursive; }
button.submit-btn { background:#cc33ff; color:white; padding:0.8rem; border:none; border-radius:25px; font-weight:bold; cursor:pointer; transition:0.3s; }
button.submit-btn:hover { background:#9933cc; }

/* Footer */
footer { background:#222; color:#aaa; text-align:center; padding:1rem; font-size:0.9rem; margin-top:2rem; }

/* Newsletter input group */
.newsletter { display:flex; gap:0.5rem; margin-top:1rem; flex-wrap:wrap; justify-content:center; }
.newsletter input { flex:1 1 auto; min-width:150px; }
.newsletter button { flex:0 0 auto; }
</style>
</head>
<body>

<header class="hero">
  <div class="logo">Spark N Snack</div>
  <nav>
    <a href="#about">About</a>
    <a href="#boxes">Boxes</a>
    <a href="#mission">Mission</a>
    <a href="#contact">Contact</a>
  </nav>
  <h2>Spark Creativity. Nourish Faith.</h2>
  <p>Each month, Gracie & Sabreana curate DIY projects, devotionals, journaling prompts, and uplifting treats.</p>
  <button class="btn" onclick="document.getElementById('boxes').scrollIntoView({behavior:'smooth'})">View Boxes</button>
</header>

<section id="about" class="section">
  <h2>About Spark N Snack</h2>
  <p style="text-align:center; max-width:700px; margin:auto;">
    Spark N Snack is a subscription box experience designed to spark creativity and nourish faith. Each month, founders Gracie and Sabreana curate a joyful collection of DIY projects, journaling prompts, devotionals, and uplifting treats—helping users pause, create, and connect in a meaningful way. Perfect for anyone looking to combine fun, personal growth, and spiritual inspiration in their everyday life.
  </p>
</section>

<section id="boxes" class="section alt">
  <h2>Our Box</h2>
  <div class="cards">
    <div class="card">
      <h3>Monthly Spark Box</h3>
      <p>DIY projects, devotionals, journaling prompts, and snacks delivered monthly.</p>
      <button class="submit-btn" onclick="window.open('https://www.paypal.com/paypalme/YOURLINK','_blank')">Subscribe / Shop</button>
    </div>
  </div>
  <h3 style="text-align:center; margin-top:2rem;">Join Our Newsletter</h3>
  <form class="newsletter" id="newsletterForm">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <button type="submit" class="submit-btn">Sign Up</button>
  </form>
  <p id="newsletterStatus" style="text-align:center; margin-top:0.5rem;"></p>
</section>

<section id="mission" class="section">
  <h2>Our Mission</h2>
  <p style="text-align:center; max-width:700px; margin:auto;">
    We believe small joys matter. Our mission is to remind people they are seen, loved, and worthy—one snack at a time.
  </p>
</section>

<section id="contact" class="section alt">
  <h2>Contact Us / Pre-Order</h2>
  <form id="contactForm">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <input type="text" placeholder="Shipping Address" required>
    <textarea placeholder="Your Message (optional)"></textarea>
    <button type="submit" class="submit-btn">Send Message</button>
  </form>
  <p id="contactStatus" style="text-align:center; margin-top:0.5rem;"></p>
</section>

<footer>
  <p>© 2026 Spark N Snack • Created by Gracie & Sabreana</p>
</footer>

<script>
// Newsletter form submission
document.getElementById("newsletterForm").addEventListener("submit", function(e){
  e.preventDefault();
  document.getElementById("newsletterStatus").textContent = "Thanks for signing up! Check your email soon.";
  this.reset();
});

// Contact / pre-order form
document.getElementById("contactForm").addEventListener("submit", function(e){
  e.preventDefault();
  document.getElementById("contactStatus").textContent = "Thanks for reaching out! We'll get back to you shortly.";
  this.reset();
});
</script>

</body>
</html>
