# Java Hello Gradle + Interview Exercise

This is a base project in Java with Gradle and JUnit. It includes a "Hello World" example and is prepared for unit testing.

---

## 🚀 How to Run

From Codespaces or any terminal with Java 17 and Gradle:

### Compile and run the project
```bash
./gradlew run
```

### Run the tests
```bash
./gradlew test
```

---

## 🧠 Business Case: Event Information System

Imagine you are developing a system that informs users about relevant system events in the order they occurred. Each event arrives in text format, as a string with the following format:

```
"HH:mm-Event description"
```

For example:
```
"08:30-System startup"
"10:15-User logged in"
"09:45-Database connected"
```

Your task is to implement a function that sorts this list of messages by time, either in ascending order (from the earliest event) or descending order (from the most recent event).

---

### 🎯 Functional Requirements

- Create a method that receives:
  - A list of strings with the format `time-event`
  - Second sprint: A boolean indicating whether the order should be ascending (`true`) or descending (`false`)
- Return the sorted messages

### ✍️ Suggested Method Signature


### 🧪 Example

Given the following input:

```java
List<String> mensajes = List.of(
    "10:15-User logged in",
    "08:30-System startup",
    "09:45-Database connected"
);
```

When executing:

```java
yourFunction(mensajes, true);
```

The output should look something like this:

```
"08:30-System startup",
"09:45-Database connected",
"10:15-User logged in"
```

---
