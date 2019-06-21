

#### NodeJs CQRS框架 代码片段!

#### Console 函数片段

#### 特此声明：如有损坏其权益请联系本人邮箱zxsxzt@gmail.com进行删除，谢谢！

@leozale
leozale CQRS框架介绍 github地址：https://github.com/cqrs2/cqrs

@leozale
leozale CQRS框架介绍 github地址：https://github.com/cqrs2/cqrs

### Snippets cqrs

键|描述
--|:--:|
cqrs|const {Actor} = require('cqrs'); // imp cqrs as Actor
cqrs actor|const {Actor} = require('cqrs'); // imp cqrs asd actor
cqrs extends|module.exports = class ClassName extends Actor{
cqrs service get|const name = await this.service.get('name',value);
cqrs service apply|this.service.apply(name,value, false);
cqrs service create|const name = await this.$.create(name, {name:value);

### 创建Actor实例

domain   // 创建Domain实例  
const {Domain} = require('cqrs');   


//创建Actor实例  
domain create|domain.create(); 

// 得到一个 Actor 实例 
domain get  
domain.get(name,value);   


// 监听所有 User 的所有事件  
domain.on({actorType:"User"},handle);

// 监听所有 User 的 changeName 事件  
domain.on({actorType:"User",type:"changeName"},handle);  

// 监听 id 为 userId 的 User 的所有事件  
domain.on({actorType:"User", actorId:userId},handle);

// 监听 id 为 userId 的 User 的 change 事件  
domain.on({actorType:"User", actorId:userId , type:"change"},handle);

// 监听所有事件！  
domain.on({},handle);

### service 的别名 $ , 所有的业务方法内部都可调用。下面是 service 服务对象的全部方法。
$.get()

$.create()

$.apply()

$.subscribe()

$.unsubscribe()

$.lock()

$.unlock()

$.sagaBegin()

$.sagaEnd()

$.rollback()

$.getHistory()


#### Snippets console

快捷键描述|键|描述
--|:--:|--:
输入信息|clg|console.log()
输入信息|clo|console.info()
输入警告|clw|console.warn()
输入错误|cle|console.error()
追踪函数的调用过程|clt|console.error()
清除当前控制台的所有输出|clr|console.clear()