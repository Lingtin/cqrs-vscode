

#### 奈何本人实在有点懒，所以在这里写了代码片段!
#### 声明，勿怪，如有损坏其权益请联系本人邮箱zxsxzt@foxmail.com进行删除，谢谢！

以下是曾亮老师的CQRS框架介绍

github地址：https://github.com/liangzeng/cqrs

### CQRS
DDD-CQRS-Actor framework.

#### CQRS 框架
这要讲起来，真的是长篇大论，所以我们从实用角度来讲一讲。

我们都太依赖于数据库了，这无可厚非，简单的 CURD 直接对数据库读写即可。

数据库为中心的程序，面对的是冷冰冰的贫血对象，这种对象甚至只能叫数据，因为对象除了数据，还应该包括方法。 所以，CQRS 提供了创建有生命周期的活对象。当然，话题就说到这儿了，如果对理论感兴趣，可以看一些 DDD / CQRS 相关资料。 这里讲的都是开发中，实际受益的编码方式，即便没有那些理论，也是可以上手开发的。

#### 框架介绍

#### Domain
我们用过各种 MVC 框架，我们知道业务应该写在 Controller 里。而 CQRS 框架，需要我们把逻辑写在领域层里，domain 可以理解为一个容器，里面有很多很多活着的 actor 实例，他们是活着的，这话千真万确，呵呵。

#### Actor
真正的逻辑，是写在 Actor 里的，也就是普通的对象方法。

#### Service
一个 actor 要想与其他 actor 交流，就可通过 service 做到。

#### Event
每个 actor 的方法，在调用时，会产生一个事件，这个事件，可以被外界或 domain 内的其他 actor 监听到。

#### Node 版本
#### 需要 node.js v8.x+

### Snippets
* cqrs
* cqrs actor
* cqrs extends
* cqrs service get
* cqrs service apply
* cqrs service create

* domain
* domain create
* domain get

* get()
* create()
* apply()
* subscribe()
* unsubscribe(event)
* lock(timeout?: number)
* unlock()
* sagaBegin()
* sagaEnd()
* rollback()
* getHistory()

***************