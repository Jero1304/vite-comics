<template>
    <div class="container">
        <div class="header-bar">
            <img src="/img/dc-logo.png" alt="">
            <nav>
                <ul class="menu">
                    <HeaderMenu v-for="(option, i) in options" 
                    :key="i" 
                    :option="option"/>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
import HeaderMenu from "./HeaderMenu.vue"
export default {
    components: {
        HeaderMenu
    },
    data() {
        return {
            options: [
                    'charter',
                    'comics',
                    'movies',
                    'TV',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop'
                ]
        }
    }
} 
</script>

<style lang="scss">
@use '../style/patrials/variables' as *;
    .header-bar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;

        .menu{
            display: flex;
            .menu-item{
                color: black;
                padding: 10px 10px;
                font-size: 15px;
                font-weight: bold;
                text-transform: uppercase;

                &.active{
                    color: $blue;
                    border-bottom: 3px solid $blue;
                }
                &:hover{
                    color: $blue;
                }
            }
        }
    }

</style>