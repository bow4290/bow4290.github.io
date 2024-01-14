---
title: 4290 Java Style Guide
version: 2024.0
---

Style Guide Version: {{ page.version }}

# 4290 Java Style Guide
This is a style guide made for writing Java code for 4290, more specifically using WPILib. This guide should follow all the specifications listed in the [Index for Style Guides](./).

## Index
  - [1. Folder & File Structure][1-0]
    - [1.1 Code Licensing][1-1]
    - [1.2 Citing Borrow Code][1-2]
    - [1.3 In-file Constants][1-3]
    - [1.4 Dedicated Control Mapping File][1-4]
  - [2. Formatting & Naming][2-0]
    - [2.1 Standard Name Cases][2-1]
    - [2.2 Indentation][2-2]
    - [2.3 No Single Letter Prefixes][2-3]

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
Indentation should be 2 spaces. This means every time a new block is indented, it should go forward 2 spaces, and back 2 at the end of the block.
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


### 2.3 No Single Letter Prefixes
Prefixes to fields containing a single letter should be avoided as much as possible, as they tend to cause more harm then good. There may be a few exceptions to this, and it generally comes down to the discretion of the maintainers on these occasions.

```java
// Should Be Avoided
public static final m_leftArmMotor

// Correct
public static final leftArmMotor

```


### 2.4 Descriptive Naming
When naming anything, the name should be descriptive of what it does, while also being concise. Abbreviations should be avoided when possible, and single letter names should not be used.


[1-0]: #1-folder--file-structure
[1-1]: #11-code-licensing
[1-2]: #12-citing-borrowed-code
[1-3]: #13-in-file-constants
[1-4]: #14-dedicated-control-mapping-file

[2-0]: #2-formatting--naming
[2-1]: #21-standard-name-cases
[2-2]: #22-indentation
[2-3]: #23-no-single-letter-prefixes
[2-4]: #24-descriptive-naming