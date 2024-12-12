<template>
    <div class="ink__header">
        <header class="header">
            <div class="header__logo block">
                <img src="../assets/Star 1.svg" alt="logo" class="header__logo pic-block">
                Ink.House
            </div>
            <hr class="header_line">
            <div class="h_menu">
                <button class="h button" @click="hActive=!Active"></button>
                <nav v-if="hActive" class="h_nav">
                    <button class="h button" @click="hActive=!hActive"></button>
                    <RouterLink to="/">Репродукции</RouterLink>
                    <RouterLink to="/">Новинки</RouterLink>
                    <RouterLink to="/">О нас</RouterLink>
                </nav>
                <RouterLink to="/"><img src="../assets/shopping-cart.svg" alt="shopping-cart" class="nav_cart pic"></RouterLink>
            </div>
            <nav class="header_nav">
                <div class="header_text_block">
                    <RouterLink to="/">Репродукции</RouterLink>
                    <RouterLink to="/">Новинки</RouterLink>
                    <RouterLink to="/">О нас</RouterLink>
                </div>
                <div class="header_nav_cart">
                    <RouterLink to="/"><img src="../assets/shopping-cart.svg" alt="shopping-cart" class="nav_cart pic"></RouterLink>
                </div>
            </nav>
        </header>
    </div>
</template>
<script>
export default {
    data() {
        return {
            hActive: false
        }
    },
}
</script>
<style scoped>
.header {
    padding: 0 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;
    max-width: 1110px;
    height: 100px;
}
.ink__header {
    background-color: #E1EDE6;
    margin: 0;
}
.header__logo.pic-block {
    margin-right: 6px;
}
.header__logo.block {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Raleway;
    font-weight: 700;
    color:#598D66;
    font-size: 20px;
}
.header_line {
    display: none;
    width: 88.5vw;
    background-color: #C3D1C6;
}

.h_menu {
    display: none;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    height: 62px;
}
.header__logo.pic-block {
    width: 35px;
    height: 35px;
}
.h.button {
    width: 30px;
    height: 30px;
    margin: 0 0 0 15px;
    padding: 0;
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
    border: none;
    background-color: transparent;
    background-image: url("../assets/Vector.svg");
}

.hamburger__icon {
    width: 24px;
    height: 24px;
}
.h_nav a {
    text-decoration: none;
    color: #2C2D35;
    font-family: Raleway;
    font-size: 18px;
    font-weight: 500;
    line-height: 21.13px;
    text-align: left;
    margin: 30px 0 20px 0;
}
.h_nav{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    background-color: #E1EDE6;
    padding: 16px 15px;
    left: 0;
    position: absolute;
    width: 100%;
    height: 433px;
    transform: translate(0, 202px);
}

.header_nav {
    display: flex;
    justify-content: space-between;
    gap: 60px;
    align-items: center;
}

.header_text_block {
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-family: Raleway;
    gap: 60px;
}

.header_nav a {
    text-decoration: none;
    color: #2C2D35;
    line-height: 23.48px;
    text-align: left;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
}

.nav_cart.pic{
    width: 24px;
    height: 24px;
}

@media screen and (width <= 769px) {
    .header {
        padding: 0 39px;
    }
    .header_nav a {
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}

@media screen and (width <= 577px) {
    .header {
        flex-direction: column;
        height: 91px;
        padding: 16px 33px;
    }

    .header_text_block {
        gap: 0;
        justify-content: space-between;
        width: 71%
    }

    .header_nav {
        width: 100%;
        justify-content: space-between;
        gap: 0;
    }

    .header_line_510 {
        display: block;
    }
}

@media screen and (width <= 376px) {
    .header {
        height: 130px;
        padding: 0;
    }

    .header__logo_pic-block {
        height: 68px;
        width: 100%;
        background-color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .header_line_510 {
        display: none;
    }

    .header_nav {
        display: none;
    }

    .h_menu {
        display: flex;
    }

    .h_nav > .h.button {
        margin: 0;
    }

    .nav_cart.pic {
        margin-right: 15px;
    } 
}
@font-face {
    font-family: Raleway;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>