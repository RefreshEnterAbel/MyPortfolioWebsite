<template>
  <main class="main">
    <!--==================== HOME ====================-->
    <section class="home section" id="home">
      <div class="home__container container grid">
        <div class="home__content grid">
          <div class="home__social">
            <a href="https://www.linkedin.com/in/ahmed-raju-bd/" target="_blank" class="home__social-icon">
              <i class="uil uil-linkedin-alt"></i>
            </a>
            <a href="https://stackoverflow.com/users/12174834/raju-ahmed" target="_blank" class="home__social-icon">
              <i class="fa fa-stack-overflow"></i>
            </a>
            <a href="https://github.com/AhmadRaju007" target="_blank" class="home__social-icon">
              <i class="uil uil-github-alt"></i>
            </a>
          </div>

          <div class="home__img">
            <svg class="home__blob" viewBox="0 0 200 187" xmlns="http://www.w3.org/2000/svg"
                 xmlns:xlink="http://www.w3.org/1999/xlink">
              <mask id="mask0" mask-type="alpha">
                <path d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346 165.547
            130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403 129.362C2.45775
            97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028 -0.149132 97.9666
            0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z"/>
              </mask>
              <g mask="url(#mask0)">
                <path d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346
            165.547 130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403
            129.362C2.45775 97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028
            -0.149132 97.9666 0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z"/>
                <image class="home__blob-img" x="12" y="18" xlink:href="assets/img/perfil.png"/>
              </g>
            </svg>

          </div>
          <div class="home__data">
            <h1 class="home__title">Hello from Raju,</h1>
            <h3 class="home__subtitle">Full-Stack Developer</h3>
            <p class="home__description">High level experience in web application development and producing quality
              work.</p>
            <a href="#contact" class="button button--flex">
              Contact Me <i class="uil uil-message button__icon"></i>
            </a>
          </div>
        </div>

        <div class="home_scroll">
          <a href="#about" class="home__scroll-button button--flex">
            <i class="uil uil-mouse-alt home__scroll-mouse"></i>
            <span class="home__scroll-name">Scroll down</span>
            <i class="uil uil-arrow-down homw__scroll-arrow"></i>
          </a>
        </div>
      </div>
    </section>

    <!--==================== ABOUT ====================-->
    <section class="about section" id="about">
      <h2 class="section__title"> About Me</h2>
      <span class="section__subtitle">My introduction</span>

      <div class="about__container container grid">
        <img src="assets/img/about.jpg" alt="" class="about__img">
        <div class="about__data">
          <p class="about__description">
            Web developer, with extensive knowledge and years of experience, working in web
            technologies and Ui/Ux design, delivering quality work.
          </p>
          <div class="about__info">
            <div>
              <span class="about__info-title">02+</span>
              <span class="about__info-name">Years <br> experience </span>
            </div>

            <div>
              <span class="about__info-title">02+</span>
              <span class="about__info-name">Companies <br> worked </span>
            </div>

            <div>
              <span class="about__info-title">07+</span>
              <span class="about__info-name">Completed <br> projects </span>
            </div>
          </div>
          <div class="about__buttons">
            <a download="" href="assets/pdf/Alexa-Cv.pdf" class="button button--flex">
              Download CV <i class="uil uil-download-alt button__icon"></i>
            </a>
          </div>
        </div>
      </div>

    </section>

    <!--==================== SKILLS ====================-->
    <section class="skills section" id="skills">
      <h2 class="section__title">Skills</h2>
      <span class="section__subtitle">My technical level</span>
      <Accordion/>
    </section>

    <!--==================== QUALIFICATION ====================-->
    <section class="qualification section">
      <h2 class="section__title">Qualifications</h2>
      <div class="section__subtitle">My personal journey</div>
      <Tabs/>
    </section>

    <!--==================== SERVICES ====================-->
    <section class="services section" id="services">
      <h2 class="section__title">Services</h2>
      <span class="section__subtitle">What I offer</span>

      <div class="services__container container grid">
        <!--===================== SERVICES 1 ====================-->
        <div class="services__content">
          <div>
            <i class="uil uil-arrow services__icon"></i>
            <h3 class="services__title">Backend <br> Developer</h3>

            <span class="button button--flex button--small button--link services__button">
              View More
              <i class="uil uil-arrow-right button__icon"/>
            </span>

            <div class="services__modal">
              <div class="services__modal-content">
                <h4 class="services__modal-title">Backend <br> Developer</h4>
                <i class="uil uil-times services__modal-close"></i>

                <ul class="services__modal-services grid">
                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I design Web Architecture.</p>
                  </li>

                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I create structural backbone of the platform.</p>
                  </li>

                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I maintain version control tools.</p>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>

        <!--===================== SERVICES 2 ====================-->
        <div class="services__content">
          <div>
            <i class="uil uil-web-grid services__icon"></i>
            <h3 class="services__title">Frontend <br> Developer</h3>

            <span class="button button--flex button--small button--link services__button">
              View More
              <i class="uil uil-arrow-right button__icon"/>
            </span>

            <div class="services__modal">
              <div class="services__modal-content">
                <h4 class="services__modal-title">Frontend <br> Developer</h4>
                <i class="uil uil-times services__modal-close"></i>

                <ul class="services__modal-services grid">
                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I develop user interface.</p>
                  </li>

                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I create web page.</p>
                  </li>

                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I restructure ui/ux components.</p>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>

        <!--===================== SERVICES 3 ====================-->
        <div class="services__content">
          <div>
            <i class="uil uil-pen services__icon"></i>
            <h3 class="services__title">Database <br> Designer</h3>

            <span class="button button--flex button--small button--link services__button">
                            View More
                            <i class="uil uil-arrow-right button__icon"></i>
                        </span>

            <div class="services__modal">
              <div class="services__modal-content">
                <h4 class="services__modal-title">Database <br> Designer</h4>
                <i class="uil uil-times services__modal-close"></i>

                <ul class="services__modal-services grid">
                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I design database.</p>
                  </li>

                  <li class="services__modal-service">
                    <i class="uil uil-check-circle services__modal-icon"></i>
                    <p>I structure data for user.</p>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!--==================== PORTFOLIO ====================-->
    <section class="portfolio section" id="portfolio">
      <h2 class="section__title">Portfolio</h2>
      <span class="section__subtitle">Most Recent Work</span>

      <div class="portfolio__container container swiper-container">
        <div class="swiper-wrapper">
          <!--======================== PORTFOLIO 1 =============-->
          <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/portfolio1.jpg" alt="" class="portfolio__img">

            <div class="portfolio__data">
              <h3 class="portfolio__title">Modern Website</h3>
              <p class="portfolio__description">
                This is test description(1) right now.
              </p>
              <a href="#" class="button button--flex button--small portfolio__button">
                Demo
                <i class="uil uil-arrow-right button__icon"></i>
              </a>
            </div>
          </div>

          <!--======================== PORTFOLIO 2 =============-->
          <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/portfolio2.jpg" alt="" class="portfolio__img">

            <div class="portfolio__data">
              <h3 class="portfolio__title">Modern Website(2)</h3>
              <p class="portfolio__description">
                This is test description(2) right now.
              </p>
              <a href="#" class="button button--flex button--small portfolio__button">
                Demo
                <i class="uil uil-arrow-right button__icon"></i>
              </a>
            </div>
          </div>

          <!--======================== PORTFOLIO 3 =============-->
          <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/portfolio3.jpg" alt="" class="portfolio__img">

            <div class="portfolio__data">
              <h3 class="portfolio__title">Modern Website(3)</h3>
              <p class="portfolio__description">
                This is test description(3) right now.
              </p>
              <a href="#" class="button button--flex button--small portfolio__button">
                Demo
                <i class="uil uil-arrow-right button__icon"></i>
              </a>
            </div>
          </div>

        </div>
        <!--============ Add Arrows =============-->
        <div class="swiper-button-next">
          <i class="uil uil-angle-right-b swiper-portfolio-icon"></i>
        </div>
        <div class="swiper-button-prev">
          <i class="uil uil-angle-left-b swiper-portfolio-icon"></i>
        </div>

        <!--============ Add Pagination =============-->
        <div class="swiper-pagination"></div>
      </div>
    </section>

    <!--==================== PROJECT IN MIND ====================-->
    <section class="project section">
      <div class="project__bg">
        <div class="project__container container grid">
          <div class="project__data">
            <h2 class="project__title">You have a new project</h2>
            <p class="project__description">Contact me now and get a 30% discount on your new project!</p>
            <a href="#contact" class="button button--flex button--white">
              Contact Me
              <i class="uil uil-message project__icon button__icon"></i>
            </a>
          </div>

          <img src="assets/img/project.png" alt="" class="project__img">
        </div>
      </div>

    </section>

    <!--==================== TESTIMONIAL ====================-->
    <section class="testimonial section">
      <!--=======This feature is skipped for now========-->
    </section>

    <!--==================== CONTACT ME ====================-->
    <section class="contact section" id="contact">
      <h2 class="section__title">Contact Me</h2>
      <span class="section__subtitle">Get in touch</span>

      <div class="contact__container container grid">
        <div>
          <div class="contact__information">
            <i class="uil uil-phone contact__icon"></i>

            <div>
              <h3 class="contact__title">Call Me</h3>
              <span class="contact__subtitle">+880-1521253077</span>
            </div>
          </div>

          <div class="contact__information">
            <i class="uil uil-envelope contact__icon"></i>

            <div>
              <h3 class="contact__title">Email</h3>
              <span class="contact__subtitle">rajuahmad6789@gmail.com</span>
            </div>
          </div>

          <div class="contact__information">
            <i class="uil uil-map-marker contact__icon"></i>

            <div>
              <h3 class="contact__title">Location</h3>
              <span class="contact__subtitle">Kamrangirchar, Dhaka-1211, Bangladesh</span>
            </div>
          </div>

          <form action="" class="contact__form grid">
            <div class="contact__inputs grid">
              <div class="contact__content">
                <label for="name" class="contact__label">Name</label>
                <input type="text" id="name" class="contact__input">
              </div>

              <div class="contact__content">
                <label for="email" class="contact__label">Email</label>
                <input type="email" id="email" class="contact__input">
              </div>
            </div>

            <div class="contact__content">
              <label for="project-contact" class="contact__label">Project</label>
              <input type="text" id="project-contact" class="contact__input">
            </div>

            <div class="contact__content">
              <label for="message-contact" class="contact__label">Message</label>
              <textarea name="" cols="0" rows="7" id="message-contact" class="contact__input"></textarea>
            </div>

            <div>
              <a href="#" class="button button--flex">Send Message</a>
              <i class="uil uil-message button__icon"></i>
            </div>
          </form>
        </div>
      </div>

    </section>
  </main>
</template>

<script setup>

</script>

<style scoped>

</style>
