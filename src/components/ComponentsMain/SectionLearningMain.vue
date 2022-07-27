<template>
    <div class="container p-2 my-5">
        <div class="row">
            <div class="col-7">
                <h1 class="ms_learning_fs fw-light">{{ title }}</h1>
                <p class="fs-3 fw-light mb-5">{{ subTitle }}</p>

                <ButtonComponent v-for="(element, index) in learningButton" :key="index"
                    :textLearning="element.textLearning"
                />
            </div>
            <div class="col-5">
                
            </div>
        </div>
    </div>
</template>

<script>
import ButtonComponent from '../ComponentCommon/ButtonComponent.vue';
export default {
    props: {
        title: String,
        subTitle: String,
        imgBg: String,
    },

    components: { ButtonComponent },

    data: function(){
        return{
            learningButton: [
                {
                    textLearning: 'Read More',
                }
            ],
        }
    },
}
</script>

<style lang="scss" scoped>

    .ms_learning_fs{
        font-size: 50px;
    }
</style>