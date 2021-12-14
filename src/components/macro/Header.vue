<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../../assets/img/dc-logo.png" alt="DC logo small">
            </div>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a v-bind:href="link.url" :class="{active: link.current}">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return { 
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false
                },
                {
                    text: "comics",
                    url: "#",
                    current: false
                },
                {
                    text: "movies",
                    url: "#",
                    current: false
                },
                {
                    text: "tv",
                    url: "#",
                    current: false
                },
                {
                    text: "games",
                    url: "#",
                    current: false
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false
                },
                {
                    text: "videos",
                    url: "#",
                    current: false
                },
                {
                    text: "fans",
                    url: "#",
                    current: false
                },
                {
                    text: "news",
                    url: "#",
                    current: false
                },
                {
                    text: "shop",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../../assets/style/partials/variables.scss';
    header {
        background-color: $background-light;

        .container  {
            padding: 10px 0;

                ul {
                    display: flex;

                    li a {
                        display: inline-block;
                        padding: 10px;
                        color: $text-dark;
                        font-size: 13px;
                        font-weight: $text-bold;
                        text-transform: $text-uppercase;

                            &.active, &:hover {
                                border-bottom: 2px solid $text-blue;
                                color: $text-blue;
                            }
                    }
                }
        }
    }
</style>