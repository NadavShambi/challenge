<template>
  <section class="cards-wrapper main-layout full">

    <section class="cards-container">
      <article class="card" v-for="card in cards">
        <card-preview :card="card" />
      </article>
    </section>
  </section>
</template>
<script>
import cardPreview from './card-preview.vue'
export default {
  name: 'app-cards',
  props: {},
  components: { cardPreview },
  data() {
    return {
      cards: [
        {
          src: '../assets/images/icon-access-anywhere.svg',
          title: 'Access your files.anywhere',
          txt: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.'
        },
        {
          src: '../assets/images/icon-security.svg',
          title: 'Security you can trust',
          txt: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.'
        },
        {
          src: '../assets/images/icon-collaboration.svg',
          title: 'Real-time collaboration',
          txt: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.'

        },
        {
          src: '../assets/images/icon-any-file.svg',
          title: 'Store any type of file',
          txt: 'Whether you\'re sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.'

        },
      ]
    };
  },
  created() { },
  methods: {
    getImgUrl(img) {
      return new URL(img, import.meta.url).href
    }
  },
  computed: {},
  unmounted() { },
};
</script>
<style>

</style>