
## 4. Vue实例生命周期及钩子函数

**目标**：了解Vue实例生命周期，生命周期的钩子函数及created函数常用场景

**分析**：

在创建vue实例的时候可以指定模板id、数据和方法；而如果要在实例化、模板渲染的过程中需要执行一些其它操作的话；那么可以使用钩子函数。

**小结**：

钩子函数会在vue实例的各个生命周期阶段自动调用；具体有：beforeCreate，created,beforeMount,mounted,updated,beforeUpdate，destroyed，beforeDestroy

created钩子函数常用场景：用于初始化数据

> 钩子函数不要使用箭头函数的方式编写。

## 5. 插值、v-text和v-html

**目标**：插值使用场景和要求；v-text和v-html的作用

**小结**：

**插值**可以使用在有需要显示vue实例数据的地方，可以在插值表达式中调用实例的数据属性和函数。

v-text和v-html的作用：可以将数据在模板中进行显示；
**区别**：v-html会对内容中出现的html标签进行渲染，而v-text会将内容当做普遍文本输出到元素里面。

>多个 checkbox 对应一个model时，model的类型是一个数组，单个checkbox值是boolean类型
>radio对应的值是input的value值
>input 和 textarea 默认对应的model是字符串
>select 单选对应字符串，多选对应也是数组


## 7. 指令-v-on使用

**目标**：了解v-on指令的语法实现按钮点击后的递增和递减

**分析**：

在没有使用vue之前；页面标签可以通过设置onXXX响应事件；在vue中可以通过v-on指令响应事件。
**事件修饰符**：语法v-on:xxxx.修饰符，常用的修饰符有：

.stop ：阻止事件冒泡
.prevent ：阻止默认事件发生
.capture ：使用事件捕获模式
.self ：只有元素自身触发事件才执行。（冒泡或捕获的都不执行）
.once ：只执行一次

