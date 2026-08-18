# Ex02 Commercial Website
## Date:17/08/26

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lumina Interiors</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Header -->
  <header class="header">
    <div class="container navbar">
      <div class="logo">Lumina <span>Interiors</span></div>
      <nav>
        <ul class="nav-links">
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Products</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
          <li><a href="#account">Account</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <div class="container hero-flex">
      <div class="hero-text">
        <h1>Designing Spaces That Feel Like Home</h1>
        <p>We create timeless interiors that blend comfort, elegance and function for the modern lifestyle.</p>
        <div class="hero-buttons">
          <a href="#products" class="btn btn-primary">Explore Collection</a>
          <a href="#contact" class="btn btn-outline">Book Consultation</a>
        </div>
      </div>
      <div class="hero-image">
        <img src="images/hero.png" alt="Living room interior design">
      </div>
    </div>
  </section>

  <!-- Products Section -->
  <section class="products" id="products">
    <div class="container">
      <h2 class="section-title">Our Products</h2>
      <div class="product-grid">

        <div class="product-card">
          <img src="images/sofa.png" alt="Luxury sofa">
          <h3>Luxury Sofa</h3>
          <p>A premium sofa set designed for maximum comfort and style.</p>
          <span class="price">₹45,000</span>
          <button class="btn btn-primary">Add to Cart</button>
        </div>

        <div class="product-card">
          <img src="images/dining.png" alt="Dining collection">
          <h3>Dining Collection</h3>
          <p>Elegant dining sets crafted from premium quality wood.</p>
          <span class="price">₹38,500</span>
          <button class="btn btn-primary">Add to Cart</button>
        </div>

        <div class="product-card">
          <img src="images/bedroom.png" alt="Bedroom furniture">
          <h3>Bedroom Furniture</h3>
          <p>Cozy and modern bedroom furniture for a peaceful retreat.</p>
          <span class="price">₹52,000</span>
          <button class="btn btn-primary">Add to Cart</button>
        </div>

        <div class="product-card">
          <img src="images/decor.png" alt="Home decor items">
          <h3>Home Decor</h3>
          <p>Handpicked decor pieces to complete your living space.</p>
          <span class="price">₹5,200</span>
          <button class="btn btn-primary">Add to Cart</button>
        </div>

      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section class="services" id="services">
    <div class="container">
      <h2 class="section-title">Our Services</h2>
      <div class="service-grid">

        <div class="service-card">
          <div class="icon-placeholder">🛋️</div>
          <h3>Interior Design</h3>
          <p>Complete interior design solutions tailored to your personality and lifestyle.</p>
        </div>

        <div class="service-card">
          <div class="icon-placeholder">📐</div>
          <h3>Space Planning</h3>
          <p>Smart layout planning to make the best use of every corner of your home.</p>
        </div>

        <div class="service-card">
          <div class="icon-placeholder">🪑</div>
          <h3>Custom Furniture</h3>
          <p>Custom made furniture designed and built exactly to your requirements.</p>
        </div>

      </div>
    </div>
  </section>

  <!-- About Section -->
  <section class="about" id="about">
    <div class="container about-flex">
      <div class="about-image">
        <img src="images/about.png" alt="About Lumina Interiors">
      </div>
      <div class="about-text">
        <h2 class="section-title">About Us</h2>
        <p>Lumina Interiors has been helping homeowners transform their spaces into elegant, comfortable and functional interiors for over a decade. We believe great design should feel personal.</p>
        <h3>Our Mission</h3>
        <p>To craft beautiful, high quality interiors that reflect the individuality of every client.</p>
        <h3>Our Vision</h3>
        <p>To become a trusted name in luxury interior design known for quality and elegance.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="contact" id="contact">
    <div class="container contact-flex">
      <div class="contact-info">
        <h2 class="section-title">Contact Us</h2>
        <p><strong>Address:</strong> 12, Anna Nagar, Chennai, Tamil Nadu</p>
        <p><strong>Phone:</strong> +91 98765 43210</p>
        <p><strong>Email:</strong> contact@luminainteriors.com</p>
        <p><strong>Working Hours:</strong> Mon - Sat, 10:00 AM - 7:00 PM</p>
      </div>
      <div class="contact-form">
        <form action="#" method="post">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" placeholder="Enter your name" required>

          <label for="email">Email</label>
          <input type="email" id="email" name="email" placeholder="Enter your email" required>

          <label for="message">Message</label>
          <textarea id="message" name="message" rows="4" placeholder="Enter your message" required></textarea>

          <button type="submit" class="btn btn-primary">Submit</button>
        </form>
      </div>
    </div>
  </section>

  <!-- User Account Section -->
  <section class="account" id="account">
    <div class="container">
      <h2 class="section-title">Login to Your Account</h2>
      <div class="login-card">
        <form action="#" method="post">
          <label for="loginEmail">Email</label>
          <input type="email" id="loginEmail" name="loginEmail" placeholder="Enter your email" required>

          <label for="loginPassword">Password</label>
          <input type="password" id="loginPassword" name="loginPassword" placeholder="Enter your password" required>

          <div class="remember-forgot">
            <label><input type="checkbox" id="remember" name="remember"> Remember Me</label>
            <a href="#">Forgot Password?</a>
          </div>

          <button type="submit" class="btn btn-primary">Login</button>
          <p class="register-text">Don't have an account? <a href="#">Register</a></p>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="container footer-flex">
      <div class="footer-col">
        <h3>Quick Links</h3>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>

      <div class="footer-col">
        <h3>Products</h3>
        <ul>
          <li><a href="#products">Luxury Sofa</a></li>
          <li><a href="#products">Dining Collection</a></li>
          <li><a href="#products">Bedroom Furniture</a></li>
        </ul>
      </div>

      <div class="footer-col">
        <h3>Services</h3>
        <ul>
          <li><a href="#services">Interior Design</a></li>
          <li><a href="#services">Space Planning</a></li>
          <li><a href="#services">Custom Furniture</a></li>
        </ul>
      </div>

      <div class="footer-col">
        <h3>Contact Info</h3>
        <p>Chennai, Tamil Nadu</p>
        <p>+91 98765 43210</p>
        <p>contact@luminainteriors.com</p>
        <div class="social-icons">
          <a href="#">FB</a>
          <a href="#">IG</a>
          <a href="#">TW</a>
        </div>
      </div>
    </div>

    <div class="footer-bottom">
      <p>&copy; 2026 Lumina Interiors. All Rights Reserved.</p>
      <p>Jayani K | Register Number: 212224040134</p>
    </div>
  </footer>

