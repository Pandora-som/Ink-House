<template>
    <div class="about-team">
        <div class="Framepic">
            <img src="Frame-pic.png" alt="frame-pic" class="frame-pic-t">
        </div>
        <div class="about-block">
            <h1 class="about-text-block1">Наша команда</h1>
            <p class="about-text-block2">
                Значимость этих проблем настолько очевидна, что базовый вектор развития
                позволяет оценить значение экспериментов, поражающих по своей масштабности и грандиозности. Мы вынуждены
                отталкиваться от того, что консультация с широким активом.
            </p>
            <div class="teams">
                <img src="Team1.png" alt="Team1" class="teams1">
                <img src="Team2.jpg" alt="Team2" class="teams1">
                <img src="Team3.jpg" alt="Team3" class="teams1">
            </div>
        </div>
    </div>
</template>
<style>
.about-team {
    max-width: 1110px;
    gap: 30px;
    display: flex;
    align-items: center;
    padding: 79px 15px 0;
    margin: 70px auto 0;
}
.frame-pic-t {
    height: 361px;
    width: 445px;
}
.Framepic {
    position: relative;
    width: 445px;
    height: 361px;
}
.about-block {
    text-align: left;
    display: flex;
    flex-direction: column;
    gap: 20px;
    align-items: flex-start;
    justify-content: center;
    font-family: Raleway;
}
.about-text-block1 {
    font-weight: 500;
    font-size: 40px;
    line-height: 44px;
    margin: 0 0 20px 0;
}
.about-text-block2{
    font-weight: 500;
    font-size: 18px;
    line-height: 27px;
}
.teams1 {
    object-position: center;
    height: 80px;
    width: 80px;
    border-radius: 50%;
    object-fit: cover;
}
.teams {
    align-items: center;
    display: flex;
    gap: 30px;
}

@media screen and (width <= 769px) {
    .Framepic, .frame-pic-t {
        height: 413px;
        width: 510px;
    }
    .about-block {
        gap: 30px;
    }
    .about-team {
        flex-direction: column;
        max-width: 690px;
        gap: 40px;
        align-items: flex-start;
    }
    .about-text-block1 {
        font-weight: 500;
        font-size: 30px;
        line-height: 33px;
        margin: 0;
    }
    .about-text-block2{
        font-weight: 500;
        font-size: 18px;
        line-height: 27px;
        margin: 0;
    }
}
@media screen and (width <= 577px) {
    .Framepic, .frame-pic-t {
        height: 304px;
        width: 375px;
    }
    .about-team {
        gap: 30px;
        max-width: 510px;
    }
    .about-block {
        gap: 20px;
    }
    .team_pic_brushes {
        height: 334px;
        width: 227px;
        left: 40px;
        bottom: 36px;
    }
    .about-text-block2 {
        font-weight: 500;
        font-size: 16px;
        line-height: 22.4px;
    }
    .about-text-block1 {
        font-weight: 500;
        font-size: 24px;
        line-height: 26.4px;
    }
}
@media screen and (width <= 376px) {
    .Framepic, .frame-pic-t {
        height: 235px;
        width: 290px;
    }
    .about-team {
        max-width: 290px;
    }
    .about-text-block2{
        font-weight: 500;
        font-size: 16px;
        line-height: 22.4px;
    }
    .about-text-block1 {
        font-weight: 500;
        font-size: 24px;
        line-height: 26.4px;
    }
}
@font-face {
    font-family: RaleWay;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>