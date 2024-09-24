<script>
import mainDelivery from './mainDelivery.vue';
import mainIndustry from './mainIndustry.vue';
import mainPricing from './mainPricing.vue';
import mainChoose from './mainChoose.vue';
export default {
    data() {
        return {          
        }
    },
    components: {
        mainDelivery,
        mainIndustry,
        mainPricing,
        mainChoose,
    }
}
</script>

<template>
    <main>
        <!-- main delivery -->
        <mainDelivery />
    
        <!-- industry leaders -->
        <mainIndustry />

        <!-- pricing table -->
        <mainPricing />

        <!-- main choose -->
         <mainChoose />
    </main>
</template>

<style lang="scss">
</style>