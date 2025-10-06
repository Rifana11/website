# Ex.07 Restaurant Website
# Date:04.10.25
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
#style.css

:root {
    --primary-color: #39012e; 
    --secondary-color: black; 
    --background-color: #8a0f63; 
    --text-color: #333333; 
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: var(--background-color);
    color: var(--text-color);
}

header {
    background-color: var(--primary-color);
    color: rgb(255, 255, 255);
    padding: 20px 0;
    text-align: center;
    border-bottom: 5px solid var(--secondary-color);
}

header h1 {
    margin: 0;
    font-size: 2.5em;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 5px;
    transition: background-color 0.3s;
}

nav ul li a:hover {
    background-color: rgba(255, 255, 255, 0.2);
}

main {
    padding: 20px;
    max-width: 1200px;
    margin: 20px auto;
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h2 {
    color: var(--primary-color);
    border-bottom: 2px solid var(--secondary-color);
    padding-bottom: 5px;
}

footer {
    background-color: var(--primary-color);
    color: white;
    text-align: center;
    padding: 10px;
    margin-top: 20px;
    font-size: 0.9em;
}

.section {
    margin-bottom: 30px;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.menu-item {
    border: 1px solid #ccc;
    padding: 15px;
    border-radius: 5px;
    text-align: center;
}

.menu-item h4 {
    color: var(--primary-color);
    margin-top: 0;
}

.admin-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
}

.admin-card {
    border: 1px solid #ccc;
    padding: 15px;
    border-radius: 8px;
    text-align: center;
}

.admin-card img {
    width: 100px;
    height: 100px;
    border-radius: 50%; 
    object-fit: cover;
    margin-bottom: 10px;
    background-color: #eee;
}

.admin-card h4 {
    margin: 5px 0 0 0;
    color: var(--primary-color);
}

.admin-card p {
    margin: 0;
    font-style: italic;
    font-size: 0.9em;
    color: #555;
}


.contact-info p {
    font-size: 1.1em;
    margin: 10px 0;
}

.contact-info strong {
    color: var(--primary-color);
}

home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - MY RESTAURANT</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>MY RESTAURANT</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="section">
            <h2>Welcome to My Restaurant</h2>
           <center>
            <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\homepage.jpg" alt="photo of homepage" width="1200px" height="500px">
           </center>
            <p>Experience the finest dining in a cozy atmosphere. We are dedicated to providing fresh, delicious food and exceptional service.</p>
            <p>Visit our Menu page to see our offerings!</p>
        </section>

        <section class="section">
            <h2>Our Specials</h2>
            <p>Try our highly-rated Signature Dish and our seasonal dessert!</p>
            </section>
    </main>

    
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu - My Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>My Restaurant</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="section">
            <h2>Our Delicious Menu</h2>
            <div class="menu-grid">
                <div class="menu-item">
                    <h4>PANNER TIKKA</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\panner.png" alt="photo of panner tikka" width="250px" height="100px" >
                    
                </div>
                <div class="menu-item">
                    <h4>VEG MANCHURIAN</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\manchurian.webp" alt="photo of veg manchurian" width="250px" height="100px">
                </div>
                <div class="menu-item">
                    <h4>DRAGON CHICKEN</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\dragon chicken.jpg" alt="photo of dragon chicken" width="250px" height="100px">
                </div>
                <div class="menu-item">
                    <h4>CHICKEN BIRIYANI</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\biriyani.jpg" alt="photo of chicken biriyani" width="250px" height="100px">
                    
                </div>
                <div class="menu-item">
                    <h4>BURGER</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\burger.jpg" alt="photo of burger" width="250px" heigth="100px">
                    
                </div>
                <div class="menu-item">
                    <h4>NOODLES</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\noodles.jpg" alt="photo of noodles" width="250px" height="180px">
                    
                </div>
                <div class="menu-item">
                    <h4>NUGGETS</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\nuggets.jpg" alt="photo of nuggets" width="250px" height="150px">
                    
                </div>
                <div class="menu-item">
                    <h4>PANNER BUTTER MASALA</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\paneer butter masala.JPG" alt="photo of butter masala" width="250px" height="150px">
                    
                </div>
                <div class="menu-item">
                    <h4>PIZZA</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\pizza.jpg" alt="photo of pizza" width="250px" height="150px">
                    
                </div>
                <div class="menu-item">
                    <h4>SOUP</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\soup.jpg" alt="photo of soup" width="220px" height="150px">
                    
                </div>
                <div class="menu-item">
                    <h4>MOCKTAIL</h4>
                     <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\juice.jpg" alt="photo of mocktail" width="220px" height="150px">
                    
                </div>
                <div class="menu-item">
                    <h4>CAKE</h4>
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\cake.avif" alt="photo of cake" width="220px" height="150px">
                    
                </div>
                </div>
        </section>
    </main>

</body>
</html>

administration.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - My Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>My Restaurant</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="section">
            <h2>Our Leadership Team</h2>
            <div class="admin-grid">
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\DAMU.jpg" alt="Photo of CEO">
                    <h4>Mr.DAMU</h4>
                    <p>Chief Executive Officer (CEO)</p>
                </div>
                
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\bhut.jpg" alt="Photo of Head Chef">
                    <h4>VENKATESH BHUT</h4>
                    <p>Head Chef & Culinary Director</p>
                </div>
                
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\operation manager.jpeg" alt="Photo of Operations Manager">
                    <h4>Mr.JOHN</h4>
                    <p>Operations Manager</p>
                </div>
                
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\Ffinance director.avif" alt="Photo of Finance Director">
                    <h4>Mr.SANJAY VALIRANI</h4>
                    <p>Finance Director</p>
                </div>
                
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\marketing manager.jpeg" alt="Photo of Marketing Manager">
                    <h4>Ms.MARIE</h4>
                    <p>Marketing Manager</p>
                </div>
                
                <div class="admin-card">
                    <img src="C:\Users\acer\OneDrive\Desktop\exp 7\food\foodapp\static\manager.jpg" alt="Photo of HR Manager">
                    <h4>EVANGELINE</h4>
                    <p>Human Resources Manager</p>
                </div>
                
            </div>
        </section>
    </main>

   
</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - My Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>My Restaurant</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="administration.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="section contact-info">
            <h2>Get in Touch</h2>
            <p><i>We'd love to hear from you! Please find our contact details below.</i></p>
            
            <h3>Location:</h3>
            <p><strong>Address:</strong> Akkaiyah naidu street,chennai</p>

            <h3>Contact Details:</h3>
            <p><strong>Phone:</strong> <a href="tel:+15551234567">9943877566</a></p>
            <p><strong>E-mail:</strong> <a href="mailto:info@myrestaurant.com">rifanabarveen0@gmail.com</a></p>
            
            <h3>Hours of Operation:</h3>
            <p>Monday - Friday: 11:00 AM - 10:00 PM</p>
            <p>Saturday - Sunday: 10:00 AM - 11:00 PM</p>
        </section>
        
        </main>

    
</body>
</html>
```
# OUTPUT:

<img width="1788" height="793" alt="Screenshot 2025-10-06 101409" src="https://github.com/user-attachments/assets/08872d98-9f72-4ea3-9357-36f278a0e4d5" />
<img width="1869" height="835" alt="Screenshot 2025-10-06 101428" src="https://github.com/user-attachments/assets/81d6364f-c74b-4472-8dfc-85fceed1f5e9" />
<img width="1866" height="885" alt="Screenshot 2025-10-06 101512" src="https://github.com/user-attachments/assets/e0e99ea2-a6f5-4d2f-ab7f-fa9e119a14c7" />
<img width="1896" height="795" alt="Screenshot 2025-10-06 101242" src="https://github.com/user-attachments/assets/132a96d0-2eb1-4cf4-9274-3b4fa5b16d04" />

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
