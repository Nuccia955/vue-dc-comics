<template>
    <section class="comics">
        <button class="btn">Current Series</button>
        <ul class="d-flex flex-wrap container">
            <ComicCard v-for="(comic,index) in Comics" :key="`comic ${index}`"
                :img="comic.thumb"
                :title="comic.series"/>
        </ul>
        <div class="link text-center">
            <a href="/" class="d-inline-block">Load More</a>
        </div>
    </section>
</template>

<script>
import Comics from '@/data/dc-comics.js'
import ComicCard from '@/components/Comic_card.vue'
export default {
    name: 'Comics',
    components: {
        ComicCard,
    },
    data() {
        return {
            Comics,
        } 
    },
}
</script>

<style lang="scss">
@import '@/styles/utilities.scss';
@import '@/styles/colors.scss';

.comics {
    position: relative;
    padding: 55px 0;
    color: #fff;
    background-color: #000;
    .btn {
        border: transparent;
        color: #fff;
        position: absolute;
        top: 0;
        left: 50px;
        transform: translateY(-50%);
        z-index: 3;
        background-color: $brand_primary;
        font-weight: 600;
        font-size: 1.2em;
        text-transform: uppercase;
        padding: 10px 30px;
        &:hover {
            cursor: pointer;
        }
    }
    &  a {
        color: #fff;
        padding: 10px 60px;
        text-transform: uppercase;
        background-color: $brand_primary;
        font-weight: 600;
        font-size: 1.2em;
    }
}
</style>