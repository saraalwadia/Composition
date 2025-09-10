# Java Composition Example

This project demonstrates the concept of **composition in Java (OOP)**.  
Composition represents a "has-a" relationship between classes. In this example, a `Person` **has a** `Job`.

---

## Classes

### 1. `Job`
Represents a job with the following properties:

- `role` – The role of the person (e.g., Manager)
- `salary` – The salary of the person
- `id` – The job ID

**Methods:**
- `getRole()`, `setRole(String role)`
- `getSalary()`, `setSalary(long salary)`
- `getId()`, `setId(int id)`

---

### 2. `Person`
Represents a person who **has a Job**. The `Person` class uses composition to hold a `Job` object.

**Methods:**
- `getSalary()` – Returns the salary from the `Job` object
- `getRole()` – Returns the role from the `Job` object

**Constructor:**
- Initializes a `Job` object with default values:
  - Salary: `1000`
  - Role: `"Manager"`

---

### 3. `Composition` (Main Class)
Demonstrates usage of the `Person` and `Job` classes.

**Example Usage:**
```java
Person person = new Person();
long salary = person.getSalary();
String role = person.getRole();
System.out.println("Salary: " + salary); // Output: 1000
System.out.println("Role: " + role);     // Output: Manager
