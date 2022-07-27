<template>
    <div class="ms_courses_card">
        <div>
            <img :src="imgUrl" alt="">
        </div>

        <div class="p-3">
            <p>{{ description }}</p>
            <h6>{{ title }}</h6>
            <span>{{ hour }} {{ stars }}</span>
            <span>{{ cost }}</span>
        </div>

    </div>
</template>

<script>
export default {
    props: {
        imgUrl: String,
        description: String,
        title: String,     
        hour: String,
        stars: String,       
        cost:  String,    
        new: Boolean,     
        hot: Boolean,     
        special: Boolean,
    }
}
</script>

<style lang="scss" scoped>

    .ms_courses_card{
        width: calc(100% / 6 - 20px);
        margin-bottom: 60px;
        border: 2px solid lightgray;

        img{
            object-fit: cover;
            height: 100%;
            width: 100%;
        }
    }
</style>