# Eclipse-studio-website
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Eclipse Studio | Creative Agency</title>
<style>
  /* Reset and base */
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #0a0a0a;
    color: #eee;
  }
  a {
    color: #00aaff;
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
  }
  html {
    scroll-behavior: smooth;
  }

  /* Navigation */
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 40px;
    background: #111;
    position: sticky;
    top: 0;
    z-index: 100;
  }
  nav .logo {
    font-weight: 900;
    font-size: 1.8rem;
    letter-spacing: 2px;
    color: #00aaff;
  }
  nav ul {
    list-style: none;
    display: flex;
    gap: 30px;
    margin: 0;
    padding: 0;
  }
  nav ul li a {
    color: #eee;
    font-size: 1rem;
    transition: color 0.3s ease;
  }
  nav ul li a:hover {
    color: #00aaff;
  }

  /* Hero Section */
  .hero {
    position: relative;
    height: 80vh;
    background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1470&q=80') center center/cover no-repeat;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
  }
  .hero::after {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(0,0,0,0.7);
  }
  .hero-content {
    position: relative;
    z-index: 1;
    max-width: 900px;
  }
  .hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 20px;
    font-weight: 900;
    color: #00aaff;
  }
  .hero-content p {
    font-size: 1.3rem;
    margin-bottom: 30px;
    color: #ccc;
  }
  .hero-content a.btn {
    background: #00aaff;
    color: #111;
    padding: 15px 40px;
    font-weight: 700;
    border-radius: 30px;
    text-transform: uppercase;
    transition: background 0.3s ease;
    display: inline-block;
  }
  .hero-content a.btn:hover {
    background: #0088cc;
  }

/* Stats Section */
  .stats {
    display: flex;
    justify-content: center;
    gap: 60px;
    background: #111;
    padding: 40px 20px;
    text-align: center;
}
  .stat-item {
    flex: 1;
    max-width: 180px;
  }
  .stat-icon {
    font-size: 3rem;
    color: #00aaff;
    margin-bottom: 10px;
  }
  .stat-number {
    font-size: 2.5rem;
    font-weight: 900;
    color: #00aaff;
  }
  .stat-label {
    font-size: 1rem;
    color: #aaa;
    margin-top: 5px;
    text-transform: uppercase;
    letter-spacing: 1.5px;
  }
  /* Services */
  .services {
    max-width: 1100px;
    margin: 60px auto;
    padding: 0 20px;
  }
  .services h2 {
    text-align: center;
    font-size: 2.8rem;
    margin-bottom: 40px;
    color: #00aaff;
  }
  .service-list {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
    gap: 30px;
  }
  .service-card {
    background: #111;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 0 15px rgba(0,170,255,0.3);
    transition: transform 0.3s ease;
  }
  .service-card:hover {
    transform: translateY(-10px);
  }
  .service-image {
    width: 100%;
    height: 180px;
    object-fit: cover;
    display: block;
  }
  .service-content {
    padding: 20px;
  }
  .service-title {
    font-size: 1.4rem;
    font-weight: 700;
    margin-bottom: 10px;
    color: #00aaff;
  }
  .service-price {
    font-weight: 900;
    font-size: 1.2rem;
    margin-bottom: 15px;
    color: #00ccff;
  }
  .service-btn {
    display: inline-block;
    background: #00aaff;
    color: #111;
    padding: 10px 25px;
    border-radius: 30px;
    font-weight: 700;
    text-transform: uppercase;
    transition: background 0.3s ease;
  }
  .service-btn:hover {
    background: #0088cc;
  }

  /* About */
  .about {
    max-width: 900px;
    margin: 80px auto 60px;
    padding: 0 20px;
    color: #ccc;
    text-align: center;
  }
  .about h2 {
    font-size: 2.8rem;
    margin-bottom: 30px;
    color: #00aaff;
  }

  /* Footer */
  footer {
    background: #111;
    padding: 20px;
    text-align: center;
    color: #aaa;
  }
/* Testimonial */
  .testimonial {
    max-width: 700px;
    margin: 60px auto 80px;
    background: #00aaff;
    color: #111;
    padding: 30px 40px;
    border-radius: 12px;
    font-style: italic;
    font-size: 1.3rem;
    text-align: center;
    box-shadow: 0 0 20px #00aaffaa;
  }

  footer a {
    margin: 0 10px;
    font-size: 1.2rem;
    color: #00aaff;
  }
