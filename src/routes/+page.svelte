<script>
//
</script>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <!-- Header -->
            <h1>Welcome to My Website</h1>
            <!-- Subheader -->
            <h2>Discover the best laptops, carefully selected to meet your needs. Whether you're a professional in need of powerful and sleek devices for work, a student seeking affordable and reliable laptops for studies, or a tech enthusiast, we offer high-quality laptops tailored to your requirements.</h2>
            <a class="cta-button" href="#">Buy Now</a>
        </div>
    </section>

    
<h2 id="why-choose">Why To Choose Our Laptops</h2>
    
    <!-- Section with header and text on the left -->
<section class="content-block left-background">
    <div class="content-text">
        <h2>High-Performance Laptops</h2>
        <p>Explore our high-performance laptops, ideal for demanding tasks. Equipped with advanced processors and ample RAM, they handle heavy software with ease. Enjoy smooth multitasking, stunning visuals, and fast data access. These laptops blend power with sleek design, offering a range of ports for connectivity. Perfect for professionals, gamers, and students who need reliable, speedy performance.</p>
    </div>
    <img src="https://img5.lalafo.com/i/posters/original_webp/19/a7/46/e47e06bcb27817c6efffb434d8.webp" alt="Laptop 1">
</section>

<!-- Section with header and text on the right -->
<section class="content-block right-background">
    <img src="https://img5.lalafo.com/i/posters/original_webp/7c/c2/bc/73b7e5033e406bf618b17f17fd.webp" alt="Laptop 2">
    <div class="content-text">
        <h2>Sleek and Lightweight</h2>
        <p>Discover our sleek and lightweight laptops, designed for life on the go. Easily portable, they're perfect for travel, offering efficient performance and long battery life. Despite their slim design, they’re powerful enough for daily tasks and feature bright displays for a comfortable viewing experience. Ideal for students and remote workers, these laptops are a great blend of style, comfort, and functionality.</p>
    </div>
</section>


    <h2 id="accessories">Laptop Accessories</h2>
<p>Enhance your laptop experience with our selection of high-quality accessories:</p>
<ul>
    <li><strong>External Hard Drives:</strong> Expand your storage with our durable and fast external hard drives.</li>
    <li><strong>Laptop Bags:</strong> Protect your laptop in style with our range of sleek and sturdy bags.</li>
    <li><strong>Wireless Mouse and Keyboards:</strong> Enjoy freedom and flexibility with our ergonomic wireless peripherals.</li>
    <li><strong>Cooling Pads:</strong> Keep your laptop cool and efficient with our high-performance cooling solutions.</li>
    <li><strong>USB Hubs:</strong> Connect all your devices effortlessly with our multi-port USB hubs.</li>
    <li><strong>Privacy Screens:</strong> Secure your sensitive information from prying eyes with our easy-to-apply privacy screens.</li>
</ul>

    <footer>
        <p>&copy; 2023 My Laptop Store</p>
    </footer>

<style>
    
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    
}

html, body {
    margin: 0;
    padding: 0;
    /* Other styles... */
    
}


body {
  font-family: Arial, sans-serif;  
  position: relative;
  
}
        /* Hero section styles */
.hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start; /* Align items to the start (left) of the container */
    height: 100vh;
    background: url("https://p3-ofp.static.pub/ShareResource/na/ftv/hero/lenovo-savings-season.jpg");
    color: white;
    text-align: left;
    padding: 0 120px; /* Keep your existing padding */
    font-family: 'Roboto', sans-serif;
}

.hero-content {
    margin-left: 5%; /* Adjust this value to move your text and CTA button more to the left */
}

.hero h1 {
    font-size: 48px;
    font-weight: bold;
    margin-bottom: 20px;
}

.hero h2 {
    font-size: 24px;
    max-width: 600px;
    line-height: 1.5;
    margin-bottom: 30px;
}

.cta-button {
    background-color: #FF5733;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    font-size: 20px;
    padding: 15px 30px;
    transition: all 0.3s ease;
}

.cta-button:hover {
    background-color: #E04830;
    transform: scale(1.05); /* Slight grow effect on hover */
}

        img {
            max-width: 25%;
            height: 50%; /* Adjusted to maintain aspect ratio */
            display: block;
            margin: 0 auto;
        }

        /* Add a style for your navigation menu */
        ul.nav-menu {
            list-style-type: none;
            padding: 0;
            background-color: #007BFF;
            text-align: center;
        }

        ul.nav-menu li {
            display: inline;
            margin-right: 20px; /* Adjust the spacing between menu items */
        }

        ul.nav-menu li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
        }

        /* Add a style for your footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
        }
      
      
      #why-choose {
    font-size: 44px; /* You can adjust the size as needed */
    text-align: center; /* Center-align the header */
    margin-top: 20px; /* Add some space between the images and the header */
}
      /* Style for content blocks with alternating backgrounds */
.content-block {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 20px;
    background-color: #f0f0f0; /* Light gray background color */
    margin-top: 20px;
}

.content-block:nth-child(even) {
    background-color: #e0e0e0; /* A slightly darker gray for alternating blocks */
}

.content-text {
    flex: 1;
    padding: 20px;
}

.content-text h3 {
    font-size: 24px;
    margin-bottom: 10px;
}

.content-text p {
    font-size: 18px;
    line-height: 1.5;
}

.content-image {
    flex: 1;
    text-align: center;
}

.content-image img {
    max-width: 100%;
    height: auto;
}
      
#accessories {
    font-size: 24px;
    margin-bottom: 10px;
}

ul {
    list-style: none; /* Removes the default list-style */
    padding: 0;
}

ul li {
    background: #f5f5f5; /* Light background for each item */
    margin-bottom: 10px; /* Space between items */
    padding: 10px; /* Padding inside each item */
    border-radius: 5px; /* Rounded corners */
    
}

ul li:hover {
    background: #e0e0e0; /* Change background on hover */
}

ul, li {
    margin: 0;
    padding: 0;
}


    </style>