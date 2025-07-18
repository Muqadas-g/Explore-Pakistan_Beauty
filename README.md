# Explore-Pakistan_Beauty
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Explore Pakistan: Nature’s Hidden Treasures</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Hero Section */
        header {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
                url('https://images.unsplash.com/photo-1551632811-561732d1e306?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }

        header h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        header p {
            font-size: 1.2rem;
            max-width: 800px;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background: #4CAF50;
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .btn:hover {
            background: #45a049;
            transform: translateY(-3px);
        }

        /* About Section */
        .about {
            padding: 80px 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            font-size: 2.5rem;
            color: #2c3e50;
        }

        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }

        .about-text {
            flex: 1;
        }

        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Parks Section */
        .parks {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .parks-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .park-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .park-card:hover {
            transform: translateY(-10px);
        }

        .park-image {
            height: 200px;
            overflow: hidden;
        }

        .park-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .park-card:hover .park-image img {
            transform: scale(1.1);
        }

        .park-info {
            padding: 20px;
        }

        .park-info h3 {
            margin-bottom: 10px;
            color: #2c3e50;
        }

        /* Wildlife Section */
        .wildlife {
            padding: 80px 0;
            background-color: white;
        }

        .wildlife-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }

        .wildlife-text {
            flex: 1;
        }

        .wildlife-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .wildlife-image img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Tips Section */
        .tips {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .tips-list {
            max-width: 800px;
            margin: 0 auto;
        }

        .tips-list ol {
            padding-left: 20px;
        }

        .tips-list li {
            margin-bottom: 15px;
        }

        /* Gallery Section */
        .gallery {
            padding: 80px 0;
            background-color: white;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .gallery-item {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .gallery-item:hover {
            transform: scale(1.05);
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }

        /* Contact Section */
        .contact {
            padding: 80px 0;
            background-color: #f5f5f5;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .form-group textarea {
            height: 150px;
        }

        .submit-btn {
            background: #4CAF50;
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 30px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .submit-btn:hover {
            background: #45a049;
        }

        /* Footer */
        footer {
            background: #2c3e50;
            color: white;
            padding: 40px 0;
            text-align: center;
        }

        .social-icons {
            margin: 20px 0;
        }

        .social-icons a {
            color: white;
            font-size: 24px;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        .social-icons a:hover {
            color: #4CAF50;
        }

        .footer-links {
            margin: 20px 0;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: #4CAF50;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }

            .about-content,
            .wildlife-content {
                flex-direction: column;
            }

            .about-image,
            .wildlife-image {
                margin-top: 30px;
            }
        }
    </style>
</head>

<body>
    <!-- Header & Hero Section -->
    <header>
        <div class="container">
            <h1>Explore Pakistan: Nature's Hidden Treasures</h1>
            <p>Discover the breathtaking beauty of Pakistan's national parks, from the towering peaks of the Himalayas
                to the serene valleys and diverse wildlife.</p>
            <a href="#parks" class="btn">Explore Parks</a>
        </div>
    </header>

    <!-- About Section -->
    <section class="about">
        <div class="container">
            <h2 class="section-title">About Pakistan's Nature</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Pakistan is home to some of the most spectacular natural landscapes in the world. From the
                        snow-capped peaks of the Karakoram range to the lush green valleys of Swat and the rugged beauty
                        of Balochistan's deserts, the country offers unparalleled natural diversity.</p>
                    <p>The national parks of Pakistan protect this incredible biodiversity, providing sanctuary to rare
                        species like the snow leopard and markhor, while offering visitors unforgettable experiences in
                        nature.</p>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1588666309990-d68f08e3d4a6?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Pakistan Landscape">
                </div>
            </div>
        </div>
    </section>

    <!-- Parks Section -->
    <section class="parks" id="parks">
        <div class="container">
            <h2 class="section-title">Featured National Parks</h2>
            <div class="parks-grid">
                <!-- Park 1 -->
                <div class="park-card">
                    <div class="park-image">
                        <img src="https://images.unsplash.com/photo-1566438480900-0609be27a4be?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                            alt="Hunza Valley">
                    </div>
                    <div class="park-info">
                        <h3>Hunza Valley</h3>
                        <p>Known for its breathtaking scenery, Hunza Valley offers stunning views of Rakaposhi and Ultar
                            Sar peaks. The valley is famous for its hospitable people, apricot blossoms, and ancient
                            forts.</p>
                    </div>
                </div>

                <!-- Park 2 -->
                <div class="park-card">
                    <div class="park-image">
                        <img src="https://images.unsplash.com/photo-1528164344705-47542687000d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                            alt="Deosai Plains">
                    </div>
                    <div class="park-info">
                        <h3>Deosai Plains</h3>
                        <p>Often called the "Land of Giants," Deosai is the second highest plateau in the world at 4,114
                            meters. In summer, it transforms into a flower-filled meadow with abundant wildlife.</p>
                    </div>
                </div>

                <!-- Park 3 -->
                <div class="park-card">
                    <div class="park-image">
                        <img src="https://images.unsplash.com/photo-1518632618336-313b8b046a1b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                            alt="Margalla Hills">
                    </div>
                    <div class="park-info">
                        <h3>Margalla Hills</h3>
                        <p>Located just north of Islamabad, Margalla Hills National Park offers numerous hiking trails
                            with panoramic views of the capital. It's home to diverse wildlife including leopards and
                            exotic birds.</p>
                    </div>
                </div>

                <!-- Park 4 -->
                <div class="park-card">
                    <div class="park-image">
                        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                            alt="Hingol National Park">
                    </div>
                    <div class="park-info">
                        <h3>Hingol National Park</h3>
                        <p>Pakistan's largest national park features dramatic landscapes from mountains to beaches. It's
                            famous for its mud volcanoes, Princess of Hope rock formation, and diverse wildlife.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Wildlife Section -->
    <section class="wildlife">
        <div class="container">
            <h2 class="section-title">Wildlife & Conservation</h2>
            <div class="wildlife-content">
                <div class="wildlife-text">
                    <p>Pakistan's national parks are home to some of the world's most majestic and endangered species.
                        The snow leopard, Pakistan's national animal, roams the northern mountains, while the markhor,
                        with its spectacular spiral horns, climbs the steep cliffs of the Himalayas.</p>
                    <p>Conservation efforts in Pakistan have helped protect these species and their habitats.
                        Community-based conservation programs have been particularly successful in increasing markhor
                        populations and reducing human-wildlife conflict.</p>
                </div>
                <div class="wildlife-image">
                    <img src="https://images.unsplash.com/photo-1474511320723-9a56873867b5?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Wildlife in Pakistan">
                </div>
            </div>
        </div>
    </section>

    <!-- Tips Section -->
    <section class="tips">
        <div class="container">
            <h2 class="section-title">Eco-Tourism Tips</h2>
            <div class="tips-list">
                <ol>
                    <li><strong>Respect wildlife:</strong> Observe animals from a distance and never feed them.</li>
                    <li><strong>Stay on marked trails:</strong> This protects fragile ecosystems and prevents soil
                        erosion.</li>
                    <li><strong>Pack out all trash:</strong> Leave no trace of your visit to preserve the natural
                        beauty.</li>
                    <li><strong>Support local communities:</strong> Choose local guides and purchase local products.
                    </li>
                    <li><strong>Conserve resources:</strong> Use water sparingly and minimize energy consumption.</li>
                </ol>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery">
        <div class="container">
            <h2 class="section-title">Photo Gallery</h2>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Mountain Landscape">
                </div>
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1470114716159-e389f8712fda?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Forest Trail">
                </div>
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1501854140801-50d01698950b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Autumn Trees">
                </div>
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1433086966358-54859d0ed716?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Waterfall">
                </div>
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Misty Mountains">
                </div>
                <div class="gallery-item">
                    <img src="https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
                        alt="Sunset Landscape">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact">
        <div class="container">
            <h2 class="section-title">Contact Us</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" required></textarea>
                    </div>
                    <button type="submit" class="submit-btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <h3>Explore Pakistan: Nature's Hidden Treasures</h3>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
            <div class="footer-links">
                <a href="#">Home</a>
                <a href="#parks">Parks</a>
                <a href="#wildlife">Wildlife</a>
                <a href="#contact">Contact</a>
            </div>
            <p>&copy; 2023 Explore Pakistan. All rights reserved.</p>
        </div>
    </footer>
</body>

</html>
