## [class 与 style 绑定](https://cn.vuejs.org/v2/guide/class-and-style.html)

for：操作元素的class列表 和 内联样式

- 绑定HTML　Class

  

  - 对象语法

    ```vue
    <div v-bind:class="{ active: isActive }"></div>
    ```

    

    

  - 数组语法

    ```vue
    <div v-bind:class="[isActive ? activeClass : '', errorClass]"></div>
    ```

    

  

   - 用在组件上

     

  

- 绑定内联样式

  - 对象语法

    ```vue
    <div v-bind:style="{ color: activeColor, fontSize: fontSize + 'px' }"></div>
    ```

    ```javascript
    data: {
      activeColor: 'red',
      fontSize: 30
    }
    ```

    

  - 数组语法

    ```vue
    <div v-bind:style="[baseStyles, overridingStyles]"></div>
    ```

    

  - 自动添加前缀

    如 `transform`，Vue.js 会自动侦测并添加相应的前缀。

  - 多重值

    ```vue
    <div :style="{ display: ['-webkit-box', '-ms-flexbox', 'flex'] }"></div>
    ```

    

  

