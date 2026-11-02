# Ex02 Commercial Website
## Date:02-11-2026
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

### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Balaji's Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Header -->
    <header>
        <h1>Balaji's Restaurant</h1>

        <nav>
            <a href="#home">Home</a>
            <a href="#menu">Menu</a>
            <a href="#about">About Us</a>
            <a href="#contact">Contact</a>
            <a href="#account">Login</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="home">
        <div>
            <h2>Welcome to Balaji's Restaurant</h2>
            <p>Enjoy Delicious Food with Amazing Taste!</p>
            <button onclick="location.href='#menu'">Explore Menu</button>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="menu">
        <h2>Our Special Menu</h2>

        <div class="food-container">

            <div class="food-card">
                <img src="img/burger.png" alt="Burger">
                <h3>Cheese Burger</h3>
                <p>Delicious burger with fresh vegetables and cheese.</p>
                <h4>₹149</h4>
            </div>

            <div class="food-card">
                <img src="img/Pizza.png" alt="Pizza">
                <h3>Italian Pizza</h3>
                <p>Freshly baked pizza with delicious toppings.</p>
                <h4>₹249</h4>
            </div>

            <div class="food-card">
                <img src="img/meals.png" alt="Restaurant food">
                <h3>Special Meals</h3>
                <p>Enjoy our delicious and traditional special meals.</p>
                <h4>₹199</h4>
            </div>

        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>
            Foodie's Restaurant provides delicious and freshly prepared
            food with excellent customer service. Our goal is to make
            every dining experience special and memorable.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: balajirestaurant@gmail.com</p>
        <p>Phone: +91 98765 43210</p>
        <p>Address: Hosur, Tamil Nadu, India</p>
    </section>

    <!-- User Account -->
    <section id="account" class="account">
        <h2>User Account</h2>
        <input type="text" placeholder="Enter Username">
        <input type="password" placeholder="Enter Password">
        <button type="button">Login</button>
    </section>

    <!-- Footer -->
    <footer>
        <p>Follow Us</p>
        <div class="social">
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.twitter.com/">Twitter</a>
        </div>

        <p>© 2026 Balaji's Restaurant. All Rights Reserved.</p>
    </footer>

</body>
</html>


```

style.css
```

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #fff8f0;
    color: #333;
}

/* Header */
header {
    background-color: #8b0000;
    color: white;
    padding: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

header h1 {
    font-size: 28px;
}

nav {
    display: flex;
    gap: 20px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: #ffd700;
    transition: 0.3s;
}

/* Home Section */
.home {
    height: 400px;
    background: linear-gradient(
        rgba(0,0,0,0.5),
        rgba(0,0,0,0.5)
    ),
    url("https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?w=1200");

    background-size: cover;
    background-position: center;

    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.home h2 {
    font-size: 40px;
    margin-bottom: 15px;
}

.home p {
    font-size: 20px;
    margin-bottom: 20px;
}

button {
    background-color: #ff4500;
    color: white;
    border: none;
    padding: 12px 25px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #8b0000;
    transition: 0.3s;
}

/* Menu Section */
.menu {
    padding: 40px 20px;
    text-align: center;
}

.menu h2 {
    font-size: 30px;
    color: #8b0000;
    margin-bottom: 30px;
}

.food-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 25px;
    flex-wrap: wrap;
}

.food-card {
    background-color: white;
    width: 280px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 4px 10px gray;
    transition: transform 0.3s;
}

.food-card:hover {
    transform: translateY(-10px);
}

.food-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.food-card h3 {
    color: #8b0000;
    margin: 12px 0;
}

.food-card p {
    margin-bottom: 10px;
}

.food-card h4 {
    color: #ff4500;
}

/* About Section */
.about {
    background-color: #ffe4c4;
    padding: 40px;
    text-align: center;
}

.about h2,
.contact h2,
.account h2 {
    color: #8b0000;
    margin-bottom: 20px;
}

.about p {
    max-width: 700px;
    margin: auto;
    line-height: 1.7;
}

/* Contact Section */
.contact {
    padding: 40px;
    text-align: center;
    line-height: 2;
}

/* User Account */
.account {
    background-color: #ffe4c4;
    padding: 40px;
    text-align: center;
}

.account input {
    display: block;
    width: 250px;
    padding: 12px;
    margin: 12px auto;
    border: 1px solid gray;
    border-radius: 5px;
}

/* Footer */
footer {
    background-color: #8b0000;
    color: white;
    text-align: center;
    padding: 25px;
}

.social {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin: 15px;
}

.social a {
    color: white;
    text-decoration: none;
}

.social a:hover {
    color: #ffd700;
}

/* Responsive Design */
@media (max-width: 600px) {
    header {
        flex-direction: column;
        gap: 15px;
    }

    nav {
        flex-wrap: wrap;
        justify-content: center;
    }

    .home h2 {
        font-size: 28px;
    }

    .food-container {
        flex-direction: column;
        align-items: center;
    }
}


```


## OUTPUT
![alt text](<Commercial Website/outputs/1.png>)
<br>

![alt text](<Commercial Website/outputs/4.png>)
<br>

![alt text](<Commercial Website/outputs/2.png>)
<br>

![alt text](<Commercial Website/outputs/3.png>)
<br>
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.