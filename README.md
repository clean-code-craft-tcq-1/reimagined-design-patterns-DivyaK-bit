# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

Adapter

Summary and example: Adapter is a structural design pattern,that works as a bridge between two incompatible interfaces. The adapter pattern converts the interface of a class into another interface clients expect. Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces. Adapters can not only convert data into various formats but can also help objects with different interfaces collaborate

The power plug and sockets standards are different in different countries. This problem can be solved by using a power plug adapter.

Advantages: Helps achieve reusability and flexibility. Client class is not complicated by having to use a different interface

Disadvantages: All requests are forwarded, so there is a slight increase in the overhead. Sometimes many adaptations are required along an adapter chain to reach the type which is required.

Builder

Summary and example: Builder is a creational design pattern,a Builder class builds the final object step by step. This builder is independent of other objects. The Builder pattern suggests that you extract the object construction code out of its own class and move it to separate objects called builders. The pattern organizes object construction into a set of steps. To create an object, you execute a series of these steps on a builder object. The important part is that you don’t need to call all of the steps. You can call only those steps that are necessary for producing a particular configuration of an object.

Home is the final end product (object) that is to be returned as the output of the construction process. It will have many steps like basement construction, wall construction and so on roof construction. Finally the whole home object is returned

Advantages: The parameters to the constructor are reduced and are provided in highly readable method calls. Builder design pattern also helps in minimizing the number of parameters in constructor and thus there is no need to pass in null for optional parameters to the constructor.

Disadvantages: Requires creating a separate ConcreteBuilder for each different type of Product.

Observer

Summary and example: Observer is a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

All users of an app on play store gets notified if there is an update

Advantages: Provides a loosely coupled design between objects that interact. Loosely coupled objects are flexible with changing requirements. Here loose coupling means that the interacting objects should have less information about each other.

Disadvantages: Memory leaks caused by Lapsed listener problem because of explicit register and unregistering of observers.

Decorator

Decorator is a structural design pattern ,that allows a user to add new functionality to an existing object without altering its structure. This pattern creates a decorator class which wraps the original class and provides additional functionality keeping class methods signature intact.

Advantages: The decorator pattern can be used to make it possible to extend (decorate) the functionality of a certain object at runtime.

Disadvantages: Decorators can complicate the process of instantiating the component because you not only have to instantiate the component, but wrap it in a number of decorators.
