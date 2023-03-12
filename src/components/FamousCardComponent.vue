<template lang="">
    <div :class="position">
        <a href="#"><img :src="require(`@/assets/${cover}`)" alt="product cover"></a>
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
    div {
        position: relative;
        aspect-ratio: 1/1;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 15px;
        cursor: pointer;

        a {
            img {
                aspect-ratio: 1/1;
                width: 100%;
                height: 100%;
                border-radius: 15px;
                box-shadow: 0px 10px 20px rgba(10, 57, 105, 0.20);

            }
        }
        &:hover::before {
            content: "Découvrir";
            position: absolute;
            z-index: 1;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: rgba(10, 57, 105, 0.7);
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border-radius: 15px;
            font-size: 20px;
            font-family: 'Yeseva One', cursive;
            text-transform: uppercase;
            color: #FFFFFF;
        }
    }
</style>