<template>
  <header id="hero">
    <!-- Navbar -->
    <nav class="navbar">
      <div class="container">
        <!-- Logo -->
        <h1 id="logo">
          <a href="#"><img src="../assets/images/Xu.png" alt="Your Logo" /></a>
        </h1>
        <!-- Navbar links -->
        <ul class="nav-menu">
          <li><a class="nav-link" href="#projects">PROJECTS</a></li>
          <li><a class="nav-link" href="">SKILLS</a></li>
          <li><a class="nav-link" href="#">CONTACT</a></li>
          <li><a class="nav-link" href="#">BlOG</a></li>
          <li>
            <a class="nav-link btn btn-primary" href="#"
              >RESUME <i class="fas fa-arrow-right"></i
            ></a>
          </li>

          <!-- Toggle switch -->
          <div class="theme-switch">
            <input type="checkbox" id="switch" />
            <label class="toggle-icons" for="switch">
              <img class="sun" src="../assets/images/sun.svg" />
              <img class="moon" src="../assets/images/moon.svg" />
            </label>
          </div>
          <!-- Hamburger menu -->
        </ul>
        <div class="hamburger">
          <span class="bar"></span>
          <span class="bar"></span>
          <span class="bar"></span>
        </div>
      </div>
    </nav>

    <section class="header-container">
      <img class="profile-image" src="../assets/images/myicon.png" alt="" />
      <h1>Hi I'm Umrbek</h1>

      <div class="content-text">
        <h2>Building websites</h2>
        <h2>Landing pages, CRM, and SPA.</h2>
        <p>
          <img src="../assets/images/VueLogo.png" height="14" alt="" />
          A Vue js Frontend Developer and Backend Developer with experience in
          web development, code quality and best practises.
        </p>
      </div>
      <a
        href="https://github.com/CommunityPro/portfolio-html"
        class="btn btn-secondary"
        target="_blank"
        >Connect With Me</a
      >
    </section>
  </header>

  <section id="skills" class="project-container container">
    <div class="division"></div>
    <div class="content-text">
      <h2>Skills</h2>
      <p>Advanced knowledge on these areas</p>
    </div>
    <article class="skill">
      <div class="chips">
        <div class="skill-info">
          <div class="skill-title" v-for="item in 7">
            <img src="../assets/images/html.png" alt="">
            <h2>HTML</h2>
          </div>
        </div>
      </div>
    </article>

  </section>


  <!-- Projects -->
  <section id="projects" class="project-container container">
    <div class="division"></div>
    <div class="content-text">
      <h2>Projects</h2>
      <p>Check out some of my personal and paid projects</p>
    </div>

    <article class="project">
      <!-- Project 1 -->
      <div class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Severyanochka</h3>
            <p>Vue 3, Vite, Tailwind</p>
          </div>
          
          <div class="project-link">
            <a href="https://github.com/Umrbek99/severyanochka" target="_blank"
              ><i class="fab fa-github"></i
            ></a>
            <a href="https://severyanochka-shop.netlify.app/" target="_blank"
              ><i class="fas fa-globe"></i
            ></a>
          </div>
        </div>
      </div>

      <!-- Project 2 -->
      <div href="" class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Project Two</h3>
            <p>React, Redux, SASS</p>
          </div>

          <div class="project-link">
            <a href="#" target="_blank"><i class="fab fa-github"></i></a>
            <a href="#" target="_blank"><i class="fas fa-globe"></i></a>
          </div>
        </div>
      </div>

      <!-- Porject 3 -->
      <div href="" class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Project Three</h3>
            <p>React, Redux, SASS</p>
          </div>

          <div class="project-link">
            <a href="#" target="_blank"><i class="fab fa-github"></i></a>
            <a href="#" target="_blank"><i class="fas fa-globe"></i></a>
          </div>
        </div>
      </div>

      <!-- Project 4 -->
      <div href="" class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Project Four</h3>
            <p>React, Redux, SASS</p>
          </div>

          <div class="project-link">
            <a href="#" target="_blank"><i class="fab fa-github"></i></a>
            <a href="#" target="_blank"><i class="fas fa-globe"></i></a>
          </div>
        </div>
      </div>

      <!-- Project 5 -->
      <div href="" class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Project Five</h3>
            <p>React, Redux, SASS</p>
          </div>

          <div class="project-link">
            <a href="#" target="_blank"><i class="fab fa-github"></i></a>
            <a href="#" target="_blank"><i class="fas fa-globe"></i></a>
          </div>
        </div>
      </div>

      <!-- Project 6 -->
      <div href="" class="card">
        <div class="project-info">
          <div class="project-bio">
            <h3>Project Six</h3>
            <p>React, Redux, SASS</p>
          </div>

          <div class="project-link">
            <a href="#" target="_blank"><i class="fab fa-github"></i></a>
            <a href="#" target="_blank"><i class="fas fa-globe"></i></a>
          </div>
        </div>
      </div>
    </article>

    <a href="#" class="btn btn-secondary" target="_blank"
      >See More <i class="fas fa-arrow-right"></i
    ></a>
  </section>

  <footer id="footer">
    <div class="container">
      <a href="mailto:communitypro47@gmail.com"
        >umrbekxudoyberganovpro@gmail.com</a
      >
      <!-- Social links -->
      <div class="social">
        <a href="#" target="_blank"
          ><img src="../assets/images/linkedin-icon.svg" alt="Linkedin"
        /></a>
        <a href="#" target="_blank"
          ><img src="../assets/images/github-icon.svg" alt="GitHub"
        /></a>
      </div>
      <!-- Attribution -->
      <p>
        Copyright &copy; UmrbekPro <span id="datee"></span>, All rights reserved
      </p>
    </div>
  </footer>
