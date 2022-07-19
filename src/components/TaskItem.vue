<template>
  <li>
    {{ task }}
  </li>
</template>

<script>
  export default{
    name: 'TaskItem',
    props:{
      task: String
    }
  }
</script>

<style>

</style>