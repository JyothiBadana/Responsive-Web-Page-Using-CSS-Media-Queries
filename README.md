# Responsive-Web-Page-Using-CSS-Media-Queries
This project transforms a static desktop-only web page into a responsive layout using CSS media queries. It adjusts content, navigation, and images for mobile devices, ensuring better usability and readability on screens smaller than 768px. Designed using HTML, CSS, and tested via Chrome DevTools.

Responsive Web Page using CSS Media Queries

##Objective

Convert a desktop-only webpage into a mobile-friendly layout using **CSS media queries**.

## Tools Used
* HTML
* CSS
* VS Code
* Chrome DevTools

##Features
Mobile-first responsive layout
Stacked columns on smaller screens
Vertical navigation menu on mobile
Scalable text and images
Clean, simple UI

##What This Project Does
This project demonstrates how to:
* Use media queries for responsive design
* Make layouts stack vertically on smaller screens
* Resize text and images for mobile
* Fix overflow and scrolling issues

## How It Works
1. Open the HTML page in VS Code
2. Identify fixed-width elements
3. Apply media queries for `max-width: 768px`
4. Adjust layout, text, and images for smaller screens
5. Test using Chrome DevTools device toolbar

##Files Included
* `index.html` — Main HTML structure
* `style.css` — CSS styling with media queries


##CODE##
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Page</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="navbar">
    <h1>My Website</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main class="container">
    <section class="content">
      <h2>Welcome</h2>
      <p>This is a sample page to demonstrate mobile responsiveness using media queries.</p>
    </section>
    <aside class="sidebar">
      <h3>Sidebar</h3>
      <p>Additional content here.</p>
    </aside>
  </main>
  <footer class="footer">&copy; 2025 My Website</footer>
</body>
</html>

/* style.css */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.6;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  color: white;
  padding: 10px 20px;
}

.navbar ul {
  display: flex;
  list-style: none;
  padding: 0;
}

.navbar ul li {
  margin-left: 20px;
}

.navbar ul li a {
  color: white;
  text-decoration: none;
}

.container {
  display: flex;
  padding: 20px;
}

.content {
  flex: 3;
  padding-right: 20px;
}

.sidebar {
  flex: 1;
  background: #f4f4f4;
  padding: 10px;
}

.footer {
  text-align: center;
  padding: 15px;
  background-color: #333;
  color: white;
}

/* Media Query for Mobile Devices */
@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }

  .navbar ul {
    flex-direction: column;
    width: 100%;
  }

  .navbar ul li {
    margin: 10px 0;
  }

  .container {
    flex-direction: column;
    padding: 10px;
  }

  .content {
    padding-right: 0;
  }

  .sidebar {
    margin-top: 20px;
  }

  h1, h2, h3 {
    font-size: 1.2rem;
  }

  p {
    font-size: 0.95rem;
  }

  img {
    max-width: 100%;
    height: auto;
  }
}









