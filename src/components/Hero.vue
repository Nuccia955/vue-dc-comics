<template>
    <section class="hero">
        <img src="../assets/jumbotron.jpg" alt="Jumbotron">
    </section>
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style lang="scss">
@import '@/styles/colors.scss';
.hero {
    img {
       width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: top;
        display: block;
    }
}
</style>