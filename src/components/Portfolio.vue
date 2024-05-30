<script>
export default {
  data() {
    return {
      arrSpecial: [
        {
          title: "Web Design",
          description: `Design web coinvolgente, intuitivo e immersivo che attira l'attenzione e accompagna gli utenti attraverso un'esperienza digitale fluida e memorabile.`,
          icon: "fa-solid fa-display",
        },
        {
          title: "Web Development",
          description: `Web development professionale e su misura, trasformando idee in codice impeccabile per siti web performanti e funzionalità innovative.`,
          icon: "fa-solid fa-code",
        },
        {
          title: "Responsive Design",
          description: `Responsive design che si adatta fluidamente a ogni dispositivo, offrendo un'esperienza utente ottimale su desktop, tablet e smartphone.`,
          icon: "fa-solid fa-mobile-screen",
        },
      ],
      arrProject: [
        {
          img: "B&B.png",
          title: "B&B",
          link: "https://github.com/Andreaserra1997/BoolBnB-Front-End",
        },
        {
          img: "Comics.jpeg",
          title: "Fumetti DC Comics",
          link: "https://github.com/Andreaserra1997/laravel-dc-comics",
        },
        {
          img: "Whatsapp.jpeg",
          title: "WhatsApp Web",
          link: "https://github.com/Andreaserra1997/vue-boolzapp",
        },
      ],
    };
  },
};
</script>

<template>
  <section id="service" class="services-mf route">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="title-box text-center">
            <h3 class="title-a pt-3">Competenze</h3>
            <div class="line-mf"></div>
          </div>
        </div>
      </div>
      <div class="row">
        <div
          v-for="special in arrSpecial"
          :key="special.title"
          class="col-md-4"
        >
          <div class="service-box">
            <div class="service-ico">
              <span class="ico-circle">
                <i :class="special.icon"></i>
              </span>
            </div>
            <div class="service-content">
              <h2 class="s-title">{{ special.title }}</h2>
              <p class="s-description text-center">{{ special.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="project" class="portfolio-mf sect-pt4 route">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="title-box text-center">
            <h3 class="title-a">Progetti</h3>
            <p class="subtitle-a">Alcuni progetti a cui ho lavorato.</p>
            <div class="line-mf"></div>
          </div>
        </div>
      </div>
      <div class="row">
        <div
          class="col-md-4"
          v-for="project in arrProject"
          :key="project.title"
        >
          <div class="work-box">
            <div class="work-img">
              <img :src="project.img" :alt="project.title" class="img-fluid" />
            </div>
            <div class="work-content">
              <h2 class="w-title">{{ project.title }}</h2>
              <a :href="project.link">
                <span>
                  <i class="fa-brands fa-github" style="font-size: 2.5rem"></i>
                </span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
