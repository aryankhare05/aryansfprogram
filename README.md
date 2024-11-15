<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3A's MEGA MART</title>
    <style>
        /* Basic Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        /* Colors */
        :root {
            --primary-color: #5a3f89; /* Deep purple */
            --secondary-color: #f4f4f8; /* Light background */
            --accent-color: #4b2a72; /* Darker accent purple */
            --text-color: #333;
            --hover-color: #7a5fa3;
            --white-color: #ffffff;
        }

        /* Navbar */
        /* Navbar */
nav {
    background-color: var(--primary-color);
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: var(--white-color);
    position: sticky;
    top: 0;
    z-index: 1000; /* Keeps navbar on top of other elements */
}
        nav h1 {
            font-size: 1.8rem;
            cursor: pointer;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        nav ul li a {
            color: var(--white-color);
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--hover-color);
        }
        .search-box {
    display: flex;
    align-items: center;
}

.search-box input[type="text"] {
    padding: 0.5rem;
    font-size: 1rem;
    border-radius: 5px;
    border: none;
    width: 200px;
    margin-right: 0.5rem; /* Adds spacing between input and button */
}

.search-button {
    padding: 0.5rem 1rem;
    background-color: var(--hover-color);
    color: var(--white-color);
    font-weight: bold;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.search-button:hover {
    background-color: var(--primary-color);
}

        /* Banner Section */
        .banner {
            background-color: var(--accent-color);
            color: var(--white-color);
            padding: 2rem;
            text-align: center;
        }

        .banner h2 {
            font-size: 2.5rem;
        }

        .banner p {
            margin: 1rem 0;
            font-size: 1.2rem;
        }

        .banner button {
            background-color: var(--hover-color);
            color: var(--white-color);
            border: none;
            padding: 1rem 2rem;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s;
            transition: transform 0.3s ease-in-out;
            ;

        }

        .banner button:hover {
            transform:scale(1.15);
            background-color: var(--primary-color);
        }
        /* Hero Image Section */
.hero-image {
    position: relative;
    width: 100%;
    height: 400px; /* Adjust height as needed */
    overflow: hidden;
}

.hero-image img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Ensures the image covers the section */
}

.hero-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: var(--white-color);
    text-align: center;
    background: rgba(0, 0, 0, 0.5); /* Adds a semi-transparent background */
    padding: 1rem;
    border-radius: 8px;
}

.hero-text h2 {
    font-size: 2rem;
    margin-bottom: 0.5rem;
}

.hero-text p {
    font-size: 1.2rem;
}
        /* Main Sections */
        .main-sections {
            padding: 2rem;
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            justify-content: space-around;
        }

        .section {
            background-color: var(--secondary-color);
            color: var(--text-color);
            padding: 1rem;
            border-radius: 8px;
            text-align: center;
            width: 23%;
            height: 400px;
            transition: transform 0.3s;
            /* box-shadow: 0 4px 8px rgba(0, 0, 0, 1); */
            box-shadow: 0 4px 8px rgba(160, 32, 240, 0.25);

        }

        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .section img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 1rem;
        }

        .section h2 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }

        .section p {
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
        }

        /* Footer */
        footer {
    background-color: var(--primary-color);
    color: var(--white-color);
    padding: 2rem;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
    border-top: 4px solid var(--hover-color);
    box-shadow: 0 -4px 8px rgba(0, 0, 0, 0.2); /* Adds shadow effect */
}

footer div {
    text-align: left;
}

footer h4 {
    margin-bottom: 1rem;
    font-size: 1.3rem;
    text-decoration: underline;
}

footer ul {
    list-style: none;
    padding: 0;
}

footer ul li {
    margin: 0.5rem 0;
}

footer ul li a {
    color: var(--white-color);
    text-decoration: none;
    transition: color 0.3s;
    font-size: 0.9rem;
}

footer ul li a:hover {
    color: var(--hover-color);
}

footer .social-icons {
    display: flex;
    gap: 0.5rem;
    margin-top: 0.8rem;
    font-weight: bold;
}

footer .social-icons a {
    display: inline-block;
    padding: 0.5rem;
    background-color: var(--hover-color);
    border-radius: 50%;
    color: var(--white-color);
    text-decoration: none;
    font-size: 1.2rem;
}
footer .footerheading{
    text-decoration: none;
}

    </style>
