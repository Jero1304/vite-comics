<template>
    <div class="card">
        <img :src="thumb" alt="">
        <h3>{{ series }}</h3>
    </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        series: String,
    }
}

</script>

<style>
.card{
    cursor: pointer;
}
.card img {
    width: 200px;
    height: 200px;
}
</style>