<script>
export default {
    data() {
        return {
            indBox: {
                who: 'WHO WE ARE',
                title: 'Industry Leaders',
                text: 'With all of this expertise and capability comes an unrivalled commitment to customer service.',
                do: 'We will work hard to understand your needs in order to develop a productive, long-term partnership.',
                link: 'READ MORE',
            }
        }
    }
}
</script>

<template>
    <!-- main industry -->
    <section class="industry">
        <div class="container">
            <div class="box">
                <ul>
                    <li>
                        <p class="blue-text">
                            {{ indBox.who }}
                        </p>
                    </li>
                    <li>
                        <h2>
                            {{ indBox.title }}
                        </h2>
                    </li>
                    <li>
                        <p>
                            {{ indBox.text }}
                        </p>
                    </li>
                    <li>
                        <p>
                            {{ indBox.do }}
                        </p>
                    </li>
                    <li>
                        <a href="#">
                            {{ indBox.link }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;
@use '../assets/scss/partials/mainIndustry.scss' as*;

.industry p {
    color: $textColorMain;
}

.industry h2 {
    color: $h2ColorText;
}

.industry .blue-text {
    color: $mainTextAColor;
}
</style>