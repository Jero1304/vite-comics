<template>
    <div class="container">
        <div class="row header-bar">
            <img src="/img/dc-logo.png" alt="">
            
            <nav>
                <ul class="menu">
                    <li class="menu-item">charters</li>
                    <li class="menu-item active">comics</li>
                    <li class="menu-item">movies</li>
                    <li class="menu-item">tv</li>
                    <li class="menu-item">games</li>
                    <li class="menu-item">collectibles</li>
                    <li class="menu-item">videos</li>
                    <li class="menu-item">fans</li>
                    <li class="menu-item">news</li>
                    <li class="menu-item">shop</li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss">
@use '../style/patrials/variables.scss';
    .header-bar{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;

        .menu{
            display: flex;
            /* padding: 10px 20px; */
            .menu-item{
                padding: 10px 10px;
                font-size: 15px;
                font-weight: bold;
                text-transform: uppercase;

                &.active{
                    color: #0282F9;
                }
            }
        }
    }

</style>