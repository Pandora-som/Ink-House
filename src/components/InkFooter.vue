<template>
<div class="inkfooter">
        <div class="footer-block">
            <div class="phone-block">
                <div class="f-logo">
                    <img src="../assets/Star 1.svg" alt="logo" class="logo-pic">
                    <p class="inkhouse">Ink. House</p>
                </div>
                <div class="p-text">
                    <p>+7 (999) 543-54-54</p>
                    <p class="p-workshop">Мастерская</p>
                </div>
            </div>
            <div class="navigation">
                <div class="rep_l navg">
                    <h3 class="footer-h">Репродукции</h3>
                    <p class="f-country f_nav">Франция</p>
                    <p class="f-country f_nav">Германия</p>
                    <p class="f-country f_nav">Англия</p>
                </div>
                <div>
                    <h3>Новинки</h3>
                    <p class="f_nav">2021</p>
                    <p class="f_nav">2020</p>
                </div>
                <div>
                    <h3>О нас</h3>
                    <p class="f_nav">Художники</p>
                    <p class="f_nav">Менеджеры</p>
                </div>
            </div>
            <hr class="contacts-block">
            <div class="contacts">
                <div class="contacts-img">
                    <img src="faceb_img.svg" alt="facebook_img" class="img-c">
                    <img src="insta_img.svg" alt="instagram_img" class="img-c">
                    <img src="yout_img.svg" alt="youtube_img" class="img-c">
                </div>
                <div class="contacts-text">
                    <p class="rights__copy">Ink. House®</p>
                    <p class="rights__reserved">All rights reserved</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.footer-block {
    font-family: Raleway;
    max-width: 1110px;
    margin: 0 auto;

    padding: 23px 15px;
    display: grid;
    align-content: flex-start;
    grid-template-columns: auto auto auto;
}
.inkfooter {
    margin-top: 70px;
    width: 100%;
    background-color: #E1EDE6;
}
.phone-block {
    flex-direction: column;
    display: flex;
    justify-content: space-between;
}
.f-logo {
    display: flex;
    align-items: center;
    gap: 8px;
}

.inkhouse {
    color: #598D66;
    font-weight: 700;
    font-size: 20px;
    line-height: 23.48px;
}
.logo-pic {
    height: 35px;
    width: 35px;
}
.p-workshop{
    font-size: 18px;
    line-height: 21.13px;
    font-weight: 500;
    color: #86928B;
}
.p-text {
    gap: 8px;
    display: flex;
    flex-direction: column;
    line-height: 23.48px;
    font-size: 20px;
    color: #2C2D35;
    font-weight: 500;
}
.navg {
    gap: 6px;
    display: flex;
    flex-direction: column;
}
.navigation {
    justify-content: space-between;
    display: flex;
    align-items: flex-start;
}
.f_nav {
    line-height: 27px;
    font-size: 18px;
    font-weight: 500;
    color: #86928B;
}
.footer-h {
    font-weight: 500;
    font-size: 20px;
    line-height: 23.48px;
}
.contacts-block {
    display: none;
    width: 100%;
    margin: -14px 0;
    background-color: #C3D1C6;
}
.contacts-img {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.contacts {
    width: 132px;
    flex-direction: column;
    gap: 10px;
    display: flex;
    justify-self: flex-end;
}
.contacts-text {
    font-weight: 500;
    color: #86928B;
    line-height: 14.4px;
    font-size: 12px;
}
.img-c {
    height: 24px;
    width: 24px;
}
@media screen and (width <= 769px) {
    .phone-block {
        align-items: center;
        flex-direction: row;
        grid-column-start: 1;
        justify-content: space-between;
        grid-column-end: span 2;
        grid-row-end: 1;
        grid-row-start: 1;
    }
    .footer-block {
        max-width: 690px;
        grid-template-columns: repeat(2, auto);
        grid-template-rows: repeat(2, auto);
        gap: 30px 75px;
    }
    .contacts {
        margin-right: 37px;
        grid-column-start: 2;
        justify-self: flex-end;
        grid-row-start: 2;
    }
    .navigation {
        grid-row-start: 2;
        grid-column-start: 1;
    }
}

@media screen and (width <= 577px) {
    .footer-block {
        align-items: center;
        height: 273px;
        display: flex;
        flex-direction: column;
        max-width: 510px;
    }
    .phone-block {
        height: 50px;
        width: 100%;
        justify-content: space-between;
        flex-direction: row;
    }
    .contacts-block {
        display: block;
    }
    .navigation {
        height: 113px;
        width: 100%;
    }
    .contacts-text {
        align-items: center;
        display: flex;
        justify-content: center;
    }
    .contacts {
        margin: 0;
        height: 48px;
        width: 176px;
    }
}
@font-face {
    font-family: Raleway;
    src: url('../assets/fonts/Raleway-VariableFont_wght.ttf');
}
</style>