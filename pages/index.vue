<template>
    <section class="section">
        <div class="container-md">
            <div class="colGridParent">
                <div class="colGridChild1">
                    <h1>Off Guards</h1>
                    <p>Capture your realest moments and hold on to the memories. </p>
                    <div class="btnWrapper">
                        <NuxtLink to='/' class="button">Book a photo shoot<span class='buttonArrow ps-3'>⟶</span>
                        </NuxtLink>
                        <div class="buttonBackBkg"></div>
                    </div>
                    <div class="colGridParent">
                        <div class="colGridChild1"><img src="~/assets/imgs/ljd3.svg" alt=""></div>
                        <div class="colGridChild2"><img src="~/assets/imgs/ljd2.svg" alt=""></div>
                    </div>
                </div>
                <div class="colGridChild2">
                    <img src="~/assets/imgs/ljd1.svg" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'

definePageMeta({
    layout: 'default'
})
</script>

<style lang='scss' scoped>
.colGridParent {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 30px;
    grid-row-gap: 30px;

    img {
        border: 1px solid $borderDark1;
        border-radius: 40px;
        margin-bottom: 20px;
    }
}

.colGridChild1 {

    p {
        font-size: 24px;
    }

    .colGridChild2 {
        margin-top: -60px;
    }

}

// .colGridChild2 {}

/* MEDIA QUERIES */
@media (max-width: 992px) {
    .colGridParent {
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: repeat(2, 1fr);
        grid-column-gap: 0px;
        grid-row-gap: 0px;
    }

    .colGridChild1 {
        .colGridChild2 {
            margin-top: 0px;
        }
    }

    // .colGridChild2 {

    // }
}
</style>


