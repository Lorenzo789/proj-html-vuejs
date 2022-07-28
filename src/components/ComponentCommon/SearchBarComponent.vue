<template>
  <div>

    <input type="text" :placeholder="text, placeHolder">
    <button>
      <i class="fa-solid" :class="{'fa-magnifying-glass': this.content == ''}"></i>
      {{ content }}
    </button>

  </div>
</template>

<script>
export default {
    props: {
      text: String,
      content: String,
      placeHolder: String,
    }
}
</script>

<style lang="scss" scoped>
@import'../../styles/variables.scss';

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