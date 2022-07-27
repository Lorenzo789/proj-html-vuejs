<template>

    <li class="d-inline px-3">

        <a class="text-decoration-none ms_color" href="#"
            :class="{'ms_selected': this.selected == true}">

            {{ nameGenre }}

        </a> 

    </li>

</template>

<script>
export default {
    props: {
        nameGenre: String,
        selected: Boolean,
    }
}
</script>

<style lang="scss">
@import'../../styles/variables.scss';

    .ms_color{
        color: $colorUlGenre;
    }

    .ms_selected{

    }
    
</style>