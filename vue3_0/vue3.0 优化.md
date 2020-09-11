## vue3.0 优化



- 源码优化







  1. 更好的代码管理方式：monorepo

     

     | vue2.x         | vue3.0             |
     | -------------- | ------------------ |
     | 源码在-src目录 | 源码在packages目录 |
     |compiler - 模板编译相关| - |
     |core - 与平台无关的通用运行时代码| - |
     |platforms - 平台专有代码| - |
     |server - 服务端渲染的相关代码| - |
     |sfc - .vue 单文件解析相关代码| - |
     |shared - 共享工具代码| - |
     

     

     


  2. 有类型的JavaScript：TypeScript

     | vue2.x                                        | vue3       |
     | --------------------------------------------- | ---------- |
     | Flow Facebook出品的JavaScript静态类型检查工具 | TypeScript |

     

- 性能优化

  1. 源码体积优化

     * 首先，移除一些冷门的 feature（比如 filter、inline-template 等）
     * 其次，引入 tree-shaking 的技术，减少打包体积

  2. 数据劫持优化

     | vue2.x                                                       | vue3      |
     | ------------------------------------------------------------ | --------- |
     | 通过 Object.defineProperty 这个 API 去劫持数据的 getter 和 setter | Proxy API |

     

  3. 编译优化

- 语法API优化：Composition API



  1. 优化逻辑组织

  2. 优化逻辑复用

     

- 引入RFC：使每个版本改动可控

  

- 过渡期