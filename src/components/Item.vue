<template>
    <li>
        <div class="item">
            <div>{{comment.name}}</div>
            <div>{{comment.msg}}</div>
            <div>
                <button>删除</button>
            </div>
        </div>
    </li>
</template>

<script>
    export default {
        name: "Item",
        // 此种写法，可以同时指定出属性的类型
        props: {
            comment: Object
        }
    }
</script>

<style scoped>
    div.item {
        background-color: #0000ff;
        height: 100px;
        width: 70%;
        margin-top: 10px;
        padding-top: 10px;
        color: white;
    }
</style>
