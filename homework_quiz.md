Polymorphism
1. What does the word 'polymorphism' mean?

Polymorphism means many forms.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

This happens when we have mulitple classes related via abstract classes and interfaces, then using the shared methods to carry out different actions.

3. What can we use to implement polymorphism in Java?

Abstract classes and interfaces. (Inheritance)

4. How many 'forms' can an object take when using polymorphism?

Multiple.

5. Give an example of when you could use polymorphism.

An example would be using an IConnect connect devices to a network, instead of using multiple methods you use one interface that can add any device to the network. This means going forward adding additional devices would require less code.

Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

When an object is part of another object, this object cannot exist without the other. A_PART_OF/IS_PART_OF

7. When would you use composition? Provide a simple example in Java.

When creating an object using objects that will not be used elsewhere, it is part of that object.

class House {
    private Roof roof;
    
    public House() {
        this.roof = new Roof();
    }

    The roof is owned by the house and when on its own can't be reused.

8. Give a difference between composition and aggregation?

With aggregation objects are built from other objects, these objects can be reused or removed. For example if you built a car and it had a faulty engine, you could remove this object and replace it with another engine object,as the car HAS_AN engine. With composition the engine would be A_PART_OF the car and couldn't be removed. The engine is created independently and used to build a car object, in composition it would be assigned to a property of the car.

9. What is/are the advantage(s) of using composition/aggregation?
- composition allows more flexability in your code
- composition makes testing objects easier.

- Aggregation helps with reusing code
- Changing an object in use in multiple classes would be easier.


10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?
The objects it is composed of are destroyed.


11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

The composed objects would still exist in any other context in which they are used.