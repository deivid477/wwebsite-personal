<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Full Stack Developer Portfolio</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');
  * {
    margin: 0; padding: 0; box-sizing: border-box;
  }
  body {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #1f1c2c, #928dab);
    color: #eee;
    min-height: 100vh;
    scroll-behavior: smooth;
  }
  header {
    background: rgba(0,0,0,0.7);
    padding: 1rem 2rem;
    position: fixed;
    width: 100%;
    top: 0; left: 0;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0,0,0,0.5);
  }
  header nav {
    display: flex; justify-content: center; gap: 2.5rem;
  }
  header nav a {
    text-decoration: none;
    color: #eee;
    font-weight: 600;
    font-size: 1.1rem;
    position: relative;
  }
  header nav a::after {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    background: #8bc6ec;
    left: 0;
    bottom: -4px;
    transition: 0.3s ease width;
  }
  header nav a:hover::after {
    width: 100%;
  }

  main {
    padding-top: 5rem;
    max-width: 900px;
    margin: 0 auto;
  }
  section {
    margin: 5rem 1rem;
    text-align: center;
  }
  h1, h2 {
    font-weight: 600;
  }
  h1 {
    font-size: 3rem;
    margin-bottom: 0.5rem;
    color: #8bc6ec;
    text-shadow: 0 0 10px #3a8ddd;
  }
  h2 {
    font-size: 2rem;
    margin-bottom: 0.8rem;
  }
  p.lead {
    font-size: 1.2rem;
    color: #ccc;
    max-width: 600px;
    margin: 0 auto 3rem auto;
  }

  /* Skills */
  .skills-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 2rem;
  }
  .skill-card {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 15px;
    width: 140px;
    height: 140px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    cursor: default;
    box-shadow: 0 0 20px rgba(139, 198, 236, 0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    position: relative;
  }
  .skill-card:hover {
    transform: translateY(-15px);
    box-shadow: 0 8px 30px rgba(139, 198, 236, 0.7);
  }
  .skill-icon {
    font-size: 3.5rem;
    margin-bottom: 0.6rem;
    color: #8bc6ec;
  }
  .skill-name {
    font-weight: 600;
    font-size: 1.2rem;
    color: #8bc6ec;
  }

  /* Animation */
  .fadeInUp {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeInUpAnim 1s forwards;
  }
  .fadeInUp.delay-1 {
    animation-delay: 0.3s;
  }
  .fadeInUp.delay-2 {
    animation-delay: 0.6s;
  }
  .fadeInUp.delay-3 {
    animation-delay: 0.9s;
  }
  .fadeInUp.delay-4 {
    animation-delay: 1.2s;
  }
  .fadeInUp.delay-5 {
    animation-delay: 1.5s;
  }
  @keyframes fadeInUpAnim {
    to {
      opacity: 1; 
      transform: translateY(0);
    }
  }

  /* Contact Section */
  .contact-btn {
    background: #8bc6ec;
    color: #1f1c2c;
    border: none;
    padding: 1rem 2rem;
    font-weight: 600;
    font-size: 1.1rem;
    border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 0 15px #8bc6ec;
    transition: background 0.3s ease, box-shadow 0.3s ease;
    text-decoration: none;
    display: inline-block;
  }
  .contact-btn:hover {
    background: #66b3f3;
    box-shadow: 0 0 25px #66b3f3;
  }

  /* Footer */
  footer {
    text-align: center;
    padding: 1rem 0;
    background: rgba(0,0,0,0.7);
    color: #aaa;
    font-size: 0.85rem;
    position: fixed;
    bottom: 0; left: 0; right: 0;
  }

  /* Responsive */
  @media (max-width: 600px) {
    .skills-container {
      justify-content: center;
      gap: 1.3rem;
    }
    .skill-card {
      width: 110px;
      height: 110px;
      font-size: 0.9rem;
    }
    h1 {
      font-size: 2.2rem;
    }
    h2 {
      font-size: 1.5rem;
    }
  }
</style>
</head>
<body>
<header>
  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<main>
  <section id="about" class="fadeInUp delay-1">
    <h1>Hello,I'm David qava wijaya</h1>
    <p class="lead">A passionate Full Stack Developer crafting clean, modern, and responsive web and software solutions with expertise in frontend and backend technologies.</p>
  </section>

  <section id="skills" class="fadeInUp delay-2">
    <h2>My Skills</h2>
    <div class="skills-container">
      <div class="skill-card" title="CSS">
        <svg class="skill-icon" xmlns="http://www.w3.org/2000/svg" fill="#8bc6ec" viewBox="0 0 24 24" width="48" height="48"><path d="M1.5 0h21l-1.91 21.562L12 24l-8.585-2.438L1.5 0zM19 6.612l-.062.697-1.851 20.7L12 23.61v-7.073h4.68l-.122-1.11h-4.56v-2.704h6.184l-.184 2.07H14.4v2.932l3.453-.97 1.007-11.406z"/></svg>
        <div class="skill-name">CSS</div>
      </div>
      <div class="skill-card" title="JavaScript">
        <svg class="skill-icon" xmlns="http://www.w3.org/2000/svg" fill="#8bc6ec" viewBox="0 0 24 24" width="48" height="48"><path d="M12 0C5.372 0 0 5.372 0 12c0 6.627 5.372 12 12 12 6.626 0 12-5.373 12-12C24 5.372 18.626.001 12 0zm3.817 17.496c-.746 1.237-2.395 1.81-3.92 1.53-1.904-.364-2.93-1.955-3.182-3.615h2.067c.134.829.781 1.457 1.923 1.352 1.052-.1 1.598-.685 1.956-1.354-.03-.83-1.022-1.166-1.812-1.42l-1.012-.37c-1.58-.576-2.583-1.785-2.566-3.72 0-2.17 1.658-4.11 4.777-3.713 2.086.254 3.571 1.34 4.277 2.941l-2.032 1.2c-.36-.645-.745-1.208-1.57-1.412-1.14-.295-1.929.62-1.929 1.22 0 .445.341.927 1.145 1.29l1.009.394c1.7.685 2.592 1.883 2.565 3.792-.011 1.178-.915 2.11-2.212 2.495z"/></svg>
        <div class="skill-name">JavaScript</div>
      </div>
      <div class="skill-card" title="Python">
        <svg class="skill-icon" xmlns="http://www.w3.org/2000/svg" fill="#8bc6ec" viewBox="0 0 24 24" width="48" height="48"><path d="M12 0c-6.63 0-12 5.37-12 12 0 6.62 5.37 12 12 12 6.63 0 12-5.38 12-12 0-6.63-5.37-12-12-12zm-1.293 6.414c.265.372.287.907.287 1.293v2h-6v2h6v4.346c0 .386-.02.92-.287 1.293-1.733-1.68-3.34-3.765-4.112-6.632-.04-.144-.078-.285-.11-.427H10.56c.026.078.048.164.054.25.12 1.84 1.027 3.396 2.492 4.44-.03-.214-.05-.43-.05-.65V12c0-.686.555-1.242 1.242-1.242h2v-2h-2c-.954 0-1.742.788-1.742 1.742v.67c-.025-.218-.05-.43-.05-.645 0-.834.666-1.5 1.5-1.5H12v-2zm2.293 10.172c-.265-.372-.287-.907-.287-1.293v-2h6v-2h-6v-4.346c0-.386.022-.92.287-1.293 1.732 1.683 3.34 3.77 4.112 6.638.039.144.078.286.11.427H13.44c-.026-.078-.047-.163-.054-.25-.122-1.84-1.028-3.396-2.493-4.44.031.214.052.43.052.65v1.538c0 .686-.554 1.242-1.243 1.242h-2v2h2c.954 0 1.742-.791 1.742-1.742v-.67c.025.218.05.43.05.645 0 .834-.668 1.5-1.5 1.5h2v2z"/></svg>
        <div class="skill-name">Python</div>
      </div>
      <div class="skill-card" title="HTML">
        <svg class="skill-icon" xmlns="http://www.w3.org/2000/svg" fill="#8bc6ec" viewBox="0 0 24 24" width="48" height="48"><path d="M1.5 0h21l-1.91 21.562L12 24l-8.585-2.438L1.5 0zm17.92 6.58l-.062.7-1.85 20.7L12 23.6v-7.1h4.68l-.123-1.1h-4.56v-2.7h6.18l-.18 2.07H14.4v2.9l3.45-.97 1 11.4z"/></svg>
        <div class="skill-name">HTML</div>
      </div>
      <div class="skill-card" title="C++">
        <svg class="skill-icon" xmlns="http://www.w3.org/2000/svg" fill="#8bc6ec" viewBox="0 0 24 24" width="48" height="48"><path d="M12 0 1.5 4.5v15L12 24l10.5-4.5v-15L12 0zm1.81 17.22c-.747 1.238-2.395 1.81-3.92 1.53-1.903-.363-2.929-1.955-3.182-3.615h2.066c.134.83.782 1.457 1.924 1.353 1.05-.1 1.597-.684 1.955-1.353-.029-.83-1.02-1.165-1.81-1.42l-1.013-.37c-1.58-.575-2.583-1.786-2.566-3.72 0-2.17 1.658-4.11 4.777-3.713 2.086.254 3.57 1.34 4.277 2.94l-2.034 1.2c-.36-.644-.745-1.208-1.57-1.412-1.14-.294-1.928.62-1.928 1.22 0 .444.34.926 1.144 1.288l1.01.394c1.698.685 2.592 1.883 2.564 3.79-.01 1.18-.914 2.11-2.21 2.497z"/></svg>
        <div class="skill-name">C++</div>
      </div>
    </div>
  </section>

  <section id="portfolio" class="fadeInUp delay-3">
    <h2>Portfolio</h2>
    <p class="lead">Coming soon: Showcase of projects including websites, applications, and software demonstrating expertise across frontend, backend, and systems programming.</p>
  </section>

  <section id="contact" class="fadeInUp delay-4">
    <h2>Contact Me</h2>
    <p class="lead">Interested in working together? Get in touch!</p>
    <a href="mailto:your.email@example.com" class="contact-btn" aria-label="Send email">Send Email</a>
  </section>
</main>

<footer>
  &copy; 2025 david. Full Stack Developer Portfolio.
</footer>

<script>
  // Animate fadeInUp elements on scroll
  window.addEventListener('scroll', () => {
    const fadeElements = document.querySelectorAll('.fadeInUp');
    fadeElements.forEach(el => {
      const rect = el.getBoundingClientRect();
      if (rect.top < window.innerHeight - 100) {
        el.style.animationPlayState = 'running';
      }
    });
  });
  // Trigger animation on page load for elements in viewport
  window.dispatchEvent(new Event('scroll'));
</script>
</body>
</html>


