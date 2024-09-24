<script>
import mainDelivery from './mainDelivery.vue';
import mainIndustry from './mainIndustry.vue';
export default {
    data() {
        return {          
        }
    },
    components: {
        mainDelivery,
        mainIndustry,
    }
}
</script>

<template>
    <main>
        <!-- main delivery -->
        <mainDelivery />
    
        <!-- industry leaders -->
        <mainIndustry />
    </main>
</template>

<style lang="scss">
</style>