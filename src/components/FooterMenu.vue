<template>
    <a href="#">
        <li>
            {{ link }}
        </li>
    </a>
    </template>

<script>
    export default {
        props:{
            title: String,
            link: String,
        }
    }
</script>

<style>

</style>