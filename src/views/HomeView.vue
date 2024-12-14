<template>
  <div class="bird-lay">
    <img alt="golub" src="../assets/bird.png" class="golub-pic">
    <div class="info-text-block">
            <h1 class="block1">
                Реплики картин от <span class="Title-main">Ink. House</span>
            </h1>
            <p class="block2">
                Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения, доступные цены.
            </p>
            <button class="product button">Продукция</button>
        </div>
  </div>
  <ReproductionBlock />
  <PromoBlock />
</template>
<style>
.bird-lay{
    max-width: 1110px;
    margin: 0 auto;
    padding: 0 15px;
    gap: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.Title-main {
    color: #598D66;
}
.golub-pic {
    width: 540px;
    height: 621px;
}
.info-text-block {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    font-family: Raleway;
    text-align: left;
}
.block1{
    font-size: 60px;
    font-weight: 500;
    line-height: 66px;
    color: #2C2D35;
    margin-bottom: 20px;
}
.block2 {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
    color: #86928B;
    margin-bottom: 60px;
}
.product.button {
    width: 225px;
    height: 65px;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    color: #598D66;
    border: 1px solid #598D66;
    background-color: transparent;
    cursor: pointer;
}
@media screen and (width <= 577px) {
    .block1 {
        line-height: 36px;
        margin-bottom: 10px;
        font-size: 36px;
        font-weight: 500;
    }
    .golub-pic {
        height: 239px;
        width: 195px;
    }
    .bird-lay {
        margin-top: 50px;
        padding: 0 33px;
    }
    .block2 {
        line-height: 24px;
        margin-bottom: 11px;
        font-size: 16px;
        font-weight: 500;
    }
    .product.button  {
        width: 178px;
        height: 50px;
        font-family: Raleway;
        font-size: 18px;
        font-weight: 500;
        line-height: 21.13px;
    }
}

@media screen and (width <= 769px) {
    .golub-pic {
        height: 380px;
        width: 330px;
    }
    .bird-lay {
        padding: 0 39px;
    }
    .block2 {
        margin-bottom: 40px;
    }
    .block1 {
        font-size: 40px;
        font-weight: 500;
        line-height: 40px;
    }
    .product.button {
        height: 60px;
        width: 210px;
    }
}
@media screen and (width <= 376px) {
    .golub-pic {
        display: none;
    }
    .bird-lay {
        margin-top: 60px;
        padding: 0 15px;
    }
    .block1 {
        line-height: 30px;
        margin-bottom: 20px;
        font-size: 30px;
        font-weight: 500;
    }
    .block2 {
        line-height: 21px;
        margin-bottom: 40px;
        font-size: 14px;
        font-weight: 500;
    }
    .product.button {
        height: 50px;
        width: 154px;
    }
}
@font-face {
    font-family: Raleway;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import PromoBlock from '@/components/PromoBlock.vue';
import ReproductionBlock from '@/components/ReproductionBlock.vue';

/*export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}*/
export default {
    data() {
        return {

        }
    },
    components: {
        ReproductionBlock,
        PromoBlock
    }
}

</script>
