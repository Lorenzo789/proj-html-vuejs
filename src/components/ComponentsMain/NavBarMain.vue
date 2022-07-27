<template>
    <div class="container p-2 d-flex justify-content-between align-items-baseline mt-3">

    <img class="align-self-center" src="../../assets/images/MasterStudy_logo.svg" alt="">

    <div class="d-flex align-items-baseline">
        <p class="ms_color ms_fs text-uppercase me-2"><i class="fa-solid fa-bars ms_fs"></i> Category</p>
        
        <SearchBarComponent v-for="(info, index) in navBarSearch" :key="index"
            :text="info.text"/>
    </div>

    <div class="d-flex align-items-baseline">
        <p class="me-3"><i class="fa-solid fa-bullhorn ms_color_icon"></i> Become an Instructor</p>
        <p class="me-3"><i class="fa-solid fa-briefcase ms_color_icon"></i> For Enterprise</p>
    </div>

    <div class="d-flex align-items-baseline">
        <p class="me-3"><i class="fa-solid fa-user ms_color_icon"></i> Log In</p>

        <ButtonComponent v-for="(content, index) in buttonContent" :key="index"
            :text="content.text"/>

        <i class="fa-solid fa-bookmark ms_color_icon fs-4 ms-4"></i>
    </div>
</div>
</template>

<script>
import SearchBarComponent from '../ComponentCommon/SearchBarComponent.vue';
import ButtonComponent from '../ComponentCommon/ButtonComponent.vue';
export default {
    components: { SearchBarComponent, ButtonComponent },
    data: function(){
        return{
            navBarSearch: [
                {
                    text: 'Search courses',
                }
            ],
            buttonContent: [
                {
                    text: 'Sign Up',
                }
            ]
        }
    },
}
</script>

<style lang="scss">
@import'../../styles/variables.scss';
    .ms_fs{
        font-size: 14px;
    }
    .ms_color_icon{
        color: $colorButton;
    }
</style>