<template>
  <div>
    <header>
      <h1>Header</h1>
      <div class="content">
        <h2>请发表对Vue的评论</h2>
      </div>
    </header>
    <div class="content">
      <Add/>
      <List :comments="comments"/>
    </div>
  </div>
</template>

<script>

import Add from './components/Add'
import List from './components/List'

export default {
  name: 'App',
  components: {
    Add,
    List
  },
  data() {
    return {
      comments:[
        {name:'鳌拜', msg:'hello!'},
        {name:'景小崽', msg:'good'},
        {name:'滚地锦', msg:'可以可以'},
      ]
    }
  }
}
</script>

<style>
  header {
    background-color: gray;
  }

  h1, h2 {
    margin: 0;
    padding: 0;
  }
</style>
