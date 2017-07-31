# angular-definit-service
[实现从1到100间整数加和](https://mingdongtu.github.io/angular-definit-service/definition.html)

AngularJs实现自定义服务一般方法总结：

【1】、首先利用app对象调用service（）方法且传入两个参数，一个是要自定义的服务，另一个是回调函数；

【2】、在回调函数里面给this添加一个方法，这个函数中即包含服务的功能

【3】、app对象再调用控制器方法，传入两个参数，一个是控制器属性值，另一个参数是回调函数，并传入两个参数：一个是作用域$scope, 另一个是自定义服务；

【4】、自定义服务调用service（）中回调函数this的方法，并传入相应参数，将其赋值给$scope的参数
