<template>
  <main>
    <section class="intro-section d-flex">
      <div class="paragraph">
        <p>Questo è un paragrafo sulla sinistra.</p>
      </div>
      <div class="image">
        <img src="" alt="Immagine Intro" />
      </div>
    </section>

    <section
      v-for="(section, index) in sections"
      :key="index"
      :class="[
        'main-section',
        'd-flex',
        index % 2 === 0 ? 'flex-row' : 'flex-row-reverse',
      ]"
    >
      <div class="image">
        <img :src="section.imgSrc" :alt="section.imgAlt" />
      </div>
      <div class="paragraph">
        <p>{{ section.text }}</p>
      </div>
    </section>

    <section class="full-width-section">
      <p>Questo paragrafo occupa tutta la larghezza dello schermo.</p>
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      sections: [
        {
          text: 'Testo della sezione 1',
          imgSrc: '',
          imgAlt: 'Immagine 1',
        },
        {
          text: 'Testo della sezione 2',
          imgSrc: '',
          imgAlt: 'Immagine 2',
        },
      ],
    };
  },
};
</script>

<style scoped>
.intro-section,
.main-section {
  padding: 40px 0;
}
  .paragraph,
  .image {
    flex: 1;
    padding: 0 20px;
  }

  .image img {
    width: 100%;
    height: auto;
  }


.full-width-section {
  width: 100%;
  text-align: center;
  padding: 20px 0;
  background-color: #f1f1f1;
}
</style>
