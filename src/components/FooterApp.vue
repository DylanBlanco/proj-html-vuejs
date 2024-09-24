<script>
import footerContact from './footerContact.vue';
import footerEnd from './footerEnd.vue';
export default {
    data() {
        return {
        }
    },
    components: {
        footerContact,
        footerEnd
    }
}
</script>

<template>
    <footer>
        <!-- contact section -->
         <footerContact />

        <!-- end footer section -->
         <footerEnd />
    </footer>
</template>

<style lang="scss" scoped>
</style>