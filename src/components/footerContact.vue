<script>
export default {
    data() {
        return {
            labelForm: {
                bluText: 'SEND A MESSAGE',
                title: 'Get in Touch',
                text: 'We will respond to your message as soon as possible.',
                button: 'SEND',
            },
            contacts: {
                title: 'Example Inc.',
                textF: 'Built to the smallest detail with a focus on feature availability.',
                textS: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
                num: '+1(305) 1234-5678',
                mail: 'hello@example.com',
                position: 'Main Avenue, 123',
                link: 'VIEW MAPP'
            },
            moreInfos: [
                {
                    opt:'- Please choose an option -'
                },
                {
                    opt:'- Sales and Purchasing -'
                },
                {
                    opt:'- Finantial and Acoounts -'
                },
                {
                    opt:'- Human Resources -'
                },
                {
                    opt:'- Another Subjects -'
                },
            ]
        }
    }
}
</script>

<template>
    <section class="footer-contact">
        <div class="container">
            <div class="my-row">
                <!-- foot form -->
                <div class="foot-form">
                    <ul>
                        <li>
                            <p class="blue-text">
                                {{ labelForm.bluText }}
                            </p>
                        </li>
                        <li>
                            <h2>
                                {{ labelForm.title }}
                            </h2>
                        </li>
                        <li>
                            <p>
                                {{ labelForm.text }}
                            </p>
                        </li>
                        <li>
                            <form>
                                <div class="my-row">
                                    <input 
                                    type="text"
                                    placeholder="Name">
                                    <input 
                                    type="text"
                                    placeholder="Email">
                                </div>
                                <div class="my-row">
                                    <input 
                                    type="text"
                                    placeholder="Phone">
                                    <select name="submit" id="">
                                        <option value=""></option>
                                        <option v-for="(info,i) in moreInfos" :key="i" value="">
                                            {{ info.opt }}
                                        </option>
                                    </select>
                                </div>
                                <div>
                                    <input class="mess" type="text"
                                    placeholder="Message">
                                </div>
                                <div>
                                    <button type="submit">
                                        {{ labelForm.button }}
                                    </button>
                                </div>
                            </form>
                        </li>
                    </ul>
                </div>

                <!-- foot contacts -->
                <div class="foot-contact">
                    <ul>
                        <li>
                            <h3>
                                {{ contacts.title }}
                            </h3>
                        </li>
                        <li>
                            <p>
                                {{ contacts.textF }}
                            </p>
                        </li>
                        <li>
                            <p>
                                {{ contacts.textS }}
                            </p>
                        </li>
                        <li>
                            Num: 
                            <a href="#">
                                {{ contacts.num }}
                            </a>
                        </li>
                        <li>
                            Mail:
                            <a href="#">
                                {{ contacts.mail }}
                            </a>
                        </li>
                        <li>
                            Position:
                            <a href="#">
                                {{ contacts.position }}
                            </a>
                        </li>
                        <li class="view">
                            <a href="#">
                                {{ contacts.link }}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use "../assets/scss/partials/reset.scss" as*;
@use '/src/assets/scss/partials/variables.scss' as*;
@use '../assets/scss/generalStyle.scss' as*;
@use '../assets/scss/partials/footerContact.scss' as*;

.footer-contact p {
    color: $textPColorFooter;
}

.footer-contact .blue-text {
    color: $textH2ColorFooter;
}

.footer-contact h2 {
    color: $textH3ColorFooter;
}

.footer-contact h3 {
    color: $textH3ColorFooter;
}

.footer-contact .foot-form button {
    color: $textAColorFooter;
    background-color: $textH2ColorFooter;
}

.footer-contact .foot-contact li {
    color: $textH2ColorFooter;
}

.footer-contact .foot-contact li a {
    color: $textH2ColorFooter;
}

.footer-contact .foot-contact .view a {
    background-color: $textH2ColorFooter;
    color: $textAColorFooter;
}
</style>