# iOS 知识点

## [￼TaggedPointer](https://blog.devtang.com/2014/05/30/understand-tagged-pointer/)
    
```    
原理：可以将一个对象的指针拆成两部分，一部分直接保存数据，另一部分作为特殊标记，表示这是一个特别的指针，不指向任何一个地址。
 
   为了节省内存和提高执行效率，苹果提出了Tagged Pointer的概念。对于 64 位程序，引入 Tagged Pointer 后，
     相关逻辑能减少一半的内存占用，
     以及 3 倍的访问速度提升，
     100 倍的创建、销毁速度提升。
```

## NSPointerArray

```
	NSPointerArray可以存放nil 可以插入删除nil
	
￼	count 属性可以设置 （用nil占位）

￼	可以初始化以保持对对象的强引用或弱引用，也可以根据NSPointerFunctionsOptions定义的任何内存或个性选项进行初始化

	￼NSCopying和NSCoding协议仅在指针数组初始化为保持对对象的强引用或弱引用时才适用
	
￼	遵循 NSFastEnumeration，可以通过 for...in 来进行遍历
```



## runtime
## runloop
## NSThread
## NSOperation
## GCD
## dispatch_queue
## dispatch_semaphore
## dispatch_barrier
## UI
## responder chain 事件传递响应链
## drawRect
## layoutSubviews
## 离屏绘制
## 自动布局
## 各端本新增特性
## instrument
## Pods
