<template>
  <header class="container-fluid border-bottom">
    <div class="container d-flex justify-content-between align-items-baseline pt-3">
            <h6 class="ms_color d-inline">English <i class="fa-solid fa-angle-down"></i> </h6>

        <div>
            <ul>
                <HeaderContent v-for="(data, index) in headerData" :key="index"
                    :title = "data.text"
                    :new = "data.new"
                />
            </ul>
        </div>
        <div>
            <!-- NON FINITO MANCA IL QUADRATINO CON NEW ROSSO -->
            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-twitter"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-instagram"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-behance"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-solid fa-basketball"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-solid fa-square-full"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-git"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-linkedin"></i>
            </a>

            <a class="ms_color text-decoration-none px-2" href="#">
                <i class="fa-brands fa-pinterest"></i>
            </a>
        </div>
    </div>
  </header>
</template>

<script>
import HeaderContent from './HeaderContent.vue';

export default {
    components: { HeaderContent,},
    data: function(){
        return{
            headerData: [
                {
                    text: 'Courses',
                    new: false,
                },
                {
                    text: 'Zoom',
                    new: true,
                },
                {
                    text: 'Pages',
                    new: false,
                },
                {
                    text: 'Bundles',
                    new: false,
                },
                {
                    text: 'Course Formats',
                    new: false,
                },
                {
                    text: 'Pages',
                    new: false,
                },
                {
                    text: 'Add Course',
                    new: true,
                },
                {
                    text: 'Demos',
                    new: false,
                },
            ],
        }
    }
}
</script>

<style lang="scss">
@import'../styles/variables.scss';


</style>