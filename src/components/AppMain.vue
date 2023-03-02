<template>
    <MainJumbotron/>
    <div id="bg-color-black">
        <div class="container">
            <div class="grid">
                <MainCard 
                v-for="(card,i) in cards" 
                :key="i"
                :thumb="card.thumb" 
                :series="card.series"/>
            </div>
        </div>
    </div>
</template>

<script>
    import MainCard from './MainCard.vue'
    import MainJumbotron from './MainJumbotron.vue'

    export default{
        components:{
            MainCard,
            MainJumbotron,
        },
        data() {
            return {
                cards: [
                    {
                        thumb: "https://cdnb.artstation.com/p/assets/images/images/003/613/605/large/marco-ferrari-batman-colori-finito-300px.jpg?1475606800",
                        price: "$19.99",
                        series: "Action Comics",
                        type: "comic book"
                    },
                    {
                        thumb: "http://img3.wikia.nocookie.net/__cb20130913191629/marvel_dc/images/thumb/0/01/Batman_Vol_2_23.2_The_Riddler.jpg/300px-Batman_Vol_2_23.2_The_Riddler.jpg",
                        price: "$3.99",
                        series: "American Vampire 1976",
                        type: "comic book"
                    },
                    {
                        thumb: "https://tomjoynerphd.files.wordpress.com/2012/10/300px-doctor_fate_vol_2_38.jpg?w=584",
                        price: "$16.99",
                        series: "Aquaman",
                        type: "graphic novel"
                    },
                    {
                        thumb: "https://comicbookrealm.com/cover-scan/366e31ce0ac426077d49bcfbb3740076/l/dc-comics-superman-war-of-the-worlds-issue-1.jpg",
                        price: "$2.99",
                        series: "Batgirl",
                        type: "comic book"
                    },
                    {
                        thumb: "https://comicvine.gamespot.com/a/uploads/original/11113/111131213/3338279-5060574551-300px.jpg",
                        price: "$3.99",
                        series: "Batman",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.comicbookdaily.com/wp-content/uploads/2010/01/300px-Booster_Gold_v.2_1.jpg",
                        price: "$2.99",
                        series: "Batman Beyond",
                        type: "comic book"
                    },
                    {
                        thumb: "https://upload.wikimedia.org/wikipedia/commons/thumb/b/b9/Batman_Comic_Book_-_NARA_-_595420.gif/300px-Batman_Comic_Book_-_NARA_-_595420.gif",
                        price: "$3.99",
                        series: "Batman/Superman",
                        type: "comic book"
                    },
                    {
                        thumb: "http://3.bp.blogspot.com/-QFvcimT3YeU/VHTtDvHCVcI/AAAAAAAAFjg/rHhUowlG86k/s1600/300px-Batman_'66_Meets_The_Green_Hornet_Vol_1_6_Textless.jpg",
                        price: "$4.99",
                        series: "Batman/Superman Annual",
                        type: "comic book"
                    },
                    {
                        thumb: "http://1.bp.blogspot.com/-0g0dqYPWSGM/UXv1gNf5fFI/AAAAAAAAFdk/MtvchZyKGqE/s1600/300px-DC_Comics_Presents_33.jpg",
                        price: "$5.99",
                        series: "Batman: The Joker War Zone",
                        type: "comic book"
                    },
                    {
                        thumb: "https://thumbnails.pcgamingwiki.com/5/56/DC_Universe_Online_cover.jpg/300px-DC_Universe_Online_cover.jpg",
                        price: "$6.99",
                        series: "Batman: Three Jokers",
                        type: "comic book"
                    },
                    {
                        thumb: "https://i.pinimg.com/736x/21/e7/ac/21e7ac0a1e74d622b9093a94286ff4d1--comic-book-covers-comic-books.jpg",
                        price: "$4.99",
                        series: "Batman: White Knight Presents: Harley Quinn",
                        type: "comic book"
                    },
                    {
                        thumb: "https://i0.wp.com/img3.wikia.nocookie.net/__cb20140520225225/marvel_dc/images/thumb/f/f4/Forever_Evil_Vol_1_7_001.jpg/300px-Forever_Evil_Vol_1_7_001.jpg",
                        price: "$16.99",
                        series: "Catwoman",
                        type: "graphic novel"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss">
@use '../style/patrials/variables' as *;
    #bg-color-black{
        background-color: $black;
        color: white;
        padding: 40px 0;

        .grid{
            display: grid;
            grid-template-columns: repeat(6,1fr);
            gap: 20px;
            row-gap: 50px;
            .card img{
                width: 200px;
                height: 200px;
            }
            .card h3{
                padding-top:20px ;
                text-transform: uppercase;
            }
        }
    }

    

</style>