<script>
export default {
  data() {
    return {
        headerNav: [
            {
                label: 'HOME'
            },
            {
                label: 'SERVICES'
            },
            {
                label: 'ABOUT'
            },
            {
                label: 'PRINCING'
            },
            {
                label: 'BLOG'
            },
            {
                label: 'GET IN TOUCH'
            },
        ]
    }
  }
}
</script>

<template>
    <header>
        <!-- contacts section -->
        <section class="header-contacts">
            <div class="container">
                <div class="my-row">
                    <div>
                        <ul>
                            <li>
                                <a href="#">
                                    <i class="fa-solid fa-clock"></i> Open Hours: Mon-Sat-9:00-18:00
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li>
                                <a href="#">
                                    <i class="fa-solid fa-phone"></i> +1(305) 1234-5678
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <i class="fa-solid fa-envelope"></i> hello@example.com
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <i class="fa-brands fa-facebook-f"></i>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <i class="fa-brands fa-twitter"></i>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <i class="fa-brands fa-linkedin-in"></i>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- jumbo section -->
        <section class="jumbo-header">
            <div class="container">
                <div class="my-row">
                    <div>
                        <ul class="logo">
                            <li>
                                <a href="#">
                                    <img src="/public/img/logo.svg" alt="logo">
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul class="nav">
                            <li v-for="(nav,i) in headerNav" :key="i">
                                <a href="#">
                                    {{ nav.label }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="my-row intro">
                    <div>
                        <ul>
                            <li>
                                <p>
                                    EXPRESS DELIVERY
                                </p>
                            </li>
                            <li>
                                <h1>
                                    What are we going to deliver
                                    <p>
                                        today?
                                    </p>
                                </h1>
                            </li>
                            <li>
                                <a href="#">GET IN TOUCH</a>
                                <a href="#">READ MORE</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/reset.scss' as*;
@use '../assets/scss/partials/variables.scss' as *;
@use '../assets/scss//headerApp.scss' as *;
@use '../assets/scss/generalStyle.scss' as*;

header .header-contacts {
  background-color: $headerBgColor;
}

a {
    color: $textColorHeader;
}
</style>