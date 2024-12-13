<template>
    <div class="card">
        <img class="card-img" :src="data.url" :alt="data.Name">
        <div class="card-description">
            <p class="card-author">{{ data.author }}</p>
            <h3 class="card-Name">{{ data.Name }}</h3>
            <p class="card-view">{{ data.description }} ({{ data.size }})</p>
            <p class="card-price"> {{ data.price }}</p>
            <button class="card button">В корзину</button>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        data: Object
    }
}
</script>
<style>
.card {
    width: 350px;
    height: 680px;
    background-color: #E1EDE6;
    padding: 20px 0 30px;
    gap: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.card-img {
    height: 422px;
    width: 310px;
    object-fit: cover;
    object-position: center;
}
.card-description {
    width: 310px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
}
.card-author {
    margin: 0 0 10px;
    line-height: 21.13px;
    font-family: Raleway;
    font-size: 18px;
    font-weight: 500;
    color: #86928B;
}
.card-Name {
    margin: 0 0 8px;
    font-weight: 500;
    line-height: 35.22px;
    font-family: Raleway;
    font-size: 30px;
    color: #2C2D35;
}
.card-view {
    margin: 0 0 30px;
    font-weight: 500;
    line-height: 21.13px;
    font-family: Raleway;
    font-size: 18px;
    color: #2C2D35;
}
.card-price {
    margin: 0 0 20px;
    font-weight: 500;
    line-height: 28.18px;
    font-family: Raleway;
    font-size: 24px;
    color: #598D66;
}
.card.button {
    height: 65px;
    width: 310px;
    border: 1px solid #598D66;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    background-color: transparent;
    line-height: 23.48px;
    padding: 21px 0;

    color: #598D66;
    cursor: pointer;
}

@media screen and (width <= 1025px) {
    .card {
        width: 330px;
    }
}
@media screen and (width <= 577px) {
    .card {
        width: 240px;
        height: 464px;
    }
    .card-description {
        width: 200px;
    }
    .card-img {
        width: 200px;
        height: 250px;
    }
    .card-author {
        font-weight: 500;
        line-height: 18.78px;
        font-size: 16px;
    }
    .card-Name {
        margin: 0 0 10px;
        line-height: 28.18px;
        font-size: 24px;
        font-weight: 500;
    }
    .card-view {
        line-height: 18.78px;
        font-size: 16px;
        font-weight: 500;
    }
    .card-price {
        font-size: 20px;
        font-weight: 500;
        margin: 0 0 10px;
        line-height: 23.48px;
    }
    .card.button {
        width: 200px;
        height: 50px;
        line-height: 21.13px;
        padding: 14.5px 0;
        font-size: 18px;
        font-weight: 500;
    }
}
@media screen and (width <= 426px) {
    .card {
        width: 290px;
        height: 464px;
    }
    .card-description {
        width: 250px;
    }
    .card-img {
        width: 250px;
        height: 250px;
    }
    .card-author {
        font-weight: 500;
        line-height: 18.78px;
        font-size: 16px;
    }
    .card-Name {
        font-size: 24px;
        font-weight: 500;
        line-height: 28.18px;
    }
    .card-view {
        line-height: 18.78px;
        font-size: 16px;
        font-weight: 500;
    }
    .card-price {
        line-height: 23.48px;
        font-size: 20px;
        font-weight: 500;
    }
    .card.button {
        width: 250px;
        height: 50px;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}
@font-face {
    font-family: Raleway;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>