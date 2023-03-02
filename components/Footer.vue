<template>
    <div>
        <section id="footer-section">
            <div class="container">
                <footer class="d-sm-flex flex-sm-column">

                    <p class='mb-0 me-auto small'>© 2023 shedidthatio</p>

                    <ul class='list-unstyled'>
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

<style scoped lang='scss'>
#footer-section {
    background-color: $lightBg;
    border-top: 1px solid $borderDark4;

    a {
        color: $darkText3;
        opacity: .8;
    }
}
</style>