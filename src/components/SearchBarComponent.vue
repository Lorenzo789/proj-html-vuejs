<template>
  <div>

    <input type="text" :placeholder="text">
    <button><img src="../assets/images/magnifier.png" alt=""></button>

  </div>
</template>

<script>
export default {
    props: {
        text: String,
    }
}
</script>

<style>
@import'../styles/variables.scss';

</style>