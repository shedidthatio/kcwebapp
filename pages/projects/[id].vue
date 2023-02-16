<template>
    <div>
        <p>Project details for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium nesciunt voluptatem vitae laudantium
            veritatis itaque doloremque esse ad officiis incidunt.</p>
</div>
</template>

<script setup lang="ts">
const { id } = useRoute().params
</script>

<style scoped></style>