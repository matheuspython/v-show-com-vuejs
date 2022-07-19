<template>
  <TheHeader text="welcome!"/>
  <div class="hello">
    <button v-on:click="showList" class="show-btn"> {{textOfBtn}} </button>
    <TaskList v-show="stateOfList"/>
  </div>
</template>

<script>
import TheHeader from './TheHeader.vue'
import TaskList from './TaskList.vue'
export default {
  name: 'HelloWorld',
  components: {
    TheHeader,
    TaskList
  },
  data() {
    return {
      stateOfList: true,
      textOfBtn: 'hide items',
      showList: () => {
        this.stateOfList = !this.stateOfList;
        this.stateOfList ? this.textOfBtn="hide items" : this.textOfBtn="show items"
      }
    }
  }

}
</script>

<style scoped>
  .show-btn{
    width: 100%;
    max-width: 250px;
    margin: 30px;
    height: 35px;
    border: 0;
    border-radius: 12px;
    color: #fff;
    background-color: rgb(220, 50, 183);
    cursor: pointer;
  }
</style>
