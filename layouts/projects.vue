<template>
    <div>
        <header>
            <nav>
                <ul>
                    <li>
                        <NuxtLink to='/'>Brand</NuxtLink>
                        <NuxtLink to='/projects'>Projects</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>

        <!-- Output the page content -->
        <div>
            <slot />
        </div>

        <footer>
            <NuxtLink to='/'>Brand</NuxtLink>
            <NuxtLink to='/projects'>Projects</NuxtLink>
            <NuxtLink to='/about'>About</NuxtLink>
        </footer>
    </div>
</template>

<script setup lang="ts">

</script>

<style scoped></style>