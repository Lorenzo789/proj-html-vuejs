<template>
    <div class="container p-2 d-flex justify-content-between align-items-baseline mt-3">

    <img class="align-self-center" src="../assets/images/MasterStudy_logo.svg" alt="">

    <div class="d-flex align-items-baseline">
        <p class="ms_color ms_fs text-uppercase me-2"><i class="fa-solid fa-bars ms_fs"></i> Category</p>
        
        <SearchBarComponent v-for="(info, index) in navBarSearch" :key="index"
            :text="info.text"
            :btnImage="info.btnImg"/>
    </div>

    <div class="d-flex align-items-baseline">
        <p><i class="fa-solid fa-bullhorn"></i> Become an Instructor</p>
        <p><i class="fa-solid fa-briefcase"></i> For Enterprise</p>
    </div>

    <div class="d-flex align-items-baseline">
        <p><i class="fa-solid fa-user"></i> Log In</p>

        <ButtonComponent />

        <i class="fa-solid fa-bookmark"></i>
    </div>
</div>
</template>

<script>
import SearchBarComponent from './SearchBarComponent.vue';
import ButtonComponent from './ButtonComponent.vue';
export default {
    components: { SearchBarComponent, ButtonComponent },
    data: function(){
        return{
            navBarSearch: [
                {
                    text: 'Search courses',
                }
            ]
        }
    },
}
</script>

<style>
@import'../styles/variables.scss';
    .ms_fs{
        font-size: 14px;
    }
</style>