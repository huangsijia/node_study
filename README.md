## node输出模块
module.exports = greet;//输出的greet函数
## node引入模块
var greet = require('./hello');//引入的greet函数

## node引入对外暴露变量
module.exports = variable;//一个模块想要对外暴露变量（函数也是变量）
## node引入其他模块暴露的变量
var ref = require('module_name');//引用其他模块暴露的变量

## module.exports vs exports
如果要输出一个键值对象{}，可以利用exports这个已存在的空对象{}，并继续在上面添加新的键值；
如果要输出一个函数或数组，必须直接对module.exports对象赋值。
