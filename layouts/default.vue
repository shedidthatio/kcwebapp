<template>
    <div>
        <header>
            <nav class="navbar navbar-expand-lg fixed-top">
                <div class="container-fluid">
                    <NuxtLink to='/' class='navbar-brand flex-sm-wrap-reverse'><img src="~/assets/imgs/brandGroup.svg"
                            alt="Brand logo of a girl taking a photo"></NuxtLink>
                    <button class="navbar-toggler hamburger me-4" type="button" data-bs-toggle="collapse"
                        data-bs-target="#hamburger" aria-controls="hamburger" aria-expanded="false"
                        aria-label="Toggle navigation">
                        <span class="barShort"></span>
                        <span class="barLong"></span>
                        <span class="barShort"></span>

                    </button>
                    <div class="collapse navbar-collapse" id="hamburger">
                        <ul id='mainUl' class="navbar-nav ps-4 me-auto mb-2 mb-lg-0">
                            <li class="nav-item">
                                <NuxtLink to='/' class='nav-link'>Off Guards</NuxtLink>
                            </li>
                            <li class="nav-item">
                                <NuxtLink to='/' class='nav-link'>Collaborations</NuxtLink>
                            </li>
                            <li class="nav-item">
                                <NuxtLink to='/' class='nav-link'>About</NuxtLink>
                            </li>
                        </ul>
                        <ul id='ctaUL' class="navbar-nav ps-4 ms-auto mb-4 mb-lg-0">
                            <li class="nav-item">
                                <NuxtLink to='/'
                                    class='nav-link social-link d-flex justify-content-center align-items-center px-3'>
                                    <i class="fa-brands fa-square-youtube"></i>
                                    <div class="social-back-bcg"></div>
                                    <div class="social-top-bcg"></div>
                                </NuxtLink>
                            </li>
                            <li class="nav-item">
                                <NuxtLink to='/'
                                    class='nav-link social-link d-flex justify-content-center align-items-center px-3'>
                                    <i class="fa-brands fa-instagram"></i>
                                    <div class="social-back-bcg"></div>
                                    <div class="social-top-bcg"></div>
                                </NuxtLink>
                            </li>
                            <li class="nav-item">
                                <NuxtLink to='/'
                                    class='nav-link social-link d-flex justify-content-center align-items-center px-3'>
                                    <i class="fa-brands fa-tiktok"></i>
                                    <div class="social-back-bcg"></div>
                                    <div class="social-top-bcg"></div>
                                </NuxtLink>
                            </li>
                            <li class="nav-item">
                                <NuxtLink to='/' id='navCTA'
                                    class='nav-link d-flex justify-content-center align-items-center mt-1 px-3'>Book
                                    It<span><img src="~/assets/imgs/small-star.svg" alt="small decorative star"
                                            class='ms-2'></span>
                                    <div class="nav-cta-back"></div>
                                </NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </header>

        <!-- Output the page content -->
        <div>
            <slot />
        </div>

        <section id="footer-section">
            <div class="container">
                <footer class="d-flex justify-space-between align-items-center">

                    <p class='mb-0 me-auto small'>© 2023 shedidthatio</p>

                    <ul class="nav justify-content-end">
                        <li class="nav-item">
                            <NuxtLink to='#' class="nav-link px-2">Home</NuxtLink>
                        </li>
                        <li class="nav-item"><a href="#" class="nav-link px-2">Off Guards</a></li>
                        <li class="nav-item"><a href="#" class="nav-link px-2">Collaborations</a></li>
                        <li class="nav-item"><a href="#" class="nav-link px-2">About</a></li>
                        <li class="nav-item"><a href="#" class="nav-link px-2">FAQs</a></li>
                    </ul>
                </footer>
            </div>
        </section>
    </div>
</template>

<script setup lang="ts">

</script>

<style lang='scss' scoped>
.navbar {
    background-color: $lightBg;
    border-bottom: 1px solid $borderDark4;
}

#navCTA {
    position: relative;
    background-color: $primary2;
    color: $darkText1;
    font-weight: 500;
    border: 1px solid $borderDark1;
    border-radius: 100px;
    z-index: 1;
    max-width: fit-content;
    transition: all 0.3s ease-in-out;

    .nav-cta-back {
        position: absolute;
        left: -2px;
        top: -2px;
        right: 2px;
        bottom: 2px;
        border: 1px solid $borderDark1;
        border-radius: 50px;
        background-color: $primary4;
        z-index: -1;
    }
}

#navCTA:hover {
    transform: translateY(10px);
}

.social-link {
    position: relative;
    width: 40px;
    height: 40px;
    margin-right: 20px;
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    -webkit-box-pack: center;
    justify-content: center;
    -webkit-justify-content: center;
    -ms-flex-pack: center;
    -webkit-box-align: center;
    align-items: center;
    -webkit-align-items: center;
    -ms-flex-align: center;
    transition: all 0.3s ease-in-out;

    i {
        position: absolute;
        z-index: 1;
        font-size: 1.25em;
    }

    .social-back-bcg {
        position: absolute;
        left: 2px;
        top: 2px;
        right: -2px;
        bottom: -2px;
        border: 1px solid $borderDark1;
        border-radius: 50px;
        background-color: $primary2;
    }

    .social-top-bcg {
        position: absolute;
        left: 0%;
        top: 0%;
        right: 0%;
        bottom: 0%;
        border: 1px solid $borderDark1;
        border-radius: 50px;
        background-color: $primary4;
    }
}

.social-link:hover {
    transform: translateY(10px);
}

.navbar-toggler:focus {
    box-shadow: none;
    border: 1px solid $startStateBg1;
}

.hamburger {
    cursor: pointer;
    border: 0;
    background-color: transparent;
    border: 1px solid transparent;
    transition: all 0.3s ease;
}

.hamburger:hover {
    border: 1px solid $startStateBg1;
}


.barShort,
.barLong {
    display: block;
    height: 2px;
    margin: 5px auto;
    -webkit-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
    background-color: $darkBg3;
    border-radius: 3px;
}

.barShort {
    width: 20px;
}

.barLong {
    width: 25px;
}

#footer-section {
    background-color: $lightBg;
    border-top: 1px solid $borderDark4;

    a {
        color: $darkText3;
        opacity: .8;
    }
}

@media (max-width: 992px) {
    #ctaUL {
        flex-direction: row;
        justify-content: space-between;
    }
}
</style>