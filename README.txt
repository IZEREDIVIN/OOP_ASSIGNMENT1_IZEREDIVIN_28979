AUCA_28979: Console School Management System

Student: Izere Divin | ID: 28979 | Group: F | Assignment: OOP Practical 1

A console-based Java application that manages departments, students, teachers, administrators, courses, classrooms, enrollments, assessments, fee payments and library loans. It demonstrates encapsulation, multilevel and hierarchical inheritance, interfaces, abstract classes, polymorphism, validation and custom exceptions.

Requirements
- Java 17 or later

 Run
Double-click `run.bat`, or compile and run manually:

```
javac -d bin src\*.java
java -cp bin Main
```

Features
- 19-option menu that loops until `0` (Exit)
- Guided registration forms with `BACK` / `CANCEL`, review and edit before saving
- Related records chosen from numbered lists, with nested registration when a prerequisite is missing
- Validation for IDs, emails, phones, dates, amounts, scores and stock
- Custom exceptions: `ValidationException`, `DuplicateRecordException`, `RecordNotFoundException`, `PrerequisiteMissingException`, `BookUnavailableException`

Structure
```
Person (abstract)
 ├── AcademicMember (abstract)
 │     ├── Student
 │     └── Teacher
 └── Administrator
```
Interfaces: `Identifiable`, `Registrable`. All other entities implement both.
