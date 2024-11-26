<template>
    <div class="header">
        <div class="logo">
            <img src="../assets/Star 1.svg">
            Ink.House
         </div>
         <nav class="nav">
            <a href="#" class="link">Репродукции</a>
            <a href="#" class="link">Новинки</a>
            <a href="#" class="link">О нас</a>
        </nav>
        <div><img src="../assets/shopping-cart.svg"></div>
    </div>
</template>
<style scoped>
    .header {
        min-height: 100px;
        background-color: #E1EDE6;
        width: 100%;
        display: flex;
        align-items: center;
        flex-direction: row;
        justify-content: space-around;
        margin: 0 auto;
        position: relative;
        flex-wrap: wrap;
    }
    .logo {
        display: flex;
        align-items: center;
        color: #598D66;
        font-weight: 700;
        font-size: 20px;
    }
    .header img {
        margin-right: 6px;
    }
    img {
        margin-left: 165px;
    }
    .nav {
        max-width: 470px;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .link {
    font-size: 20px;
    color: #000;
    text-decoration: none;
    }
</style>