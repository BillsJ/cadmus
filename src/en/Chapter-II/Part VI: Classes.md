Classes
===

## Creating Classes
I've already alluded to classes before. Classes are the blueprints for objects. What are objects? Objects are designed to represent entities in real life. For example you might have a class called `Car`, which has properties such as `speed` and methods such as `setGear()`. You cannot actually use the properties or methods till you instatiate the `Car` class, however. Objects are classes when instantiated. "Instantiated" is a posh word for "created". For instance let's say I have the code:

```java
public class Book {
  private String title;
  private String author;
  private String publisher;

  public Book(String bookTitle, String authorName, String publisherName) {
    title = bookTitle;
    author = authorName;
    publisher = publisherName;
  }

  public static void main(String[] args) {
    Book firstBook = new Book("Horton Hears A Who!","Dr. Seuss","Random House");
  }
}
```

The first three statements within the class are variable declarations. They declare properties or attributes of the class. These are the variables that a `Book` is composed of. Note that a class does not necessarily have to be composed of primitives. A class can be composed of other classes such as `String` in the example. The keyword `private` means that you can only access it inside methods of that class, but not statics. For example, this in the `main` method would fail to compile:

```java
Book firstBook = new Book("Horton Hears A Who!","Dr. Seuss","Random House");
System.out.println(firstBook.title);
```

If I, however, make the property `public` then it will. The non-static method called `Book` of class `Book` is the **constructor**. You know it's the constructor because the method has the same name as the class. A constructor is the method called when you do:

```java
new Book("Horton Hears A Who!","Dr. Seuss","Random House");
```

Notice that the way in which you create an object is similar to how you create a variable, you have the type then the name of the object then the equals sign; the only difference comes after the equals sign.  Now, you have the word `new` which just tells the interpreter that the object that you are creating is a new object, and then you have what we call a *constructor method*. The characteristics of the object are passed as parameters.

### Ex 1
Rewrite the code into Java, and instantiate your favourite book.

### Ex 2
Change the code to create an array of books, and populate it with your favourite books.

## Non-static methods
Non-static methods are methods that belong to an instance of a class, not to the class itself, like static methods, which are all you have created so far, except for the `Book` constructor. If you haven't guessed it, the only difference in defining non-static methods, is you omit the `static` keyword. For example imagine beneath the constructor I added this method:

```java
public String getTitle() {
  return title;
}

public static void main(String[] args) {
  Book harryPotter = new Book("Harry Potter", "J.K. Rowling", "Bloomsbury Publishing");
  System.out.println(harryPotter.getTitle());
}

```

As a non-static method, this will be available on every instance, that is to say object, of `Book`, and returns a `String`. Now we have a way to get the book title. Another advantage of this is that the title cannot be changed externally, but can be accessed.

### Ex 3
Add a method to get the author and publisher of a `Book`.

[Once more into the breach &rarr;](../Chapter-III/Part-I:-ArrayLists.html)
