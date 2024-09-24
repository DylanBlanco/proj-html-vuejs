<script>
export default {
    data() {
        return {
            textChoose: {
                title: 'Why choose us?',
                text: 'We work intensively in search of ideals that can add up in the lives of our costumers. This is what motivates us to improve every day.',
                link: 'GET IN TOUCH',
            }
        }
    }
}
</script>

<template>
    <section class="mainChoose">
        <div class="container">
            <div class="box">
                <ul>
                    <li>
                        <h1>
                            {{ textChoose.title }}
                        </h1>
                    </li>
                    <li>
                        <p>
                            {{ textChoose.text }}
                        </p>
                    </li>
                    <li>
                        <a href="#">
                            {{ textChoose.link }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;
@use '../assets/scss/partials/mainChoose.scss' as*;

.mainChoose h1 {
    color: white;
}

.mainChoose p {
    color: $textColorMain;
}

.mainChoose a {
    color: white;
    background-color: $mainTextAColor;
}
</style>