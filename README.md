
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Twin Cities Animal Rescue</title>

    <style>
        :root {
            --primary-color: #2c5f2d;
            --secondary-color: #97bc62;
            --accent-color: #d65a31;
            --text-color: #333333;
            --bg-color: #ffffff;
            --light-bg: #f4f7f1;
        }

        * {
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--bg-color);
        }

        header {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 35px 20px;
        }

        header h1 {
            margin-top: 0;
            margin-bottom: 10px;
        }

        nav {
            background-color: var(--light-bg);
            padding: 12px 20px;
        }

        nav ul {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            list-style: none;
            padding: 0;
            margin: 0;
        }

        nav a {
            color: var(--primary-color);
            text-decoration: none;
            font-weight: bold;
            padding: 8px;
        }

        nav a:hover,
        nav a:focus-visible {
            color: var(--accent-color);
            text-decoration: underline;
        }

        .hero {
            text-align: center;
            padding: 45px 20px;
            background-color: #edf3e7;
        }

        .hero h2 {
            color: var(--primary-color);
            font-size: 2rem;
            margin-top: 0;
        }

        .hero p {
            max-width: 650px;
            margin: 0 auto 20px;
        }

        .button {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            border: none;
            border-radius: 5px;
            padding: 11px 18px;
            font: inherit;
            font-weight: bold;
            text-decoration: none;
            cursor: pointer;
        }

        .button:hover,
        .button:focus-visible {
            background-color: #b94725;
        }

        .button:focus-visible,
        a:focus-visible {
            outline: 3px solid var(--secondary-color);
            outline-offset: 3px;
        }

        main {
            max-width: 1100px;
            margin: 0 auto;
            padding: 25px 20px 45px;
        }

        .section-heading {
            text-align: center;
            color: var(--primary-color);
            margin-bottom: 8px;
        }

        .section-intro {
            text-align: center;
            margin: 0 auto 28px;
            max-width: 650px;
        }

        .animal-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 25px;
        }

        .animal-card {
            border: 1px solid #dddddd;
            border-radius: 10px;
            overflow: hidden;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
        }

        .animal-card img {
            display: block;
            width: 100%;
            height: 240px;
            object-fit: cover;
        }

        .animal-info {
            padding: 20px;
        }

        .animal-info h3 {
            color: var(--primary-color);
            font-size: 1.4rem;
            margin: 0 0 8px;
        }

        .animal-info p {
            margin: 8px 0;
        }

        .pet-tag {
            display: inline-block;
            background-color: #edf3e7;
            color: var(--primary-color);
            border-radius: 20px;
            padding: 4px 10px;
            font-size: 0.9rem;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .animal-info .button {
            margin-top: 12px;
        }

        .services {
            background-color: var(--light-bg);
            border-radius: 10px;
            padding: 25px;
            margin-top: 45px;
        }

        .services h2,
        #contact h2 {
            color: var(--primary-color);
        }

        #contact {
            padding: 30px 0 10px;
            text-align: center;
        }

        footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 20px;
        }

        footer p {
            margin: 5px 0;
        }

        @media (min-width: 600px) {
            nav ul {
                flex-direction: row;
                justify-content: center;
                flex-wrap: wrap;
                gap: 20px;
            }

            .animal-grid {
                grid-template-columns: repeat(2, minmax(0, 1fr));
            }
        }

        @media (min-width: 900px) {
            .animal-grid {
                grid-template-columns: repeat(3, minmax(0, 1fr));
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>Twin Cities Animal Rescue</h1>
        <p>Helping animals find loving homes.</p>
    </header>

    <nav aria-label="Main navigation">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#animals">Available Animals</a></li>
            <li><a href="#services">Our Services</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>

    <section class="hero" id="home">
        <h2>Give an Animal a Second Chance</h2>
        <p>
            Every animal deserves a safe, caring home.
            Meet some of our featured pets and discover how
            you can make a difference through adoption.
        </p>
        <a class="button" href="#animals">Meet Our Animals</a>
    </section>

    <main>
        <section id="animals">
            <h2 class="section-heading">Meet Your New Best Friend</h2>
            <p class="section-intro">
                Browse our featured pets. Each animal has a unique
                personality and is looking for a loving family.
            </p>

            <div class="animal-grid">

                <!-- Dog listing -->
                <article class="animal-card">
                    <img
                        src="https://images.unsplash.com/photo-1552053831-71594a27632d?auto=format&fit=crop&w=800&q=80"
                        alt="Golden retriever sitting outdoors"
                        loading="lazy"
                    >

                    <div class="animal-info">
                        <span class="pet-tag">Dog</span>
                        <h3>Buddy</h3>
                        <p><strong>Age:</strong> 3 years</p>
                        <p><strong>Personality:</strong> Friendly, playful, and enjoys walks.</p>
                        <p>
                            Buddy is a sample listing for a lovable dog
                            who would enjoy an active, caring family.
                        </p>
                        <button
                            class="button"
                            type="button"
                            onclick="showPetInfo('Buddy')">
                            Meet Buddy
                        </button>
                    </div>
                </article>

                <!-- Cat listing -->
                <article class="animal-card">
                    <img
                        src="https://images.unsplash.com/photo-1514888286974-6c03e2ca1dba?auto=format&fit=crop&w=800&q=80"
                        alt="Cat looking toward the camera"
                        loading="lazy"
                    >

                    <div class="animal-info">
                        <span class="pet-tag">Cat</span>
                        <h3>Luna</h3>
                        <p><strong>Age:</strong> 2 years</p>
                        <p><strong>Personality:</strong> Curious, gentle, and affectionate.</p>
                        <p>
                            Luna is a sample listing for a sweet cat
                            who might enjoy a calm and comfortable home.
                        </p>
                        <button
                            class="button"
                            type="button"
                            onclick="showPetInfo('Luna')">
                            Meet Luna
                        </button>
                    </div>
                </article>

                <!-- Dog listing -->
                <article class="animal-card">
                    <img
                        src="https://images.unsplash.com/photo-1543466835-00a7907e9de1?auto=format&fit=crop&w=800&q=80"
                        alt="Happy dog outdoors"
                        loading="lazy"
                    >

                    <div class="animal-info">
                        <span class="pet-tag">Dog</span>
                        <h3>Charlie</h3>
                        <p><strong>Age:</strong> 1 year</p>
                        <p><strong>Personality:</strong> Energetic, cheerful, and curious.</p>
                        <p>
                            Charlie is a sample listing for a young dog
                            who would enjoy playtime and learning new skills.
                        </p>
                        <button
                            class="button"
                            type="button"
                            onclick="showPetInfo('Charlie')">
                            Meet Charlie
                        </button>
                    </div>
                </article>

            </div>
        </section>

        <section class="services" id="services">
            <h2>Our Services</h2>
            <ul>
                <li>Animal adoption information</li>
                <li>Pet care and responsible ownership education</li>
                <li>Community support for animals in need</li>
                <li>Guidance for prospective adopters</li>
            </ul>
        </section>

        <section id="contact">
            <h2>Ready to Adopt?</h2>
            <p>
                Contact our rescue team to learn about adoption
                requirements and currently available animals.
            </p>
            <p>
                Please replace this sample contact section with
                your rescue's real contact information.
            </p>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Twin Cities Animal Rescue</p>
        <p>Every paw deserves a place to call home.</p>
    </footer>

    <script>
        function showPetInfo(petName) {
            alert(
                "Thanks for your interest in " + petName + "!\n\n" +
                "This is a demonstration listing. Please contact " +
                "the rescue team to confirm animal availability and " +
                "learn about the adoption process."
            );
        }
    </script>

</body>
</html>
