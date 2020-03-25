#vue学习记录

## 生命周期函数

### init Events

### 第一个生命周期函数：beforeCreate
    在beforeCreate生命周期函数执行的时候，data和methods中的数据都还没有初始化
    
### init injection & reactivity

### 第二个生命周期函数：created
    在created中，data和methods都已经被初始化好了
    如果要调用methonds中的方法或者操作data中的数据，最早只能在created中操作
    
### 第三个生命周期函数：beforeMount
    表示 模板已经在内存中编辑完成了，但是尚未把模板渲染到页面中。beforeMount执行的时候，页面中的元素，还没有被
    真正替换过来，只是之前写的一些模板字符串。

### 第四个生命周期函数：mounted
    表示内存中的模板，已经真实的挂载到了页面中，用户已经可以看到渲染好的页面了
    mounted是 示例创建期间的最后一个生命周期函数，当执行完 mounted 就表示，实例已经被完全创建好了，此时 如果没有其他操作的话，
    这个实例就静静的躺在我们的内存中，一动不动。
    
接下来是运行中的两个事件
### beforeUpdated
    这时候表示 我们的界面还没有被更新【数据更新了吗？数据肯定被更新了，只是页面上的数据显示还没有更新】
   
### updated
    此时页面和data 数据已经保持一致了，都是最新的
    
## vue-resource实现get、post、jsonp请求
    除了vue-resource之外，还可以使用`axios`的第三方包实现数据的请求
    
