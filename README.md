<!--
 * @Author: t-anying.fan fan02288@163.com
 * @Date: 2023-02-28 15:24:21
 * @LastEditors: t-anying.fan fan02288@163.com
 * @LastEditTime: 2023-02-28 18:13:47
 * @FilePath: \vue-pop-colorpicker-master\README.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# vue-pop-colorpicker
基于vue-color和element-ui的一个弹出式的颜色选择组件。

支持直接手动更改hex或rgba等颜色值。

支持多种样式的颜色选择器，目前支持：`chrome`, `compact`, `material`, `photoshop`, `sketch`, `slider`, `swatches`。默认为`chrome`。

## 安装

> npm install vue-pop-colorpicker --save

## 使用

### 全局组件

```
import VueColorpicker from 'vue-colorPicker'
Vue.use(VueColorpicker)
```


### 局部组件

```
import { VueColorpicker } from 'vue-colorPicker'

new Vue({
  components: {
    'color-picker': VueColorpicker
  },
  data () {
    return {
      color: '#fff',
    }
  },
  methods: {
    onChange (color) {
      console.log(color)
    }
  }
})

<color-picker v-model="color" @change="onChange"></color-picker>
```

## 其他

- 颜色选择器功能是vue-color中fork的
- popup功能是element-ui中fork的
