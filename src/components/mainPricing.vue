<script>
export default {
    data() {
        return {
            pricing: 
            {
                blueText: 'MONTHLY PLANS',
                title: 'Pricing Table',
                text: 'We can help you deliver and execute your future, wherever you compete, using the latest technologies, from strategy development to implementation.',
            },

            cardSub: [
                {
                    type: 'Standard',
                    price: '490',
                    label: {
                        textF: {
                            text: 'National overage',
                            YoN: '✓',
                        },
                        textS: {
                            text: 'Ultimate Motoboy',
                            YoN: '✓',
                        },
                        textT: {
                            text: 'Address Collection',
                            YoN: 'x',
                        },
                        textFo: {
                            text: 'Mobile App Tracking',
                            YoN: 'x',
                        },
                        textFi: {
                            text: 'Cargo Insurance',
                            YoN: 'x',
                        },
                    }
                },
                {
                    most: 'Most Popular',
                    type: 'Professional',
                    price: '890',
                    label: {
                        textF: {
                            text: 'National overage',
                            YoN: '✓',
                        },
                        textS: {
                            text: 'Ultimate Motoboy',
                            YoN: '✓',
                        },
                        textT: {
                            text: 'Address Collection',
                            YoN: '✓',
                        },
                        textFo: {
                            text: 'Mobile App Tracking',
                            YoN: 'x',
                        },
                        textFi: {
                            text: 'Cargo Insurance',
                            YoN: 'x',
                        },
                    }
                },
                {
                    type: 'Ultimate',
                    price: '1.390',
                    label: {
                        textF: {
                            text: 'National overage',
                            YoN: '✓',
                        },
                        textS: {
                            text: 'Ultimate Motoboy',
                            YoN: '✓',
                        },
                        textT: {
                            text: 'Address Collection',
                            YoN: '✓',
                        },
                        textFo: {
                            text: 'Mobile App Tracking',
                            YoN: '✓',
                        },
                        textFi: {
                            text: 'Cargo Insurance',
                            YoN: '✓',
                        },
                    }
                },
            ]
        }
    }
}
</script>

<template>
    <section class="main-pricing">
        <div class="container">
            <div class="box">
                <ul>
                    <li>
                        <p class="blue-text">
                            {{ pricing.blueText }}
                        </p>
                    </li>
                    <li>
                        <h3>
                            {{ pricing.title }}
                        </h3>
                    </li>
                    <li>
                        <p>
                            {{ pricing.text }}
                        </p>
                    </li>
                </ul>
            </div>

            <div class="my-row">
                <a v-for="(card,i) in cardSub" :key="i" class="card">
                    <ul>
                        <p class="most-pop">{{ card.most }}</p>
                        <li>
                            cdn
                        </li>
                        <li>
                            <h3>
                                {{ card.type }}
                            </h3>
                        </li>
                        <li>
                            <h2 class="blue-text">
                                <p>$</p>
                                {{ card.price }}
                                <p>/mo</p>
                            </h2>
                        </li>
                        <li>
                            <p>
                                {{ card.label.textF.text }}
                            </p>
                            <p>
                                {{ card.label.textF.YoN }}
                            </p>
                        </li>
                        <li>
                            <p>
                                {{ card.label.textS.text }}
                            </p>
                            <p>
                                {{ card.label.textS.YoN }}
                            </p>
                        </li>
                        <li>
                            <p>
                                {{ card.label.textT.text }}
                            </p>
                            <p>
                                {{ card.label.textT.YoN }}
                            </p>
                        </li>
                        <li>
                            <p>
                                {{ card.label.textFo.text }}
                            </p>
                            <p>
                                {{ card.label.textFo.YoN }}
                            </p>
                        </li>
                        <li>
                            <p>
                                {{ card.label.textFi.text }}
                            </p>
                            <p>
                                {{ card.label.textFi.YoN }}
                            </p>
                        </li>
                    </ul>
                </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;
@use '../assets/scss/partials/mainPricing.scss' as*;

.main-pricing p {
    color:$textColorMain;
}

.main-pricing h3 {
    color: $h3ColorText;
}

.main-pricing .blue-text {
    color: $mainTextAColor;
}
</style>