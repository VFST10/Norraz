<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=3.0">
    <link rel="stylesheet" href="styles.css">
    <title>Norraz Store SD</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-image: url(''); /* Replace with the actual URL of your background image */
            background-size: cover;
            background-position: center;
        }

        /* Add the rest of your existing styles here */

        header {
            background-color: #232f3e;
            color: #fff;
            padding: 3em;
            text-align: center;
            width: 100%;
        }
        header .logo {
            font-size: 4em; /* Adjust the font size as needed */
            font-weight: bold;
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
        }

        /* ... (rest of your existing CSS) ... */
        .cart-icon {
        position: absolute;
        top: 20px;
        right: 20px;
        font-size: 3em;
        cursor: pointer;
        color: #fff;
        }

        .cart-icon:hover {
        color: #fff;
        }

        main {
            padding:20px;
            width: 100%;
        }

        #home h2 {
            font-size: 2em; /* Adjust the size as needed */
        }

        section {
            margin-bottom: 20px;
            text-align: center;
        }

        .product {
            border: 0px solid #ddd;
            padding: 20px;
            text-align: center;
            margin-bottom: 20px;
            font-size: 2em;
        }
      #slider {
          overflow: hidden;
          width: auto;
          max-height: auto; /* Adjust the max-height as needed */
          margin-top: 20px;
          max-width: auto;
      }

      #slider img {
          width: auto;
          height: auto;
      }
    </style>
    <img src="Norraz removed bg.png" alt="Norraz Logo">
</head>
<body style='background-color: aliceblue;'>
    <header>
        <div class="logo">Norraz Store SD</div>
        <div class="cart-icon" onclick="viewCart()">🛒</div>
        <nav>
            <ul>
                <li><a href="#home"> Home </a></li><br>
                <li><a href=" #products "> Products </a></li><br>
                <li><a href=" #contact "> Contact </a></li>
            </ul>
        </nav>
    </header>
    <div id="slider">
        <img src="Slider 1.png" alt="Slider Image 1">
        <img src="Slider 2.png" alt="Slider Image 2">
        <img src="Slider 3.png" alt="Slider Image 3">
        <!-- Add more images as needed -->
    </div>
    <main>
        <section id="home">
            <h2>Welcome to Norraz Store SD</h2>
            <p>Discover a wide range of products for every occasion.</p>
            <p>Here's An Introductory Video</p>
      <video width="600" height="450"  <video autoplay loop muted playsinline>>
          <source src="norraz.mp4" type="video/mp4">
          Your browser does not support the video tag
      </video>
        </section>
        <section id="products">
            <div class="product">
              <p><b>Here's a List of Our Current Products</b></p>  
              <img src="Cute cat keychain.png" alt="Cute Cat Keychain">
                <h3>Cute Cat Keychain</h3>
                <p class="price">৳250.00</p>
                <button onclick="addToCart(1)">Add to Cart</button>
            </div>
            <!-- Repeat similar structure for other products -->
            <div class="product">
                <img src="Cute panda keychain.png" alt="Cute Panda Keychain">
                <h3>Cute Panda Keychain</h3>
                <p class="price">৳250.00</p>
                <button onclick="addToCart(2)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="lightening bolt.png" alt="Lightning bolt pendant">
                <h3>Lightning bolt pendant</h3>
                <p class="price">৳350.00</p>
                <button onclick="addToCart(3)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="poker ring(sharpened).png" alt="Poker Ring">
                <h3>Poker Ring</h3>
                <p class="price">৳380.00</p>
                <button onclick="addToCart(4)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="Akatsuki cloud necklace.png" alt="Akatsuki Cloud Pendant">
                <h3>Akatsuki Cloud Pendant</h3>
                <p class="price">৳300.00</p>
                <button onclick="addToCart(5)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="pearl earing.png" alt="Pearl earing">
                <h3>Pearl earing</h3>
                <p class="price">৳200.00</p>
                <button onclick="addToCart(6)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="Round Leaf Chain.png" alt="Round leaf chain">
                <h3>Round leaf chain</h3>
                <p class="price">৳200.00</p>
                <button onclick="addToCart(7)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="couples beads.png" alt="Black and white beads/couples matching bracelets">
                <h3>Black and white beads/couples matching bracelets</h3>
                <p class="price">৳400.00</p>
                <button onclick="addToCart(8)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="Ace Cards.png" alt="Ace Card Pendant">
                <h3>Ace Card Pendant</h3>
                <p class="price">৳400.00</p>
                <button onclick="addToCart(9)">Add to Cart</button>
            </div>
            <div class="product">
                <img src="Mini Soda Bottles.png" alt="Mini Soda Bottle">
                <h3>Mini Soda Bottle</h3>
                <p class="price">৳300.00</p>
                <button onclick="addToCart(10)">Add to Cart</button>
            </div>
        </section>
        <section id="contact">
            <h2>Contact Us For Buying Products or Other Inquires</h2>
            <p>Email: norrazstore.sd@gmail.com</p>
            <p>Instagram: norrazstore.sd</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 Norraz Store SD. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
    <script>
        let cart = [];
        const productNames = [
            "Cute Cat Keychain",
            "Cute Panda Keychain",
            "Lightning bolt pendant",
            "Poker Ring",
            "Akatsuki Cloud Pendant",
            "Pearl earring",
            "Round leaf chain",
            "Black and white beads/couples matching bracelets",
            "Ace Card Pendant",
            "Mini Soda Bottle"
        ];
        const productPrices = [
            250.00,  // Adjust the prices accordingly
            250.00,
            350.00,
            380.00,
            300.00,
            200.00,
            200.00,
            400.00,
            400.00,
            300.00
        ];

        function addToCart(productId) {
            let product = {
                id: productId,
                name: productNames[productId - 1], // Adjust index
                price: productPrices[productId - 1] // Adjust index
            };
            cart.push(product);
            alert(`Product added to cart!`);
        }

        function viewCart() {
            // Display the cart details
            if (cart.length === 0) {
                alert('Your cart is empty.');
            } else {
                let cartDetails = 'Cart Contents:\n\n';
                cart.forEach(product => {
                    cartDetails += `${product.name}, Price: ৳${product.price.toFixed(2)}\n`;
                });
                alert(cartDetails);
            }
        }
    </script>
    <script>
        // JavaScript for the image slider
        let currentSlide = 0;
        const slides = document.querySelectorAll('#slider img');
        const slideInterval = setInterval(nextSlide, 2000);

        function nextSlide() {
            slides[currentSlide].style.display = 'none';
            currentSlide = (currentSlide + 1) % slides.length;
            slides[currentSlide].style.display = 'block';
        }
    </script>
</body>
</html>
