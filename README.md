<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Ashoka Women's Engineering College</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap');

  /* Reset & base */
  *, *:before, *:after {
    box-sizing: border-box;
  }
  html {
    font-size: 16px;
    scroll-behavior: smooth;
  }
  body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    line-height: 1.6;
    background: #f9fafb;
    color: #1e293b;
    background-color: #f3f6f8;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  a {
    color: #0c9488;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  a:hover, a:focus {
    color: #065f5b;
    outline: none;
  }
  h1,h2,h3,h4 {
    line-height: 1.2;
    color: #0f172a;
  }

  /* Container with max width and horizontal padding */
  .container {
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
    padding-left: 24px;
    padding-right: 24px;
  }

  /* HEADER */

  header {
    background: #064e54;
    color: white;
    position: sticky;
    top: 0;
    z-index: 200;
    box-shadow: 0 2px 8px rgb(0 0 0 / 0.15);
  }
  .header-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 16px 24px;
  }
  .logo {
    font-weight: 800;
    font-size: 1.5rem;
    color: #a5f3fc;
    user-select: none;
  }
  nav {
    display: flex;
    gap: 24px;
  }
  nav a {
    color: #a5f3fc;
    font-weight: 600;
    padding: 8px 12px;
    border-radius: 8px;
  }
  nav a:hover, nav a:focus {
    background-color: #0e8388;
    color: #d1fae5;
  }


  /* Mobile nav toggle */
  .mobile-menu-button {
    display: none;
    background: none;
    border: none;
    color: #a5f3fc;
    font-size: 1.8rem;
    cursor: pointer;
  }

  /* Mobile nav panel */
  .mobile-nav {
    display: none;
    flex-direction: column;
    background: #064e54;
    padding: 24px 12px;
  }
  .mobile-nav a {
    padding: 12px 16px;
    margin: 4px 0;
    font-weight: 600;
    border-radius: 8px;
  }
  .mobile-nav a:hover, .mobile-nav a:focus {
    background-color: #0e8388;
    color: #d1fae5;
  }

  /* HERO SECTION */

  .hero {
    background: linear-gradient(135deg, #0c9488cc, #135e6166), url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a09d673a-1f2a-4bfe-b6ef-8d3f57260bbe.png') no-repeat center center/cover;
    color: #e0f2f1;
    min-height: 70vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 0 24px;
  }

  .hero-content {
    max-width: 700px;
  }

  .hero h1 {
    font-size: 2.8rem;
    font-weight: 800;
    margin-bottom: 16px;
    text-shadow: 0 0 15px rgba(0, 0, 0, 0.6);
  }
  .hero p {
    font-size: 1.25rem;
    font-weight: 500;
    margin-bottom: 32px;
    text-shadow: 0 0 10px rgba(0, 0, 0, 0.4);
  }
  .hero button {
    background: #14b8a6;
    border: none;
    padding: 16px 32px;
    font-weight: 700;
    color: white;
    font-size: 1.1rem;
    border-radius: 12px;
    cursor: pointer;
    box-shadow: 0 8px 15px rgba(20, 184, 166, 0.6);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .hero button:hover,
  .hero button:focus {
    background: #0f766e;
    box-shadow: 0 12px 25px rgba(15, 118, 110, 0.8);
    transform: translateY(-3px);
    outline: none;
  }

  /* SECTION HEADINGS */
  section h2 {
    font-size: 2.25rem;
    font-weight: 800;
    margin-bottom: 24px;
    color: #064e54;
    text-align: center;
  }

  /* ABOUT SECTION */

  .about-section {
    background: white;
    padding: 72px 24px;
  }
  .about-inner {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 48px;
    max-width: 1100px;
    margin: 0 auto;
    align-items: center;
  }
  .about-inner img {
    width: 100%;
    border-radius: 20px;
    box-shadow: 0 6px 20px rgba(6, 78, 84, 0.12);
    object-fit: cover;
  }
  .about-inner div {
    font-size: 1.1rem;
    line-height: 1.65;
    color: #334155;
  }
  .about-inner div p + p {
    margin-top: 1rem;
  }

  /* COURSES SECTION */

  .courses-section {
    background: #e0f2f1;
    padding: 72px 24px;
  }
  .courses-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px,1fr));
    gap: 32px;
    max-width: 1100px;
    margin: 0 auto;
  }
  .course-card {
    background: white;
    border-radius: 20px;
    padding: 32px 24px;
    box-shadow: 0 4px 16px rgba(6, 78, 84, 0.1);
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: box-shadow 0.3s ease;
  }
  .course-card:hover, .course-card:focus-within {
    box-shadow: 0 8px 32px rgba(20, 184, 166, 0.3);
    outline: none;
  }
  .course-icon {
    font-size: 3.5rem;
    color: #14b8a6;
    margin-bottom: 16px;
  }
  .course-title {
    font-weight: 700;
    font-size: 1.35rem;
    margin-bottom: 12px;
    color: #064e54;
    text-align: center;
  }
  .course-desc {
    text-align: center;
    color: #475569;
    font-weight: 500;
  }

  /* FACULTY SECTION */

  .faculty-section {
    background: white;
    padding: 72px 24px;
  }
  .faculty-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 32px;
    max-width: 1100px;
    margin: 0 auto;
  }
  .faculty-card {
    background: #f1f5f9;
    border-radius: 20px;
    box-shadow: 0 4px 16px rgba(6, 78, 84, 0.1);
    padding: 24px;
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: box-shadow 0.3s ease;
  }
  .faculty-card:hover, .faculty-card:focus-within {
    box-shadow: 0 8px 32px rgba(20, 184, 166, 0.3);
    outline: none;
  }
  .faculty-image {
    width: 120px;
    height: 120px;
    border-radius: 9999px;
    object-fit: cover;
    margin-bottom: 16px;
    box-shadow: 0 3px 15px rgba(6, 78, 84, 0.15);
  }
  .faculty-name {
    font-size: 1.25rem;
    font-weight: 700;
    color: #064e54;
    margin-bottom: 6px;
    text-align: center;
  }
  .faculty-title {
    font-size: 1rem;
    font-weight: 600;
    color: #0f172a;
    margin-bottom: 8px;
    text-align: center;
  }
  .faculty-bio {
    font-size: 0.9rem;
    color: #475569;
    text-align: center;
  }

  /* ADMISSIONS SECTION */

  .admissions-section {
    background: #e0f2f1;
    padding: 72px 24px;
  }
  .admissions-content {
    max-width: 900px;
    margin: 0 auto;
    text-align: center;
  }
  .admissions-content p {
    font-size: 1.15rem;
    margin-bottom: 36px;
    color: #334155;
  }
  .admissions-button {
    background-color: #14b8a6;
    border: none;
    padding: 18px 42px;
    font-weight: 700;
    color: white;
    font-size: 1.1rem;
    border-radius: 14px;
    cursor: pointer;
    box-shadow: 0 8px 15px rgba(20, 184, 166, 0.6);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .admissions-button:hover,
  .admissions-button:focus {
    background-color: #0f766e;
    box-shadow: 0 12px 25px rgba(15, 118, 110, 0.8);
    transform: translateY(-3px);
    outline: none;
  }

  /* EVENTS & NEWS */

  .events-section {
    background: white;
    padding: 72px 24px;
  }
  .events-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 32px;
    max-width: 1100px;
    margin: 0 auto;
  }
  .event-card {
    border-radius: 20px;
    box-shadow: 0 4px 12px rgba(6, 78, 84, 0.1);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    background: #f1f5f9;
    transition: box-shadow 0.3s ease;
  }
  .event-card:hover, .event-card:focus-within {
    box-shadow: 0 8px 24px rgba(20, 184, 166, 0.3);
    outline: none;
  }
  .event-image {
    width: 100%;
    height: 180px;
    object-fit: cover;
  }
  .event-content {
    padding: 20px 24px;
  }
  .event-title {
    font-size: 1.25rem;
    font-weight: 700;
    margin-bottom: 8px;
    color: #064e54;
  }
  .event-date {
    font-size: 0.95rem;
    color: #0f766e;
    font-weight: 600;
    margin-bottom: 12px;
  }
  .event-description {
    font-size: 1rem;
    color: #475569;
  }

  /* TESTIMONIALS */

  .testimonials-section {
    background: #e0f2f1;
    padding: 72px 24px;
  }
  .testimonials-list {
    max-width: 900px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 32px;
  }
  .testimonial {
    background: white;
    border-radius: 20px;
    box-shadow: 0 4px 16px rgba(6, 78, 84, 0.1);
    padding: 32px 24px;
    font-style: italic;
    position: relative;
  }
  .testimonial::before {
    content: "“";
    position: absolute;
    font-size: 6rem;
    color: #14b8a6;
    left: 18px;
    top: 8px;
    font-weight: 900;
    line-height: 1;
    font-family: serif;
  }
  .testimonial-text {
    font-size: 1.15rem;
    color: #334155;
    margin-bottom: 16px;
    padding-left: 36px;
  }
  .testimonial-author {
    font-weight: 700;
    font-size: 1.05rem;
    color: #064e54;
    text-align: right;
    font-style: normal;
    padding-right: 18px;
  }

  /* CONTACT SECTION */

  .contact-section {
    background: white;
    padding: 72px 24px;
  }
  .contact-inner {
    max-width: 900px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 48px;
  }
  .contact-info {
    color: #334155;
  }
  .contact-info h3 {
    font-weight: 700;
    font-size: 1.5rem;
    margin-bottom: 16px;
    color: #064e54;
  }
  .contact-info p {
    margin-bottom: 12px;
    font-size: 1.1rem;
  }
  .contact-info a {
    color: #0c9488;
    font-weight: 600;
  }
  form.contact-form {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .contact-form label {
    font-weight: 600;
    color: #475569;
  }
  .contact-form input,
  .contact-form textarea {
    font-family: 'Inter', sans-serif;
    font-size: 1rem;
    padding: 12px 16px;
    border: 2px solid #d1d5db;
    border-radius: 12px;
    transition: border-color 0.3s ease;
    resize: vertical;
  }
  .contact-form input:focus,
  .contact-form textarea:focus {
    outline: none;
    border-color: #14b8a6;
  }
  .contact-form button {
    width: max-content;
    background-color: #14b8a6;
    border: none;
    padding: 14px 42px;
    font-weight: 700;
    color: white;
    font-size: 1.1rem;
    border-radius: 14px;
    cursor: pointer;
    box-shadow: 0 8px 15px rgba(20, 184, 166, 0.6);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .contact-form button:hover,
  .contact-form button:focus {
    background-color: #0f766e;
    box-shadow: 0 12px 25px rgba(15, 118, 110, 0.8);
    transform: translateY(-3px);
    outline: none;
  }

  /* FOOTER */

  footer {
    background: #064e54;
    color: #a5f3fc;
    padding: 32px 24px;
    margin-top: auto;
    font-size: 0.9rem;
    text-align: center;
  }
  footer a {
    color: #a5f3fc;
    font-weight: 600;
    margin: 0 8px;
  }
  footer a:hover,
  footer a:focus {
    color: #d1fae5;
    outline: none;
  }
  .footer-links {
    margin-bottom: 12px;
  }

  /* Responsive */

  @media (max-width: 1024px) {
    .about-inner {
      grid-template-columns: 1fr;
      text-align: center;
    }
    .faculty-grid,
    .courses-grid,
    .events-grid {
      grid-template-columns: 1fr 1fr;
    }
    .contact-inner {
      grid-template-columns: 1fr;
    }
  }
  @media (max-width: 640px) {
    nav {
      display: none;
    }
    .mobile-menu-button {
      display: block;
    }
    .mobile-nav.show {
      display: flex;
    }
    .faculty-grid,
    .courses-grid,
    .events-grid {
      grid-template-columns: 1fr;
    }
    .hero h1 {
      font-size: 2rem;
    }
  }

</style>
</head>
<body>

<header>
  <div class="header-inner container">
    <div class="logo" tabindex="0">Ashoka Women's Engineering College</div>
    <nav role="navigation" aria-label="Primary Navigation">
      <a href="#about">About</a>
      <a href="#courses">Courses</a>
      <a href="#faculty">Faculty</a>
      <a href="#admissions">Admissions</a>
      <a href="#events">Events</a>
      <a href="#testimonials">Testimonials</a>
      <a href="#contact">Contact</a>
    </nav>
    <button class="mobile-menu-button" aria-label="Toggle menu" aria-expanded="false" aria-controls="mobile-menu">&#9776;</button>
  </div>
  <nav id="mobile-menu" class="mobile-nav" role="navigation" aria-label="Mobile Primary Navigation">
    <a href="#about" tabindex="-1">About</a>
    <a href="#courses" tabindex="-1">Courses</a>
    <a href="#faculty" tabindex="-1">Faculty</a>
    <a href="#admissions" tabindex="-1">Admissions</a>
    <a href="#events" tabindex="-1">Events</a>
    <a href="#testimonials" tabindex="-1">Testimonials</a>
    <a href="#contact" tabindex="-1">Contact</a>
  </nav>
</header>

<main>
  <section class="hero" aria-label="College introduction">
    <div class="hero-content">
      <h1>Empowering Women Through Engineering Excellence</h1>
      <p>At Ashoka Women's Engineering College, we nurture innovation, diversity, and leadership in technology for a better tomorrow.</p>
      <button onclick="location.href='#admissions'" aria-label="Go to admissions section">Apply Now</button>
    </div>
  </section>

  <section id="about" class="about-section" tabindex="0" aria-label="About Ashoka Women's Engineering College">
    <div class="about-inner">
      <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1d88e58a-e4b5-474a-b40b-654ce4f4dd4f.png" alt="Modern campus building surrounded by greenery at Ashoka Women's Engineering College" />
      <div>
        <h2>About Us</h2>
        <p>Ashoka Women's Engineering College is committed to fostering a supportive and innovative environment where women engineers thrive. Established with a vision to empower women in technology, our college offers world-class education, state-of-the-art facilities, and strong industry connections.</p>
        <p>Our curriculum balances rigorous academic programs with hands-on experience, preparing students for successful careers in engineering disciplines.</p>
      </div>
    </div>
  </section>

  <section id="courses" class="courses-section" tabindex="0" aria-label="Engineering courses offered">
    <h2>Our Courses</h2>
    <div class="courses-grid">
      <article class="course-card" tabindex="0" aria-labelledby="course-cse-title">
        <div class="course-icon" aria-hidden="true">💻</div>
        <h3 id="course-cse-title" class="course-title">Computer Science & Engineering</h3>
        <p class="course-desc">Learn cutting-edge computing concepts, software development, and AI technologies to drive innovation in the digital world.</p>
      </article>
      <article class="course-card" tabindex="0" aria-labelledby="course-ece-title">
        <div class="course-icon" aria-hidden="true">📡</div>
        <h3 id="course-ece-title" class="course-title">Electronics & Communication Engineering</h3>
        <p class="course-desc">Explore integrated electronics, communications systems, and embedded technologies powering modern devices.</p>
      </article>
      <article class="course-card" tabindex="0" aria-labelledby="course-mech-title">
        <div class="course-icon" aria-hidden="true">⚙️</div>
        <h3 id="course-mech-title" class="course-title">Mechanical Engineering</h3>
        <p class="course-desc">Design, analyze, and build mechanical systems, robotics, and manufacturing technologies that shape industries.</p>
      </article>
      <article class="course-card" tabindex="0" aria-labelledby="course-civil-title">
        <div class="course-icon" aria-hidden="true">🏗️</div>
        <h3 id="course-civil-title" class="course-title">Civil Engineering</h3>
        <p class="course-desc">Develop sustainable infrastructure solutions and master modern construction technologies.</p>
      </article>
      <article class="course-card" tabindex="0" aria-labelledby="course-it-title">
        <div class="course-icon" aria-hidden="true">🖥️</div>
        <h3 id="course-it-title" class="course-title">Information Technology</h3>
        <p class="course-desc">Focus on software infrastructure, data management, and cybersecurity in the digital age.</p>
      </article>
    </div>
  </section>

  <section id="faculty" class="faculty-section" tabindex="0" aria-label="Faculty members">
    <h2>Meet Our Faculty</h2>
    <div class="faculty-grid">
      <article class="faculty-card" tabindex="0" aria-labelledby="faculty-1-name">
        <img class="faculty-image" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/10b40628-4f88-4538-8c5f-ee270941de37.png" alt="Photo of Professor Asha, Head of Computer Science Department" />
        <h3 id="faculty-1-name" class="faculty-name">Prof. Asha Verma</h3>
        <p class="faculty-title">Head of Computer Science Department</p>
        <p class="faculty-bio">Expert in artificial intelligence and machine learning with over 15 years of teaching and research experience.</p>
      </article>
      <article class="faculty-card" tabindex="0" aria-labelledby="faculty-2-name">
        <img class="faculty-image" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/12babdbe-2c46-4c30-bda5-16b0810ec7d1.png" alt="Photo of Dr. Neha Singh, Senior Lecturer in Electronics" />
        <h3 id="faculty-2-name" class="faculty-name">Dr. Neha Singh</h3>
        <p class="faculty-title">Senior Lecturer - Electronics & Communication</p>
        <p class="faculty-bio">Specializes in wireless communication systems and IoT applications, contributing extensively to academic journals.</p>
      </article>
      <article class="faculty-card" tabindex="0" aria-labelledby="faculty-3-name">
        <img class="faculty-image" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/1b078fd9-4e03-4e03-998a-dfb8c5899981.png" alt="Photo of Dr. Priya Sharma, Mechanical Engineering Faculty" />
        <h3 id="faculty-3-name" class="faculty-name">Dr. Priya Sharma</h3>
        <p class="faculty-title">Associate Professor - Mechanical Engineering</p>
        <p class="faculty-bio">Researching sustainable mechanical design and renewable energy solutions, passionate about mentoring students.</p>
      </article>
    </div>
  </section>

  <section id="admissions" class="admissions-section" tabindex="0" aria-label="Admissions information">
    <h2>Admissions</h2>
    <div class="admissions-content">
      <p>Join Ashoka Women's Engineering College and become a part of a vibrant community poised to shape the future of engineering. We offer undergraduate and postgraduate courses with a strong emphasis on innovation and hands-on learning.</p>
      <p>Applications for the 2025 academic year are open. Apply today to start your journey!</p>
      <button onclick="location.href='#contact'" aria-label="Contact admissions">Contact Admissions</button>
    </div>
  </section>

  <section id="events" class="events-section" tabindex="0" aria-label="Events and news">
    <h2>Upcoming Events & News</h2>
    <div class="events-grid">
      <article class="event-card" tabindex="0" aria-labelledby="event1-title">
        <img class="event-image" src="https://ticktocktech.com/wp-content/uploads/2023/01/Biggest-tech-conferences-2023.jpg" alt="Poster banner for Tech Symposium 2024 event" />
        <div class="event-content">
          <h3 id="event1-title" class="event-title">Tech Symposium 2024</h3>
          <p class="event-date" aria-label="Date: March 7, 2024">March 7, 2024</p>
          <p class="event-description">A day-long symposium featuring innovations from students and leading engineers to spark collaboration and inspiration.</p>
        </div>
      </article>
      <article class="event-card" tabindex="0" aria-labelledby="event2-title">
        <img class="event-image" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c5766730-9089-467e-a461-ba59e7f4c317.png" alt="Banner image of Annual Cultural Fest showing students performing on stage" />
        <div class="event-content">
          <h3 id="event2-title" class="event-title">Annual Cultural Fest 2024</h3>
          <p class="event-date" aria-label="Date: February 20 to 22, 2024">Feb 20–22, 2024</p>
          <p class="event-description">Celebrating creativity and unity with music, dance, and tech exhibitions promoting student talents.</p>
        </div>
      </article>
    </div>
  </section>

  <section id="testimonials" class="testimonials-section" tabindex="0" aria-label="Student testimonials">
    <h2>What Our Students Say</h2>
    <div class="testimonials-list">
      <blockquote class="testimonial" tabindex="0">
        <p class="testimonial-text">Ashoka Women's Engineering College provided me with the skills and confidence to succeed. The faculty's support and the state-of-the-art facilities empower every day.</p>
        <footer class="testimonial-author">– Simran Kaur, Computer Science Graduate</footer>
      </blockquote>
      <blockquote class="testimonial" tabindex="0">
        <p class="testimonial-text">The environment here is truly empowering and inclusive. It’s a place where women engineers thrive and break new ground.</p>
        <footer class="testimonial-author">– Anjali Mehta, Electronics & Communication Student</footer>
      </blockquote>
    </div>
  </section>

  <section id="contact" class="contact-section" tabindex="0" aria-label="Contact Ashoka Women's Engineering College">
    <h2>Contact Us</h2>
    <div class="contact-inner">
      <div class="contact-info">
        <h3>College Address</h3>
        <p>Ashoka Women's Engineering College</p>
        <p>123 Academic Lane</p>
        <p>Dupadu(518002),kurnool,Andhrapradesh</p>
        <p>Phone: <a href="tel:+1234567890">(123) 456-7890</a></p>
        <p>Email: <a href="mailto:info@ashokawomenengineering.edu">info@ashokawomenengineering.edu</a></p>
        <p>Website: <a href="https://www.ashokawomenengineering.edu" target="_blank" rel="noopener noreferrer">www.ashokawomenengineering.edu</a></p>
      </div>
      <form class="contact-form" action="#" method="post" aria-label="Contact form">
        <label for="name">Full Name</label>
        <input id="name" name="name" type="text" required autocomplete="name" placeholder="Your full name" />
        <label for="email">Email Address</label>
        <input id="email" name="email" type="email" required autocomplete="email" placeholder="you@example.com" />
        <label for="message">Message</label>
        <textarea id="message" name="message" rows="4" required placeholder="Write your message here..."></textarea>
        <button type="submit" aria-label="Send message to Ashoka Women's Engineering College">Send Message</button>
      </form>
    </div>
  </section>

</main>

<footer>
  <div class="footer-links">
    <a href="#about">About</a> | 
    <a href="#courses">Courses</a> | 
    <a href="#faculty">Faculty</a> | 
    <a href="#admissions">Admissions</a> | 
    <a href="#events">Events</a> | 
    <a href="#contact">Contact</a>
  </div>
  <div>© 2024 Ashoka Women's Engineering College. All rights reserved.</div>
</footer>

<script>
  // Mobile menu toggle
  const mobileBtn = document.querySelector('.mobile-menu-button');
  const mobileNav = document.getElementById('mobile-menu');

  mobileBtn.addEventListener('click', () => {
    const expanded = mobileBtn.getAttribute('aria-expanded') === 'true' || false;
    mobileBtn.setAttribute('aria-expanded', !expanded);
    mobileNav.classList.toggle('show');
    
    const links = mobileNav.querySelectorAll('a');
    if (mobileNav.classList.contains('show')) {
      // Make links keyboard focusable in mobile menu open state
      links.forEach(link => link.setAttribute('tabindex', '0'));
      links[0].focus();
    } else {
      // Make links unfocusable when menu closed
      links.forEach(link => link.setAttribute('tabindex', '-1'));
    }
  });
</script>

</body>
</html>

```
