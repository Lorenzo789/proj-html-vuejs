<template>
    <div class="ms_courses_card">
        <div>
            <img :src="imgUrl" alt="">
        </div>

        <div class="p-3">
            <p>{{ description }}</p>
            <h6 class="fs-6">{{ title }}</h6>
            <hr>

            <div class="position-relative d-flex justify-content-between">
                
                <div>
                    <span>
                        <i class="p-2 fa-solid" :class="{'fa-clock': this.hour !== ''}"></i>{{ hour }}
                    </span>
    
                    <span class="ms_star">
                        {{ stars }}      
                    </span>
    
                    <span>
                        {{ numberStars }}      
                    </span>
                </div>

                <span class="position-absolute ms_pos">
                    {{ oldCost }}
                </span>

                <span class="fs-6 fw-bold">
                    {{ cost }}
                </span>

            </div>
            
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
        numberStars: String,       
        cost:  String,
        oldCost: String,    
        new: Boolean,     
        hot: Boolean,     
        special: Boolean,
    },
}
</script>

<style lang="scss" scoped>
@import'../../styles/variables.scss';

    .ms_courses_card{
        width: calc(100% / 6 - 20px);
        height: 350px;
        margin-bottom: 60px;
        border: 2px solid lightgray;

        img{
            object-fit: cover;
            height: 100%;
            width: 100%;
        }

        p{
            color: #b9b4b2;
            font-size: 13px;
        }

        .ms_star{
            color: #efb467;
            font-size: 18px;
        }

        .ms_pos{
            top: -15px;
            right: 0;
            text-decoration-line: line-through;
            color: lightgray;
        }
    }
</style>