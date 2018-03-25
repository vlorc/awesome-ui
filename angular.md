# Angular

#### 状态管理和通信控制
1. [ngrx](https://github.com/ngrx/store)
2. [ngxs](https://ngxs.gitbooks.io/ngxs)
3. [rxjs](http://reactivex.io/rxjs)
4. [mobx](https://github.com/mobxjs/mobx-angular)

##### mobx 
###### 简介
MobX以声明式，简单和高性能的方式解决了前端应用程序中状态管理的问题

###### MobX的基本组成：
+ observables（可观察）： 定义可跟踪的属性
+ computed（计算）： 定义派生状态
+ actions（行动)： 改变状态
+ reactions（反应）： 对更改做出反应（更新UI）


[官方链接](https://mobx.js.org)

***参考文献***
https://benmccormick.org/2017/01/09/mobx-first-impressions
https://500tech.com/blog/all/tic-tac-toe-using-angular-mobx

##### rxjs 
###### 简介
RxJS（Reactive Extensions for JavaScript）是一个使用observables进行反应式编程的库，可以更容易地编写异步或基于回调的代码（RxJS Docs）。

###### Rxjs的基本组成：
+ observable（可观察序列）： 用于发布事件
+ observer（观察者）： 订阅事件
	+ onNext（下一个）：在可观察序列中每个事件调用。
	+ onError（错误）：仅在错误情况下调用一次。
	+ onCompleted（完成）：当流完成时只调用一次。（只有一次）
+ operator（操作符)： 对事件的操作
+ stream（流）： 事件流

***一切都是流。跟我重复！***

[官方链接](http://reactivex.io)

***参考文献***
https://segmentfault.com/a/1190000008886598
https://medium.com/google-developer-experts/angular-introduction-to-reactive-extensions-rxjs-a86a7430a61f

##### ngrx 
###### 简介
ngrx/store的灵感来源于Redux，是一款集成RxJS的Angular状态管理库。

###### Ngrx的基本模块：
+ [store](https://github.com/ngrx/platform/blob/master/docs/store/README.md)（状态容器）
+ [effects](https://github.com/ngrx/platform/blob/master/docs/effects/README.md)（效果）： 动作响应效果
+ [devtools](https://github.com/ngrx/platform/blob/master/docs/store-devtools/README.md)（调试工具）
+ [monitor](https://github.com/ngrx/store-log-monitor/blob/master/README.md)（日志监视器）
+ [router](https://github.com/ngrx/platform/blob/master/docs/router-store/README.md)（路由）
+ [db](https://github.com/ngrx/db/blob/master/README.md)（数据库)：用于Angular应用程序的IndexedDB
+ [notify](https://github.com/ngrx/notify/blob/master/README.md)（通知）： 在Angular 2中轻松创建和处理桌面通知

###### Ngrx的基本组成：
+ action（动作）
+ reducer（响应）
+ store（监听和分发）


[官方链接](http://ngrx.github.io/)


***参考文献***


##### ngxs 
###### 简介
NGXS模仿在像Redux和NGRX这样的库中普遍实现的CQRS模式，但通过使用类和装饰器等现代TypeScript特性来减少样板。

***参考文献***
https://medium.com/@amcdnl/why-another-state-management-framework-for-angular-b4b4c19ef664