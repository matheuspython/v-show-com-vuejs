<template>
  <ul>
    <TaskItemVue task="item 1"/>
    <TaskItemVue task="item 2"/>
    <TaskItemVue task="item 3"/>
    <TaskItemVue task="item 4"/>
    <TaskItemVue task="item 5"/>
    <TaskItemVue task="item 6"/>
    <TaskItemVue task="item 7"/>
    <TaskItemVue task="item 8"/>
    <TaskItemVue task="item 9"/>
  </ul>
</template>

<script>
  import TaskItemVue from './TaskItem.vue'
  export default {
    name: 'TaskList',
    components: {
      TaskItemVue
    }
  }
</script>


<style>

</style>