</body>
</html>
```
style.css

```
/***** style.css *****/

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  background-color: #F8F5F0;
  color: #2E2E2E;
  line-height: 1.6;
}

.container {
  width: 90%;
  max-width: 1150px;
  margin: 0 auto;
}

h1, h2, h3 {
  font-weight: 600;
}

/* Buttons */
.btn {
  display: inline-block;
  padding: 10px 22px;
  border-radius: 6px;
  text-decoration: none;
  font-size: 15px;
  cursor: pointer;
  border: none;
  transition: background-color 0.3s ease;
}

.btn-primary {
  background-color: #8B5E3C;
  color: #FFFFFF;
}

.btn-primary:hover {
  background-color: #6f4a2f;
}

.btn-outline {
  background-color: transparent;
  color: #8B5E3C;
  border: 2px solid #8B5E3C;
}

.btn-outline:hover {
  background-color: #8B5E3C;
  color: #FFFFFF;
}

/* Header */
.header {
  background-color: #FFFFFF;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
  position: sticky;
  top: 0;
  z-index: 100;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 18px 0;
}

.logo {
  font-size: 22px;
  font-weight: 700;
  color: #2E2E2E;
}

.logo span {
  color: #8B5E3C;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 28px;
}

.nav-links a {
  text-decoration: none;
  color: #2E2E2E;
  font-size: 15px;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #8B5E3C;
}

/* Hero Section */
.hero {
  padding: 70px 0;
  background-color: #F8F5F0;
}

.hero-flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 30px;
}

.hero-text {
  flex: 1 1 450px;
}

.hero-text h1 {
  font-size: 40px;
  color: #2E2E2E;
  margin-bottom: 18px;
}

.hero-text p {
  font-size: 16px;
  color: #555;
  margin-bottom: 25px;
  max-width: 480px;
}

.hero-buttons {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}

.hero-image {
  flex: 1 1 400px;
  text-align: center;
}

.hero-image img {
  width: 100%;
  max-width: 500px;
  border-radius: 10px;
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
}

/* Section Title */
.section-title {
  text-align: center;
  font-size: 28px;
  margin-bottom: 40px;
  color: #2E2E2E;
}

/* Products Section */
.products {
  padding: 70px 0;
}

.product-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 25px;
  justify-content: center;
}

.product-card {
  background-color: #FFFFFF;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
  padding: 18px;
  width: 260px;
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 8px 18px rgba(0, 0, 0, 0.12);
}

.product-card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 12px;
}

.product-card h3 {
  font-size: 18px;
  margin-bottom: 8px;
}

.product-card p {
  font-size: 14px;
  color: #555;
  margin-bottom: 10px;
}

.price {
  display: block;
  font-weight: 600;
  color: #8B5E3C;
  margin-bottom: 12px;
}

/* Services Section */
.services {
  padding: 70px 0;
  background-color: #F1ECE4;
}

