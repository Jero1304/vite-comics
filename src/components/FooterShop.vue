<template>
    <li class="menu-item">
        <img :src="icon" alt="">
        <p>{{ text }}</p>
    </li>
</template>

<script>
export default {
    props: {
        icon: String,
        text: String,
    }
}
</script>

<style></style>