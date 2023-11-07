# 4290 Programming Training Ch 1.2 - Comments
## About Comments
Comments exist in most programming languages in some form, and are used to tell the program to ignore the text. Comments can be used for documentation, explanations of abstract code, or even to ignore lines of code.

## Writing Comments

### Single Line
Single line comments start with two forward slashes. Any text between // and the end of the line will be ignored when the code runs.

```java
// I am comment
System.out.println("This code will run");

// The code below won't run  
// System.out.println("This code has been commented out")
```

### Multi Line
Multi Line comments take up multiple lines, Any text Between `/*` and `*/` will be ignored when the code runs.

```java
/* I am a comment.
The code below will print "Hello World" */
System.out.println("Hello World");

// The code below will not run
/* 
void sayHello(){
    System.out.println("Hello");
} 
*/
```
---

### [<< Previous](./1_syntax_variables.md) | Next (Coming Soon) >>