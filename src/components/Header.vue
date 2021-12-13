<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo small">
            </div>
            <nav>
                <ul>
                    <li><a href="#">characters</a></li>
                    <li><a href="#">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">collectibles</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">fans</a></li>
                    <li><a href="#">news</a></li>
                    <li><a href="#">shop</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';
    header {
        background-color: $background-light;
    }

    ul {
        display: flex;

        li a {
            display: inline-block;
            padding: 10px;
            color: $text-dark;
            font-size: 13px;
            font-weight: $text-bold;
            text-transform: $text-uppercase;
        }
    }
</style>