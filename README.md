```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>John Kenneth P. Lucero | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #111827;
            color: #f9fafb;
            line-height: 1.6;
        }

        header {
            padding: 20px 8%;
            background: #030712;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
        }

        nav ul {
            display: flex;
            gap: 20px;
            list-style: none;
        }

        a {
            color: #60a5fa;
            text-decoration: none;
        }

        nav a {
            color: white;
        }

        a:hover {
            color: #38bdf8;
        }

        button {
            padding: 10px 15px;
            background: #2563eb;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background: #1d4ed8;
        }

        .hero {
            text-align: center;
            padding: 70px 20px;
            background: #1f2937;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero span {
            color: #60a5fa;
        }

        .hero p {
            margin: 0 auto 20px;
            max-width: 550px;
            color: #d1d5db;
        }

        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 0 20px;
        }

        section {
            margin-bottom: 25px;
            padding: 25px;
            background: #1f2937;
            border-radius: 8px;
        }

        section h2 {
            color: #60a5fa;
            margin-bottom: 10px;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 20px;
        }

        .card {
            padding: 18px;
            background: #374151;
            border-radius: 6px;
        }

        .card h3 {
            margin-bottom: 8px;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 15px;
        }

        input,
        textarea {
            padding: 12px;
            border: 1px solid #4b5563;
            border-radius: 5px;
            background: #111827;
            color: white;
            font: inherit;
        }

        textarea {
            resize: vertical;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #030712;
        }

        /* Light mode */
        body.light {
            background: #f3f4f6;
            color: #111827;
        }

        .light header,
        .light footer {
            background: #e5e7eb;
        }

        .light nav a {
            color: #111827;
        }

        .light .hero,
        .light section {
            background: white;
        }

        .light .hero p {
            color: #4b5563;
        }

        .light .card {
            background: #e5e7eb;
        }

        .light input,
        .light textarea {
            background: white;
            color: #111827;
            border-color: #d1d5db;
        }

        @media (max-width: 700px) {
            nav {
                flex-direction: column;
            }

            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }

            .hero h1 {
                font-size: 28px;
            }

            .cards {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>

    <header>
        <nav>
            <h2>JKL Portfolio</h2>

            <ul>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

            <button id="themeButton" type="button">
                Light Mode
            </button>
        </nav>
    </header>

    <div class="hero">
        <h1>Hello, I'm <span>John Kenneth P. Lucero</span></h1>
        <p>
            I create websites, develop systems, and manage databases
            to help solve business problems.
        </p>
        <a href="#contact">
            <button type="button">Contact Me</button>
        </a>
    </div>

    <main>

        <section id="projects">
            <h2>My Projects</h2>
            <p>Some of my development projects.</p>

            <div class="cards">
                <div class="card">
                    <h3>Personal Portfolio</h3>
                    <p>A website that presents my skills and work.</p>
                </div>

                <div class="card">
                    <h3>Payroll System</h3>
                    <p>A system for managing employee salaries.</p>
                </div>

                <div class="card">
                    <h3>Compliance Monitoring</h3>
                    <p>A system for tracking compliance requirements.</p>
                </div>
            </div>
        </section>

        <section id="services">
            <h2>My Services</h2>

            <div class="cards">
                <div class="card">
                    <h3>Web Development</h3>
                    <p>Creating responsive websites.</p>
                </div>

                <div class="card">
                    <h3>System Development</h3>
                    <p>Building systems for business needs.</p>
                </div>

                <div class="card">
                    <h3>Database Management</h3>
                    <p>Organizing and managing data.</p>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>Contact Me</h2>
            <p>Have a project in mind? Send me a message.</p>

            <form id="contactForm">
                <label for="name">Name</label>
                <input type="text" id="name" placeholder="Enter your name" required>

                <label for="email">Email</label>
                <input type="email" id="email" placeholder="Enter your email" required>

                <label for="message">Message</label>
                <textarea id="message" rows="4" placeholder="Write your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>

            <p id="formStatus" aria-live="polite"></p>
        </section>

    </main>

    <footer>
        <p>&copy; 2026 John Kenneth P. Lucero. </p>
    </footer>

    <script>
        // Switch between dark and light mode
        const themeButton = document.getElementById("themeButton");

        themeButton.addEventListener("click", function () {
            document.body.classList.toggle("light");

            themeButton.textContent =
                document.body.classList.contains("light")
                    ? "Dark Mode"
                    : "Light Mode";
        });

        // Contact form message
        document.getElementById("contactForm")
            .addEventListener("submit", function (event) {
                event.preventDefault();

                document.getElementById("formStatus").textContent =
                    "Thank you! A backend is needed to deliver your message.";

                this.reset();
            });
    </script>

</body>

</html>
```
