
# multiCascaderBaseEle
基于element-ui实现的多选级联组件，完全继承element-ui级联组件功能

基于[ZhenyuCheng/multiCascaderBaseEle](https://github.com/ZhenyuCheng/multiCascaderBaseEle)组件fork之后修改

# Usage

#### 直接在package.json中的dependencies字段粘贴以下代码
```json
"multi-cascader-base-ele": "git://github.com/fanwenlie/multiCascaderBaseEle.git"
```
然后`yarn install`, 即可下载安装

#### use
``` js

import multiCascader from 'multi-cascader-base-ele'

Vue.use(multiCascader)

```

``` html
<template>
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
</template>
```
# 功能实例，以及选项
[查看demo](https://zhenyucheng.github.io/multiCascaderBaseEle/dist/index.html)

# 备注

1. 如果`el-multi-cascader`组件默认值为空时显示undefined，临时解决方案为

```js

this.$nextTick(() => {
  const input = document.querySelector('.multi-cascader .el-input__inner');
  const inputVal = input.value;
  if (inputVal === '' || inputVal === 'undefined') {
    input.value = '';
  }
});

```

# 更新

1. 2019-05-21

- 修复了main.vue监听options字段，代码中console.log()没注释的bug；

- 修复了menu.vue中只要点击menu或者checkbox会自动滚动到顶部的bug；


