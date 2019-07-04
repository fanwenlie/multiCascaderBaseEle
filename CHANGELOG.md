#### 2019-06-19

- 优化：优化样式；生成环境压缩代码

#### 2019-06-18
  
- fixed: element-ui-2.9.1版本原生cascader组件添加多选功能，导致该组件样式完全错乱，修复样式错乱的问题
- fixed: 修复搜索时，父元素disabledCheckbox为true，disabledCheckbox为false的子元素无法选择的bug

#### 2019-05-28

- fixed: 修复点击一次checkbox，change事件触发多次的问题

#### 2019-05-22

- fixed: 修复了当组件有值时，在第二个input中不断输入单词，第一个input值也会显示出来的bug
- add: props增加disabledCheckbox字段，用来实现在多选时禁止选中checkbox，但又保留能选择children的功能

#### 2019-05-21

- fixed: 修复了main.vue监听options字段，代码中console.log()没注释的bug；

- fixed: 修复了menu.vue中只要点击menu或者checkbox会自动滚动到顶部的bug；