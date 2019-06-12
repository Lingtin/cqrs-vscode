

#### NodeJs CQRS框架 代码片段!

#### console 函数片段

#### 特此声明：如有损坏其权益请联系本人邮箱zxsxzt@gmail.com进行删除，谢谢！

曾亮老师的  CQRS框架介绍 github地址：https://github.com/liangzeng/cqrs

曾亮老师的  CQRS框架介绍 github地址：https://github.com/liangzeng/cqrs

### Snippets cqrs

键|描述
--|:--:|
cqrs|const {Actor} = require('cqrs'); // imp cqrs as Actor
cqrs actor|const {Actor} = require('cqrs'); // imp cqrs asd actor
cqrs extends|module.exports = class ClassName extends Actor{
cqrs service get|const name = await this.service.get('name',value);
cqrs service apply|this.service.apply(name,value, false);
cqrs service create|const name = await this.$.create(name, {name:value);

### Snippets domain
键|描述
--|:--:|
domain|
domain create|
domain get|

### Snippets $
键|描述
--|:--:|
$.get()|
$.create()|
$.apply()|
$.subscribe()|
$.unsubscribe()|
$.lock()|
$.unlock()|
$.sagaBegin()|
$.sagaEnd()|
$.rollback()|
$.getHistory()|

#### Snippets console

快捷键描述|键|描述
--|:--:|--:
输入信息|clg|console.log()
输入信息|clo|console.info()
输入警告|clw|console.warn()
输入错误|cle|console.error()
追踪函数的调用过程|clt|console.error()
清除当前控制台的所有输出|clr|console.clear()