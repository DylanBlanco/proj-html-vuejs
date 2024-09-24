<script>
export default {
    data() {
        return {
            mainCardDel: [
                {
                    title: 'Motoboy',
                    text: 'Functional motoboy for delivery of documents and small objects.',
                },
                {
                    title: 'Shuttle Van',
                    text: 'Suitable for medium sized loads that need digital tracking.',
                },
                {
                    title: 'Mini Truck',
                    text: 'For dry cargo deliveries with more cubic allocation.',
                },
            ]            
        }
    }
}
</script>

<template>
    <main>
        <!-- logistics-service -->
        <section class="logistics-service">
            <div class="container">
                <div class="my-row">
                    <div class="box">
                        <ul>
                            <li>
                                <p>
                                    WHAT WE DO
                                </p>
                            </li>
                            <li>
                                <h2>
                                    We offer a full range of 
                                    <p>
                                        delivery 
                                    </p>
                                    methods.
                                </h2>
                            </li>
                        </ul>
                    </div>                     
                    <a href="#" class="box card shipping-fast">
                        <ul>
                            <li class="d-flex justify-content-between">
                                <i class="fa-solid fa-truck-fast"></i>
                                <i class="fa-solid fa-arrow-right"></i>
                            </li>
                            <li>
                                <h3>
                                    Shipping fast
                                </h3>
                            </li>
                            <li>
                                <p>
                                    Special fast delivery service that guarantees the arrival of the object on the same day as postage. Included monitoring via miobile app.
                                </p>
                            </li>
                        </ul>
                    </a>
                    
                    <a v-for="(card,i) in mainCardDel" :key="i"  href="#" class="box card">
                        <ul>
                            <li class="d-flex justify-content-between">
                                <i class="fa-solid fa-truck-fast"></i>
                                <i class="fa-solid fa-arrow-right"></i>
                            </li>
                            <li>
                                <h3>
                                    {{ card.title }}
                                </h3>
                            </li>
                            <li>
                                <p>
                                    {{ card.text }}
                                </p>
                            </li>
                        </ul>
                    </a>
                    
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss">
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;
@use '../assets/scss/mainApp.scss' as*;

main .logistics-service {
    background-color: $mainBgColor;
}

main .logistics-service {
    color: white;
}

main .logistics-service a {
    background-color: $mainTextAColor;
}

main .logistics-service .card {
    background-color: $mainCardBgColor;
}
</style>