</head>
<body>

    <!-- Navbar -->
    <nav>
        <h1>3A's MEGA MART</h1>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Categories</a></li>
            <li><a href="#">Offers</a></li>
            <li><a href="#">Support</a></li>
            <li><a href="#">Cart</a></li>
            <li><a href="#">Account</a></li>
        </ul>
        <div class="search-box">
            <input type="text" placeholder="3A's.search">
            <button class="search-button">search</button>
        </div>
    </nav>

    <!-- Banner Section -->
    <div class="banner">
        <h2>Welcome to 3A's MEGA MART!</h2>
        <p>Find the best deals on clothes, electronics, groceries, and more.</p>
        <button>Shop Now</button>
    </div>
     <!-- Hero Image Section -->
<div class="hero-image">
    <img src="pexels-rostislav-10458835.jpg" alt="Mega Sale! Up to 70% Off on Mobile Accessories">
    <div class="hero-text">
        <h2>Mobile Accessories</h2>
        <p>Up to 70% off</p>
    </div>
</div>
  <!-- Main Sections -->
    <div class="main-sections">
        <!-- Boxes with Various Categories and Offers -->
        <div class="section">
            <img src="clothesimage.jpg" alt="Clothes">
            <h2>Clothes</h2>
        </div>
        <div class="section">
            <img src="electronics.jpg" alt="Electronics">
            <h2>Electronics</h2>
        </div>
        <div class="section">
            <img src="grocery.jpg" alt="Groceries">
            <h2>Groceries</h2>
        </div>
        <div class="section">
            <img src="fitness.jpg" alt="Fitness">
            <h2>Fitness</h2>
        </div>
        <div class="section">
            <img src="toys1.jpg" alt="Toys">
            <h2>Toys</h2>
        </div>
        <div class="section">
            <img src="makeup.jpg" alt="Makeup">
            <h2>Makeup</h2>
        </div>
        <div class="section">
            <img src="trending.jpg" alt="Trending">
            <h2>Trending</h2>
        </div>
        <div class="section">
            <img src="budget.jpg"alt="Budget Store">
            <h2>Budget Store</h2>
        </div>

        <!-- Additional Boxes with Offers -->
        <div class="section">
            <h2>Starting ₹149</h2>
             <img src="149.jpg.png" alt="staring 149">
            <h2>Headphones</h2>
        </div>
        <div class="section">
            <h2>Up to 60% off</h2>
            <img src="women.jpg.png" alt="60% off">
            <h2>Styles for Women</h2>
        </div>
        <div class="section">
            <h2>Most-Loved Products</h2>
            <img src="mostloved.jpg.png" alt="most loved products">
            <h2>Customer favorites</h2>
        </div>
        <div class="section">
            <h2>Up to 50% off</h2>
            <img src="50percent.jpg" alt="up to 50% off">
            <h2>International Brands</h2>
        </div>
        <div class="section">
            <h2>Best Sellers</h2>
            <img src="beauty.jpg" alt="best seller">
            <h2>Top Beauty Picks</h2>
        </div>
        <div class="section">
            <h2>Starting ₹99</h2>
            <img src="starting99.jpg.png" alt="staring 99">
            <h2>3A's Brands & More</h2>
        </div>
        <div class="section">
            <h2>Up to 60% off</h2>
            <img src="60per.jpg.png" alt="upto 60 percent off">
            <h2>Car & Bike Accessories</h2>
        </div>
        <div class="section">
            <h2>Festival Special</h2>
            <img src="festival1.jpg" alt="festival Special">
            <h2>Top Festive Items</h2>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div>
            <h4 class="footerheading">Get to Know Us</h4>
            <ul>
                <li><a href="#">About 3A's MEGA MART</a></li>
                <li><a href="#">Careers</a></li>
                <li><a href></a></li>
            </div>
            <div>
                <h4 class="footerheading">Connect With Us</h4>
                <div class="social-icons">
                    <a href="#">facebook<i class="fab fa-facebook-f"></i></a>
                    <a href="#">twitter<i class="fab fa-twitter"></i></a>
                    <a href="#">instagram<i class="fab fa-instagram"></i></a>
                    <a href="#">linkedin<i class="fab fa-linkedin-in"></i></a>
                </div>
            </div>
            
            
