<script>
export default {
  data() {
    return { 
      message: 'proj-html-vuejs'
    }
  }
}
</script>

<template>
    <header>
        <h1>
        {{ message }}
        </h1>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
  background-color: $headerBgColor;
  text-align: center;
  padding: 20px 0;
}

h1 {
  color: $headerBgColor;
}
</style>