<script>
export default {
    data() {
        return {
            footText: {
                text: 'Enjoy the low price. We are tracking any intention of privacy.',
                label: '© 2024 - All rights reserved. Nexgen is maintained by Codings Group.',
            }
        }
    }
}
</script>

<template>
    <section class="footer-end">
        <div class="container">
            <div class="my-row">
                <div>
                    <p>
                        {{ footText.text }}
                    </p>
                </div>
                <div>
                    <a href="#">
                        {{ footText.label }}
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;
@use '/src/assets/scss/partials/footerEnd.scss' as*;

</style>