# multiCascaderBaseEle
基于element-ui实现的多选级联组件，完全继承element-ui级联组件功能

# 更新
基于[ZhenyuCheng/multiCascaderBaseEle](https://github.com/ZhenyuCheng/multiCascaderBaseEle)组件fork之后修改

修复了main.vue监听options字段，代码中console.log()没注释的bug；
修复了menu.vue中只要点击menu或者checkbox会自动滚动到顶部的bug；

# Usage
## install
``` bash
npm i multi-cascader-base-ele --save
```
## use
``` js
import Vue from 'vue'
import Element from 'element-ui'
import App from './App.vue'
import multiCascader from 'multi-cascader-base-ele'
import 'element-ui/lib/theme-chalk/index.css';

Vue.config.productionTip = false
Vue.config.devtools = true


Vue.use(Element)
Vue.use(multiCascader)

new Vue({
    el: '#app',
    components: { App },
    template: '<App/>'
})
```

``` html
<el-multi-cascader class="multi-cascader" :options="options" multiple filterable select-children clearable collapse-tags
only-out-put-leaf-node
change-on-select v-model="selectedOptions"> </el-multi-cascader>
```
# 功能实例，以及选项
[查看demo](https://zhenyucheng.github.io/multiCascaderBaseEle/dist/index.html)

