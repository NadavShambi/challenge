<template>
    <img :src="getImgUrl(card.src)">
    <h4>{{ card.title }}</h4>
    <p>{{ card.txt }}</p>
</template>
<script>
export default {
    name: 'card-preview',
    props: { card: Object },
    components: {},
    data() {
        return {};
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