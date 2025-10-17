<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Style Edit | Fashion Blog & Boutique</title>
    <!-- Load Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Use Inter font and configure custom colors -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'primary': '#4a4e69', // Deep Purple/Slate
                        'accent': '#ffb7c3',  // Soft Rose Pink
                        'background': '#f4f4f8',
                        'text-dark': '#1e1e24',
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom styles for a touch of elegance */
        .card-shadow {
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        .card-shadow:hover {
            transform: translateY(-4px);
        }
    </style>
</head>
<body class="bg-background text-text-dark font-sans">

    <!-- Header & Navigation -->
    <header class="bg-white sticky top-0 z-10 shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <a href="#" class="text-3xl font-serif font-bold text-primary tracking-wider">
                The Style Edit
            </a>

            <!-- Desktop Navigation -->
            <nav class="hidden md:flex space-x-8 text-lg font-medium">
                <a href="#blog" class="hover:text-accent transition duration-150">Blog</a>
                <a href="#shop" class="hover:text-accent transition duration-150">Shop</a>
                <a href="#" class="hover:text-accent transition duration-150">About</a>
                <a href="#" class="text-accent border-2 border-accent px-3 py-1 rounded-full hover:bg-accent hover:text-white transition duration-200">
                    Cart (0)
                </a>
            </nav>

            <!-- Mobile Menu Button -->
            <button id="mobile-menu-button" class="md:hidden text-primary focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
            </button>
        </div>

        <!-- Mobile Menu (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden">
            <nav class="px-2 pt-2 pb-3 space-y-1 sm:px-3 text-center bg-gray-50 border-t border-gray-200">
                <a href="#blog" class="block py-2 text-primary hover:bg-gray-200 rounded-lg">Blog</a>
                <a href="#shop" class="block py-2 text-primary hover:bg-gray-200 rounded-lg">Shop</a>
                <a href="#" class="block py-2 text-primary hover:bg-gray-200 rounded-lg">About</a>
                <a href="#" class="block py-2 text-accent bg-accent/10 border border-accent rounded-lg">Cart (0)</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="bg-white py-16 md:py-24">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <h1 class="text-5xl md:text-7xl font-serif font-extrabold text-primary mb-4">
                Timeless Style, Curated Daily.
            </h1>
            <p class="text-xl md:text-2xl text-gray-600 mb-8 max-w-3xl mx-auto">
                Discover the latest trends and shop our exclusive collection of sustainable, high-quality fashion staples.
            </p>
            <a href="#shop" class="inline-block bg-accent text-white text-lg font-medium py-3 px-8 rounded-full card-shadow hover:bg-pink-400 transition duration-300 transform hover:scale-105">
                Explore the Collection
            </a>
        </div>
    </section>

    <!-- Blog Section -->
    <section id="blog" class="py-16 bg-background">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-4xl font-serif font-bold text-center mb-12 text-primary">Latest Features & Insights</h2>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-10">

                <!-- Blog Post 1 -->
                <article class="bg-white rounded-xl overflow-hidden card-shadow">
                    <img src="https://placehold.co/600x400/DCCCE8/555?text=FW+24+Lookbook" alt="Fall/Winter Lookbook" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <span class="text-sm text-gray-500 font-medium uppercase tracking-wider">October 17, 2025</span>
                        <h3 class="text-2xl font-serif font-bold text-text-dark my-2 hover:text-accent cursor-pointer">
                            The Cozy Revolution: Must-Have Knitwear
                        </h3>
                        <p class="text-gray-600 line-clamp-3 mb-4">
                            Knitwear is back and bolder than ever. We dive into the sustainable sources and luxurious textures that define the Fall/Winter 2024 season...
                        </p>
                        <a href="#" class="text-primary font-medium hover:text-accent">Read Full Article &rarr;</a>
                    </div>
                </article>

                <!-- Blog Post 2 -->
                <article class="bg-white rounded-xl overflow-hidden card-shadow">
                    <img src="https://placehold.co/600x400/96BBE0/555?text=Denim+Guide" alt="Denim Style Guide" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <span class="text-sm text-gray-500 font-medium uppercase tracking-wider">October 10, 2025</span>
                        <h3 class="text-2xl font-serif font-bold text-text-dark my-2 hover:text-accent cursor-pointer">
                            Your Ultimate Guide to Sustainable Denim
                        </h3>
                        <p class="text-gray-600 line-clamp-3 mb-4">
                            Finding the perfect pair of jeans is an art. This guide covers cuts, washes, and the brands committed to eco-friendly production...
                        </p>
                        <a href="#" class="text-primary font-medium hover:text-accent">Read Full Article &rarr;</a>
                    </div>
                </article>

                <!-- Blog Post 3 -->
                <article class="bg-white rounded-xl overflow-hidden card-shadow">
                    <img src="https://placehold.co/600x400/E5E5E0/555?text=Accessory+Trends" alt="Accessory Trends" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <span class="text-sm text-gray-500 font-medium uppercase tracking-wider">October 1, 2025</span>
                        <h3 class="text-2xl font-serif font-bold text-text-dark my-2 hover:text-accent cursor-pointer">
                            The Mini-Bag Renaissance: Size Doesn't Matter
                        </h3>
                        <p class="text-gray-600 line-clamp-3 mb-4">
                            Small bags are having a huge moment. We show you how to style the season's hottest micro-accessories for maximum impact...
                        </p>
                        <a href="#" class="text-primary font-medium hover:text-accent">Read Full Article &rarr;</a>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- Shop Section -->
    <section id="shop" class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <h2 class="text-4xl font-serif font-bold text-center mb-12 text-primary">Shop Our Curated Boutique</h2>

            <div class="grid grid-cols-2 md:grid-cols-4 gap-6 md:gap-8">

                <!-- Product 1: The Silk Slip Dress -->
                <div class="bg-background rounded-lg overflow-hidden card-shadow p-4 text-center">
                    <img src="https://placehold.co/400x500/F5C8CB/333?text=Silk+Slip" alt="Silk Slip Dress" class="w-full h-64 object-cover rounded-lg mb-4">
                    <h3 class="text-lg font-semibold text-text-dark">The Luxe Silk Slip</h3>
                    <p class="text-primary font-bold text-xl my-2">$149.00</p>
                    <button onclick="addToCart('The Luxe Silk Slip')" class="w-full bg-primary text-white py-2 rounded-full text-sm hover:bg-primary/90 transition duration-150 transform hover:scale-[1.02]">
                        Add to Bag
                    </button>
                </div>

                <!-- Product 2: Cropped Knit Cardigan -->
                <div class="bg-background rounded-lg overflow-hidden card-shadow p-4 text-center">
                    <img src="https://placehold.co/400x500/E8DCCC/333?text=Knit+Cardigan" alt="Cropped Knit Cardigan" class="w-full h-64 object-cover rounded-lg mb-4">
                    <h3 class="text-lg font-semibold text-text-dark">Cropped Knit Cardigan</h3>
                    <p class="text-primary font-bold text-xl my-2">$75.00</p>
                    <button onclick="addToCart('Cropped Knit Cardigan')" class="w-full bg-primary text-white py-2 rounded-full text-sm hover:bg-primary/90 transition duration-150 transform hover:scale-[1.02]">
                        Add to Bag
                    </button>
                </div>

                <!-- Product 3: High-Rise Trousers -->
                <div class="bg-background rounded-lg overflow-hidden card-shadow p-4 text-center">
                    <img src="https://placehold.co/400x500/B8B8D1/333?text=Tailored+Trousers" alt="High-Rise Trousers" class="w-full h-64 object-cover rounded-lg mb-4">
                    <h3 class="text-lg font-semibold text-text-dark">Tailored High-Rise Trouser</h3>
                    <p class="text-primary font-bold text-xl my-2">$99.00</p>
                    <button onclick="addToCart('Tailored High-Rise Trouser')" class="w-full bg-primary text-white py-2 rounded-full text-sm hover:bg-primary/90 transition duration-150 transform hover:scale-[1.02]">
                        Add to Bag
                    </button>
                </div>

                <!-- Product 4: Minimalist Gold Necklace -->
                <div class="bg-background rounded-lg overflow-hidden card-shadow p-4 text-center">
                    <img src="https://placehold.co/400x500/F4E181/333?text=Gold+Necklace" alt="Minimalist Gold Necklace" class="w-full h-64 object-cover rounded-lg mb-4">
                    <h3 class="text-lg font-semibold text-text-dark">Minimalist Gold Necklace</h3>
                    <p class="text-primary font-bold text-xl my-2">$55.00</p>
                    <button onclick="addToCart('Minimalist Gold Necklace')" class="w-full bg-primary text-white py-2 rounded-full text-sm hover:bg-primary/90 transition duration-150 transform hover:scale-[1.02]">
                        Add to Bag
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Notification Message Box -->
    <div id="notification-box" class="fixed bottom-5 right-5 p-4 rounded-lg bg-green-500 text-white shadow-xl transition-opacity duration-300 opacity-0 z-50">
        <!-- Notification text goes here -->
    </div>

    <!-- Footer -->
    <footer class="bg-primary text-white py-12 mt-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center md:flex md:justify-between md:items-center">
            <div class="mb-6 md:mb-0">
                <p class="text-xl font-serif font-bold mb-2">The Style Edit</p>
                <p class="text-sm text-gray-300">&copy; 2025 All Rights Reserved. | Fashion & Commerce</p>
            </div>
            <div class="space-x-6 text-sm">
                <a href="#" class="hover:text-accent transition duration-150">Privacy Policy</a>
                <a href="#" class="hover:text-accent transition duration-150">Terms of Use</a>
                <a href="#" class="hover:text-accent transition duration-150">Contact</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript for interactivity -->
    <script>
        // --- Mobile Menu Toggle ---
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // --- Simple Add to Cart Logic (using a message box instead of alert) ---
        function addToCart(productName) {
            const notificationBox = document.getElementById('notification-box');
            
            // 1. Update Cart Display (Mock)
            const cartNav = document.querySelector('a[href="#"].text-accent');
            let currentCount = parseInt(cartNav.textContent.match(/\((\d+)\)/)[1]);
            currentCount++;
            cartNav.textContent = `Cart (${currentCount})`;

            // 2. Show Notification
            notificationBox.textContent = `${productName} added to your bag!`;
            notificationBox.classList.add('opacity-100');
            notificationBox.classList.add('translate-y-0');
            
            // 3. Hide after 3 seconds
            setTimeout(() => {
                notificationBox.classList.remove('opacity-100');
                notificationBox.classList.remove('translate-y-0');
            }, 3000);
        }
    </script>
</body>
</html>
