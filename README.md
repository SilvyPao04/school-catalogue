# 🏫 School Catalogue

## 📖 Project Overview

This project implements a digital school catalog for the New York City Department of Education, allowing quick reference for each school in the city. The project focuses on **object-oriented programming (OOP)** principles like inheritance, encapsulation, and polymorphism.

The main goal of this project is to demonstrate the application of OOP principles in a real-world scenario, by creating a catalog that efficiently manages data for different types of schools using JavaScript classes and inheritance.

## 🚀 Features

- **Parent `School` Class**: 
  - Properties: `name`, `level`, and `numberOfStudents`
  - Methods: `.quickFacts()`, `.pickSubstituteTeacher()`
- **Child `PrimarySchool` and `HighSchool` Classes**: 
  - `PrimarySchool` adds a `pickupPolicy` property.
  - `HighSchool` adds a `sportsTeams` property.
- **Static Methods**: 
  - A static method to randomly select substitute teachers.

## 🛠️ Technologies Used

- **JavaScript (ES6)**: Classes, inheritance, static methods, getters, and setters.
- **Object-Oriented Programming (OOP)**: Emphasizing inheritance and encapsulation.

## 📚 Classes Overview

### 1. `School` (Parent Class)

**Properties**:
- `_name` (string): The name of the school.
- `_level` (string): The school level (e.g., 'primary', 'middle', 'high').
- `_numberOfStudents` (number): The number of students enrolled.

**Methods**:
- `quickFacts()`: Logs a quick fact about the school to the console.
- `static pickSubstituteTeacher(substituteTeachers)`: Randomly selects and returns a substitute teacher from an array of names.

### 2. `PrimarySchool` (Subclass)

**Additional Property**:
- `_pickupPolicy` (string): The school’s pickup policy.

### 3. `HighSchool` (Subclass)

**Additional Property**:
- `_sportsTeams` (array): List of sports teams at the high school.

## 💻 Example Usage

```javascript
const lorraineHansbury = new PrimarySchool('Lorraine Hansbury', 514, 'Students must be picked up by a parent, guardian, or family member over the age of 13.');
lorraineHansbury.quickFacts();

School.pickSubstituteTeacher(['Jamal Crawford', 'Lou Williams', 'J.R. Smith', 'James Harden', 'Jason Terry', 'Manu Ginobli']);

const alSmith = new HighSchool('Al E. Smith', 415, ['Baseball', 'Basketball', 'Volleyball', 'Track and Field']);
alSmith.sportsTeams;
```

🔮 ## Future Improvements

- Add more school types like `MiddleSchool`.
- Implement additional properties like `average test scores` or `school overview`.
- Build a `SchoolCatalog` class to manage different schools.

## 🙌 Acknowledgements
- This project is part of the **Learn Intermediate JavaScript** course on Codecademy.
- Thanks to Codecademy for the course material and inspiration.
