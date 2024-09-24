<script>
// Importazione macro componenti
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';

export default {
    data() {
        return {
        }
    },
    components: {
        HeaderApp,
        MainApp,
        FooterApp
    },
}
</script>

<template>
    <div>
        <!-- Header macro component -->
        <HeaderApp />

        <!-- MainApp macro component -->
        <MainApp />

        <!-- Footer macro component -->
        <FooterApp />
    </div>
</template>

<style lang="scss">
// Import all of Bootstrap's CSS
@import "bootstrap/scss/bootstrap";
</style>
