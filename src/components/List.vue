<template>
  <div class="content">
      <h1>List</h1>
      <ul>
          <Item v-for="(comment, index) in comments" :key="index" :comment="comment">
              
          </Item>
      </ul>
  </div>
</template>

<script>
    import Item from './Item'
    
    export default {
        name: "List",
        components: {Item},
        // 声明接收属性，会成为组件对象的属性
        props:['comments'],
        comments:{
            Item
        },
        data() {
            return {
                
            }
        }
    }
</script>

<style scoped>
  .content {
    float: left;
    background-color: #00c900;
    height: 500px;
    width: 500px;
  }
</style>
