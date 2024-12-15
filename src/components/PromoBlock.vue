<template>
    <div class="promo-block">
        <div class="promo-block2">
            <div class="promo-title">
                <img src="../assets/Star 2.svg" alt="star" class="promo-pic">
                <h1 class="promo-text-block">Новая коллекция французских авторов</h1>
            </div>
            <p class="promo-info text1">
                Сложно сказать, почему акционеры крупнейших компаний призывают нас к новым
                свершениям, которые, в свою очередь, должны быть заблокированы в рамках своих собственных рациональных
                ограничений.
            </p>
            <p class="promo-info text2">
                Принимая во внимание показатели успешности, граница обучения кадров предопределяет высокую
                востребованность
                направлений прогрессивного развития.
            </p>
            <button class="promo-bt button">Ознакомиться</button>
        </div>
    </div>
</template>

<style>
.promo-block {
    color: #FFF;
    background-image: url("../assets/pic_background.png");
    color: #FFF;
    text-align: left;
    font-family: Raleway;
    margin-top: 70px;
    position: relative;
    width: 100%;
}
.promo-block2 {
    display: flex;
    flex-direction: column;
    max-width: 1110px;
    padding: 70px 0;
    margin: 0 auto;
    align-items: flex-start;
    justify-content: center;
}
.promo-block::before {
    content: "";
    position: absolute;
    background-position: center;
    height: 100%;
    width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
    z-index: -1;
}
.promo-pic {
    width: 80px;
    height: 80px;
}
.promo-title {
    display: flex;
    align-items: center;
    gap: 20px;
}
.promo-text-block {
    font-size: 40px;
    line-height: 40px;
    font-weight: 500;
    width: 421px;
}
.promo-info.text1 {
    margin-top: 20px;
    margin-bottom: 20px;
}
.promo-info {
    max-width: 540px;
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
}
.promo-bt.button {
    height: 65px;
    width: 257px;
    background-color: #EEDB6D;
    font-weight: 500;
    line-height: 23.48px;
    font-family: Raleway;
    font-size: 20px;
    padding: 21px 0;
    margin-top: 60px;
    border: none;
}

@media screen and (width <= 769px) {
    .promo-text-block {
        font-size: 30px;
        font-weight: 500;
        line-height: 30px;
        width: 370px;
    }
    .promo-block2 {
        max-width: 690px;
    }
    .promo-pic {
        height: 60px;
        width: 60px;
    }
    .promo-info.text1 {
        margin-top: 30px;
    }
    .promo-info {
        max-width: 690px;
        line-height: 27px;
        font-size: 18px;
        font-weight: 500;
    }
    .promo-bt.button {
        width: 210px;
        height: 60px;
        line-height: 23.48px;
        padding: 18.5px 0;
        margin-top: 30px;
        font-size: 20px;
        font-weight: 500;
    }
}

@media screen and (width <= 577px) {
    .promo-text-block {
        line-height: 24px;
        width: 261px;
        font-size: 24px;
        font-weight: 500;
    }
    .promo-block2 {
        padding: 50px 0;
        max-width: 510px;
    }
    .promo-pic {
        height: 50px;
        width: 50px;
    }
    .promo-info {
        max-width: 510px;
        line-height: 22.4px;
        font-size: 16px;
        font-weight: 500;
    }
    .promo-bt.button {
        width: 190px;
        height: 50px;
        line-height: 21.13px;
        padding: 14.5px 0;
        margin-top: 20px;
        font-size: 18px;
        font-weight: 500;
    }
    .promo-info.text1 {
        margin-top: 20px;
    }
}
@media screen and (width <= 376px) {
    .promo-text-block {
        line-height: 24px;
        width: 230px;
        font-size: 24px;
        font-weight: 500;
    }
    .promo-block2 {
        max-width: 290px;
    }
    .promo-bt.button {
        margin-top: 30px;
        font-size: 18px;
        font-weight: 500;
        width: 290px;
        height: 50px;
        line-height: 21.13px;
    }
    .promo-info {
        font-weight: 500;
        line-height: 22.4px;
        max-width: 510px;
        font-size: 16px;
    }
}
@font-face {
    font-family: Raleway;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>