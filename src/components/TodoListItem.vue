<!--  -->
<template>
<div class=''>
     <div class="todo-item">
                  <label >
                      <input type="checkbox" >
                      todo1
                      <span class="check-button"></span>
                  </label>
              </div>
                            <div class="todo-item">
                  <label >
                      <input type="checkbox" >
                      todo2
                      <span class="check-button"></span>
                  </label>
              </div>
                            <div class="todo-item">
                  <label >
                      <input type="checkbox" >
                      todo3
                      <span class="check-button"></span>
                  </label>
              </div>
</div>
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';

export default {
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {

};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style scoped>
.todo-item {
  background: white;
  padding: 16px;
  border-radius: 8px;
  color: #626262;
}
.todo-item label {
  position: relative;
  display: flex;
  align-items: center;
  cursor: pointer;
}
.todo-item.done label {
  text-decoration: line-through;
  font-style: italic;
}
.todo-item label span.check-button {
  position: absolute;
  top: 0;
}
.todo-item label span.check-button::before,
.todo-item label span.check-button::after {
  content: "";
  display: block;
  position: absolute;
  width: 18px;
  height: 18px;
  border-radius: 50%;
}
.todo-item label span.check-button::before {
  border: 1px solid #b382f9;
}
.todo-item label span.check-button::after {
  transition: 0.8s;
  background: #b382f9;
  transform: translate(1px, 1px) scale(0.8);
  opacity: 0;
}
.todo-item input {
  margin-right: 16px;
  opacity: 0;
}
.todo-item input:checked + span.check-button::after {
  opacity: 1;
}
</style>