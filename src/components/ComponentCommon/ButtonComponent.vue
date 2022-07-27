<template>
  <div>

    <button>{{ text }} {{ textInvesting }} {{ textLearning }}</button>

  </div>
</template>

<script>
export default {
  props: {
    text: String,
    textInvesting: String,
    textLearning: String,
  }
}
</script>

<style lang="scss" scoped>
@import'../../styles/variables.scss';

button{
  background-color: $colorButton;
  border-color: $colorButton;
  color: white;
  padding: 15px 40px;
  border-radius: 30px;
  font-weight: bold;
  text-transform: uppercase;
}
</style>