/* Responsive */
  @media (max-width: 600px) {
    .hero-content h1 {
      font-size: 2.2rem;
    }
    .hero-content p {
      font-size: 1rem;
    }
    nav ul {
      gap: 15px;
    }
</style>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />
</head>
<body>
  <!-- Nav -->
  <nav>
    <div class="logo">Eclipse Studio</div>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-content">
      <h1>Eclipsing Ordinary</h1>
      <p>We capture creativity and transform ideas into stunning visual stories.</p>
     
    </div>
  </section>

<section class="stats" aria-label="Company statistics">
  <div class="stat-item">
    <div class="stat-icon"><i class="fas fa-users"></i></div>
    <div class="stat-number">50+</div>
    <div class="stat-label">Happy Clients</div>
  </div>
  <div class="stat-item">
    <div class="stat-icon"><i class="fas fa-globe"></i></div>
    <div class="stat-number">03+</div>
    <div class="stat-label">Countries Served</div>
  </div>
  <div class="stat-item">
    <div class="stat-icon"><i class="fas fa-briefcase"></i></div>
    <div class="stat-number">5+</div>
    <div class="stat-label">Years Experience</div>
  </div>
</section>

<section id="services" class="services" aria-label="Our services">
 <h2>Our Services</h2>
 <div class="service-list"> 
<article class="service-card">
 <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=600&q=80" alt="Brand Identity Design" class="service-image" />
 <div class="service-content"> 
<h3 class="service-title">Brand Identity Design</h3>
 <div class="service-price">₨ 55,000</div> 

</div> 

</article>
 <article class="service-card">
 <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=600&q=80" alt="Digital Marketing" class="service-image" />
 <div class="service-content"> 
<h3 class="service-title">Digital Marketing</h3>
 <div class="service-price">₨ 55,000</div> 

 </div>
 </article> 

<article class="service-card"> 
<img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=600&q=80" alt="Video Production" class="service-image" /> 
<div class="service-content"> <h3 class="service-title">Video Production</h3> 
<div class="service-price">₨ 55,000</div> 
</div> 
</article>

 <article class="service-card"> <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=600&q=80" alt="Photography" class="service-image" /> 
<div class="service-content"> <h3 class="service-title">Photography</h3>
 <div class="service-price">₨ 45,000</div> 

</div> 
</article>

 <article class="service-card"> <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=600&q=80" alt="Social Media Management" class="service-image" />
 <div class="service-content"> 
<h3 class="service-title">Social Media Management</h3> 
<div class="service-price">₨ 45,000</div> 

</div>
 </article>

 <article class="service-card">
 <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=600&q=80" alt="Content Creation" class="service-image" /> 
<div class="service-content">
 <h3 class="service-title">Content Creation</h3> 
<div class="service-price">₨ 45,000</div> 

</div> 
</article>

 <article class="service-card"> <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=600&q=80" alt="SEO Optimization" class="service-image" />
 <div class="service-content"> <h3 class="service-title">SEO Optimization</h3>
 <div class="service-price">₨ 45,000</div> 

</div>
 </article> 
</div>
 </section>

<section id="about" class="about" aria-label="About Eclipse Studio">
  <h2>About Eclipse Studio</h2>
  <p>
    Welcome to Eclipse Studio, your premier creative agency dedicated to delivering high-quality design, development, and marketing solutions. We cater to startups, established businesses, and professionals seeking to elevate their brand presence. Our team pledges excellence, creativity, and client satisfaction with every project.
  </p>
  <p>
    From branding and website development to digital marketing and content creation, Eclipse Studio offers a comprehensive suite of services tailored to your unique needs. Trust us to bring your vision to life with authenticity and precision.
  </p>
</section>

<section class="testimonial" aria-label="Client testimonial">
  <p>"I trust the performance that Eclipse Studio provided — no issues, exceptional creativity and professionalism."</p>
</section>

<!-- Contact Section -->
<section id="contact" style="display: flex; justify-content: space-between; align-items: flex-start; gap: 600px; padding: 40px; background: #111; color: #eee;">

  <!-- Contact Information (Left) -->
  <div style="flex: 1;">
    <h2>Contact Information</h2>
    <p><i class="fas fa-map-marker-alt"></i> Office Address: FF 244, First Floor, Deans Trade Center, Saddar, Peshawar, Pakistan</p>
    <p><i class="fas fa-phone-alt"></i> Phone: <a href="tel:+923259712403" style="color:#00aaff;">+92 32 5971 2403</a></p>
    <p><i class="fas fa-envelope"></i> Email: <a href="mailto:eclipsestudio@gmail.com" style="color:#00aaff;">eclipsestudio@gmail.com</a></p>
  </div>

  <!-- Contact Form (Right) -->
  <div style="flex: 1;">
    <h2>Contact Us</h2>
    <p>Let’s bring your vision to life! Reach out today.</p>
    <form>
      <input type="text" placeholder="Your Name" required style="width:100%; padding:10px; margin-bottom:15px; border-radius:5px; border:none;" />
      <input type="email" placeholder="Your Email" required style="width:100%; padding:10px; margin-bottom:15px; border-radius:5px; border:none;" />
      <textarea placeholder="Your Message" required style="width:100%; padding:10px; margin-bottom:15px; border-radius:5px; border:none; height:120px;"></textarea>
      <button type="submit" style="background:#00aaff; color:#111; padding:12px 25px; border:none; border-radius:30px; font-weight:bold; cursor:pointer;">Send</button>
    </form>
  </div>

</section>


  <!-- Footer -->
  <footer>
    <p>© 2025 Eclipse Studio. All rights reserved.</p>
    <p>
      <a href="https://facebook.com/eclipse.studio" aria-label="Facebook" target="_blank" rel="noopener"><i class="fab fa-facebook-f"></i></a>
      <!-- ✅ Instagram fixed -->
      <a href="https://www.instagram.com/eclipse_studios00/" aria-label="Instagram" target="_blank" rel="noopener"><i class="fab fa-instagram"></i></a>
    </p>
  </footer>
</body>
</html>
