#### 问题:

#### 谈谈你对MVC、MVP和MVVM的理解?



##### 回答:

###### MVC

M代表Model，V代表View，C代表Controller

分别指模型层、视图层、控制层

- 模型层含有业务逻辑和数据存储
- 视图层含展示界面，可接收用户输入

- 控制层相当于模型层和视图层之间的桥梁，当用户操作view时controller去相应修改model，当model发生变化时controller去相应更新对应的view。

Model不依赖于View，View依赖于Model，View可以访问到Model



###### MVP

M代表Model，V代表View，P代表Presenter

分别指模型层、视图层、呈现层

- 模型层含业务逻辑和数据存储
- 视图层含展示界面，可接受用户交互
- 呈现层处理View和Model之间的交互

Presenter把Model和View真正进行了分离，View无法访问到Model了



###### MVVM

分成了三层: Model、View和ViewModel

模型层、视图层、视图模型

- 模型层含业务逻辑和相关数据
- 视图层，展现界面和视图，可接受用户交互
- 视图模型层，模型层和视图层沟通的桥梁。

视图层和模型层不直接通信，通过ViewModel连接，类似MVP结构。与MVP的Presenter不同的是，ViewModel采用双向绑定，View的变动自动反映在ViewModel上，ViewModel的改变也自动体现在View上。