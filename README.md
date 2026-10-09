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
            background: #f4f6f8;
            color: #222;
            line-height: 1.6;
            transition: 0.3s;
        }


        body.dark {
            background: #121826;
            color: #f4f4f4;
        }

        header {
            background: #1e293b;
            color: white;
            padding: 20px 8%;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
        }

        nav h2 {
            font-size: 22px;
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: 0.3s;
        }

        nav a:hover {
            color: #38bdf8;
        }

        button {
            padding: 10px 16px;
            border: none;
            border-radius: 6px;
            background: #2563eb;
            color: white;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            background: #1d4ed8;
        }


        .hero {
            text-align: center;
            padding: 80px 20px;
            background: #e0f2fe;
        }

        .dark .hero {
            background: #1e293b;
        }

        .hero h1 {
            font-size: 42px;
            margin-bottom: 15px;
        }

        .hero h1 span {
            color: #2563eb;
        }

        .hero p {
            max-width: 600px;
            margin: 0 auto 25px;
            color: #475569;
        }

        .dark .hero p {
            color: #cbd5e1;
        }


        main {
            max-width: 1100px;
            margin: 40px auto;
            padding: 0 20px;
        }

        section {
            margin-bottom: 30px;
            padding: 30px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.06);
        }

        .dark section {
            background: #1e293b;
        }

        section h2 {
            margin-bottom: 15px;
            color: #2563eb;
        }


        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 20px;
        }

        .card {
            padding: 20px;
            background: #f1f5f9;
            border-radius: 8px;
        }

        .dark .card {
            background: #334155;
        }

        .card h3 {
            margin-bottom: 8px;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        input,
        textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            font: inherit;
            background: white;
            color: #222;
        }

        textarea {
            resize: vertical;
        }

        .dark input,
        .dark textarea {
            background: #334155;
            color: white;
            border-color: #475569;
        }

        form button {
            align-self: flex-start;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #1e293b;
            color: white;
        }


        @media (max-width: 700px) {
            nav {
                flex-direction: column;
            }

            nav ul {
                flex-wrap: wrap;
                justify-content: center;
                gap: 15px;
            }

            .hero h1 {
                font-size: 32px;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            section {
                padding: 20px;
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

            <button id="switch" type="button">Dark Mode</button>
        </nav>
    </header>


    <div class="hero">
        <h1>Hello, I'm <span>John Kenneth P. Lucero</span></h1>
        <p>
            I create websites, build systems, manage databases,
            and develop solutions that help businesses grow.
        </p>
        <a href="#contact">
            <button type="button">Work With Me</button>
        </a>
    </div>

    <main>


        <section id="projects">
            <h2>My Projects</h2>
            <p>Here are some of the projects I work on.</p>

            <div class="cards">
                <div class="card">
                    <h3>Personal Portfolio</h3>
                    <p>A website showcasing skills and experience.</p>
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
            <p>Solutions designed to meet your business needs.</p>

            <div class="cards">
                <div class="card">
                    <h3>Web Development</h3>
                    <p>Modern and responsive website creation.</p>
                </div>

                <div class="card">
                    <h3>System Development</h3>
                    <p>Custom systems for business operations.</p>
                </div>

                <div class="card">
                    <h3>AI Automation</h3>
                    <p>Automating repetitive tasks and workflows.</p>
                </div>

                <div class="card">
                    <h3>Database Management</h3>
                    <p>Organizing and maintaining business data.</p>
                </div>

                <div class="card">
                    <h3>Project Management</h3>
                    <p>Planning and coordinating project activities.</p>
                </div>

                <div class="card">
                    <h3>Systems Analysis</h3>
                    <p>Analyzing business needs and system requirements.</p>
                </div>
            </div>
        </section>


        <section id="contact">
            <h2>Let's Build Together!</h2>
            <p>Have a project in mind? Send me a message.</p>

            <form id="contactForm">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" rows="5" placeholder="Write your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>

            <p id="formStatus" aria-live="polite"></p>
        </section>

    </main>


    <footer>
        <p>&copy; 2026 John Kenneth P. Lucero. All rights reserved.</p>
    </footer>

    <script>
        // Dark and light mode switch
        const switchButton = document.getElementById("switch");

        switchButton.addEventListener("click", function () {
            document.body.classList.toggle("dark");

            if (document.body.classList.contains("dark")) {
                switchButton.textContent = "Light Mode";
            } else {
                switchButton.textContent = "Dark Mode";
            }
        });


        document.getElementById("contactForm")
            .addEventListener("submit", function (event) {
                event.preventDefault();

                document.getElementById("formStatus").textContent =
                    "Thank you! Your form is ready, but a backend is needed to deliver your message.";

                this.reset();
            });
    </script>

</body>

</html>
