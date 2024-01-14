---
title: 4290 Java Style Guide
version: 2024pre1
---

Style Guide Version: {{ page.version }} (WIP)

# 4290 Java Style Guide
This is a style guide made for writing Java code for 4290, more specifically using WPILib. This guide should follow all the specifications listed in the [Index for Style Guides](./).

## Index
  - [1. Folder & File Structure](#1-folder--file-structure)
    - [1.1 Code Licensing](#11-code-licensing)
    - [1.2 Citing Borrow Code](#12-citing-borrowed-code)
    - [1.3 Constants File](#13-in-file-constants)
    - [1.4 Mapping Controls](#14-mapping-controls)
  - [2. Formatting & Naming](#2-formatting--naming)
    - [2.1 Name Cases](#21-name-cases)
    - [2.2 Indentation](#22-indentation)

## 1. Folder & File Structure
### 1.1 Code Licensing
All robot, and/or utility code for robots should be licensed under the [MIT license](https://choosealicense.com/licenses/mit/), and while any other codebases are up to the discretion of the maintainers, the MIT License is heavily recommended.


### 1.2 Citing Borrowed Code
Any file that uses copied code from any external source, especially other FIRST teams, should be mentioned with a comment at the top of the file. Unless the implementation is very standard, a general rule of thumb is to just cite it. 

This comment should contain the name of the source, what was used, and a viable link to the source. An example of this would be:
```java
/* The 'Elevator Up' command was borrowed from FRC 4290, https://www.bow4290.org/ */

class Elevator {
    ...
}
```


### 1.3 In-File Constants
All constants should be contained within their relevant classes. For instance, if there is a constant called 'OPERATOR_CONTROLLER_PORT', this constant should be situated within the 'Controls.java' file.

If a constant seems too general to be contained in a specific class, then it should be put into 'RobotContainer.java', and **not** a 'Constants.java' file.


### 1.4 Dedicated Control Mapping File
All controller mappings should be contained in a dedicated 'Controls.java' file in the root of the project.

The controls file should be documented with comments at the top of the file, explaining every mapping and its functionality, as well as comments above the implementation of each mapping, explaining what it does. An example of a this:

```java
/* 
 * □ / X - Run Intake 
 */
  

...

// Runs the intake
controller.square_x.whileTrue(bot.intake.runIntake(Args);

```


## 2. Formatting & Naming
### 2.1 Standard Name Cases
Casing for any names should follow Java's standards, as follows:
- Most variables and methods use camel case (eg. camelCase), with the first word being all lower case, and each new word starting with a capital letter.
  
- Class, interface, and file names use pascal case (eg. PascalCase), with each word starting with a capital letter.

- Constants use upper snake case (eg. UPPER_SNAKE_CASE), with all words being entirely uppercase, and each word separated with underscores.

```java
// Class using Pascal Case, as well as file with same name.
public class ExampleClass(){
  // Constant using UPPER_SNAKE_CASE
  public static final VALUE_MULTIPLIER = 4;

  // Method and Variable using camelCase
  public int myValue = 2;

  public int myFunction(){
    return exampleVariable * VALUE_MULTIPLIER;
  }
}
```


### 2.2 Indentation
Indentation should be 2 spaces. This means every time a new block is indented, it should go forward 2 spaces, and back 2 at the end of the block. An example of this is shown below:
```java
// Correct
public int twoSpaces(){
  // This is the correct indentation size
  return 2;
}

// Incorrect
public int fourSpaces(){
    // This is the incorrect indentation size
    return 4;
}

```

