<template>
    <div>
        <p v-if="!aboutreproduction">Загрузка...</p>
        <div v-else>
            <div class="filter">
                <h2 class="h-rep">Репродукции</h2>
                <div class="country">
                    <button class="countries button" v-for="(element, key) in aboutreproduction" :key="key"
                        @click="nextReproduction(element)">{{ element.Country }}</button>
                </div>
            </div>
            <div class="reproductions__grid">
                <PicturesRep v-for="(picturecard, i) in reproductions" :key="i" :data="picturecard" />
            </div>
        </div>
    </div>
</template>

<script>
import PicturesRep from './PicturesRep.vue';

export default {
    data() {
        return {
            aboutreproduction: null,
            reproductions: null
        }
    },
    methods: {
        nextReproduction(element) {
            this.reproductions = element.Reproductions;
        }
    },
    mounted() {
        fetch("aboutreproduction.json")
        .then(resp => resp.json())
        .then(json => {
            this.aboutreproduction = json;
            this.reproductions = this.aboutreproduction.ForFranceRep.Reproductions;
        });
    },
    components: {
        PicturesRep
    }
}
</script>

<style>
.h-rep {
    font-weight: 500;
    line-height: 44px;
    font-family: Raleway;
    font-size: 40px;
    color: #2C2D35;
}
.filter {
    max-width: 1110px;
    margin: 0 auto 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}
.country::-webkit-scrollbar {
    width: 0;
}
.country {
    overflow-x: scroll;
    gap: 0 32px;
    display: flex;
    justify-content: flex-start;
    align-items: center;
}
.reproductions__grid {
    align-items: center;
    justify-items: center;
    gap: 30px;
    margin: 0 auto;
    display: grid;
    max-width: 1110px;
    grid-template-columns: repeat(3, 350px);
    grid-template-rows: repeat(2, 730px);
    justify-content: center;
}
.countries.button {
    border-radius: 20px;
    font-family: Raleway;
    font-size: 20px;
    font-weight: 500;
    line-height: 23.48px;
    border: none;
    padding: 10px 20px;
    background-color: #D4E8D9;
    color: #2C2D35;
}

@media screen and (width <= 1025px) {
    .h-rep {
        font-weight: 500;
        line-height: 33px;
        font-size: 30px;
    }
    .filter {
        max-width: 690px;
        padding: 0 39px;
    }
    .reproductions__grid {
        max-width: 690px;
        grid-template-rows: repeat(3, 730px);
        grid-template-columns: repeat(2, 330px);
    }
    .countries.button {
        font-weight: 500;
        line-height: 23.48px;
        font-size: 20px;
    }
}

@media screen and (width <= 577px) {
    .h-rep {
        font-weight: 500;
        line-height: 26.4px;
        margin: 20px inherit;
        font-size: 24px;
    }
    .filter {
        padding: 0 33px;
        margin: 0 auto 20px;
        max-width: 510px;
    }
    .reproductions__grid {
        grid-template-columns: repeat(2, 240px);
        grid-template-rows: repeat(3, 514px);
        max-width: 510px;
    }
    .countries.button {
        font-weight: 500;
        line-height: 21.13px;
        font-size: 18px;
    }
}

@media screen and (width <= 426px) {
    .h-rep {
        font-weight: 500;
        line-height: 26.4px;
        font-size: 24px;
    }
    .filter {
        max-width: 290px;
        padding: 0 15px;
    }
    .country{
        gap: 0 20px;
    }
    .reproductions__grid {
        grid-template-columns: repeat(1, 290px);
        grid-template-rows: repeat(6, 514px);
        max-width: 510px;
    }
    .countries.button {
        font-weight: 500;
        line-height: 21.13px;
        font-size: 18px;
    }
}
@font-face {
    font-family: Raleway;
    src: url("../assets/fonts/Raleway-VariableFont_wght.ttf");
}
</style>