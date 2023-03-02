<template>
    <section class="section" id='homeTopSection'>
        <img src="~/assets/imgs/stars-group.svg" class="absImg" alt="">
        <div class="container-md">
            <div class="colGridParent">
                <div class="colGridChildText">
                    <div class="wrapWBg fadeInLeft">
                        <Heading1 />
                        <p class='my-4'>Capture your realest moments <br /> and hold on for life.</p>
                        <div class="btnWrapper">
                            <NuxtLink to='/' class="button">Book a photo shoot<span class='buttonArrow ps-3'>⟶</span>
                            </NuxtLink>
                            <div class="buttonBackBkg"></div>
                        </div>
                    </div>
                    <div class="colGridParent">
                        <div class="colGridChildImg"><img src="~/assets/imgs/ljd3.svg" alt="3rd off guard image of couple"
                                class='borderDark1 fadeInLeft'>
                        </div>
                        <div class="colGridChildImg" id='img2'><img src="~/assets/imgs/ljd2.svg"
                                alt="2nd off guard image of couple" class='borderDark1 fadeInLeft'>
                        </div>
                    </div>
                </div>
                <div class="colGridChildImg">
                    <img src="~/assets/imgs/ljd1.svg" alt="1st off guard image of couple" class='borderDark1 fadeInLeft'>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'
</script>

<style lang='scss' scoped>
#homeTopSection {
    position: relative;

    .absImg {
        position: absolute;
        z-index: 50;
        top: 8%;
        right: 5%;
        transform: translate(50%, -50%);
        max-width: 80px;
    }

    .colGridParent {
        position: relative;
        z-index: 1;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: 1fr;
        grid-column-gap: 30px;
        grid-row-gap: 30px;

        p {
            font-size: 1.2rem;
        }

        .borderDark1 {
            border: 1px solid $borderDark1;
            border-radius: 40px;
            margin-bottom: 20px;
        }

        .fadeInLeft {
            -webkit-animation: fade-in-bl 2s cubic-bezier(0.390, 0.575, 0.565, 1.000) both;
            animation: fade-in-bl 2s cubic-bezier(0.390, 0.575, 0.565, 1.000) both;

            @-webkit-keyframes fade-in-bl {
                0% {
                    -webkit-transform: translateX(-200px) translateY(50px);
                    transform: translateX(-200px) translateY(50px);
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
                    -webkit-transform: translateX(-200px) translateY(50px);
                    transform: translateX(-200px) translateY(50px);
                    opacity: 0;
                }

                100% {
                    -webkit-transform: translateX(0) translateY(0);
                    transform: translateX(0) translateY(0);
                    opacity: 1;
                }
            }
        }

        #img2 {
            margin-top: -120px;
        }
    }

    /* MEDIA QUERIES */
    @media (max-width: 992px) {
        .absImg {
            position: absolute;
            z-index: 100;
            top: 5%;
            right: 16%;
            max-width: 100px;
        }

        .colGridParent {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: repeat(2, 1fr);
            grid-column-gap: 0px;
            grid-row-gap: 0px;

            #img2 {
                margin-top: 0px;
            }
        }
    }

    @media (max-width: 798px) {
        .absImg {
            position: absolute;
            z-index: 100;
            top: 4%;
            right: 10%;
            max-width: 100px;
        }

        .colGridParent {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: repeat(2, 1fr);
            grid-column-gap: 0px;
            grid-row-gap: 0px;

            #img2 {
                margin-top: 0px;
            }
        }
    }

    @media (max-width: 412px) {
        .absImg {
            position: absolute;
            z-index: 100;
            top: 12%;
            right: 15%;
            max-width: 60px;
        }

        .colGridParent {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: repeat(2, 1fr);
            grid-column-gap: 0px;
            grid-row-gap: 0px;

            #img2 {
                margin-top: 0px;
            }
        }
    }


}
</style>


