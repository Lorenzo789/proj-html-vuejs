<template>
    <li class="d-inline px-2"> 
        <a class="ms_color text-decoration-none" href="#"
            :class="{'ms_new': this.new == true}">

            {{ title }}

        </a>
    </li>
</template>

<script>
export default {
    props: {
        title: String,
        new: Boolean,
    },
}
</script>

<style lang="scss" scoped>
@import'../styles/variables.scss';

.ms_color{
    color: $textColor;
}
.ms_new{

}

</style>