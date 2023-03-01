<template>
    <section class="section">
        <div class="container-md">
            <div class="colGridParent">
                <div class="colGridChild1">
                    <h1 class='homeTopLeft'>Off Guards</h1>
                    <p class='homeTopLeft'>Capture your realest moments <br /> and hold on for life.</p>
                    <img src="~/assets/imgs/stars-group.svg" alt="magical stars" class='homeTopLeft border-0 pAbsolute'>
                    <div class="btnWrapper homeTopLeft">
                        <NuxtLink to='/' class="button">Book a photo shoot<span class='buttonArrow ps-3'>⟶</span>
                        </NuxtLink>
                        <div class="buttonBackBkg"></div>
                    </div>
                    <div class="colGridParent">
                        <div class="colGridChild1"><img src="~/assets/imgs/ljd3.svg" class="fadeInTl" id="ljdImg3"
                                alt="3rd off guard image of couple">
                        </div>
                        <div class="colGridChild2"><img src="~/assets/imgs/ljd2.svg" class="fadeInTl" id="ljdImg2"
                                alt="2nd off guard image of couple">
                        </div>
                    </div>
                </div>
                <div class="colGridChild2">
                    <img src="~/assets/imgs/ljd1.svg" class="fadeInTr" id="ljdImg1" alt="1st off guard image of couple">
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'

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

.homeTopLeft {
    -webkit-animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 0.5s both;
    animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 0.5s both;

    @-webkit-keyframes fade-in-bl {
        0% {
            -webkit-transform: translateX(-50px) translateY(50px);
            transform: translateX(-50px) translateY(50px);
            opacity: 0;
        }

        100% {
            -webkit-transform: translateX(0) translateY(0);
            transform: translateX(0) translateY(0);
            opacity: 1;
        }
    }

    @keyframes fade-in-bl {
        0% {
            -webkit-transform: translateX(-50px) translateY(50px);
            transform: translateX(-50px) translateY(50px);
            opacity: 0;
        }

        100% {
            -webkit-transform: translateX(0) translateY(0);
            transform: translateX(0) translateY(0);
            opacity: 1;
        }
    }
}

.colGridChild1 {
    position: relative;


    p {
        font-size: 20px;
    }

    img.pAbsolute {
        position: absolute;
        top: -40px;
        left: 84%;
        -webkit-animation: blink-2 3s cubic-bezier(0.455, 0.030, 0.515, 0.955) 4s infinite both;
        animation: blink-2 3s cubic-bezier(0.455, 0.030, 0.515, 0.955) 4s infinite both;

        @-webkit-keyframes blink-2 {
            0% {
                opacity: 1;
            }

            50% {
                opacity: 0.2;
            }

            100% {
                opacity: 1;
            }
        }

        @keyframes blink-2 {
            0% {
                opacity: 1;
            }

            50% {
                opacity: 0.2;
            }

            100% {
                opacity: 1;
            }
        }
    }

    .colGridChild2 {
        margin-top: -90px;
    }

}

.colGridChild1,
.colGridChild2 {

    #ljdImg3 {
        -webkit-animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 1.5s both;
        animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 1.5s both;

        @-webkit-keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }

        @keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }
    }

    #ljdImg2 {
        -webkit-animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 2s both;
        animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 2s both;

        @-webkit-keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }

        @keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }

    }

    #ljdImg1 {
        -webkit-animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 2.5s both;
        animation: fade-in-bl 1s cubic-bezier(0.390, 0.575, 0.565, 1.000) 2.5s both;

        @-webkit-keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }

        @keyframes fade-in-bl {
            0% {
                -webkit-transform: translateX(-50px) translateY(50px);
                transform: translateX(-50px) translateY(50px);
                opacity: 0;
            }

            100% {
                -webkit-transform: translateX(0) translateY(0);
                transform: translateX(0) translateY(0);
                opacity: 1;
            }
        }
    }
}

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


