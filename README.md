# day03--2025-03-28-
# Spring Boot REST API

## Project Overview
This is a simple Spring Boot REST API for managing student information, providing endpoints to retrieve student details based on various criteria.

## Project Structure
- `AppController.java`: Main REST controller with endpoints for student operations
- `Student.java`: Model class representing student attributes

## Prerequisites
- Java 8 or higher
- Spring Boot
- Maven or Gradle

## Dependencies
- Spring Web
- Java Utilities

## Endpoints

### 1. Welcome Message
- **URL:** `/app/msg`
- **Method:** GET
- **Response:** "Hello Spring Boot!"
    ## output

  ![Screenshot (969)](https://github.com/user-attachments/assets/9fa1de4c-b641-4cf1-90ac-c29ab3e18e42)

### 2. Age Endpoint
- **URL:** `/app/age/{age}`
- **Method:** GET
- **Description:** Returns a message with the provided age
- **Example:** `/app/age/23` returns "My age is 23"
    ## output

     -![Screenshot (970)](https://github.com/user-attachments/assets/a7b892f3-c05d-47c8-900c-955820880baf)

      
### 3. Get Single Student
- **URL:** `/app/student`
- **Method:** GET
- **Description:** Returns the first predefined student (s1)
    ## output

-![Screenshot (971)](https://github.com/user-attachments/assets/65682061-6336-4d8b-b239-88b3b7424134)

### 4. Get All Students
- **URL:** `/app/students`
- **Method:** GET
- **Description:** Returns a list of all predefined students
    ## output

    ![Screenshot (973)](https://github.com/user-attachments/assets/29d443bf-aeb8-4a51-a474-f56d1a97f5b4)
    ![Screenshot (972)](https://github.com/user-attachments/assets/401b2637-260f-4ad0-aa49-e25f8b8b9c9f)

### 5. Get Student by Registration Number
- **URL:** `/app/students/{regNo}`
- **Method:** GET
- **Description:** Returns a specific student by their registration number
- **Example:** `/app/students/2020ICT47`
     ## output

  -![Screenshot (978)](https://github.com/user-attachments/assets/279a25ba-23f8-443f-a935-1396ed219e4e)

### 6. Get Students by Age Range
- **URL:** `/app/ages`
- **Method:** GET
- **Description:** Returns students between ages 20-23
     ## output

    -![Screenshot (975)](https://github.com/user-attachments/assets/a71d475b-d8a5-4230-90a5-e35550308adc)

### 7. Get Students Sorted by GPA
- **URL:** `/app/students/gpa`
- **Method:** GET
- **Description:** Returns students sorted by GPA in ascending order
     ## output
    -![Screenshot (976)](https://github.com/user-attachments/assets/414b7aff-b63a-4fcd-9213-c620e70c25cf)
    -![Screenshot (977)](https://github.com/user-attachments/assets/fba9a9c0-8365-418b-a2ed-8bdfc814d138)

## Student Model
The `Student` class has the following attributes:
- `regNo`: Registration Number (String)
- `name`: Student Name (String)
- `age`: Student Age (Integer)
- `course`: Student's Course (String)
- `gpa`: Student's Grade Point Average (Double)


## Running the Application
1. Ensure you have Java and Spring Boot installed
2. Clone the repository
3. Build the project using Maven or Gradle
4. Run the Spring Boot application
5. Access endpoints via `http://localhost:8080/app/...`

## Potential Improvements
- Add error handling
- Implement database persistence
- Add POST, PUT, and DELETE endpoints
- Implement more advanced filtering and sorting

## Authors
- Maleesha Rathnayake(maleesharathnayake840@gmial.com)
