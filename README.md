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
            background-color: #f9f9f9;
        }

        header {
            background-color: #2c3e50;
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 40px;
        }

        header nav a {
            color: white;
            margin-left: 20px;
            text-decoration: none;
            font-size: 1.1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #18bc9c;
        }

        .hero {
            text-align: center;
            background: linear-gradient(to right, #2c3e50, #18bc9c);
            color: white;
            padding: 100px 20px;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        .hero button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 15px 40px;
            cursor: pointer;
            font-size: 1.2rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .hero button:hover {
            background-color: #1abc9c;
        }

        section {
            padding: 60px 20px;
            text-align: center;
        }

        .about {
            background-color: #ffffff;
            margin: 20px auto;
            border-radius: 10px;
            padding: 40px;
            max-width: 900px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
        }

        .about h2 {
            font-size: 2rem;
            margin-bottom: 20px;
        }

        .about p {
            font-size: 1.1rem;
            line-height: 1.6;
            color: #555;
        }

        .services, .quote {
            background-color: #f4f4f4;
            margin: 20px auto;
            border-radius: 10px;
            padding: 40px;
            max-width: 900px;
        }

        .service-cards {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }

        .card {
            background-color: white;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 250px;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .card h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        .card p {
            font-size: 0.95rem;
            color: #666;
        }

        .quote form {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }

        .quote input, .quote select, .quote textarea {
            padding: 10px;
            width: 80%;
            max-width: 400px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .quote button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 15px 40px;
            cursor: pointer;
            font-size: 1.1rem;
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
            padding: 20px;
            font-size: 0.9rem;
        }
    </style>
    <script>
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
                Quote Request from Elite Floor Finishers:
                ---------------------------------------
                Name: ${name}
                Email: ${email}
                Phone: ${phone}
                Rooms: ${rooms}
                Type: ${type}
                Square Footage: ${squareFootage}
                Additional Details: ${details}
                ---------------------------------------
                `;

                window.location.href = `mailto:christiansinchi1@hotmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
            });
        });

        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({ behavior: 'smooth' });
        }
    </script>
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
    <section id="about" class="about">
        <h2>About Us</h2>
        <p>Christian Sinchi co-founded Elite Floor Finishers with a mission to provide exceptional flooring solutions. After years of searching for a business that showcased his talent for selling, he discovered flooring services—a job that sells itself. Customers who want beautiful, durable floors know they can trust us to deliver the best results at the best prices.</p>
        <p>As a family-owned and operated business, we stand by our work for a lifetime, ensuring you receive the best quality and service. Whether it’s your garage, basement, or custom space, we’ve got you covered with our trusted expertise.</p>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
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
            <select id="rooms" name="rooms">
                <option value="" disabled selected>Number of rooms?</option>
                <option value="one">One</option>
                <option value="two">Two</option>
                <option value="three">Three or more</option>
            </select>
            <select id="type" name="type">
                <option value="" disabled selected>Garage or basement?</option>
                <option value="garage">Garage</option>
                <option value="basement">Basement</option>
                <option value="both">Both</option>
            </select>
            <select id="squareFootage" name="squareFootage">
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
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p><strong>Christian Sinchi</strong></p>
        <p>Phone: 1 (347) 702-2499</p>
        <p>Email: christiansinchi1@hotmail.com</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2024 Elite Floor Finishers. All Rights Reserved.</p>
    </footer>
</body>
</html>
