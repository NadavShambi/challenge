<template>
    <section class="app-about">
        <article class="" v-for="(user, idx) in 3">
            <p>Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has
                become a well-oiled collaboration machine.</p>
            <div class="profile">
                <img class="profile-photo" :src="getImgUrl(`../assets/images/profile-${idx + 1}.jpg`)" alt="">
                <div class="profile-name">Satish Patel</div>
                <p class="profile-pos">Founder & CEO, Huddle</p>
            </div>
        </article>
    </section>
</template>
<script>

export default {
    name: 'app-section',
    props: {},
    components: {},
    data() {
        return {
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