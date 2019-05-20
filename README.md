

# 更新
基于[ZhenyuCheng/multiCascaderBaseEle](https://github.com/ZhenyuCheng/multiCascaderBaseEle)组件fork之后修改

- 修复了main.vue监听options字段，代码中console.log()没注释的bug；

- 修复了menu.vue中只要点击menu或者checkbox会自动滚动到顶部的bug；

# multiCascaderBaseEle
基于element-ui实现的多选级联组件，完全继承element-ui级联组件功能

# Usage

## 直接在package.json中的dependencies字段粘贴以下代码
```json
"multi-cascader-base-ele": "git://github.com/fanwenlie/multiCascaderBaseEle.git"
```
## use
``` js

import multiCascader from 'multi-cascader-base-ele'

Vue.use(multiCascader)

```

``` html
<el-multi-cascader 
  class="multi-cascader" 
  :options="options"
  v-model="selectedOptions" 
  multiple 
  filterable 
  select-children 
  clearable 
  collapse-tags
  only-out-put-leaf-node
  change-on-select 
  ></el-multi-cascader>
```
# 功能实例，以及选项
[查看demo](https://zhenyucheng.github.io/multiCascaderBaseEle/dist/index.html)

