<template>
    <section class="tools">
        <ul class="container d-flex justify-content-around align-items-center">
            <li v-for="(tool, index) in tools" :key="`tool ${index}`" class="d-flex align-items-center">
                <img :src="tool.img" :alt="tool.text">
                <span>{{ tool.text }}</span>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
    name: 'Tools',
    data() {
        return {
            tools: [
                {
                    img: require('@/assets/buy-comics-digital-comics.png'),
                    text: 'Digital Comics'
                },
                {
                    img: require('@/assets/buy-comics-merchandise.png'),
                    text: 'DC Merchandise'
                },
                {
                    img: require('@/assets/buy-comics-shop-locator.png'),
                    text: 'Subscription'
                },
                {
                    img: require('@/assets/buy-comics-subscriptions.png'),
                    text: 'Comic Shop Locator'
                },
                {
                    img: require('@/assets/buy-dc-power-visa.svg'),
                    text: 'DC Power Visa'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import '@/styles/utilities.scss';
@import '@/styles/colors.scss';

.tools {
    background-color: $brand_primary ;
    padding: 50px 0;

    img {
        width: 45px;
        margin-right: 15px;
    }

    span {
        color: #fff;
        text-transform: uppercase;
        font-size: 0.8em;
    }
}

</style>