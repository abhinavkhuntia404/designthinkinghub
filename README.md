
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Design Thinking for Students</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Global Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #e7e9f1;
            color: #333;
            line-height: 1.6;
        }

        h1, h2, h3, h4 {
            font-family: 'Roboto', sans-serif;
            font-weight: 700;
            color: #2a2a2a;
            text-transform: uppercase;
        }

        a {
            text-decoration: none;
        }

        /* Header Styling */
        header {
            background: linear-gradient(135deg, #6a11cb, #2575fc);
            color: white;
            padding: 1rem 2rem;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease-in-out;
        }

        header:hover {
            background: linear-gradient(135deg, #2575fc, #6a11cb);
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
            font-family: 'Roboto', sans-serif;
        }

        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: space-between;
        }

        nav ul li {
            margin: 0 1rem;
        }

        nav ul li a {
            color: white;
            font-size: 1.2rem;
            letter-spacing: 0.5px;
            transition: color 0.3s ease;
        }

        nav ul li a:hover {
            color: #ff8c00;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            background: url("C:\Users\prati\Downloads\abhi.jpg") no-repeat center center/cover;
            padding: 4rem 2rem;
            color: black;
            position: relative;
            overflow: hidden;
            animation: fadeIn 2s ease-in-out;
            transition: opacity 1s ease-out;
        }

        .hero h1 {
            text-align: center;
            background: url('desktop-image.jpg') no-repeat center center/cover;
            padding: 4rem 2rem;
            color: white;
            position: relative;
            overflow: hidden;
            animation: fadeIn 2s ease-in-out;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation: slideUp 1s ease-out;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            animation: slideUp 1.5s ease-out;
        }

        .hero a.btn {
            padding: 1rem 2rem;
            background-color: #ff8c00;
            color: white;
            border-radius: 5px;
            font-size: 1.1rem;
            text-transform: uppercase;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .hero a.btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
        }

        /* Section Styles */
        section {
            padding: 3rem 2rem;
            margin: 2rem auto;
            max-width: 1200px;
            background: white;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            animation: fadeIn 2s ease-in-out;
        }

        /* Upcoming Seminars Section */
        .seminars {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            animation: fadeInUp 2s ease-out;
        }

        .seminar-item {
            background-color: #f7f9fc;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .seminar-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .seminar-item h4 {
            font-size: 1.5rem;
            margin: 1rem 0;
        }

        .seminar-item p {
            font-size: 1rem;
            color: #555;
        }

        /* Online Video Resources Section */
        .videos {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            animation: fadeInUp 2s ease-out;
        }

        .video-item {
            background-color: #f7f9fc;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .video-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .video-item h4 {
            font-size: 1.5rem;
            margin: 1rem 0;
        }

        .video-item iframe {
            width: 100%;
            height: 315px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        /* Animations */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Media Queries for responsiveness */
        @media (max-width: 768px) {
            .seminars, .videos {
                grid-template-columns: 1fr;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1.1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Design Thinking Hub</h1>
            <nav>
                <ul>
                    <li><a href="#home"><i class="fas fa-home"></i> Home</a></li>
                    <li><a href="#about"><i class="fas fa-info-circle"></i> About</a></li>
                    <li><a href="#courses"><i class="fas fa-book"></i> Courses</a></li>
                    <li><a href="#resources"><i class="fas fa-tools"></i> Resources</a></li>
                    <li><a href="#videos"><i class="fas fa-video"></i> Videos</a></li>
                    <li><a href="#seminars"><i class="fas fa-calendar"></i> Seminars</a></li>
                    <li><a href="#projects"><i class="fas fa-lightbulb"></i> Projects</a></li>
                    <li><a href="#contact"><i class="fas fa-envelope"></i> Contact</a></li>
                    <li><a href="#contact"><i class="fas fa-envelope"></i> testimonials</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h2>Welcome to Design Thinking Hub</h2>
            <p>Your journey to innovation and creativity begins here. Explore, learn, and transform your ideas into reality.</p>
            <a href="#courses" class="btn">Explore Courses</a>
        </div>
    </section>

    <section id="seminars" class="seminars">
        <div class="container">
            <h2>Upcoming Seminars</h2>
            <div class="seminar-item">
                <h4>Design Thinking 101</h4>
                <p>Date: March 10, 2025 | Time: 10:00 AM</p>
                <p>A foundational seminar on design thinking processes, tools, and case studies.</p>
            </div>
            <div class="seminar-item">
                <h4>Innovation in Engineering</h4>
                <p>Date: April 5, 2025 | Time: 1:00 PM</p>
                <p>Learn how engineering and design thinking can drive innovation in today's world.</p>
            </div>
            <div class="seminar-item">
                <h4>Applying Design Thinking to Business</h4>
                <p>Date: May 15, 2025 | Time: 3:00 PM</p>
                <p>Join us to explore how businesses use design thinking for better problem-solving and product development.</p>
            </div>
        </div>
    </section>

    <section id="videos" class="videos">
        <div class="container">
            <h2>Online Video Resources</h2>
            <div class="video-item">
                <h4>Introduction to Design Thinking</h4>
                <iframe src="https://www.youtube.com/embed/8aGtyTLZ1ck" title="Introduction to Design Thinking"></iframe>
            </div>
            <div class="video-item">
                <h4>Design Thinking Process</h4>
                <iframe src="https://www.youtube.com/embed/0QyA2T9g1P8" title="Design Thinking Process"></iframe>
            </div>
            <div class="video-item">
                <h4>How to Apply Design Thinking in Real Life</h4>
                <iframe src="https://www.youtube.com/embed/U6t0pW6jBck" title="Apply Design Thinking"></iframe>
            </div>
        </div>
    </section>
    <section id="resources" class="resources">
    <div class="container">
        <h2>Design Thinking Resources</h2>

        <!-- Articles Section -->
        <div class="resource-category">
            <h3>Articles</h3>
            <div class="resource-item">
                <h4><a href="https://www.ideou.com/blogs/inspiration/what-is-design-thinking" target="_blank">What is Design Thinking?</a></h4>
                <p>Explore the fundamentals of design thinking and how it's applied to problem-solving in various industries.</p>
            </div>
            <div class="resource-item">
                <h4><a href="https://www.mindtools.com/pages/article/newCT_02.htm" target="_blank">The 5 Stages of Design Thinking</a></h4>
                <p>This article walks you through each stage of the design thinking process and how to apply it to your own projects.</p>
            </div>
        </div>

        <!-- Books Section -->
        <div class="resource-category">
            <h3>Books</h3>
            <div class="resource-item">
                <h4><a href="https://www.amazon.com/Change-Think-Design-Thinking-Problem/dp/0062850908" target="_blank">Change by Design</a></h4>
                <p>Author: Tim Brown. A comprehensive guide to design thinking, with case studies and strategies for innovation.</p>
            </div>
            <div class="resource-item">
                <h4><a href="https://www.amazon.com/Design-Thinking-Human-Centered-Innovation-Strategies/dp/0470877756" target="_blank">Design Thinking: Understanding How Designers Think and Work</a></h4>
                <p>Author: Nigel Cross. A book that introduces the principles and practices behind design thinking, ideal for beginners.</p>
            </div>
        </div>

        <!-- Online Tutorials Section -->
        <div class="resource-category">
            <h3>Online Tutorials</h3>
            <div class="resource-item">
                <h4><a href="https://www.coursera.org/learn/innovation-design-thinking" target="_blank">Coursera: Design Thinking for Innovation</a></h4>
                <p>A free course from the University of Virginia that teaches the design thinking process for driving innovation.</p>
            </div>
            <div class="resource-item">
                <h4><a href="https://www.udemy.com/course/design-thinking/" target="_blank">Udemy: Design Thinking</a></h4>
                <p>An online course on Udemy that covers the design thinking methodology with practical, hands-on exercises.</p>
            </div>
        </div>

        <!-- Tools Section -->
        <div class="resource-category">
            <h3>Design Thinking Tools</h3>
            <div class="resource-item">
                <h4><a href="https://www.miro.com" target="_blank">Miro: Visual Collaboration Platform</a></h4>
                <p>A digital whiteboard tool for visual collaboration, brainstorming, and mapping ideas using design thinking techniques.</p>
            </div>
            <div class="resource-item">
                <h4><a href="https://www.figma.com" target="_blank">Figma: Design and Prototyping Tool</a></h4>
                <p>A cloud-based tool for designing and prototyping user interfaces, commonly used in the design thinking process.</p>
            </div>
        </div>

        <!-- Podcasts Section -->
        <div class="resource-category">
            <h3>Podcasts</h3>
            <div class="resource-item">
                <h4><a href="https://www.designbetter.co/podcast" target="_blank">Design Better Podcast</a></h4>
                <p>A podcast about design thinking, innovation, and leadership in design-driven companies.</p>
            </div>
            <div class="resource-item">
                <h4><a href="https://www.creativebloq.com/inspiration/the-7-best-design-thinking-podcasts" target="_blank">Best Design Thinking Podcasts</a></h4>
                <p>Creative Bloq lists top podcasts that cover design thinking concepts and best practices from design experts.</p>
            </div>
        </div>

    </div>
</section>
 
    <section id="projects" class="projects">
        <div class="container">
            <h2>Student Projects</h2>
            <!-- Projects Section with Categories for Each Engineering Discipline -->
            <div class="project-category">
                <h3>Computer Science</h3>
                <div class="project-list">
                    <div class="project-item">
                        <h4>AI Chatbot</h4>
                        <p>An intelligent chatbot that answers questions based on natural language processing.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Smart Home System</h4>
                        <p>Automating homes using IoT devices and machine learning algorithms.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Blockchain-based Voting</h4>
                        <p>A secure and transparent voting system utilizing blockchain technology.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                </div>
            </div>

            <div class="project-category">
                <h3>Mechanical Engineering</h3>
                <div class="project-list">
                    <div class="project-item">
                        <h4>Automated Drone</h4>
                        <p>A drone that can autonomously navigate and complete tasks like delivery or surveillance.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Hydraulic Arm</h4>
                        <p>A robotic arm powered by hydraulics, capable of lifting heavy objects with precision.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Wind Turbine Efficiency</h4>
                        <p>Optimizing wind turbine designs to increase energy efficiency and reduce costs.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                </div>
            </div>

            <div class="project-category">
                <h3>Chemical Engineering</h3>
                <div class="project-list">
                    <div class="project-item">
                        <h4>Water Filtration System</h4>
                        <p>A low-cost water filtration system that utilizes chemical processes to purify water in rural areas.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Green Energy from Biomass</h4>
                        <p>Developing bioenergy solutions using agricultural waste to produce eco-friendly energy.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                    <div class="project-item">
                        <h4>Carbon Capture Technology</h4>
                        <p>Designing a system to capture and store CO2 emissions to reduce environmental pollution.</p>
                        <a href="#" class="btn">View Project</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="projects" class="submit-project">
        <h2>Submit Your Project</h2>
        <form action="/submit" method="POST" enctype="multipart/form-data">
            <label for="title">Project Title</label>
            <input type="text" id="title" name="title" required>

            <label for="category">Category</label>
            <select id="category" name="category" required>
                <option value="design">Design</option>
                <option value="engineering">Engineering</option>
                <option value="business">Business</option>
                <option value="innovation">Innovation</option>
            </select>

            <label for="description">Project Description</label>
            <textarea id="description" name="description" required></textarea>

            <label for="file">Upload Project File</label>
            <input type="file" id="file" name="file">

            <button type="submit">Submit Project</button>
        </form>
    </section>
     <section id="contact" class="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Have any questions? Reach out to us for more information or feedback.</p>
            <form action="#">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" placeholder="Your Message" rows="4" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>
    <section id="testimonials" class="testimonials">
    <div class="container">
        <h2>What Our Participants Say</h2>
        <div class="testimonial-item">
            <p>"Design Thinking Hub has transformed my approach to problem-solving. The seminars and resources are top-notch!"</p>
            <p><strong>John Doe</strong>, Engineer</p>
        </div>
        <div class="testimonial-item">
            <p>"The hands-on projects and online videos helped me apply Design Thinking in real-world scenarios. Highly recommend!"</p>
            <p><strong>Jane Smith</strong>, Business Owner</p>
        </div>
        <div class="testimonial-item">
            <p>"The seminar on Innovation in Engineering was insightful and gave me practical tools to incorporate into my work."</p>
            <p><strong>Mark Wilson</strong>, Product Designer</p>
        </div>
    </div>
</section>
<section id="newsletter" class="newsletter">
    <div class="container">
        <h2>Stay Updated</h2>
        <p>Subscribe to our newsletter for the latest updates on Design Thinking seminars, projects, and resources.</p>
        <form action="#" method="POST">
            <input type="email" placeholder="Enter your email" required>
            <button type="submit">Subscribe</button>
        </form>
    </div>
</section>
<button class="back-to-top" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
    <i class="fas fa-arrow-up"></i> Back to Top
</button>

<script>
    // Example: Google Analytics Script
    (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
    (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
    m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
    })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');
    ga('create', 'UA-XXXXX-Y', 'auto');
    ga('send', 'pageview');
</script>


    <footer>
        <p>&copy; 2025 Design Thinking Hub. All rights reserved.</p>
    </footer>
 <script>
        window.addEventListener('scroll', function() {
            let heroSection = document.querySelector('.hero');
            if (window.scrollY > 50) {
                heroSection.classList.add('fade-out');
            } else {
                heroSection.classList.remove('fade-out');
            }
        });
    </script>
    <section id="home" class="hero">
    <div class="container">
        <h2>Welcome to Design Thinking Hub</h2>
        <p>Your journey to innovation and creativity begins here. Explore, learn, and transform your ideas into reality.</p>
        <img src="your-image-path.jpg" alt="Hero Image" class="hero-image">
        <a href="#courses" class="btn">Explore Courses</a>
    </div>
</section>
<div class="search-bar">
    <input type="text" placeholder="Search..." id="searchInput">
    <button>Search</button>
</div>

</body>
</html>