</template>
<script>
export default {
  date() {
    return {
      hamburger: null,
      navMenu: null,
      navLink: null,
      toggleSwitch: null,
    };
  },
  methods: {
    mobileMenu() {
      this.hamburger.classList.toggle("active");
      this.navMenu.classList.toggle("active");
    },
    closeMenu() {
      this.hamburger.classList.remove("active");
      this.navMenu.classList.remove("active");
    },
    switchTheme(e) {
      if (e.target.checked) {
        document.documentElement.setAttribute("data-theme", "dark");
        localStorage.setItem("theme", "dark");
      } else {
        document.documentElement.setAttribute("data-theme", "light");
        localStorage.setItem("theme", "light");
      }
    },
  },
  mounted() {
    this.hamburger = document.querySelector(".hamburger");
    this.navMenu = document.querySelector(".nav-menu");
    this.navLink = document.querySelectorAll(".nav-link");
    this.toggleSwitch = document.querySelector(
      '.theme-switch input[type="checkbox"]'
    );

    this.hamburger.addEventListener("click", this.mobileMenu);

    this.navLink.forEach((n) => n.addEventListener("click", this.closeMenu));

    this.toggleSwitch.addEventListener("change", this.switchTheme, false);

    const currentTheme = localStorage.getItem("theme")
      ? localStorage.getItem("theme")
      : null;
    if (currentTheme) {
      document.documentElement.setAttribute("data-theme", currentTheme);
      if (currentTheme === "dark") {
        toggleSwitch.checked = true;
      }
    }

    let myDate = document.querySelector("#datee");

    const yes = new Date().getFullYear();
    myDate.innerHTML = yes;
  },
};
</script>
<style>
/* This is the required project styling. Will contain essential CSS styles like:
   * Flex property
   * Grid layout
   * Cards and sections
*/
@import url(../assets/utilities.css);

@import url(https://fonts.googleapis.com/css?family=Raleway:100,200,300,regular,500,600,700,800,900,100italic,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic);

/* variables */
:root {
  /* Colors */
  --primary-color: #ffcd42;
  --secondary-color: #ffd35c;
  --bg-primary: #ffffff;
  --text-color: #222222;
  --text-color-two: #ffffff;
  --bg-secondary: #000000;
  --card-background: #f4f4f4;
  --bg-secondary-two: #111111;

  --shadow: 0 10px 40px rgba(0, 0, 0, 0.2);

  /* Font Weight */
  --weight-small: 400;
  --weight-semibold: 600;
  --weight-bold: 800;

  /* Max width */
  --width-small: 600px;
  --width-medium: 1100px;
  --width-large: 1300px;
}

[data-theme="dark"] {
  --primary-color: #ffcd42;
  --secondary-color: #ffd35c;
  --bg-primary: #000000;
  --text-color: #ffffff;
  --text-color-two: #222222;
  --bg-secondary: #ffffff;
  --card-background: #111111;
  --bg-secondary-two: #f4f4f4;
  --shadow: 0 2px 10px rgba(95, 95, 95, 0.2);
}

html {
  font-size: 100%;
  scroll-behavior: smooth;
}

/* Reset default styling */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  color: var(--text-color);
}

