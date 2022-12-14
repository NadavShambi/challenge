<template>
  <section class="main-layout">

    <app-header />
    <app-hero />
    <app-cards />
    <app-section />
    <app-about />
    <app-contact />
    <app-footer />
  </section>
</template>
<script>
import appHeader from './cmps/app-header.vue'
import appHero from './cmps/app-hero.vue'
import appCards from './cmps/app-cards.vue'
import appSection from './cmps/app-section.vue'
import appAbout from './cmps/app-about.vue'
import appContact from './cmps/app-contact.vue'
import appFooter from './cmps/app-footer.vue'
export default {
  name: 'App',
  props: {},
  components: {
    appHeader, appHero, appCards, appSection,
    appAbout, appContact, appFooter
  },
  data() {
    return {};
  },
  created() { },
  methods: {},
  computed: {},
  unmounted() { },
};
</script>
<style>

</style>