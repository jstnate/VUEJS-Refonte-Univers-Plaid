<template lang="">
    <div id="famous-card" :class="position">
        <img :src="require(`@/assets/${cover}`)" alt="product cover">
        <a href="#">Découvrir</a>
    </div>
</template>
<script>
export default {
    name: "FamousCardComponent",
    props: {
        cover: {
            type: String,
            required: true
        },
        position: {
            type: String,
            required: true
        }
    }
}
</script>
<style lang="scss" scoped>
    #famous-card {
        position: relative;
        aspect-ratio: 1/1;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 15px;
        cursor: pointer;

        img {
            aspect-ratio: 1/1;
            width: 100%;
            height: 100%;
            border-radius: 15px;
            box-shadow: 0px 10px 20px rgba(10, 57, 105, 0.15);

        }

        a {
            width: 100%;
            height: 100%;
            background-color: rgba(10, 57, 105, .6);
            position: absolute;
            top: 0;
            left: 0;
            border-radius: 10px;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            text-decoration: none;
            font-family: 'Yeseva One', cursive;
            font-size: 24px;
            display: none;
        }

        &:hover a {
            display: flex;
        }
    }
</style>