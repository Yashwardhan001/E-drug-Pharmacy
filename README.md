
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Pharmacy Drug House</title>
    <meta name="description" content="E-Pharmacy Drug House: Your trusted online pharmacy for medicines, healthcare products, and wellness essentials.">
    <meta name="keywords" content="pharmacy, online pharmacy, medicines, healthcare, drugs, wellness, health products, order medicines online, E-Pharmacy Drug House, Indore pharmacy, Madhya Pradesh pharmacy">
    <meta name="robots" content="index, follow">
    <meta name="author" content="E-Pharmacy Drug House">
    <meta property="og:title" content="E-Pharmacy Drug House: Your Trusted Online Pharmacy">
    <meta property="og:description" content="Order medicines online with ease. Wide range of products, fast delivery, and excellent customer service.">
    <meta property="og:url" content="https://yourdomain.com/">
    <meta property="og:type" content="website">
    <meta property="og:image" content="https://images.unsplash.com/photo-1587854691374-2dd5b29bc81a">
    <meta property="og:site_name" content="E-Pharmacy Drug House">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="E-Pharmacy Drug House: Your Trusted Online Pharmacy">
    <meta name="twitter:description" content="Order medicines online with ease. Wide range of products, fast delivery, and excellent customer service.">
    <meta name="twitter:image" content="https://images.unsplash.com/photo-1587854691374-2dd5b29bc81a">
    <link rel="icon" href="https://images.unsplash.com/photo-1587854691374-2dd5b29bc81a?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=32&h=32" type="image/png">
    <link rel="apple-touch-icon" sizes="180x180" href="https://images.unsplash.com/photo-1587854691374-2dd5b29bc81a?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=180&h=180">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f3f4f6;
        }
        .product-card img {
            height: 200px;
            width: 100%;
            object-fit: cover;
            border-radius: 0.5rem;
        }
        .error {
            color: #e53e3e;
            font-size: 0.875rem;
            margin-top: 0.25rem;
            display: none;
        }
        .success-message {
            color: #2f855a;
            font-size: 0.875rem;
            margin-top: 0.5rem;
            display: none;
        }
        #all-products-section {
            display: none;
        }
        .service-icon {
            width: 64px;
            height: 64px;
            object-fit: cover;
            border-radius: 0.25rem;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="bg-blue-600 shadow-md sticky top-0 z-10">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <a href="/" class="flex items-center text-white text-xl font-semibold" aria-label="E-Pharmacy Drug House Home">
                <img src="https://kaireedesign.com/wp-content/uploads/2014/12/21b.jpg?crop=entropy&cs=tinysrgb&w=32&h=32" alt="E-Pharmacy Drug House Logo" class="mr-2 h-8 w-8">
                E-Pharmacy Drug House
            </a>
            <nav class="hidden md:flex space-x-6" aria-label="Main Navigation">
                <a href="/" class="text-gray-200 hover:text-white transition-colors">Home</a>
                <a href="#all-products-section" class="text-gray-200 hover:text-white transition-colors shop-now-btn">Products</a>
                <a href="/about.html" class="text-gray-200 hover:text-white transition-colors">About Us</a>
                <a href="/services.html" class="text-gray-200 hover:text-white transition-colors">Services</a>
                <a href="/contact.html" class="text-gray-200 hover:text-white transition-colors">Contact Us</a>
                <a href="/cart.html" class="text-gray-200 hover:text-white transition-colors">Cart</a>
            </nav>
            <button id="hamburger-btn" class="md:hidden text-white focus:outline-none" aria-label="Toggle Navigation" aria-expanded="false">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-16 6h16"></path>
                </svg>
            </button>
        </div>
    </header>

    <!-- Mobile Menu -->
    <div id="mobile-menu" class="hidden fixed inset-0 bg-gray-900 bg-opacity-90 z-20" aria-hidden="true">
        <div class="bg-gray-800 w-80 h-full absolute right-0 p-6">
            <button id="close-menu-btn" class="text-white mb-4 focus:outline-none self-end" aria-label="Close Menu">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                </svg>
            </button>
            <nav class="flex flex-col space-y-4" aria-label="Mobile Navigation">
                <a href="/" class="text-gray-200 hover:text-white text-lg transition-colors">Home</a>
                <a href="#all-products-section" class="text-gray-200 hover:text-white text-lg transition-colors shop-now-btn">Products</a>
                <a href="/about.html" class="text-gray-200 hover:text-white text-lg transition-colors">About Us</a>
                <a href="/services.html" class="text-gray-200 hover:text-white text-lg transition-colors">Services</a>
                <a href="/contact.html" class="text-gray-200 hover:text-white text-lg transition-colors">Contact Us</a>
                <a href="/cart.html" class="text-gray-200 hover:text-white text-lg transition-colors">Cart</a>
            </nav>
        </div>
    </div>

    <!-- Hero Section -->
    <section class="bg-gradient-to-r from-blue-100 to-purple-100 py-16 md:py-24 text-center">
        <div class="container mx-auto px-4">
            <h1 class="text-3xl md:text-5xl font-semibold text-gray-800 mb-4">Welcome to E-Pharmacy Drug House</h1>
            <p class="text-lg md:text-xl text-gray-600 mb-8">Your trusted online source for quality medicines and healthcare products.</p>
            <a href="#all-products-section" class="bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-6 rounded-full transition-colors shop-now-btn">Shop Now</a>
        </div>
    </section>

    <!-- Featured Products -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-gray-800 text-center mb-8">Featured Products</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="bg-white rounded-lg shadow-md p-4 flex flex-col product-card">
                    <img src="https://images.unsplash.com/photo-1588718889344-f7bd7a565d20?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8NHx8cGlsbHx8MHx8fHwxNjI3NzY0MTAx&ixlib=rb-1.2.1&q=80&w=1080" alt="Fever Relief Tablets" loading="lazy">
                    <h3 class="text-lg font-semibold text-gray-800 mt-4 mb-2">Fever Relief Tablets</h3>
                    <p class="text-gray-600 text-sm mb-2">Relief from fever and pain with fast-acting formula.</p>
                    <p class="text-gray-700 font-semibold mb-4">₹150.00</p>
                    <button class="bg-indigo-500 hover:bg-indigo-600 text-white font-semibold py-2 px-4 rounded-full transition-colors add-to-cart-btn" data-product-id="1" aria-label="Add Fever Relief Tablets to Cart">Add to Cart</button>
                </div>
                <div class="bg-white rounded-lg shadow-md p-4 flex flex-col product-card">
                    <img src="https://images.unsplash.com/photo-1667058015056-b03fa4974abf?blend=000000&blend-alpha=10&blend-mode=normal&blend-w=1&crop=faces%2Cedges&h=630&mark=https:%2F%2Fimages.unsplash.com%2Fopengraph%2Flogo.png&mark-align=top%2Cleft&mark-pad=50&mark-w=64&w=1200&auto=format&fit=crop&q=60&ixid=M3wxMjA3fDB8MXxhbGx8fHx8fHx8fHwxNzE4MDYzNTQzfA&ixlib=rb-4.0.3" alt="Digestive Health Capsules" loading="lazy">
                    <h3 class="text-lg font-semibold text-gray-800 mt-4 mb-2">Digestive Health Capsules</h3>
                    <p class="text-gray-600 text-sm mb-2">Supports digestive health with natural ingredients.</p>
                    <p class="text-gray-700 font-semibold mb-4">₹250.00</p>
                    <button class="bg-indigo-500 hover:bg-indigo-600 text-white font-semibold py-2 px-4 rounded-full transition-colors add-to-cart-btn" data-product-id="2" aria-label="Add Digestive Health Capsules to Cart">Add to Cart</button>
                </div>
                <div class="bg-white rounded-lg shadow-md p-4 flex flex-col product-card">
                    <img src="https://media.istockphoto.com/id/1366960245/photo/man-pouring-cough-syrup-into-spoon.webp?b=1&s=170667a&w=0&k=20&c=7BeXjPQEvxu6OFRI7m9fr8i-nlTzEj4zr2_Evt-8cSs=" alt="Immunity Booster Syrup" loading="lazy">
                    <h3 class="text-lg font-semibold text-gray-800 mt-4 mb-2">Immunity Booster Syrup</h3>
                    <p class="text-gray-600 text-sm mb-2">Boosts immunity with essential vitamins.</p>
                    <p class="text-gray-700 font-semibold mb-4">₹300.00</p>
                    <button class="bg-indigo-500 hover:bg-indigo-600 text-white font-semibold py-2 px-4 rounded-full transition-colors add-to-cart-btn" data-product-id="3" aria-label="Add Immunity Booster Syrup to Cart">Add to Cart</button>
                </div>
            </div>
            <div class="text-center mt-8">
                <a href="#all-products-section" class="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-3 px-6 rounded-full transition-colors shop-now-btn">View All Products</a>
            </div>
        </div>
    </section>

    <!-- All Products -->
    <section id="all-products-section" class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-gray-800 text-center mb-8">All Products</h2>
            <div id="all-products-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6"></div>
        </div>
    </section>

    <!-- About Us -->
    <section class="bg-blue-100 py-16">
        <div class="container mx-auto px-4 grid md:grid-cols-2 gap-8 items-center">
            <div>
                <h2 class="text-2xl font-semibold text-blue-700 mb-4">About Us</h2>
                <p class="text-gray-600 text-lg mb-6">E-Pharmacy Drug House is your trusted online pharmacy, offering a seamless way to access medicines and healthcare products. We prioritize quality, convenience, and customer satisfaction.</p>
                <p class="text-gray-600 text-lg">With a commitment to health and well-being, our experienced team ensures secure and prompt delivery of genuine products to your doorstep.</p>
            </div>
            <div class="text-center">
                <img src="https://images.unsplash.com/photo-1576091160550-2173dba999ef?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=600&h=400&fit=crop" alt="About Us - E-Pharmacy Drug House" class="rounded-lg shadow-md w-full" loading="lazy">
            </div>
        </div>
    </section>

    <!-- Services -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-gray-800 text-center mb-8">Our Services</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white rounded-lg shadow-md p-6 flex flex-col items-center text-center">
                    <img src="https://images.unsplash.com/photo-1585435557343-3b092031a831?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=64&h=64&fit=crop" alt="Wide Range of Products" class="service-icon mb-4" loading="lazy">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Wide Range of Products</h3>
                    <p class="text-gray-600 text-sm">Explore a diverse selection of medicines and wellness products.</p>
                </div>
                <div class="bg-white rounded-lg shadow-md p-6 flex flex-col items-center text-center">
                    <img src="https://images.unsplash.com/photo-1516321497487-e288fb19713f?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=64&h=64&fit=crop" alt="Convenient Online Ordering" class="service-icon mb-4" loading="lazy">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Convenient Online Ordering</h3>
                    <p class="text-gray-600 text-sm">Order effortlessly from the comfort of your home.</p>
                </div>
                <div class="bg-white rounded-lg shadow-md p-6 flex flex-col items-center text-center">
                    <img src="https://images.unsplash.com/photo-1583394838336-acd977736f90?ixlib=rb-4.0.3&crop=entropy&cs=tinysrgb&w=64&h=64&fit=crop" alt="Fast Delivery" class="service-icon mb-4" loading="lazy">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Fast Delivery</h3>
                    <p class="text-gray-600 text-sm">Reliable and swift delivery to your doorstep.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Us -->
    <section class="bg-gray-100 py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-gray-800 text-center mb-8">Contact Us</h2>
            <div class="bg-white rounded-lg shadow-md p-6 md:p-10">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div>
                        <h3 class="text-xl font-semibold text-gray-800 mb-4">E-Pharmacy Drug House</h3>
                        <ul class="text-gray-600 text-lg">
                            <li class="mb-2"><strong>Address:</strong> Vrindavan Palace Colony, Pipliya Kumar, Indore, Madhya Pradesh 452010</li>
                            <li class="mb-2"><strong>Phone:</strong> +919926576929</li>
                            <li class="mb-2"><strong>Email:</strong> info@epharmacy.com</li>
                            <li><a href="https://yourdomain.com" target="_blank" rel="noopener noreferrer" class="text-blue-500 hover:text-blue-700 transition-colors">Website</a></li>
                        </ul>
                    </div>
                    <div>
                        <form id="contact-form" class="space-y-4" novalidate>
                            <input type="hidden" name="csrf_token" value="YOUR_CSRF_TOKEN_HERE">
                            <div>
                                <label for="name" class="block text-gray-700 text-sm font-bold mb-2">Your Name</label>
                                <input type="text" id="name" name="name" placeholder="Your Name" class="w-full py-3 px-4 border rounded focus:outline-none focus:ring-2 focus:ring-blue-500" required aria-describedby="name-error">
                                <p id="name-error" class="error">Please enter your name.</p>
                            </div>
                            <div>
                                <label for="email" class="block text-gray-700 text-sm font-bold mb-2">Your Email</label>
                                <input type="email" id="email" name="email" placeholder="Your Email" class="w-full py-3 px-4 border rounded focus:outline-none focus:ring-2 focus:ring-blue-500" required aria-describedby="email-error">
                                <p id="email-error" class="error">Please enter a valid email address.</p>
                            </div>
                            <div>
                                <label for="message" class="block text-gray-700 text-sm font-bold mb-2">Your Message</label>
                                <textarea id="message" name="message" placeholder="Your Message" class="w-full py-3 px-4 border rounded focus:outline-none focus:ring-2 focus:ring-blue-500 h-32" required aria-describedby="message-error"></textarea>
                                <p id="message-error" class="error">Please enter your message.</p>
                            </div>
                            <button type="submit" class="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-3 px-6 rounded-full transition-colors">Send Message</button>
                            <p id="form-success" class="success-message">Thank you for your message! We will get back to you soon.</p>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ -->
    <section class="bg-blue-100 py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-blue-700 text-center mb-8">Frequently Asked Questions</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <div>
                    <h3 class="text-lg font-semibold text-gray-800 mb-2">What is E-Pharmacy Drug House?</h3>
                    <p class="text-gray-600 text-sm mb-4">E-Pharmacy Drug House is an online pharmacy offering convenient access to medicines and healthcare products.</p>
                    <h3 class="text-lg font-semibold text-gray-800 mb-2">How do I place an order?</h3>
                    <p class="text-gray-600 text-sm mb-4">Browse products, add to cart, and check out. Log in or create an account to complete your order.</p>
                </div>
                <div>
                    <h3 class="text-lg font-semibold text-gray-800 mb-2">Is it safe to buy medicines online?</h3>
                    <p class="text-gray-600 text-sm mb-4">Yes, we ensure all products are genuine and stored properly for your safety.</p>
                    <h3 class="text-lg font-semibold text-gray-800 mb-2">What is your delivery policy?</h3>
                    <p class="text-gray-600 text-sm mb-4">We provide fast, reliable delivery with times varying by location.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl font-semibold text-gray-800 text-center mb-8">What Our Customers Say</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-white rounded-lg shadow-md p-4 text-center">
                    <p class="text-gray-600 text-sm italic mb-4">"Fast delivery and excellent service. Highly recommend!"</p>
                    <p class="text-gray-700 font-semibold">- Rajesh Sharma</p>
                </div>
                <div class="bg-white rounded-lg shadow-md p-4 text-center">
                    <p class="text-gray-600 text-sm italic mb-4">"Great product range and easy-to-use website."</p>
                    <p class="text-gray-700 font-semibold">- Priya Patel</p>
                </div>
                <div class="bg-white rounded-lg shadow-md p-4 text-center">
                    <p class="text-gray-600 text-sm italic mb-4">"Prompt delivery and fantastic customer support."</p>
                    <p class="text-gray-700 font-semibold">- Rohan Singh</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-gray-200 py-6">
        <div class="container mx-auto px-4 text-center">
            <p class="text-md">© 2025 E-Pharmacy Drug House. All rights reserved. | 
                <a href="/privacy.html" class="hover:text-white transition-colors">Privacy Policy</a> | 
                <a href="/terms.html" class="hover:text-white transition-colors">Terms of Service</a>
            </p>
        </div>
    </footer>

    <script>
        // Debounce Utility
        const debounce = (func, wait) => {
            let timeout;
            return (...args) => {
                clearTimeout(timeout);
                timeout = setTimeout(() => func(...args), wait);
            };
        };

        // Check LocalStorage Availability
        const isLocalStorageAvailable = () => {
            try {
                const test = '__storage_test__';
                localStorage.setItem(test, test);
                localStorage.removeItem(test);
                return true;
            } catch (e) {
                console.warn('localStorage is not available:', e);
                return false;
            }
        };

        // Mobile Menu Toggle
        const hamburgerBtn = document.getElementById('hamburger-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const closeMenuBtn = document.getElementById('close-menu-btn');
        const mobileMenuLinks = mobileMenu.querySelectorAll('a');

        const toggleMobileMenu = () => {
            const isHidden = mobileMenu.classList.toggle('hidden');
            hamburgerBtn.setAttribute('aria-expanded', !isHidden);
            mobileMenu.setAttribute('aria-hidden', isHidden);
        };

        hamburgerBtn.addEventListener('click', toggleMobileMenu);
        closeMenuBtn.addEventListener('click', toggleMobileMenu);
        mobileMenuLinks.forEach(link => link.addEventListener('click', toggleMobileMenu));
        document.addEventListener('click', (e) => {
            if (!mobileMenu.classList.contains('hidden') && !mobileMenu.contains(e.target) && e.target !== hamburgerBtn) {
                toggleMobileMenu();
            }
        });

        // Product Data
        const products = [
            { id: "1", name: "Fever Relief Tablets", description: "Relief from fever and pain with fast-acting formula.", price: 150.00, image: "https://images.unsplash.com/photo-1588718889344-f7bd7a565d20?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwxMjA3fDB8MXxzZWFyY2h8NHx8cGlsbHx8MHx8fHwxNjI3NzY0MTAx&ixlib=rb-1.2.1&q=80&w=1080" },
            { id: "2", name: "Digestive Health Capsules", description: "Supports digestive health with natural ingredients.", price: 250.00, image: "https://images.unsplash.com/photo-1667058015056-b03fa4974abf?blend=000000&blend-alpha=10&blend-mode=normal&blend-w=1&crop=faces%2Cedges&h=630&mark=https:%2F%2Fimages.unsplash.com%2Fopengraph%2Flogo.png&mark-align=top%2Cleft&mark-pad=50&mark-w=64&w=1200&auto=format&fit=crop&q=60&ixid=M3wxMjA3fDB8MXxhbGx8fHx8fHx8fHwxNzE4MDYzNTQzfA&ixlib=rb-4.0.3" },
            { id: "3", name: "Immunity Booster Syrup", description: "Boosts immunity with essential vitamins.", price: 300.00, image: "https://media.istockphoto.com/id/1366960245/photo/man-pouring-cough-syrup-into-spoon.webp?b=1&s=170667a&w=0&k=20&c=7BeXjPQEvxu6OFRI7m9fr8i-nlTzEj4zr2_Evt-8cSs=" },
            { id: "4", name: "Vitamin C Tablets", description: "Enhances immunity and promotes healthy skin.", price: 200.00, image: "https://images.unsplash.com/photo-1623066733140-964b08f4cb36?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" },
            { id: "5", name: "Pain Relief Gel", description: "Fast-acting gel for muscle and joint pain relief.", price: 180.00, image: "https://images.unsplash.com/photo-1600585154340-be6161a56a0c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=1080" }
        ];

        // Render Products
        const renderProducts = () => {
            const productGrid = document.getElementById('all-products-grid');
            productGrid.innerHTML = '';
            products.forEach(product => {
                const productCard = document.createElement('div');
                productCard.className = 'bg-white rounded-lg shadow-md p-4 flex flex-col product-card';
                productCard.innerHTML = `
                    <img src="${product.image}" alt="${product.name}" class="rounded-md" loading="lazy">
                    <h3 class="text-lg font-semibold text-gray-800 mt-4 mb-2">${product.name}</h3>
                    <p class="text-gray-600 text-sm mb-2">${product.description}</p>
                    <p class="text-gray-700 font-semibold mb-4">₹${product.price.toFixed(2)}</p>
                    <button class="bg-indigo-500 hover:bg-indigo-600 text-white font-semibold py-2 px-4 rounded-full transition-colors add-to-cart-btn" data-product-id="${product.id}" aria-label="Add ${product.name} to Cart">Add to Cart</button>
                `;
                productGrid.appendChild(productCard);
            });

            productGrid.querySelectorAll('.add-to-cart-btn').forEach(button => {
                button.addEventListener('click', () => addToCart(button));
            });
        };

        // Show All Products Section
        document.querySelectorAll('.shop-now-btn').forEach(button => {
            button.addEventListener('click', (e) => {
                e.preventDefault();
                const allProductsSection = document.getElementById('all-products-section');
                allProductsSection.style.display = 'block';
                renderProducts();
                allProductsSection.scrollIntoView({ behavior: 'smooth' });
            });
        });

        // Smooth Scroll for Anchor Links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', (e) => {
                e.preventDefault();
                const target = document.querySelector(anchor.getAttribute('href'));
                if (target) target.scrollIntoView({ behavior: 'smooth' });
            });
        });

        // Cart Functionality
        let cart = [];
        const hasLocalStorage = isLocalStorageAvailable();
        if (hasLocalStorage) cart = JSON.parse(localStorage.getItem('cart')) || [];

        const saveCart = () => {
            if (hasLocalStorage) {
                try {
                    localStorage.setItem('cart', JSON.stringify(cart));
                } catch (error) {
                    console.warn('Failed to save cart:', error);
                }
            }
        };

        const addToCart = debounce((button) => {
            const productId = button.dataset.productId;
            const product = products.find(p => p.id === productId);
            if (!product) return;

            const itemInCart = cart.find(item => item.id === productId);
            if (itemInCart) {
                itemInCart.quantity += 1;
            } else {
                cart.push({ id: product.id, name: product.name, price: product.price, image: product.image, quantity: 1 });
            }

            saveCart();
            const notification = document.createElement('div');
            notification.className = 'fixed bottom-4 right-4 bg-green-500 text-white px-4 py-2 rounded shadow';
            notification.textContent = `${product.name} added to cart!`;
            document.body.appendChild(notification);
            setTimeout(() => notification.remove(), 3000);
        }, 300);

        document.querySelectorAll('.add-to-cart-btn').forEach(button => {
            button.addEventListener('click', () => addToCart(button));
        });

        // Contact Form Validation
        const contactForm = document.getElementById('contact-form');
        const successMessage = document.getElementById('form-success');

        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            let isValid = true;

            const nameInput = document.getElementById('name');
            const emailInput = document.getElementById('email');
            const messageInput = document.getElementById('message');
            const nameError = document.getElementById('name-error');
            const emailError = document.getElementById('email-error');
            const messageError = document.getElementById('message-error');

            [nameError, emailError, messageError].forEach(error => error.style.display = 'none');
            successMessage.style.display = 'none';

            if (!nameInput.value.trim()) {
                nameError.style.display = 'block';
                isValid = false;
            }
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailInput.value.trim() || !emailRegex.test(emailInput.value.trim())) {
                emailError.style.display = 'block';
                isValid = false;
            }
            if (!messageInput.value.trim()) {
                messageError.style.display = 'block';
                isValid = false;
            }

            if (isValid) {
                console.log('Form submitted:', { name: nameInput.value, email: emailInput.value, message: messageInput.value });
                successMessage.style.display = 'block';
                contactForm.reset();
                setTimeout(() => successMessage.style.display = 'none', 5000);
            }
        });

        // Keyboard Accessibility for Mobile Menu
        mobileMenu.addEventListener('keydown', (e) => {
            if (e.key === 'Escape' && !mobileMenu.classList.contains('hidden')) {
                toggleMobileMenu();
                hamburgerBtn.focus();
            }
        });
    </script>
</body>
</html>