---
layout: page
title: Java Style Guide
version: pre2024
---

Version: {{ page.version }}

# 4290 Java Style Guide
This is a style guide made for writing Java code for 4290, more specifically using WPILib. This guide should follow all the specifications listed in the [Index for Style Guides](./).

## Index
  - [1. Folder \& File Structure](#1-folder--file-structure)
    - [1.1 Code Licensing](#11-code-licensing)
    - [1.2 Citing Borrow Code](#12-citing-borrowed-code)
    - [1.3 Constants File](#13-in-file-constants)
    - [1.4 Mapping Controls](#14-mapping-controls)
  - [2. Formatting](#2-formatting)
  - [3. Naming](#3-naming)

## 1. Folder & File Structure
### 1.1 Code Licensing
Codebases should be licensed under one of the two following licenses:
- A. [MIT License](https://choosealicense.com/licenses/mit/)
- B. [Apache License](https://choosealicense.com/licenses/apache-2.0/)

All *robot* code should be licensed under MIT, and while any other codebases are up to the discretion of the maintainers, they should still use one of the previously listed licenses.


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

If a constant seems to general to be contained in a specific class, then it should be put into 'RobotContainer.java', and **not** a 'Constants.java' file.


### 1.4 Mapping Controls
All controller mappings should be contained in a dedicated 'Controls.java' file in the root of the project.

The controls file should be documented with comments at the top of the file, explaining every mapping and its functionality, as well as comments above the implementation of each mapping, explaining what it does. An example of a this:

```java
/*
□ / X - Run Intake
*/

...

// Runs the intake
controller.square_x.whileTrue(bot.intake.runIntake(Args);

```


## 2. Formatting

## 3. Naming