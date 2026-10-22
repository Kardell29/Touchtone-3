
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twin Cities Animal Rescue</title>
    <style>
        /* Base Styles (Mobile First) */
        :root {
            --primary-color: #2c5f2d;
            --secondary-color: #97bc62;
            --accent-color: #d65a31;
            --text-color: #333333;
            --bg-color: #ffffff;
        }

        body {
            font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--bg-color);
            margin: 0;
        }

        header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav ul {
            display: flex;
            flex-direction: column;
            list-style: none;
            padding: 0;
            gap: 10px;
        }

        nav a {
            color: var(--primary-color);
            text-decoration: none;
            font-weight: bold;
        }

        main {
            padding: 20px;
        }

        button {
            background-color: var(--accent-color);
            color: white;
            border: none;
            padding: 10px 16px;
            cursor: pointer;
            border-radius: 4px;
        }

        @media (min-width: 768px) {
            nav ul {
                flex-direction: row;
                justify-content: space-around;
            }

            main {
                max-width: 900px;
                margin: 0 auto;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Twin Cities Animal Rescue</h1>
        <p>Helping animals find loving homes.</p>
    </header>

    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#animals">Available Animals</a></li>
            <li><a href="#services">Our Services</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>

    <main id="home">
        <h2>Give an Animal a Second Chance</h2>
        <p>We help animals find safe, caring, and permanent homes.</p>
        <button onclick="alert('Thank you for supporting animal rescue!')">
            Learn More
        </button>

        <section id="animals">
            <h2>Available Animals</h2>
            <p>Meet the animals waiting for their forever homes.</p>
        </section>

        <section id="services">
            <h2>Our Services</h2>
            <p>Adoption support, animal care, and community education.</p>
        </section>

        <section id="contact">
            <h2>Contact Us</h2>
            <p>Get in touch to learn about adoption opportunities.</p>
        </section>
    </main>
</body>
</html>
