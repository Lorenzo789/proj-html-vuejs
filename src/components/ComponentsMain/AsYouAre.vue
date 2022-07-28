<template>
    <div class="container-fluid p-5 my-5 ms_bg_come">
        <div class="ms_container p-5 my-5" v-for="(element, index) in comeAsYouAreData" :key="index">
            <h1 class="fw-light p-3">{{ element.title }}</h1>
            <p class="fw-light fs-5 p-3">{{ element.text }}</p>
            <div>
                <h4 class="fs-5 p-3 pb-0">{{ element.infoName }}</h4>
                <span class="fs-6 p-3">{{ element.infoRole }}</span>
                <i class="fa-solid fa-triangle-exclamation"></i>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function(){
        return{
            comeAsYouAreData: [
                {
                    title: 'Come As You Are',
                    text: 'MasterStudy used is an excellent workshop wheter you come as a counselor, advisor, administrator or faculty member. I am going home empowered. I am looking forward to attending the On Course MasterStudy and the MasterStudy National conference next year and facilitating the use of this excellent retention/student success course at my college.',
                    infoName: 'Tim Sab',
                    infoRole: 'General Developer, Stylemix Themes',
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
.ms_bg_come{
    background-image: url('../../assets/images/brooke-cagle-224821-unsplash-1-1920x700.jpg');
    background-size: cover;
    .ms_container{
        width: 700px;
        margin: 0px auto 0px 350px;
        background-color: white;
        position: relative;
        i{
            padding: 10px;
            color: #fff;
            position: absolute;
            top: 200px;
            right: -50px;
            rotate: 90deg;
            font-size: 50px;
        }
    }
}
</style>