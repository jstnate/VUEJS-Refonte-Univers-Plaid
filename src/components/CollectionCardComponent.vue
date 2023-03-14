<template lang="">
    <div class="collection">
        <img :src="require(`@/assets/${cover}`)" alt="collection cover">
        <h4>{{ title }}</h4>
        <p>{{ description }}</p>
        <a href="#">
            Découvrir
        </a>
    </div>
</template>
<script>
    export default {
        name: 'CollectionCardComponent',
        props: {
            title: {
                type: String,
                required: true
            },
            description: {
                type: String,
                required: true
            },
            cover: {
                type: String,
                required: true
            }
        }
    }
</script>
<style lang="scss" scoped>
    .collection {
        position: relative;
        width: 90%;
        border-radius: 10px;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 15px;
        text-align: center;
        color: #0A3969;
        overflow: hidden;
        height: 60vh;
        box-shadow: 0px 5px 20px rgba(10, 57, 105, 0.15);

        @media screen and (min-width: 1024px) {
            height: 50vh;
        }

        img {
            width: 100%;
            border-radius: 10px;
        }

        h4 {
            margin-top: 20px;
            font-size: 24px;
            font-weight: 900;
            @media screen and (min-width: 1024px) {
                font-size: 24px;   
            }
        }

        p {
            width: 90%;
            @media screen and (min-width: 1024px) {
                font-size: 16px;
            }
        }

        a {
            position: absolute;
            background-color: rgba(10, 57, 105, 1);
            color: #FFFFFF;
            font-family: 'Yeseva One', cursive;
            font-size: 24px;
            font-weight: 900;
            text-decoration: none;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 150px;
            width: 150px;
            border-radius: 50%;
            bottom: -85px;
            left: -85px;
            transition: all .3s ease;
            @media screen and (min-width: 1024px) {
                bottom: -100px;
                left: -100px;
            }
        }

        &:hover a {
            background-color: rgba(10, 57, 105, .7);
            height: 100%;
            width: 100%;
            border-radius: 0;
            bottom: 0;
            left: 0;
        }
    }
</style>