```java
public class Ex1 {
  public static void main(String[] args) {
    System.out.println("Hello World");
    System.out.println("Hello Java");
    System.out.println("Hello, I am a programmer");
    System.out.println("Bonjour, je suis un programmeur");
    System.out.println("Saluton, mi estas programisto");
    System.out.println("Guten Tag, Hola, Ni Hao");
  }
}
```

### What you should get as output
--- IMAGE HERE ---

### Explanation
1. Look at the curly brackets (`{` and `}`). There are 2 pairs of curly brackets in the code above. Notice that for each opening curly bracket (`{`), there is a corresponding closing curly bracket ('}'). The curly brackets represent code blocks and everything contained within them is part of that code block. That is why their contents are indented.
2. Forget about everything other than the innermost code block (lines 3 to 8) from the moment. The innermost code block contains lines that each begin with `System.out.println(` and end with `);`.
3. Inside the parentheses (`(` and `)`), you have quotations marks, and inside the quotation marks you have the text that you want to print out.
4. The quotation marks tell the computer that what's enclosed in them is not computer code, but data that you want your computer code to manipulate/use. Textual data are called **strings**. They are as pointed out, always enclosed by quotation marks, to make clear that they are not computer code. They are also highlighted differently from the rest of the code.
5. `System.out.println` is a **method**. A method is just some computer code that does something. `System.out.println` is provided by the computer automatically. To use a method, you write its name `System.out.println` in this case, and you put parentheses next to it, so `System.out.println()`. This tells the computer to run that method.
6. But some methods, such as `System.out.println` take data as input. The data is called **arguments**. `System.out.println` takes in one argument, and that argument in a string. As you've probably guessed the job of `System.out.println` is to write to the terminal its argument.
7. Each line must end with `;`.

### Bonus Exercises
1. What happens if you call `System.out.println` with no arguments?
2. What happens if you put `//` at the beginning of a line
3. What happens if rather than calling `System.out.println` you call `System.out.print` for one or more of the lines.