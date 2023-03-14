<template lang="">
    <div>
        <img :src="require(`@/assets/${icon}`)" alt="service icon">
        <h4>{{ title }}</h4>
        <p>{{ description }}</p>
    </div>
</template>
<script>
export default {
    name: 'ServiceComponent',
    props: {
        title: {
            type: String,
            required: true
        },
        description: {
            type: String,
            required: false
        },
        icon: {
            type: String,
            required: true
        }
    }    
}
</script>
<style lang="scss" scoped>
    div {
        width: 90%;
        color: #0A3969;
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 10px;

        @media screen and (min-width: 1024px) {
            width: 40%;
            gap: 20px;
        }

        img {
            width: 70px;

            @media screen and (min-width: 1024px) {
                width: 100px;
            }
        }
        h4 {
            font-size: 24px;
            font-weight: bold;

            @media screen and (min-width: 1024px) {
                font-size: 36px;
            }
        }
        p {
            font-size: 20px;
            font-weight: 100;
            font-style: italic;

            @media screen and (min-width: 1024px) {
                font-size: 28px;
            }
        }
    }
</style>