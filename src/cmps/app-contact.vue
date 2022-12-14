<template>
    <section class="app-contact-wrapper full">
        <section class="app-contact">
            <h1>Get early access today</h1>
            <p>It only takes a minute to sign up and our free starter tier is extremely generous. If you have any
                questions,
                our support team would be happy to help you.</p>
            <form @submit.prevent>
                <input type="text" placeholder="email@example.com">
                <button>Get Started For Free</button>
            </form>
        </section>
    </section>
</template>
<script>
export default {
    name: 'app-contact',
    props: {},
    components: {},
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