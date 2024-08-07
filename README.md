# Data Mapping and Relationships in Spring Boot

This project is a Spring Boot application that manages departments and employees. It uses Java and Maven for build automation.

## Technologies Used

- **Java**
- **Spring Boot**
- **Maven**

## Project Structure

### Services

- **DepartmentService.java**: Contains methods to manage departments and their relationships with employees.

### Entities

- **EmployeeEntity.java**: Represents an employee with relationships to departments.
- **DepartmentEntity.java**: Represents a department with relationships to employees.

## Key Classes and Methods

### DepartmentService

- **assignManagerToDepartment**: Assigns a manager to a department.
- **getAssignedDepartmentOfManager**: Retrieves the department managed by a specific employee.
- **assignWorkerToDepartment**: Assigns a worker to a department.
- **assignFreelancerToDepartment**: Assigns a freelancer to a department.

### EmployeeEntity

- **id**: Unique identifier for the employee.
- **name**: Name of the employee.
- **managedDepartment**: Department managed by the employee.
- **workerDepartment**: Department where the employee works.
- **freelanceDepartments**: Departments where the employee works as a freelancer.

### DepartmentEntity

- **id**: Unique identifier for the department.
- **title**: Title of the department.
- **manager**: Manager of the department.
- **workers**: Set of employees working in the department.
- **freelancers**: Set of employees working as freelancers in the department.

## Database Relationships

- **One-to-One**: Between `DepartmentEntity` and `EmployeeEntity` for the manager.
- **Many-to-One**: Between `DepartmentEntity` and `EmployeeEntity` for workers.
- **Many-to-Many**: Between `DepartmentEntity` and `EmployeeEntity` for freelancers.

## How to Run

1. **Clone the repository**:
    ```bash
    git clone https://github.com/rudradcruze/DataMappingTutorial.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd DataMappingTutorial
    ```

3. **Build the project using Maven**:
    ```bash
    mvn clean install
    ```

4. **Run the application**:
    ```bash
    mvn spring-boot:run
    ```

## 🚀 About Me

Tech-savvy learner/programmer pushing boundaries of online tech. Passionate about new tools, seeking challenges to advance skills.

## 🔗 Social Links

![Name](https://img.shields.io/badge/Name-Francis%20Rudra%20D%20Cruze-yellowgreen?style=for-the-badge)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rudradcruze)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/rudradcruze)
[![Facebook](https://img.shields.io/badge/facebook-4267B2?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/rudradcruze)
[![francisrudra@gmail.com](https://img.shields.io/badge/gmail-4267B2?style=for-the-badge&logo=gmail&logoColor=white)](mailto:francisrudra@gmail.com)