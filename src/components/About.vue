<script>
export default {
  data() {
    return {
      arrSkill: [
        {
          icon: "fa-brands fa-html5",
        },
        {
          icon: "fa-brands fa-css3-alt",
        },
        {
          icon: "fa-brands fa-js",
        },
        {
          icon: "fa-brands fa-vuejs",
        },
        {
          icon: "fa-brands fa-php",
        },
        {
          icon: "fa-brands fa-laravel",
        },
        {
          icon: "fa-brands fa-java",
        },
      ],
    };
  },
};
</script>

<template>
  <div id="home" class="intro route bg-image" style="background-color: #0078ff">
    <div class="overlay-itro"></div>
    <div class="intro-content display-table">
      <div class="table-cell">
        <div class="container">
          <h1 class="intro-title mb-4">Andrea Serra</h1>
          <p class="intro-subtitle">
            <span class="text-slider-items"
              >Junior Full Stack Web Developer</span
            ><strong class="text-slider"></strong>
          </p>
        </div>
      </div>
    </div>
  </div>

  <section id="about" class="about-mf sect-pt4 route">
    <div class="container pt-5">
      <div class="box-shadow-full pb-3">
        <img src="../assets/Andrea.jpg" alt="Andrea" class="myimg" />
        <div class="title-box-2">
          <h5 class="title-left">Chi sono</h5>
        </div>
        <div class="about-me pt-4 pt-md-0">
          <p class="lead" style="width: 80%">
            Sono un ragazzo che ha sempre cercato di sperimentare in ambito
            lavorativo, provando diversi lavori per trovare quello che più mi si
            addice. Con la programmazione mi sono finalmente sentito a mio agio
            e portato per questa disciplina.
          </p>
          <p class="lead">
            Da sempre vicino al mondo dell'informatica, ho consolidato le mie
            competenze seguendo un corso di Full Stack Web Developer, che mi ha
            permesso di sviluppare competenze che ho ulteriormente approfondito
            con un corso per sviluppatori Java. Ho imparato le basi del
            linguaggio, la programmazione orientata agli oggetti e le principali
            librerie.
          </p>
          <p class="lead">
            Sono sempre aggiornato e in continua formazione, aperto al
            cambiamento e pronto per nuove esperienze lavorative. Le mie
            caratteristiche distintive sono la dinamicità e la capacità di
            lavorare in gruppo, cogliendo il meglio da ogni situazione.
          </p>
        </div>
        <div class="socials pt-0 pb-0">
          <ul class="d-flex justify-content-center ps-0 icoabout">
            <li
              v-for="skill in arrSkill"
              :key="skill.icon"
              style="width: 100%"
              class="d-flex justify-content-center pt-3"
            >
              <span class="about-circle">
                <i :class="skill.icon"></i>
              </span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
