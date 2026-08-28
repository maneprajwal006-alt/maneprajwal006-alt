<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Prajwal Mane | Portfolio</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0b0f19;
            color: white;
            line-height: 1.6;
        }

        /* NAVBAR */

        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: #0b0f19;
            border-bottom: 1px solid #263244;
        }

        nav {
            max-width: 1200px;
            margin: auto;
            padding: 18px 20px;

            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
        }

        .logo span {
            color: #00e5ff;
        }

        .nav-links {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: white;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #00e5ff;
        }

        #menu {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 25px;
        }


        /* HERO */

        .hero {
            min-height: 90vh;
            max-width: 1200px;
            margin: auto;

            display: flex;
            justify-content: space-between;
            align-items: center;

            padding: 60px 20px;
        }

        .hero-content {
            max-width: 650px;
        }

        .hello {
            color: #00e5ff;
            font-size: 20px;
        }

        .hero h1 {
            font-size: 65px;
            margin: 10px 0;
        }

        .hero h1 span {
            color: #00e5ff;
        }

        .hero h2 {
            color: #ccc;
            font-size: 25px;
        }

        .hero p {
            color: #aaa;
            margin: 20px 0;
        }

        .buttons {
            display: flex;
            gap: 15px;
            margin: 25px 0;
        }

        .btn {
            text-decoration: none;
            background: #00e5ff;
            color: #061018;

            padding: 12px 25px;
            border-radius: 8px;

            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
        }

        .outline {
            background: transparent;
            color: white;
            border: 1px solid #00e5ff;
        }

        .social {
            display: flex;
            gap: 20px;
        }

        .social a {
            color: #00e5ff;
            text-decoration: none;
        }


        /* PROFILE */

        .profile {
            width: 280px;
            height: 280px;

            border: 5px solid #00e5ff;
            border-radius: 50%;

            display: flex;
            justify-content: center;
            align-items: center;

            font-size: 70px;
            font-weight: bold;

            box-shadow: 0 0 50px rgba(0, 229, 255, 0.3);
        }


        /* SECTIONS */

        section {
            max-width: 1200px;
            margin: auto;
            padding: 90px 20px;
        }

        .title {
            text-align: center;
            font-size: 40px;
            margin-bottom: 50px;
        }

        .title span {
            color: #00e5ff;
        }


        /* ABOUT */

        .about {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 30px;
        }

        .card {
            background: #111827;
            border: 1px solid #263244;
            border-radius: 15px;
            padding: 25px;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: #00e5ff;
        }

        .card h3 {
            color: #00e5ff;
            margin-bottom: 15px;
        }

        .card p {
            color: #aaa;
            margin-bottom: 12px;
        }

        .info {
            display: grid;
            gap: 15px;
        }


        /* SKILLS */

        .skills {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .skill-list {
            list-style: none;
        }

        .skill-list li {
            background: #1a2332;
            padding: 10px;
            margin: 8px 0;
            border-radius: 6px;
        }

        .skill-list li:hover {
            color: #00e5ff;
        }


        /* PROJECTS */

        .projects {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .project {
            background: #111827;
            border: 1px solid #263244;
            padding: 25px;
            border-radius: 15px;
            transition: 0.3s;
        }

        .project:hover {
            transform: translateY(-7px);
            border-color: #00e5ff;
        }

        .project-number {
            font-size: 35px;
            color: #00e5ff;
            font-weight: bold;
        }

        .project h3 {
            font-size: 24px;
            margin: 10px 0;
        }

        .project p {
            color: #aaa;
        }

        .tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 20px 0;
        }

        .tech span {
            border: 1px solid #00e5ff;
            color: #00e5ff;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 13px;
        }

        .project-links {
            display: flex;
            gap: 15px;
        }

        .project-links a {
            text-decoration: none;
            color: white;
            border: 1px solid #555;
            padding: 8px 15px;
            border-radius: 5px;
        }

        .project-links a:hover {
            color: #00e5ff;
            border-color: #00e5ff;
        }


        /* EDUCATION */

        .education {
            max-width: 800px;
            margin: auto;
        }

        .education-box {
            border-left: 3px solid #00e5ff;
            padding: 25px;
            background: #111827;
            border-radius: 10px;
        }

        .education-box h3 {
            color: #00e5ff;
        }

        .education-box p {
            color: #aaa;
            margin-top: 10px;
        }


        /* ACHIEVEMENTS */

        .achievements {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .achievement {
            background: #111827;
            border: 1px solid #263244;
            border-radius: 15px;
            padding: 25px;
            text-align: center;
        }

        .achievement h3 {
            font-size: 35px;
            color: #00e5ff;
        }


        /* GOALS */

        .goals {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .goal {
            background: #111827;
            border: 1px solid #263244;
            border-radius: 15px;
            padding: 25px;
        }

        .goal h3 {
            color: #00e5ff;
        }


        /* CONTACT */

        .contact {
            text-align: center;
        }

        .contact p {
            color: #aaa;
            margin-bottom: 30px;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .contact-links a {
            text-decoration: none;
            color: white;
            background: #111827;
            border: 1px solid #263244;
            padding: 15px 25px;
            border-radius: 10px;
        }

        .contact-links a:hover {
            color: #00e5ff;
            border-color: #00e5ff;
        }


        /* FOOTER */

        footer {
            text-align: center;
            padding: 40px;
            border-top: 1px solid #263244;
        }

        footer span {
            color: #00e5ff;
        }

        footer p {
            color: #777;
            margin-top: 10px;
        }


        /* MOBILE */

        @media (max-width: 768px) {

            .nav-links {
                display: none;

                position: absolute;
                top: 65px;
                left: 0;

                width: 100%;
                background: #0b0f19;

                flex-direction: column;
                text-align: center;

                padding: 20px;
            }

            .nav-links.active {
                display: flex;
            }

            #menu {
                display: block;
            }

            .hero {
                flex-direction: column-reverse;
                text-align: center;
                gap: 40px;
            }

            .hero h1 {
                font-size: 45px;
            }

            .hero h2 {
                font-size: 20px;
            }

            .buttons,
            .social {
                justify-content: center;
            }

            .profile {
                width: 200px;
                height: 200px;
                font-size: 50px;
            }

            .about,
            .skills,
            .projects {
                grid-template-columns: 1fr;
            }

            .achievements {
                grid-template-columns: repeat(2, 1fr);
            }

            .goals {
                grid-template-columns: 1fr;
            }

            .title {
                font-size: 32px;
            }
        }

    </style>
</head>


<body>


<!-- NAVBAR -->

<header>

    <nav>

        <div class="logo">
            Prajwal<span>.</span>
        </div>

        <ul class="nav-links">

            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>

        </ul>

        <button id="menu">☰</button>

    </nav>

</header>



<!-- HOME -->

<section class="hero" id="home">

    <div class="hero-content">

        <div class="hello">
            Hello, I'm
        </div>

        <h1>
            Prajwal <span>Mane</span>
        </h1>

        <h2>
            Computer Science Engineering Student
        </h2>

        <p>
            I am a passionate Computer Science Engineering student
            interested in Web Development, JavaScript, Backend
            Development, Data Structures and Software Development.
        </p>

        <div class="buttons">

            <a href="#projects" class="btn">
                View Projects
            </a>

            <a href="#contact" class="btn outline">
                Contact Me
            </a>

        </div>

        <div class="social">

            <a href="https://github.com/" target="_blank">
                GitHub
            </a>

            <a href="https://linkedin.com/" target="_blank">
                LinkedIn
            </a>

        </div>

    </div>


    <div>

        <div class="profile">
            PM
        </div>

    </div>

</section>



<!-- ABOUT -->

<section id="about">

    <h2 class="title">
        About <span>Me</span>
    </h2>

    <div class="about">

        <div class="card">

            <h3>Who am I?</h3>

            <p>
                I am Prajwal Mane, a B.Tech Computer Science
                Engineering student with a strong interest in
                technology and software development.
            </p>

            <p>
                I enjoy creating websites, learning JavaScript,
                working with APIs and developing practical projects.
            </p>

            <p>
                Currently, I am focusing on backend development,
                programming fundamentals and Data Structures.
            </p>

        </div>


        <div class="info">

            <div class="card">

                <h3>🎓 Education</h3>

                <p>
                    B.Tech – Computer Science Engineering
                </p>

            </div>


            <div class="card">

                <h3>💻 Current Focus</h3>

                <p>
                    JavaScript & Backend Development
                </p>

            </div>


            <div class="card">

                <h3>🚀 Interests</h3>

                <p>
                    Web Development, APIs, DSA and Software Development
                </p>

            </div>

        </div>

    </div>

</section>



<!-- SKILLS -->

<section id="skills">

    <h2 class="title">
        My <span>Skills</span>
    </h2>


    <div class="skills">


        <div class="card">

            <h3>🌐 Web Development</h3>

            <ul class="skill-list">

                <li>HTML</li>
                <li>CSS</li>
                <li>Bootstrap</li>
                <li>JavaScript</li>
                <li>Responsive Web Design</li>

            </ul>

        </div>


        <div class="card">

            <h3>💻 Programming</h3>

            <ul class="skill-list">

                <li>C</li>
                <li>C++</li>
                <li>JavaScript</li>
                <li>Python – Learning</li>
                <li>Java – Learning</li>

            </ul>

        </div>


        <div class="card">

            <h3>🧠 Computer Science</h3>

            <ul class="skill-list">

                <li>Data Structures</li>
                <li>Algorithms</li>
                <li>Object-Oriented Programming</li>
                <li>Problem Solving</li>
                <li>Git & GitHub</li>

            </ul>

        </div>


        <div class="card">

            <h3>⚙️ Currently Learning</h3>

            <ul class="skill-list">

                <li>Advanced JavaScript</li>
                <li>Node.js</li>
                <li>Backend Development</li>
                <li>REST APIs</li>
                <li>Data Structures & Algorithms</li>
                <li>LeetCode</li>

            </ul>

        </div>

    </div>

</section>



<!-- PROJECTS -->

<section id="projects">

    <h2 class="title">
        My <span>Projects</span>
    </h2>


    <div class="projects">


        <!-- PROJECT 1 -->

        <div class="project">

            <div class="project-number">
                01
            </div>

            <h3>
                Apna College Clone
            </h3>

            <p>
                A responsive educational website inspired by
                the Apna College website. Created to practice
                HTML, CSS, Bootstrap and responsive design.
            </p>

            <div class="tech">

                <span>HTML</span>
                <span>CSS</span>
                <span>Bootstrap</span>

            </div>

            <div class="project-links">

                <a href="#" target="_blank">
                    GitHub
                </a>

                <a href="#" target="_blank">
                    Live Demo
                </a>

            </div>

        </div>



        <!-- PROJECT 2 -->

        <div class="project">

            <div class="project-number">
                02
            </div>

            <h3>
                Linktree Clone
            </h3>

            <p>
                A responsive Linktree-style profile website
                containing social media links with a clean
                modern user interface.
            </p>

            <div class="tech">

                <span>HTML</span>
                <span>CSS</span>
                <span>JavaScript</span>

            </div>

            <div class="project-links">

                <a href="#" target="_blank">
                    GitHub
                </a>

                <a href="#" target="_blank">
                    Live Demo
                </a>

            </div>

        </div>



        <!-- PROJECT 3 -->

        <div class="project">

            <div class="project-number">
                03
            </div>

            <h3>
                Weather App
            </h3>

            <p>
                A weather application that uses an API to
                fetch and display weather information.
                Created to practice JavaScript and APIs.
            </p>

            <div class="tech">

                <span>HTML</span>
                <span>CSS</span>
                <span>JavaScript</span>
                <span>API</span>

            </div>

            <div class="project-links">

                <a href="#" target="_blank">
                    GitHub
                </a>

                <a href="#" target="_blank">
                    Live Demo
                </a>

            </div>

        </div>



        <!-- PROJECT 4 -->

        <div class="project">

            <div class="project-number">
                04
            </div>

            <h3>
                Amazon Clone
            </h3>

            <p>
                A frontend e-commerce project created to
                practice webpage layouts, UI design,
                responsiveness and JavaScript.
            </p>

            <div class="tech">

                <span>HTML</span>
                <span>CSS</span>
                <span>JavaScript</span>

            </div>

            <div class="project-links">

                <a href="#" target="_blank">
                    GitHub
                </a>

                <a href="#" target="_blank">
                    Live Demo
                </a>

            </div>

        </div>


    </div>

</section>



<!-- EDUCATION -->

<section id="education">

    <h2 class="title">
        My <span>Education</span>
    </h2>

    <div class="education">

        <div class="education-box">

            <h3>
                B.Tech – Computer Science Engineering
            </h3>

            <h4>
                Ashokrao Mane Group of Institutions
            </h4>

            <p>
                Currently pursuing Computer Science Engineering
                with an interest in software development,
                web technologies and problem solving.
            </p>

        </div>

    </div>

</section>



<!-- ACHIEVEMENTS -->

<section>

    <h2 class="title">
        My <span>Achievements</span>
    </h2>


    <div class="achievements">


        <div class="achievement">

            <h3>9.59</h3>

            <p>
                SGPA
            </p>

        </div>


        <div class="achievement">

            <h3>#1</h3>

            <p>
                Division Rank
            </p>

        </div>


        <div class="achievement">

            <h3>4+</h3>

            <p>
                Projects
            </p>

        </div>


        <div class="achievement">

            <h3>SIH</h3>

            <p>
                Hackathon Interest
            </p>

        </div>


    </div>

</section>



<!-- CERTIFICATE -->

<section>

    <h2 class="title">
        Certificate & <span>Learning</span>
    </h2>


    <div class="card">

        <h3>
            C++ Essentials 1
        </h3>

        <p>
            Cisco Networking Academy
        </p>

        <p>
            Completed C++ fundamentals and programming concepts
            through the Cisco Networking Academy program.
        </p>

    </div>

</section>



<!-- GOALS -->

<section>

    <h2 class="title">
        My <span>Goals</span>
    </h2>


    <div class="goals">


        <div class="goal">

            <h3>01</h3>

            <p>
                Master JavaScript
            </p>

        </div>


        <div class="goal">

            <h3>02</h3>

            <p>
                Learn Backend Development
            </p>

        </div>


        <div class="goal">

            <h3>03</h3>

            <p>
                Strengthen DSA
            </p>

        </div>


        <div class="goal">

            <h3>04</h3>

            <p>
                Build Real-World Projects
            </p>

        </div>


        <div class="goal">

            <h3>05</h3>

            <p>
                Practice LeetCode
            </p>

        </div>


        <div class="goal">

            <h3>06</h3>

            <p>
                Become a Software Developer
            </p>

        </div>


    </div>

</section>



<!-- CONTACT -->

<section id="contact" class="contact">

    <h2 class="title">
        Contact <span>Me</span>
    </h2>

    <p>
        Let's connect, collaborate and build something useful.
    </p>


    <div class="contact-links">

        <a href="mailto:YOUR_EMAIL@gmail.com">
            📧 Email
        </a>

        <a href="https://github.com/YOUR_USERNAME"
           target="_blank">
            💻 GitHub
        </a>

        <a href="https://www.linkedin.com/in/YOUR_USERNAME/"
           target="_blank">
            🔗 LinkedIn
        </a>

    </div>

</section>



<!-- FOOTER -->

<footer>

    <h3>
        Prajwal<span>.</span>
    </h3>

    <p>
        Building • Learning • Improving 🚀
    </p>

    <p>
        © 2026 Prajwal Mane
    </p>

</footer>



<!-- JAVASCRIPT -->

<script>

    const menu = document.getElementById("menu");

    const navLinks = document.querySelector(".nav-links");


    menu.addEventListener("click", function () {

        navLinks.classList.toggle("active");

    });


    document.querySelectorAll(".nav-links a").forEach(function (link) {

        link.addEventListener("click", function () {

            navLinks.classList.remove("active");

        });

    });


</script>


</body>
</html>
