<template>
  <div class="content">
    <h1>Add</h1>
    <span>用户名</span>
    <input type="text" />
    <br>
    <span>内容</span>
    <textarea rows="10" cols="50">

    </textarea>
    <br>
    <button>提交</button>
  </div>
</template>

<script>
    export default {
        name: "Add"
    }
</script>

<style scoped>
  .content {
    float: left;
    background-color: yellow;
    height: 500px;
    width: 500px;
  }
</style>
