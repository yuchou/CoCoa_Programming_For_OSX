# CoCoa Programe for OS X 学习笔记
### 第一章 开始
- “The AppDelegate’s job is to manage the interaction between your application and the system. The system launches the application and notifies the app delegate. ”
- XIB，XML Interface Builder
- 绑定操作：@IBOutlet 展示，@IBAction 操作
- 下划线『\_』代表忽略区间值的每一项

### 第二章 Swift 类型
- Swift 被分为三个基本类型：结构体、类、枚举，他们都有属性，构造函数，实例方法，类或静态方法，关键点是可选型 Optional
- 按住 option 键可以快速查看帮助
- 推断类型、特定类型、集合类型
- 可选项的定义和解包

### 第三章 结构体和类

- 定义实例方法
- 重载运算符
- 类的构造函数(init)不能为空，但不需要提供默认值，结构体可以省略构造函数
- 便利构造函数(convenience)，
- 继承
- 类是引用类型，结构体是值类型
- Obj-C 和 Swift 类型区别
- as 强制转化 数组强制转化时用 as! 先解包
- 错误：程序错误和 Recoverable 错误

### 第五章 控制

- 创建一个 Swift 文件，然后创建一个 Interface 文件，将两者连接
- 控件中的 Cell 是什么？用来处理控件的属性
- 完成 Challenge：Busy Board

### 第六章 委托

- didSet，设置值后立刻被调用
- willSet，设置值前立刻被调用
- 委托是一种设计模式，它允许类或结构体将一些他们需要负责的功能交给其他类型的实例
- 委托的实现：定义协议来封装那些需要委托的函数或者方法，使其遵循着拥有这些委托的函数和方法
- 委托中常见的错误
    - 忘记设置委托属性，window 需要在 xib 里设置连接
    - Swift 大小写敏感，拼写错方法
- cocoa 框架的大部分工作是去学习如何执行正确的操作方法、委托方法、通知监控，让代码在合适的时候运行

### 第七章 Table Views 使用

- NSTableViewDataSource 绑定数据
- 将 text field 与 table cell view 绑定
-『Table View Cell』 bind to 『Table Cell View』

### 第八章 KVC、KVO、and bingdings

- Key-value coding
- Key-value observing
- dynamic var 
- bind value to file’s ower and type model key path
- 按钮的 value 可以和 dynamic var 值绑定，直接控制开关
- 以上同理与按钮的 enable 属性
- 调试：lldb 和 调试区


### 第九章 NSArrayController
- NSTableView 与 NSArrayController 绑定
    - Content，content 是 NSArrayController 的输入，他与 arrangedObject 输出绑定
    - selection Index
    - Sort Descriptors
- NSArrayController 与 Document 绑定
    -Employees

### 第十章 Formatter and Validation

- 用绑定的方式做格式校验
- validateKey 重写验证过程

### 第十一章 撤销

- undo stack 和 redo stack
- key value observing
- inEmployeesAtIndex index: Int （内部和外部参数名）
- 最近几章大部分内容只会用，还没理解，需要靠自己做的例子来巩固


### 第十二章 存档

- 存档依赖于 NSCoding 协议
- 存档包括：存储数据，加载数据，展示数据
- Uniform type identifiers UTI
- info.plist 是一个 xml key-value 文件


### 第十三章 基础核心数据

- 这个章节主要内容为不通过代码来创建一个核心数据的 App
- 分布操作
	1. 创建 Entity
	2. 绑定 Array Controller 和 Entity
	3. 完成页面布局
	4. 进行数据绑定和连接
- 持久化存储类型：SQLite、XML、二进制文件
- 将之前章节的内容在该章节再温习一边，如默认编辑选中，排序等

### 第十四章 NSUserDefault

- 创建一个 PreferenceManager 的类，主要使用 NSUserDefaults 来实现和存储默认的设置
- 可以存储的内容
	- plist data
	- 所有 Object C 的类型
- 优先级较高的存储
	- 参数
	- 程序
	- 全局默认
	- 语言
	- 注册默认
- 存储路径：/Library/Preference

### 第十五章 弹窗和闭包

- NSAlert，默认初始化、设置参数、展示
- 闭包语法表达式
- 函数式编程
