<script>
import mainDelivery from './mainDelivery.vue';
import mainIndustry from './mainIndustry.vue';
import mainPricing from './mainPricing.vue';
export default {
    data() {
        return {          
        }
    },
    components: {
        mainDelivery,
        mainIndustry,
        mainPricing,
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
    </main>
</template>

<style lang="scss">
</style>