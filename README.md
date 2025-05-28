# Ex02 Commercial Website
## Date:

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
<!-- index.html (Home Page) -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GlowSkin - Home</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="logo">GlowSkin</div>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="login.html">Login</a></li>
        <li><a href="cart.html">Cart</a></li>
      </ul>
    </nav>
  </header>

  <section class="banner">
    <h1>Radiance in Every Drop</h1>
    <p>Shop our luxurious range of facial skincare products</p>
  </section>

  <section class="featured">
    <h2>Bestsellers</h2>
    <div class="products">
      <div class="product">
        <img src="serum.png" alt="Serum">
        <h3>Hydrating Serum</h3>
      </div>
      <div class="product">
        <img src="fox.png" alt="Moisturizer">
        <h3>Glow Moisturizer</h3>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 GlowSkin. All rights reserved.</p>
  </footer>
</body>
</html>
```
login.html
```
<!-- login.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login - GlowSkin</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="logo">GlowSkin</div>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="login.html">Login</a></li>
        <li><a href="cart.html">Cart</a></li>
      </ul>
    </nav>
  </header>

  <section class="login">
    <h1>Login</h1>
    <form action="#" method="post">
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required>

      <button type="submit">Login</button>
    </form>
  </section>
  <footer>
    <p>&copy; 2025 GlowSkin. All rights reserved.</p>
  </footer>
</body>
</html>

```
about.html
```
<!-- about.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About - GlowSkin</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="logo">GlowSkin</div>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="login.html">Login</a></li>
        <li><a href="cart.html">Cart</a></li>
      </ul>
    </nav>
  </header>
  <section class="about">
    <h1>About Us</h1>
    <p>GlowSkin is a luxury skincare brand focused on clean, cruelty-free ingredients to bring out your natural radiance. Our mission is to help you glow with confidence using high-quality, ethically sourced products.</p>
    <img src="ing.jpg" alt="Natural Ingredients">
  </section>
  <footer>
    <p>&copy; 2025 GlowSkin. All rights reserved.</p>
  </footer>
</body>
</html>
```
cart.html
```

<!-- cart.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cart - GlowSkin</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <div class="logo">GlowSkin</div>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="login.html">Login</a></li>
        <li><a href="cart.html">Cart</a></li>
      </ul>
    </nav>
  </header>
  <section class="cart">
    <h1>Your Cart</h1>
    <div class="cart-item">
      <p>Hydrating Serum - $30 <button>Remove</button></p>
    </div>
    <div class="cart-item">
      <p>Glow Moisturizer - $25 <button>Remove</button></p>
    </div>
    <p>Total: $55</p>
    <button>Proceed to Checkout</button>
  </section>
  <footer>
    <p>&copy; 2025 GlowSkin. All rights reserved.</p>
  </footer>
</body>
</html>
```
style.css
```

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #fffafc;
  color: #333;
}

header {
  background-color: #fce4ec;
  padding: 20px 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
  color: #e91e63;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
  margin: 0;
}

nav a {
  text-decoration: none;
  color: #e91e63;
  font-weight: 500;
}

nav a:hover {
  color: #ad1457;
}

.banner {
  background-image: url('ban.png');
  background-size: cover;
  background-position: center;
  text-align: center;
  padding: 100px 20px;
  color: white;
}

.banner h1 {
  font-size: 3rem;
  margin-bottom: 10px;
}

.banner p {
  font-size: 1.2rem;
}

.featured {
  padding: 60px 40px;
  text-align: center;
  background-color: #fff0f5;
}

.featured h2 {
  font-size: 2rem;
  margin-bottom: 20px;
}

.products {
  display: flex;
  gap: 40px;
  justify-content: center;
}

.product {
  background: white;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  width: 220px;
}

.product img {
  max-width: 100%;
  border-radius: 8px;
}

.about, .login, .cart {
  padding: 60px 40px;
  max-width: 700px;
  margin: auto;
  background-color: #fff0f5;
  border-radius: 10px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}

.about img {
  max-width: 100%;
  margin-top: 20px;
  border-radius: 8px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

input[type="email"],
input[type="password"] {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  background-color: #e91e63;
  color: white;
  padding: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background 0.3s;
}

button:hover {
  background-color: #d81b60;
}

.cart-item {
  background-color: #ffffff;
  padding: 15px;
  border-radius: 5px;
  margin-bottom: 10px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #fce4ec;
  color: #e91e63;
  margin-top: 40px;
}

```


## OUTPUT
![image](https://github.com/user-attachments/assets/042a13ee-38bb-427c-8dda-05f25ce85f20)
![image](https://github.com/user-attachments/assets/5361b77d-2df6-4339-9c8f-65df436b8c35)
![image](https://github.com/user-attachments/assets/c30b92e0-f213-485e-85e1-722cac3f2fd5)
![image](https://github.com/user-attachments/assets/1c77cf14-b420-46dc-933a-486bfed07591)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
