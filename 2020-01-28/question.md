#### 问题:

#### 谈谈你对Vue组件之间通信的理解。



##### 回答:

vue组件之间通信是很常见的使用场景，包括父子组件间的通信，兄弟组件之间的通信，祖先和后代组件(大于二层)之间的通信等三种情况。



通用于这三种情况的通信方式有:

- EventBus总线
- Vuex状态管理



适用于父子组件通信的方式有:

- props
- emit
- \$parent和\$children
- \$root
- \$refs
- provide/inject



适用于祖先后代组件通信的方式有:

- props配合\$attrs
- \$root
- provide/inject



适用于兄弟组件通信的方式有:

部分情况下可通过路由,传递和接收路由参数params达到通信目的