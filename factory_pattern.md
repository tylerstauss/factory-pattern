Factory pattern is the most used design pattern in languages like Java and C#

The intent:
create objects without exposing the instantiation logic to the client
refers to the newly created object through a common interface

The implementation:
The client needs a product, but instead of creating it directly, it asks the factory object for a new product, providing info about the type of object it needs
The factory instantiates a new concrete product and returns to the client the newly created product
The client uses the products as abstract products, without being aware about their concrete implementation

An example:
The client is using a graphical design application and decides to create a new circle. They click the button to create a new circle. Instead of the application just creating a new instance of the circle class, the information is passed to the parent, shape class, which then decides to create a circle class from it. This is then returned to the framework as an abstract shape, and the client never knows that it was a circle object.

The advantage is that new shapes can be added without changing a single line of code in the framework. 

Most commonly used in Java.