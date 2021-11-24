<template>
    <li class="comic">
        <img :src="img" :alt="title">
        <span>{{ title }}</span>
    </li>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        img: String,
        title: String,
    }
}
</script>

<style lang="scss">
@import '@/styles/colors.scss';
.comic {
    width: calc((100% / 6) - 26px);
    margin: 0 13px 50px;
    img {
        width: 100%;
        height: 185px;
        object-fit:cover;
        object-position: top;
        margin-bottom: 20px;
    }
    span {
        font-size: 0.8em;
        text-transform: uppercase;
        margin-bottom: 3px;
    }
}

</style>