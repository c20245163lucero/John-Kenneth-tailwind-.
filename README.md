<!DOCTYPE html>
<html lang="en" class="dark">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>John Kenneth P. Lucero | Portfolio</title>
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>

    <style type="text/tailwindcss">
        @custom-variant dark (&:where(.dark, .dark *));

        @theme {
            --color-primary: #b91c1c;
        }

        @layer components {
            .btn-primary {
                @apply rounded-lg bg-primary px-6 py-3 font-semibold text-white transition-colors hover:bg-red-700;
            }

            .section-title {
                @apply mb-3 text-3xl font-bold text-slate-900 dark:text-white;
            }

            .card {
                @apply rounded-xl border border-slate-200 bg-white p-6 shadow-sm transition hover:-translate-y-1 hover:shadow-lg dark:border-slate-700 dark:bg-slate-900;
            }

            .form-input {
                @apply w-full rounded-lg border border-slate-300 bg-white px-4 py-3 text-slate-900 outline-none focus:border-red-700 dark:border-slate-700 dark:bg-slate-900 dark:text-white;
            }
        }

        html { scroll-behavior: smooth; }
        body { font-family: Arial, sans-serif; }

        #themeButton {
            transform-origin: center;
        }
    </style>
</head>

<body class="bg-slate-50 text-slate-800 transition-colors dark:bg-slate-950 dark:text-slate-200">

    <header class="sticky top-0 z-50 border-b border-slate-200 bg-white/95 dark:border-slate-800 dark:bg-slate-950/95">
        <nav class="mx-auto flex max-w-6xl items-center justify-between gap-4 px-6 py-4">
            <a href="#home" class="text-xl font-bold text-red-700">
                JK<span class="text-slate-900 dark:text-white">.Portfolio</span>
            </a>

            <ul class="hidden items-center gap-6 text-sm font-medium md:flex">
                <li><a href="#about" class="hover:text-red-700">About</a></li>
                <li><a href="#projects" class="hover:text-red-700">Projects</a></li>
                <li><a href="#services" class="hover:text-red-700">Services</a></li>
                <li><a href="#contact" class="hover:text-red-700">Contact</a></li>
            </ul>

            <button id="themeButton"
                class="rounded-lg border border-slate-300 px-4 py-2 text-sm font-semibold hover:border-red-700 dark:border-slate-700"
                type="button">
                ☀ Light Mode
            </button>
        </nav>
    </header>

    <main>

        <section id="home" class="mx-auto grid max-w-6xl items-center gap-12 px-6 py-20 md:grid-cols-2 md:py-28">
            <div>
                <p class="mb-4 font-semibold uppercase tracking-widest text-red-700">My Portfolio</p>

                <h1 class="text-4xl font-bold leading-tight text-slate-900 dark:text-white md:text-6xl">
                    I'm, <span class="text-red-700">John Kenneth P. Lucero</span>
                </h1>

                <h2 class="mt-4 text-xl font-semibold text-slate-600 dark:text-slate-300">
                    Information Systems Student
                </h2>

                <p class="mt-5 max-w-lg leading-7 text-slate-600 dark:text-slate-400">
                    I am passionate about technology, web development, and creating systems
                    that solve real-world problems. I enjoy learning new skills and improving
                    my programming knowledge.
                </p>

                <div class="mt-8 flex flex-wrap gap-4">
                    <a href="#projects" class="btn-primary">View My Work</a>
                    <a href="#contact"
                        class="rounded-lg border border-slate-300 px-6 py-3 font-semibold hover:border-red-700 hover:text-red-700 dark:border-slate-700">
                        Contact Me
                    </a>
                </div>
            </div>

            <div class="flex justify-center">
                <div
                    class="flex h-64 w-64 items-center justify-center rounded-full border-8 border-red-700 bg-slate-900 shadow-xl md:h-80 md:w-80">
                    <div class="text-center">
                        <p class="text-7xl font-bold text-white md:text-8xl">JK</p>
                        <p class="mt-3 text-sm tracking-widest text-red-400">FUTURE IT PROFESSIONAL</p>
                    </div>
                </div>
            </div>
        </section>


        <section id="about" class="bg-white py-20 dark:bg-slate-900">
            <div class="mx-auto max-w-4xl px-6">
                <p class="mb-2 font-semibold uppercase tracking-widest text-red-700">Get to know me</p>
                <h2 class="section-title">About Me</h2>

                <p class="leading-8 text-slate-600 dark:text-slate-400">
                    My name is John Kenneth P. Lucero, and I am an Information Systems
                    student at Colegio de Sta. Ana de Victorias, Inc. I am interested in
                    web development, system development, and database management. I enjoy
                    exploring technology, solving problems, and learning how to build useful
                    applications. My goal is to improve my technical skills and become a
                    professional who can create reliable and user-friendly information systems.
                </p>

                <h3 class="mb-4 mt-8 text-xl font-bold text-slate-900 dark:text-white">My Skills</h3>

                <div class="flex flex-wrap gap-3">
                    <span
                        class="rounded-full bg-red-100 px-4 py-2 text-sm font-semibold text-red-800 dark:bg-red-950 dark:text-red-300">HTML</span>
                    <span
                        class="rounded-full bg-red-100 px-4 py-2 text-sm font-semibold text-red-800 dark:bg-red-950 dark:text-red-300">CSS</span>
                    <span
                        class="rounded-full bg-red-100 px-4 py-2 text-sm font-semibold text-red-800 dark:bg-red-950 dark:text-red-300">Tailwind
                        CSS</span>
                    <span
                        class="rounded-full bg-red-100 px-4 py-2 text-sm font-semibold text-red-800 dark:bg-red-950 dark:text-red-300">PHP
                        / Laravel</span>
                    <span
                        class="rounded-full bg-red-100 px-4 py-2 text-sm font-semibold text-red-800 dark:bg-red-950 dark:text-red-300">Database
                        Management</span>
                </div>
            </div>
        </section>


        <section id="projects" class="mx-auto max-w-6xl px-6 py-20">
            <p class="mb-2 font-semibold uppercase tracking-widest text-red-700">My Work</p>
            <h2 class="section-title">My Projects</h2>
            <p class="mb-10 text-slate-600 dark:text-slate-400">
                Here are some projects I have worked on or plan to develop.
            </p>

            <div class="grid gap-6 md:grid-cols-3">
                <article class="card">
                    <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">Personal Portfolio</h3>
                    <p class="leading-7 text-slate-600 dark:text-slate-400">
                        A website that introduces me, presents my skills, and showcases my work.
                    </p>
                    <p class="mt-4 text-sm font-semibold text-red-700">HTML · Tailwind CSS · JavaScript</p>
                </article>

                <article class="card">
                    <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">Payroll System</h3>
                    <p class="leading-7 text-slate-600 dark:text-slate-400">
                        A proposed system for organizing employee information and managing salary records.
                    </p>
                    <p class="mt-4 text-sm font-semibold text-red-700">System Development</p>
                </article>

                <article class="card">
                    <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">Digital Canteen System</h3>
                    <p class="leading-7 text-slate-600 dark:text-slate-400">
                        A web-based project designed to let customers view menus and place canteen orders.
                    </p>
                    <p class="mt-4 text-sm font-semibold text-red-700">Web · Database · Ordering</p>
                </article>
            </div>
        </section>


        <section id="services" class="bg-white py-20 dark:bg-slate-900">
            <div class="mx-auto max-w-6xl px-6">
                <p class="mb-2 font-semibold uppercase tracking-widest text-red-700">What I am learning</p>
                <h2 class="section-title">My Services</h2>
                <p class="mb-10 text-slate-600 dark:text-slate-400">
                    Areas where I am building my skills and experience.
                </p>

                <div class="grid gap-6 md:grid-cols-3">
                    <div class="card">
                        <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">Web Development</h3>
                        <p class="leading-7 text-slate-600 dark:text-slate-400">
                            Building simple, responsive, and user-friendly websites.
                        </p>
                    </div>

                    <div class="card">
                        <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">System Development</h3>
                        <p class="leading-7 text-slate-600 dark:text-slate-400">
                            Learning to develop systems that organize information and improve everyday tasks.
                        </p>
                    </div>

                    <div class="card">
                        <h3 class="mb-3 text-xl font-bold text-slate-900 dark:text-white">Database Management</h3>
                        <p class="leading-7 text-slate-600 dark:text-slate-400">
                            Organizing data and learning to create structured databases and relationships.
                        </p>
                    </div>
                </div>
            </div>
        </section>


        <section id="contact" class="mx-auto max-w-3xl px-6 py-20">
            <p class="mb-2 font-semibold uppercase tracking-widest text-red-700">Get in touch</p>
            <h2 class="section-title">Contact Me</h2>
            <p class="mb-8 leading-7 text-slate-600 dark:text-slate-400">
                Have a question or want to discuss a project? Send me a message.
            </p>

            <form id="contactForm" class="space-y-5">
                <div>
                    <label for="name" class="mb-2 block font-semibold">Name</label>
                    <input type="text" id="name" name="name" class="form-input" placeholder="Enter your name" required>
                </div>

                <div>
                    <label for="email" class="mb-2 block font-semibold">Email</label>
                    <input type="email" id="email" name="email" class="form-input" placeholder="Enter your email"
                        required>
                </div>

                <div>
                    <label for="message" class="mb-2 block font-semibold">Message</label>
                    <textarea id="message" name="message" rows="5" class="form-input" placeholder="Write your message"
                        required></textarea>
                </div>

                <button type="submit" class="btn-primary">Send Message</button>
                <p id="formStatus" aria-live="polite" class="text-sm font-medium text-red-700"></p>
            </form>
        </section>
    </main>

    <footer class="border-t border-slate-200 bg-white py-6 text-center dark:border-slate-800 dark:bg-slate-950">
        <p class="text-sm text-slate-500 dark:text-slate-400">
            © 2026 John Kenneth P. Lucero. All rights reserved.
        </p>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/gsap@3.15/dist/gsap.min.js"></script>\
    <script>
        console.log("GSAP version:", gsap.version);


        gsap.to("h1", { x: -200, duration: 1, rotation: 360, scale: 1 }),
        gsap.from("h2", { y: 60, opacity: 0, duration: 1, rotation: 360, scale: 1 });
        gsap.fromto("h1", { opacity: 1, duration: 1, rotation: 360, scale: 1 });

        gsap.from("h1", { y: -60, opacity: 0, duration: 1, ease: "power2 out " });
        gsap.from("h1", { y: -60, opacity: 0, duration: 1, ease: "back out  2.5 " });
        gsap.from("h1", { y: -60, opacity: 0, duration: 1, ease: "bounce  out " });
        gsap.from("h1", { y: -60, opacity: 0, duration: 1, ease: "elastime 1,03 " });

        gsap.from("nav a", { y: -20, opacity: 0, duration: 0.1, ease: "power2 out:stagger : 45 " });

    </script>

    </script>
    <script>
        const tl = gsap.timeline({ defaults: { duration: 0.1, ease: "power2.out" } });
        tl.from("h1", { x: -50, opacity: 0 });
        tl.from("nav a", { y: -30, opacity: 0, stagger: 0.1 });
        tl.from("main section", { y: 50, opacity: 0, stagger: 0.2 });
    </script>

    <script>
        const themeButton = document.getElementById("themeButton");
        const page = document.documentElement;

        themeButton.addEventListener("click", function () {

            themeButton.animate(
                [
                    { transform: "rotate(0deg)" },
                    { transform: "rotate(360deg)" }
                ],
                {
                    duration: 500,
                    easing: "ease-in-out"
                }
            );

            page.classList.toggle("dark");

            if (page.classList.contains("dark")) {
                themeButton.textContent = "☀ Light Mode";
            } else {
                themeButton.textContent = "☾ Dark Mode";
            }
        });

        const contactForm = document.getElementById("contactForm");
        const formStatus = document.getElementById("formStatus");

        contactForm.addEventListener("submit", function (event) {
            event.preventDefault();

            formStatus.textContent =
                "Thank you! Your form was submitted, but a backend is needed to deliver your message.";

            contactForm.reset();
        });
    </script>
</body>

</html>
