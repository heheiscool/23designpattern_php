# 23种设计模式可以分为三类：创建型、结构型、行为型
面向对象/接口编程的一些心得体会
* 关于设计原则，最重要是开闭原则（OCP:Open Closed Principle），开闭原则是指对于一个软件实体、函数、类我们需要对功能 ***开放拓展，关闭对功能修改*** 。是面向接口编程的基本原则，面向抽象编程，依赖抽象，这样可以写出可维护代码，提高代码可拓展性。
* 面向接口编程，单纯的interface编程可以统一抽象出的对象的方法调用，但是无法统一对象的实力化。
创建型模式用来说明在不同的应用场景下如何优雅的创建对象，包括：Factory Method,Abstract Factory, Builder, Prototype, Singleton;

结构型模式用来说明如何安全、统一（按照面向对象程序设计原则）地对对象进行访问或修改，包括：Adapter,Bridge, Composite, Decorator, Facade, Flyweight, Proxy;

行为型模式则用来说明对象如何更好地执行方法以及如何优雅地同其他对象发生交互，或者对象间如何优雅地进行协同工作，包括：Interpreter, Template Method, Chain of Responsibility, Command,Iterator, Mediator, Memento, Observer, State, Strategy, Visitor.
##    AbstractFactory

Provide an interface for creating families of related or dependent object without specifying their concrete classes.

中文：抽象工厂模式

提供一个创建一系列相关或相互依赖对象的接口，而无需指定它们的具体类。

 

##    Adapter

Convert the interface of a class into another interface clients except. Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces.

中文：适配器模式

将一个类的接口转换成客户希望的另一个接口。Adapter模式使得原本由于接口不兼容而不能一起工作的那些了可以一起工作。

 

##    Bridge

Decouple an abstraction from its implementation so that the two can vary independently.

中文：桥梁模式

将抽象部分与它的实现部分分离，使他们都可以独立地变化。

 

##    Builder

Separate the construction of a complex object from its representation so that the same construction process can create different representations.

中文：构建者模式

将一个复杂对象的构建与它的表示分离，使得同样的构建过程可以创建不同的表示。

 

##    Chain of Responsibility

Avoid coupling the sender of a requestits receiver by giving more than one object a chance to handle the request.Chain the receiving objects and pass the request along the chain until anobject handles it.

中文：责任链模式

为解除请求的发送者和接收者之间的耦合，而使多个对象都有机会处理这个请求。将这些对象连成一条链，并沿着这条链传递该请求，直到有对象处理它。

 

##    Command

Encapsulate a request as an object,thereby letting you parameterize clients with different requests, queue or log requests, and support undoable operations.

中文：命令模式

将一个请求封装为一个对象，从而使你可用不同的请求对客户进行参数化，对请求排队或记录请求日志，以及支持可取消的操作。

 

##    Composite

Compose object into tree structures torepresent part-whole hierarchy. Composite lets clients treat individual objectsand compositions of objects uniformly.

中文：组合模式

将对象组合成树形结构以表示“部分-整体”的层次结构。Composite 使得客户对单个对象和复合对象的使用具有一致性。

 

##    Decorator

Attach additional responsibilities to an object dynamically. Decorators provides a flexible alternative to subclasses for extending functionality.

中文：装饰者模式

动态地给一个对象添加一些额外的职责。就扩展功能而言，Decorator模式比生成子类的方式更为灵活。

 

##    Façade

Provide a unified interface to a set ofinterfaces in a subsystem. Façade defines a higher-level interface that makesthe subsystem easier to use.

中文：门面模式

为子系统中的一组接口提供一个一致的接口。Façade模式定义了一个高层接口，这个接口使得这一子系统更加容易使用。

 

##   FactoryMethod

Define an interface for creating anobject, but let subclasses decide which class to instantiate. Factory methodlets a class defer instantiation to subclasses.

中文：工厂方法模式

定义一个用于创建对象的接口，让子类决定将哪一个类实例化，FactoryMethod使一个类的实例化延迟到其子类。

 

##   Flyweight

Use sharing to support large numbers offine-grained objects efficiently.

中文：享元模式

运用共享技术有效地支持大量细粒度的对象。

 

##   Interpreter

Given a language, define are presentation for its grammar along with an interpreter that uses there presentation to interpret sentences in the language.

中文：解释器模式

定义一个语言，定义它的文法的一种表示，并定义一个解释器，该解释器使用该表示来解释语言中的句子。

 

##   Iterator

Provide a way to access the elements ofan aggregate object sequentially without exposing its underlying representation.

中文：迭代器模式

提供一种方法顺序访问一个聚合对象中各个元素，而又不需暴露该对象的内部表示。

 

##   Mediator

Define an object that encapsulates howa set of objects interact. Mediator promotes loose coupling by keeping objectsfrom referring to each other explicitly and it lets you vary their interactionindependently.

中文：中介者模式

用一个中介对象来封装一系列的对象交互。中介者使各对象不需要显示地相互引用，从而使其耦合松散，而且可以独立地改变它们之间的交互。

 

##   Memento

Without violating encapsulates, captureand externalize an object’s internal state so that the object can be restored to this state later.

中文：备忘录模式

在不破坏封装性的前提下，捕获一个对象的内部状态，并在该对象之外保持该状态，这样以后就可以将该对象恢复到保存的状态。

 

##   Observer

Define a one-to-many dependency between objects so that when one object changes state all its dependents are notified and updated automatically.

中文：观察者模式

定义对象间的一种一对多的依赖关系，以便当一个对象的状态发生改变时，所有依赖于它的对象都得到通知并自动刷新。

 

##   Prototype

Specify the kinds of objects to create using a prototypical instance, and create new objects by copying the prototype.

中文：原型模式

用原型实例指定创建对象的种类，并且通过拷贝这个原型来创建新的对象。

 

##   Singleton

Ensure a class only has one instance,and provide a globe point of access to it.

中文：单例模式

保证一个类仅有一个对象，并提供一个访问它的全局访问点。

 

##   State

Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.

中文：状态模式

允许一个对象在其内部状态改变时改变它的行为。对象看起来似乎修改了它所属的类。

 

##   Strategy

Define a family of algorithms,encapsulate each one and make them interchangeable. Strategy lets the algorithmvary independently from clients that use it.

中文：策略模式

定义一系列的算法，把它们一个个封装起来，并且使他们可相互替换。本模式使得算法的变化可以独立于使用它的客户。

 

##   TemplateMethod

Define the skeleton of an algorithm inan operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing thealgorithm’s structure.

中文：模板方法

定义一个操作中的算法的骨架，而将一些步骤延迟到子类。TemplateMethod 使得子类可以不改变一个算法的结构即可重定义该算法的某些特定步骤。

 

##   Proxy

Provide a surrogate or placeholder foranther object to control access to it.

中文：代理模式

为其他对象提供一个代理以控制对这个对象的访问。

 

##   Visitor

Represent an operation to be performedon the elements of an object structure. Visitor lets you define a new operation without changing the classes of the elements on which it operates.

中文：访问者模式

表示一个作用于某对象结构中的各元素的操作。它使你可以在不改变各元素类别的前提下定义作用于这些元素的新操作。

 


