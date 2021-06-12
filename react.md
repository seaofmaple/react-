### React

-  用于展现用户界面的js库即将数据渲染为开源的js库
-  在React里面的类组件的构造函数只有两种处理情况
   -  通过给this.state初始化内部state
   -  为事件处理函数绑定实例
-  jsx语法规则
   - script标签里面的type属性为text/bable
   - 定义虚拟DOM的时候声明变量写一个html模板不要添加单引号
   - class类不能用于定义一个标签的样式要用className
   - style添加内联样式的时候要用{{}}，外面的{}表示要写js语法，里面的{}则是表示写的是一个对象
   - 只有一个跟标签
   - 标签必须闭合
   -  标签首字母
      - 若首字母为小写字母则转换为html标签的同名元素，若无同名元素则报错
      - 若大写字母开头，则去渲染对应的组件，若没有定义则报错

- 类式组件

  ```
  class MyComponent extends React.Component {
  	render() {
  		return ()
  	}
  }
  ```

- 函数式组件

  ```
  function MyComponent() {
  	return ()
  }
  ```

- 渲染组件到页面

  ```
  ReactDOM.render(<MyComponent>, document.getElementById())
  ```

  