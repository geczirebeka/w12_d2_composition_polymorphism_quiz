# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

poly means multiple/many and morphism means form, so many forms.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.



3. What can we use to implement polymorphism in Java?

We can use both abstart classes and interfaces.

4. How many 'forms' can an object take when using polymorphism?

Depends if it inherits from an abstract class then 2, but we can implement as many inerfaces as we need in classes so then as many as we need.

5. Give an example of when you could use polymorphism.

When we have one class that has an ArrayList that is composed of instances of multiple different classes that have a common behaviour, therefore they could all take up the type of that interface that has the shared behaviour.Thus making the code not having to repeat methods for the different classes and create many arraylists.



# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

That an object is part of another object. This second object is made up of other objects and it also takes over their ownership.

7. When would you use composition? Provide a simple example in Java.

When an object is part of an other object and cannot exist without it.

class Book {
    private String title;
    private String author;
}

class Library {
    private Book book;

    public Library() {
        this.book = new Book();
    }
}

8. Give a difference between composition and aggregation?

In aggregation, objects can exist indepedently of the object which it composes and in composition they can't.

9. What is/are the advantage(s) of using composition/aggregation?

They allow a class to use behaviour from a group of other classes, and make it possible for that behaviour to change.

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?
They are also destroyed.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?
They can still exist independently.