.service-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 25px;
  justify-content: center;
}

.service-card {
  background-color: #FFFFFF;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
  padding: 30px;
  width: 300px;
  text-align: center;
  transition: transform 0.3s ease;
}

.service-card:hover {
  transform: translateY(-6px);
}

.icon-placeholder {
  font-size: 36px;
  margin-bottom: 15px;
}

.service-card h3 {
  margin-bottom: 10px;
}

.service-card p {
  font-size: 14px;
  color: #555;
}

/* About Section */
.about {
  padding: 70px 0;
}

.about-flex {
  display: flex;
  align-items: center;
  gap: 40px;
  flex-wrap: wrap;
}

.about-image {
  flex: 1 1 400px;
  text-align: center;
}

.about-image img {
  width: 100%;
  max-width: 450px;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.about-text {
  flex: 1 1 400px;
}

.about-text h3 {
  margin-top: 15px;
  margin-bottom: 6px;
  color: #8B5E3C;
}

.about-text p {
  font-size: 15px;
  color: #444;
  margin-bottom: 10px;
}

/* Contact Section */
.contact {
  padding: 70px 0;
  background-color: #F1ECE4;
}

.contact-flex {
  display: flex;
  gap: 40px;
  flex-wrap: wrap;
}

.contact-info {
  flex: 1 1 350px;
}

.contact-info p {
  margin-bottom: 10px;
  font-size: 15px;
}

.contact-form {
  flex: 1 1 400px;
  background-color: #FFFFFF;
  padding: 25px;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
}

.contact-form form {
  display: flex;
  flex-direction: column;
}

.contact-form label {
  font-size: 14px;
  margin-bottom: 6px;
  margin-top: 10px;
  font-weight: 500;
}

.contact-form input,
.contact-form textarea {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-family: 'Poppins', sans-serif;
  font-size: 14px;
}

.contact-form button {
  margin-top: 18px;
  align-self: flex-start;
}

/* Account Section */
.account {
  padding: 70px 0;
}

.login-card {
  max-width: 400px;
  margin: 0 auto;
  background-color: #FFFFFF;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
}

.login-card form {
  display: flex;
  flex-direction: column;
}

.login-card label {
  font-size: 14px;
  margin-bottom: 6px;
  margin-top: 12px;
  font-weight: 500;
}

.login-card input[type="email"],
.login-card input[type="password"] {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-family: 'Poppins', sans-serif;
  font-size: 14px;
}

.remember-forgot {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 13px;
  margin-top: 14px;
}

.remember-forgot a {
  color: #8B5E3C;
  text-decoration: none;
}

.login-card button {
  margin-top: 20px;
}

.register-text {
  text-align: center;
  font-size: 14px;
  margin-top: 15px;
}

.register-text a {
  color: #8B5E3C;
  text-decoration: none;
  font-weight: 500;
}

/* Footer */
.footer {
  background-color: #2E2E2E;
  color: #F8F5F0;
  padding: 50px 0 20px;
}

.footer-flex {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: space-between;
}

.footer-col {
  flex: 1 1 220px;
}

.footer-col h3 {
  color: #C9A66B;
  margin-bottom: 15px;
  font-size: 17px;
}

.footer-col ul {
  list-style: none;
}

.footer-col ul li {
  margin-bottom: 8px;
}

.footer-col ul li a {
  color: #F8F5F0;
  text-decoration: none;
  font-size: 14px;
}

.footer-col ul li a:hover {
  color: #C9A66B;
}

.footer-col p {
  font-size: 14px;
  margin-bottom: 6px;
}

.social-icons {
  display: flex;
  gap: 12px;
  margin-top: 12px;
}

.social-icons a {
  color: #F8F5F0;
  text-decoration: none;
  border: 1px solid #F8F5F0;
  padding: 6px 10px;
  border-radius: 5px;
  font-size: 13px;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.social-icons a:hover {
  background-color: #C9A66B;
  color: #2E2E2E;
  border-color: #C9A66B;
}

.footer-bottom {
  text-align: center;
  border-top: 1px solid #444;
  margin-top: 35px;
  padding-top: 18px;
  font-size: 13px;
  color: #ccc;
}

/* Responsive */
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    gap: 12px;
  }

  .nav-links {
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
  }

  .hero-text h1 {
    font-size: 30px;
  }

  .hero-flex,
  .about-flex,
  .contact-flex {
    flex-direction: column;
    text-align: center;
  }

  .hero-buttons {
    justify-content: center;
  }

  .product-card,
  .service-card {
    width: 100%;
    max-width: 320px;
  }
}
```



## OUTPUT
<img width="1661" height="947" alt="image" src="https://github.com/user-attachments/assets/a13c8115-cd59-4812-b1dc-d0c3619280b9" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
