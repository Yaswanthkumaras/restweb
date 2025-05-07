# Ex.07 Restaurant Website
## Date:07.05.2025
## REG NO:212224230310

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>La Table Élégante - Menu</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Roboto&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Roboto', sans-serif;
      background: url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1920&q=80') no-repeat center center fixed;
      background-size: cover;
      padding: 40px 20px;
      color: #fff;
    }

    .overlay {
      background-color: rgba(0, 0, 0, 0.6);
      padding: 40px;
      border-radius: 20px;
    }

    .menu-wrapper {
      max-width: 1100px;
      margin: auto;
    }

    .menu-header {
      text-align: center;
      font-family: 'Playfair Display', serif;
      margin-bottom: 50px;
    }

    .menu-header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      color: #ecf0f1;
    }

    .menu-header p {
      color: #bdc3c7;
      font-style: italic;
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
    }

    .menu-card {
      background: #ffffff;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
      transition: transform 0.2s ease;
      color: #2c3e50;
    }

    .menu-card:hover {
      transform: translateY(-5px);
    }

    .menu-image {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .menu-content {
      padding: 20px;
    }

    .menu-title {
      font-size: 1.4rem;
      font-weight: bold;
      margin-bottom: 10px;
      color: #34495e;
    }

    .menu-desc {
      color: #7f8c8d;
      font-size: 0.95rem;
      margin-bottom: 15px;
    }

    .menu-price {
      color: #e67e22;
      font-size: 1.1rem;
      font-weight: bold;
    }

    .contact-section {
      margin-top: 50px;
      text-align: center;
      color: #ecf0f1;
    }

    .contact-section h2 {
      font-size: 2rem;
      margin-bottom: 15px;
    }

    .contact-info {
      font-size: 1.1rem;
      margin-bottom: 20px;
    }

    .contact-info span {
      display: block;
      margin-bottom: 10px;
    }

    .contact-form input,
    .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border-radius: 5px;
      border: none;
    }

    .contact-form button {
      padding: 12px 20px;
      background-color: #e67e22;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 1rem;
      cursor: pointer;
    }

    .contact-form button:hover {
      background-color: #d35400;
    }

    @media (max-width: 600px) {
      .menu-header h1 {
        font-size: 2.2rem;
      }
    }
  </style>
</head>
<body>
  <div class="overlay">
    <div class="menu-wrapper">
      <div class="menu-header">
        <h1>La Table Élégante</h1>
        <p>Where every bite tells a story</p>
      </div>

      <div class="menu-grid">
        <!-- Truffle Mushroom Soup -->
        <div class="menu-card">
          <img class="menu-image" src="C:\Users\admin\Downloads\mario-raj-ysmeQt1dzcw-unsplash.jpg" alt="Truffle Mushroom Soup">
          <div class="menu-content">
            <div class="menu-title">Chicken Biriyani</div>
            <div class="menu-desc">Creamy wild mushroom soup infused with truffle oil and herbs.</div>
            <div class="menu-price">$9.50</div>
          </div>
        </div>

        <!-- Seared Salmon Fillet -->
        <div class="menu-card">
          <img class="menu-image" src="C:\Users\admin\Downloads\side-view-pilaf-with-stewed-beef-meat-plate.jpg">
          <div class="menu-content">
            <div class="menu-title">Mutton Biriyani</div>
            <div class="menu-desc">Served with garlic butter asparagus and roasted baby potatoes.</div>
            <div class="menu-price">$21.00</div>
          </div>
        </div>

        <!-- Butternut Squash Risotto -->
        <div class="menu-card">
          <img class="menu-image" src="C:\Users\admin\Downloads\pexels-ali-dashti-506667798-17649369.jpg" alt="Butternut Squash Risotto">
          <div class="menu-content">
            <div class="menu-title">Fish Biriyani</div>
            <div class="menu-desc">Arborio rice with slow-roasted squash, sage, and parmesan.</div>
            <div class="menu-price">$21.00</div>
          </div>
        </div>
      </div>

      <!-- Contact Section -->
      <div class="contact-section">
        <h2>Contact Us</h2>
        <div class="contact-info">
          <span>Phone: (123) 456-7890</span>
          <span>Email: yaswanthkumar@gmail.com</span>
          <span>Address:Hari Bavanam,100, Mount Road, Chennai, Tamil Nadu 600006, India</span>
        </div>
        
        <div class="contact-form">
          <h3>Send Us a Message</h3>
          <form action="#">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" rows="4" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</body>
</html>

```


## OUTPUT:
![Screenshot 2025-05-07 111857](https://github.com/user-attachments/assets/71196b34-0685-4a1c-8dd9-7d0d109aa99d)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
