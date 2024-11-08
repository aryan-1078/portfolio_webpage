# portfolio_webpage

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aryan Kore - Portfolio</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            line-height: 1.6;
            color: #333;
            background-color: #f5f5f5;
        }

        header {
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .profile-info {
            margin-top: 2rem;
        }

        .profile-info p {
            margin: 0.5rem 0;
        }

        .section {
            background: white;
            padding: 3rem 2rem;
            margin: 2rem 0;
            border-radius: 10px;
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        h2 {
            color: #1e3c72;
            margin-bottom: 1.5rem;
            font-size: 1.8rem;
        }

        .education-item, .project-item {
            margin-bottom: 2rem;
        }

        .education-item h3, .project-item h3 {
            color: #2a5298;
            margin-bottom: 0.5rem;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 1rem;
            margin-top: 1rem;
        }

        .skill-item {
            background: #f8f9fa;
            padding: 1rem;
            border-radius: 5px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .skill-item:hover {
            transform: translateY(-5px);
            background: #e9ecef;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 1rem;
        }

        .contact-info a {
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .project-item ul {
            list-style-type: none;
            padding-left: 1rem;
        }

        .project-item li {
            margin-bottom: 0.5rem;
            position: relative;
        }

        .project-item li::before {
            content: "•";
            color: #1e3c72;
            font-weight: bold;
            position: absolute;
            left: -1rem;
        }

        @media (max-width: 768px) {
            .skills-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .contact-info {
                flex-direction: column;
                align-items: center;
                gap: 1rem;
            }
        }

        #scroll-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #1e3c72;
            color: white;
            width: 40px;
            height: 40px;
            text-align: center;
            line-height: 40px;
            border-radius: 50%;
            cursor: pointer;
            display: none;
            transition: opacity 0.3s ease;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Aryan Kore</h1>
            <div class="profile-info">
                <p>Computer Science Engineering Student</p>
                <div class="contact-info">
                    <a href="mailto:korearyan9@gmail.com">
                        <i class="fas fa-envelope"></i> korearyan9@gmail.com
                    </a>
                    <a href="tel:+919082204137">
                        <i class="fas fa-phone"></i> +91 9082204137
                    </a>
                    <a href="#">
                        <i class="fas fa-map-marker-alt"></i> Thane, Maharashtra
                    </a>
                </div>
            </div>
        </div>
    </header>

    <main class="container">
        <section class="section">
            <h2>Education</h2>
            <div class="education-item">
                <h3>Bachelor of Technology in Computer Science and Engineering</h3>
                <p>Symbiosis Institute of Technology, Pune</p>
                <p>CGPA: 7.65</p>
                <p>2022 - 2026</p>
            </div>
            <div class="education-item">
                <h3>XII - Arya Gurukul International Jr. College</h3>
                <p>Percentage: 86.33%</p>
            </div>
            <div class="education-item">
                <h3>X - DAV Public School</h3>
                <p>Percentage: 95.83%</p>
                <p>2007 - 2022</p>
            </div>
        </section>

        <section class="section">
            <h2>Projects</h2>
            <div class="project-item">
                <h3>Sales Prediction using ML algorithms</h3>
                <ul>
                    <li>Developed a reliable and accurate system for forecasting retail sales using machine learning algorithms</li>
                    <li>Utilized XG Boost and Random Forest algorithms</li>
                    <li>Implemented using Python with NumPy, Pandas, Seaborn, and Matplotlib.Pyplot</li>
                    <li>Key outcome: XGboost showed superior accuracy in point predictions compared to Random Forest model</li>
                </ul>
            </div>
            <div class="project-item">
                <h3>Arduino UNO based Automated Parking Sensor</h3>
                <ul>
                    <li>Created an efficient parking system for vehicle management</li>
                    <li>Implemented vehicle type differentiation using IR sensors</li>
                    <li>Used Arduino UNO, IR Sensors, LEDs, and various hardware components</li>
                    <li>Successfully distinguished between two-wheeler and four-wheeler vehicles based on height and length measurements</li>
                </ul>
            </div>
        </section>

        <section class="section">
            <h2>Skills</h2>
            <div class="skills-grid">
                <div class="skill-item">Python</div>
                <div class="skill-item">C</div>
                <div class="skill-item">DSA</div>
                <div class="skill-item">SQL</div>
                <div class="skill-item">HTML</div>
                <div class="skill-item">Problem-solving</div>
                <div class="skill-item">Creativity</div>
                <div class="skill-item">Time Management</div>
                <div class="skill-item">Eye for Detail</div>
                <div class="skill-item">Leadership</div>
            </div>
        </section>
    </main>

    <div id="scroll-top">
        <i class="fas fa-arrow-up"></i>
    </div>

    <script>
        // Scroll to top button functionality
        const scrollButton = document.getElementById('scroll-top');
        
        window.onscroll = function() {
            if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
                scrollButton.style.display = "block";
            } else {
                scrollButton.style.display = "none";
            }
        };

        scrollButton.addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Add smooth scroll to all links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
