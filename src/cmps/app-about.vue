<template>
    <div class="container  full">

        <section class="app-about">
            <article class="user-preview" v-for="(user, idx) in 3">
                <img v-if="idx === 0" class="quotes" src="../assets/images/bg-quotes.png" alt="">
                <p>Fylo has improved our team productivity by an order of magnitude. Since making the switch our team
                    has
                    become a well-oiled collaboration machine.</p>
                <div class="profile">
                    <img class="profile-photo" :src="getImgUrl(`../assets/images/profile-${idx + 1}.jpg`)" alt="">
                    <div class="info">
                        <h4>Satish Patel</h4>
                        <p>Founder & CEO, Huddle</p>
                    </div>
                </div>
            </article>
        </section>
    </div>

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