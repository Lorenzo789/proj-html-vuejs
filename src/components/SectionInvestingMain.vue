<template>
    <div class="container p-2">
        <div class="row mt-5 align-items-center">
            <div class="col-6 p-4">
                <h1 class="ms_investing_fs fw-light">{{ title }}</h1>
                <p class="fs-3 fw-light mb-5">{{ subTitle }}</p>

                <ButtonComponent v-for="(text, index) in textInvesting" :key="index"
                    :textInvesting="text.content"/>

            </div>
            <div class="col-6 mt-5 position-relative">
                <img class="ms_img" src="../assets/images/base.png" alt="">
                <img class="ms_book1" src="../assets/images/book1.png" alt="">
                <img class="ms_book2" src="../assets/images/book2.png" alt="">
                <img class="ms_magnifier" src="../assets/images/magnifier.png" alt="">
                <img class="ms_bubble" src="../assets/images/bubblespeech.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
import ButtonComponent from './ButtonComponent.vue';
export default {

    props: {
        title: String,
        subTitle: String,
    },

    components: { ButtonComponent },

    data: function(){
        return{
            textInvesting: [
                {
                    content: 'Join For Free',
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import'../styles/variables.scss';

    .ms_investing_fs{
        font-size: 65px;
    }

    .ms_img{
        object-fit: cover;
        height: 100%;
        width: 100%;
    }

    .ms_book1{
        position: absolute;
        top: 115px;
        right: 50px
    }

    .ms_book2{
        position: absolute;
        top: 290px;
        right: 175px;
    }

    .ms_magnifier{
        position: absolute;
        bottom: 110px;
        right: 90px;
    }

    .ms_bubble{
        position: absolute;
        top: 65px;
        right: 50px;
    }

</style>