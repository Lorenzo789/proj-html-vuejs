<template>
  <header class="container-fluid">
    <div class="container d-flex justify-content-between">
        <ul>
            <li class="ms_color">English <i class="fa-solid fa-angle-down"></i> </li>
        </ul>

        <div>
            <ul>
                <HeaderContent v-for="(data, index) in headerData" :key="index"
                    :title = "data.text"
                    :new = "data.new"
                />
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-behance"></i></a>
                <a href="#"><i class="fa-solid fa-basketball"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
            </ul>
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