/* Main styling */
body {
  background: var(--bg-primary);
  color: var(--text-color);
  font-family: "Raleway", sans-serif;
  line-height: 1.5;
}

/* Navbar */
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 20;
  background: var(--bg-primary);
}

.navbar .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 20;
  height: 80px;
  width: 100%;
}

.navbar .nav-menu {
  display: flex;
  align-items: center;
  background: var(--bg-primary);
}

.navbar .nav-link {
  margin: 0 1rem;
  font-size: 0.8rem;
  font-weight: var(--weight-semibold);
}

.navbar #logo img {
  display: block;
  width: 40px;
}

.navbar .btn {
  margin-right: 1.5rem;
}

.fas.fa-arrow-right {
  margin-left: 0.5rem;
  font-size: 0.9rem;
}

/* hamburger */
.hamburger {
  margin-bottom: 0.1rem;
  display: none;
}

.bar {
  display: block;
  width: 23px;
  height: 3px;
  margin: 4px auto;
  transition: all 0.3s ease-in-out;
  border-radius: 30px;
  background-color: var(--bg-secondary);
}

/* Hero section */
#hero {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.profile-image {
  width: 150px;
  border-radius: 50%;
  animation: bounce 1s infinite alternate;
}

@keyframes bounce {
  from {
    transform: translateY(0px);
  }

  to {
    transform: translateY(-10px);
  }
}

.division {
  width: 100%;
  height: 2px;
  background-color: var(--card-background);
  margin: 5.5rem 0;
}
/* Projects */
#projects {
  display: flex;
  flex-direction: column;
  margin: 2rem auto 5rem;
}

#projects .btn {
  align-self: center;
  margin: 2rem 0;
}

.project {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: minmax(250px, auto);
  grid-gap: 0.9rem;
}

.card .project-bio p {
  font-size: 0.83rem;
}

.card .project-bio h3 {
  font-size: 0.9rem;
}

.project-info {
  display: flex;
  justify-content: space-between;
  opacity: 0;
  position: relative;
  transition: 0.5s ease-in-out;
}

.project-bio {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  position: relative;
  top: 160px;
  left: 10px;
}

/* Footer */
#footer {
  background: #111111;
}

#footer .container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: #ffffff;
  min-height: 160px;
  text-align: center;
}

#footer a {
  font-size: 0.8rem;
  color: #fff;
}

#footer a:hover {
  opacity: 0.6;
}

#footer .social {
  margin: 0.9rem 0;
}

#footer .social img {
  width: 20px;
  height: 20px;
}

#footer .social a {
  margin: 0 0.5rem;
}

#footer p {
  font-size: 0.8rem;
}

/* Responsiveness */

@media (max-width: 1000px) {
  .project {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
}

@media (max-width: 670px) {
  .navbar .nav-menu {
    position: fixed;
    right: -100vw;
    top: 4.5rem;
    flex-direction: column;
    width: calc(80% - 10px);
    transition: 0.3s;
    box-shadow: var(--shadow);
    padding: 2rem;
    border-radius: 5px;
    align-items: flex-start;
  }

  .navbar .btn {
    margin: 0;
    margin-top: 1rem;
  }

  .nav-menu.active {
    right: 20px;
  }

  .nav-menu .nav-link {
    font-size: 0.9rem;
    margin: 0 0.2rem;
  }

  .nav-menu li {
    margin-bottom: 0.5rem;
    width: 100%;
  }

  .nav-menu .btn {
    width: 100%;
    text-align: center;
    margin-top: 0.5rem;
  }

  .hamburger {
    display: block;
    cursor: pointer;
    padding: 0.2rem 0.4rem;
  }

  .hamburger.active {
    border: 1px dotted gray;
  }

  .hamburger.active .bar:nth-child(2) {
    opacity: 0;
  }

  .hamburger.active .bar:nth-child(1) {
    transform: translateY(6px) rotate(45deg);
  }

  .hamburger.active .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
  }
}

@media (max-width: 600px) {
  .project {
    display: grid;
    grid-template-columns: 1fr;
  }

  .header-container .btn {
    border-radius: 5px;
    width: 80%;
  }
}
</style>
