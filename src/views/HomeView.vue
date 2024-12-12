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
</template>
<style>
.bird-lay{
    display: flex;
    align-items: center;
    justify-content: center;
    max-width: 1110px;
    margin: 0 auto;
    padding: 0 15px;
    gap: 30px;
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
.Title-main {
    color: #598D66;
}
.block2 {
    font-size: 18px;
    font-weight: 500;
    line-height: 27px;
    color: #86928B;
    margin-bottom: 60px;
}
.product.button {
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    color: #598D66;
    border: 1px solid #598D66;
    background-color: transparent;
    width: 225px;
    height: 65px;
    cursor: pointer;
}
</style>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

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
        
    }
}

</script>
