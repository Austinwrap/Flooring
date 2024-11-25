<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Floor Finishers</title>
    <style>
        /* General Reset */
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background: #000;
            background-image: radial-gradient(circle, #fff 1px, transparent 1px),
                              radial-gradient(circle, #18bc9c 1px, transparent 1px),
                              radial-gradient(circle, #3498db 1px, transparent 1px),
                              radial-gradient(circle, #f39c12 1px, transparent 1px),
                              radial-gradient(circle, #e74c3c 1px, transparent 1px);
            background-size: 80px 80px;
            background-position: 0 0, 40px 40px, 20px 60px, 60px 20px, 30px 70px;
            color: white;
            overflow-x: hidden;
        }

        header {
            background-color: #2c3e50;
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        header nav a {
            color: white;
            margin-left: 15px;
            text-decoration: none;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #18bc9c;
        }

        .hero {
            text-align: center;
            background: linear-gradient(to right, #2c3e50, #18bc9c);
            color: white;
            padding: 80px 20px;
        }

        .hero h2 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1rem;
            margin-bottom: 20px;
        }

        .hero button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 10px 30px;
            cursor: pointer;
            font-size: 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .hero button:hover {
            background-color: #1abc9c;
        }

        section {
            padding: 40px 15px;
            text-align: center;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            margin: 15px auto;
            max-width: 90%;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
            color: #333;
        }

        .services .service-cards {
            display: flex;
            flex-direction: column;
            gap: 20px;
            align-items: center;
        }

        .card {
            background-color: white;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            padding: 15px;
            width: 100%;
            max-width: 300px;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .card h3 {
            font-size: 1.1rem;
            margin-bottom: 8px;
        }

        .card p {
            font-size: 0.9rem;
            color: #666;
        }

        .quote form {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }

        .quote input,
        .quote select,
        .quote textarea {
            padding: 8px;
            width: 100%;
            max-width: 300px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 0.9rem;
        }

        .quote select {
            height: 35px;
        }

        .quote textarea {
            height: 60px;
        }

        .quote button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 10px 30px;
            cursor: pointer;
            font-size: 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .quote button:hover {
            background-color: #1abc9c;
        }

        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 0.8rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header nav a {
                font-size: 0.9rem;
                margin-left: 10px;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 0.9rem;
            }

            .hero button {
                font-size: 0.9rem;
                padding: 10px 25px;
            }

            .card {
                max-width: 90%;
            }

            .quote input,
            .quote select,
            .quote textarea {
                font-size: 0.85rem;
                padding: 8px;
            }

            footer {
                font-size: 0.75rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="logo">
            <h1>Elite Floor Finishers</h1>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About Us</a>
            <a href="#services">Services</a>
            <a href="#free-quote">Free Quote</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h2>Transforming Floors, Transforming Spaces</h2>
        <p>Premium garage & basement floor coatings for Hartford County.</p>
        <button onclick="scrollToSection('free-quote')">Get a Free Quote</button>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Us</h2>
        <p>Christian Sinchi co-founded Elite Floor Finishers with a mission to provide exceptional flooring solutions. After years of searching for a business that showcased his talent for selling, he discovered flooring services—a job that sells itself. Customers who want beautiful, durable floors know they can trust us to deliver the best results at the best prices.</p>
        <p>As a family-owned and operated business, we stand by our work for a lifetime, ensuring you receive the best quality and service. Whether it’s your garage, basement, or custom space, we’ve got you covered with our trusted expertise.</p>
    </section>

    <!-- Services Section -->
    <section id="services">
        <h2>Our Services</h2>
        <div class="service-cards">
            <div class="card">
                <h3>Garage Floors</h3>
                <p>Durable, sleek finishes for any garage.</p>
            </div>
            <div class="card">
                <h3>Basement Floors</h3>
                <p>Transform your basement into a functional, modern space.</p>
            </div>
            <div class="card">
                <h3>Custom Finishes</h3>
                <p>Decorative flakes & unique designs available.</p>
            </div>
        </div>
    </section>

    <!-- Free Quote Section -->
    <section id="free-quote" class="quote">
        <h2>Free Quote</h2>
        <form id="quoteForm">
            <input type="text" id="name" name="name" placeholder="Your Name" required>
            <input type="email" id="email" name="email" placeholder="Your Email" required>
            <input type="tel" id="phone" name="phone" placeholder="Your Phone" required>
            <select id="rooms" name="rooms" required>
                <option value="" disabled selected>Number of rooms?</option>
                <option value="one">One</option>
                <option value="two">Two</option>
                <option value="three">Three or more</option>
            </select>
            <select id="type" name="type" required>
                <option value="" disabled selected>Garage or basement?</option>
                <option value="garage">Garage</option>
                <option value="basement">Basement</option>
                <option value="both">Both</option>
            </select>
            <select id="squareFootage" name="squareFootage" required>
                <option value="" disabled selected>Square footage?</option>
                <option value="less100">Less than 100 sq. ft.</option>
                <option value="100to500">100–500 sq. ft.</option>
                <option value="500plus">500+ sq. ft.</option>
            </select>
            <textarea id="details" name="details" placeholder="Additional details (optional)"></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p><strong>Christian Sinchi</strong></p>
        <p>Phone: 1 (347) 702-2499</p>
        <p>Email: christiansinchi1@hotmail.com</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2024 Elite Floor Finishers. All Rights Reserved.</p>
    </footer>

    <!-- Script -->
    <script>
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({ behavior: 'smooth' });
        }

        document.addEventListener('DOMContentLoaded', () => {
            document.getElementById('quoteForm').addEventListener('submit', function (e) {
                e.preventDefault();
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const phone = document.getElementById('phone').value;
                const rooms = document.getElementById('rooms').value;
                const type = document.getElementById('type').value;
                const squareFootage = document.getElementById('squareFootage').value;
                const details = document.getElementById('details').value;

                const subject = `Quote Request from ${name}`;
                const body = `
                Name: ${name}\n
                Email: ${email}\n
                Phone: ${phone}\n
                Rooms: ${rooms}\n
                Type: ${type}\n
                Square Footage: ${squareFootage}\n
                Details: ${details}\n
                `;
                window.location.href = `mailto:christiansinchi1@hotmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
            });
        });
    </script>
</body>
</html>
