---
order: 4
title:
  zh-CN: 使用脚本调用
  en-US: Type
---

## zh-CN

可以直接使用组件实例调用方法,比如：

- `Message.success(content, duration)`
- `Message.error(content, duration)`
- `Message.info(content, duration)`
- `Message.warning(content, duration)`
- `Message.loading(content, duration)`

## en-US


````jsx
<v-button @click.native="showMessage">
  点我会弹出提示
</v-button>
````


````vue-script
new Vue({
  el: 'body',
  components: {
    vButton: atui.Button
  },
  methods: {
    showMessage () {
      atui.Message.success('成功啦',3000)
    }
  }

})
````
