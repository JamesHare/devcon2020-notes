# Features of Java after Java 8

A look at features of Java after Java 8.

### Java 9

Java Platform Module System (JMPS)

* Make the Java SE Platform, and the JDK, more easily scalable down to small computing devices;
* Improve the security and maintainability of Java SE Platform Implementations in general, and the JDK in particular;
* Enable improved application performance; and
* Make it easier for developers to construct and maintain libraries and large applications, for both the Java SE and EE Platforms.
To achieve these goals we propose to design and implement a standard module system for the Java SE Platform and to apply that system to the Platform itself, and to the JDK. The module system should be powerful enough to modularize the JDK and other large legacy code bases, yet still be approachable by all developers.

JLink

JLink is a tool that generates a custom Java runtime image that contains only the platform modules that are required for a given application. Such a runtime image acts exactly like the JRE but contains only the modules we picked and the dependencies they need to function.

Read more: https://www.baeldung.com/jlink

Collection Factory Methods

* List.of()
* Map.of()
* Collection.of()

An example:

final List<Integer> list = List.of(1, 2, 3, 4, 5);

### Java 10

Local variable type inference - VAR

* Not dynamic like JavaScript.

### Java 11

* A native HTTP Client
* Java Flight Recorder

### Java 13

* Switch Expressions
    * The switch case is being evaluated and returned at the same time.

### Java 14

* Java Flight Recorder (JFR) Event Streaming
* JPackage - A possible replacement for Maven
* Helpful NullPointerException messages