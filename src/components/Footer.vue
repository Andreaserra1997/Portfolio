<script>
export default {
  data() {
    return {
      arrLink: [
        {
          icon: "fa-solid fa-location-dot",
          link: "https://github.com/Andreaserra1997",
          text: "Alghero",
        },
        {
          icon: "fa-brands fa-github",
          link: "https://github.com/Andreaserra1997",
          text: "GitHub",
        },
        {
          icon: "fa-brands fa-linkedin",
          link: "https://www.linkedin.com/in/andrea-serra-b914ba285/",
          text: "Linkedin",
        },
        {
          icon: "fa-regular fa-envelope",
          link: "mailto:serra.andrea1997@gmail.com",
          text: "serra.andrea1997@gmail.com",
        },
      ],
    };
  },
};
</script>

<template>
  <section
    class="paralax-mf footer-paralax bg-image sect-mt4 route"
    id="footer"
  >
    <div class="overlay-mf"></div>
    <div class="container">
      <div class="row">
        <div id="contact" class="box-shadow-full">
          <div class="socials">
            <ul class="d-flex justify-content-between" style="list-style: none">
              <li v-for="link in arrLink" :key="link.link">
                <a :href="link.link">
                  <div class="ico-circle">
                    <i :class="link.icon"></i>
                  </div>
                </a>
                <p>{{ link.text }}</p>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
