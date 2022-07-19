<template>
  <header>
    {{ text }}
  </header>
</template> 

<script>
  export default {
    name: 'TheHeader',
    props:{
      text: String
    } 
  }
</script>

<style scoped>
  header{
    height: 75px;
    width: 100%;
    background-color: #b9149d;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>