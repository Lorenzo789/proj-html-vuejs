<template>
  <div>

    <input type="text" :placeholder="text">
    <button><i class="fa-solid fa-magnifying-glass"></i></button>

  </div>
</template>

<script>
export default {
    props: {
      text: String,
    }
}
</script>

<style lang="scss" scoped>
@import'../styles/variables.scss';

input{
  padding: 10px;
  background-color: lightgray;
  border-color: lightgray;
}
button{
  padding: 10px 15px;
  color: white;
  background-color: $colorButton;
  border-color: $colorButton;
}
</style>