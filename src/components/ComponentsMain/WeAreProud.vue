<template>
<div class="ms_bg_proud">
    <div class="container-fluid mt-5">
        <h1>We Are Proud</h1>
        <p>Certificate courses are instructed by higly educated and qualified instructors who hold doctoral and master's level degree</p>
        <div class="row ms_bi justify-content-center">
            <div class="col-2">
                <h1>{{ students }}</h1>
                <span>Students</span>
            </div>
            <div class="col-2 border-start">
                <h1>{{ courses }}</h1>
                <span>Courses</span>
            </div>
            <div class="col-2 border-start">
                <h1>{{ videoHours }}</h1>
                <span>Hours Video</span>
            </div>
            <div class="col-2 border-start">
                <h1>{{  reachedCountries }}</h1>
                <span>Countries Reached</span>
            </div>
        </div>
    </div>

    <!-- SEARCHBAR WE ARE PROUD -->
    <div class="container-fluid ms_bg_emailbar p-4">
        <div class="container d-flex justify-content-around align-items-center">
            <div class="me-5">
                <h5>Subscribe our newsletter</h5>
                <span>There are many variations of passages of lorem Ipsum available, but the majority have suffered alteration in some form, by injected humor, or randomise word</span>
            </div>
            <div>
                <label class="mb-3" for="">YOUR EMAIL ADDRESS</label>
                <SearchBarComponent v-for="(element, index) in searchBarProud" :key="index"
                    :placeHolder="element.placeHolder"
                    :content="element.text"
                />
            </div>
        </div>
    </div>
    <!-- SEARCHBAR WE ARE PROUD -->
</div>
</template>

<script>
import SearchBarComponent from '../ComponentCommon/SearchBarComponent.vue';
export default {
    props: {
        students: Number,
        courses: Number,
        videoHours: Number,
        reachedCountries: Number,
    },
    components: { SearchBarComponent },
    data: function(){
        return{
            searchBarProud: [
                {
                    placeHolder: 'Enter Your E-mail',
                    text: 'Subscribe',
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import'../../styles/variables.scss';

    .ms_bg_proud{
        background-color: $bgWeProud;
        text-align: center;
        h1{
            font-size: 50px;
            font-weight: 100;
            margin-bottom: 15px;
            padding-top: 100px;
        }
        p{
            font-weight: 100;
            font-size: 20px;
            margin-bottom: 50px;
        }
    }

    div.ms_bi{
        background-image: url('../../assets/images/we_proud.png');
        background-repeat: no-repeat;
        background-size: cover;
        padding-bottom: 300px;
        h1{
            font-size: 65px;
            font-weight: 100;
        }
        span{
            font-weight: 100;
            font-size: 30px;
        }
    }
        
    .ms_bg_emailbar{
        background-color: $bgSearchProud;
        color: white;
        text-align: left;
        div.me-5{
            max-width: 750px
        }
    }
</style>