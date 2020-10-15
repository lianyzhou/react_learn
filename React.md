## React入门

### 课程大纲


+ React是什么
+ 如何快速的在网页中使用React
+ JSX
  + JSX基础
  + 在JSX中使用CSS
+ 组件
  + 什么是组件
  + 组件的编写方式
    + Class组件
    + Function组件
  + 如何为组件添加dom事件
  + 组件的状态管理
  + 组件的调试
+ 回顾总结



#### 自我介绍

称呼：周连毅 (Jack)

简介：

​       10年前端开发经验，曾就职于新浪微博、阿里云，做过PC、移动端的大型项目，精通web和移动端开发。



#### 课程代码
https://github.com/lianyzhou/react_learn  

#### React是什么

https://reactjs.bootcss.com/

React是一个用于构建用户界面的JS库
+ 用户界面

  + 界面展示
  + 界面交互
+ JS库
  + 使用JS进行编写
  + 需要配合HTML、CSS进行使用



React的特点：

+ 声明式
  + 以一种可靠的方式对UI进行描述（Props、State）
  + 正确并有效的（Virtual DOM）渲染视图
  + 状态与视图分离，减少DOM操作
+ 组件化
  + 可复用
  + 可测试
+ 一次学习、随处编写
  + 服务端渲染  （SSO优化）
  + React Native



#### 如何快速的在网页中使用React

+ 标准html中，使用script标签引入三个JS资源

+ 在页面上放置一个<div id="root"></div>

+ 添加script标记并书写代码
```
    <script type="text/babel">
      // 此处书写React代码
    </script>

```
+ ReactDOM.render
  ```
  ReactDOM.render(JSX, container[, callback])
  ```

  在提供的 `container` 里渲染JSX，如果提供了可选的回调函数，该回调将在组件被渲染或更新之后被执行


#### JSX语法

##### JSX基础
  + JSX是什么
      + JSX的作用是用于描述视图
      + JSX是一个JavaScript的语法糖
      + 在JSX中可以使用 模板 + CSS
  + JSX中使用表达式
      + 使用 {} 显示属性值
      + 使用数组的map方法进行遍历
  + 使用逻辑判断，选择性的输出JSX
      + 可以提取不同的function对JSX分段输出

##### CSS的使用

+ JSX中使用style属性

  + style属性
  + px值的简写
  + 属性使用驼峰或横线，都支持

+ JSX中使用className属性

  + className属性

  + 工具classNames的使用

    https://github.com/JedWatson/classnames

#### 组件
#### 什么是组件

​	组件允许你讲UI拆分成独立可复用的代码片段，将应用的复杂度降低。

​	说白了，组件就是用来实现某个功能效果的代码集合。

​	组件进行提取之后，复用程度更高，执行效率更高，更利于维护。

#### 组件的编写方式
##### Class组件

+ 继承自 React.Component
+ 重写render方法
+ 组件的默认属性defaultProps
+ 可选的重写constructor方法
+ 特殊的props.children

##### Function组件

+ 接收一个参数props
+ 返回一段JSX

#### 如何为组件添加dom事件

* 驼峰式事件名   onClick  onMouseEnter

* 第一个参数是event对象

* 支持的事件列表

  https://zh-hans.reactjs.org/docs/events.html#transition-events

#### 组件的状态管理

+ this.state
+ this.setState 的使用
+ this.setState 的异步和同步

#### 组件的调试

+ React Developer Tools