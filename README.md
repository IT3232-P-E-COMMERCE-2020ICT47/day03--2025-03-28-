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
  
   - ![Screenshot (969)](https://github.com/user-attachments/assets/9fa1de4c-b641-4cf1-90ac-c29ab3e18e42)

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

      -![Screenshot (971)](https://github.com/user-attachments/assets/c55a8381-1fb9-4387-8133-8e7ee4a2555a)


### 4. Get All Students
- **URL:** `/app/students`
- **Method:** GET
- **Description:** Returns a list of all predefined students
    ## output

       -![Screenshot (972)](https://github.com/user-attachments/assets/36aa6208-1bb0-4033-aee1-970c36384cdc)
       -![Screenshot (973)](https://github.com/user-attachments/assets/3311f945-8a15-4955-ae8a-c92766bf5c4c)



### 5. Get Student by Registration Number
- **URL:** `/app/students/{regNo}`
- **Method:** GET
- **Description:** Returns a specific student by their registration number
- **Example:** `/app/students/2020ICT47`
     ## output

       - ![Screenshot (978)](https://github.com/user-attachments/assets/8d1f83c3-9b0e-4a92-92c6-49cccba3b887)


### 6. Get Students by Age Range
- **URL:** `/app/ages`
- **Method:** GET
- **Description:** Returns students between ages 20-23
     ## output

       -![Screenshot (975)](https://github.com/user-attachments/assets/95912f6f-7417-4ac8-a125-3ad2f25cabb3)


### 7. Get Students Sorted by GPA
- **URL:** `/app/students/gpa`
- **Method:** GET
- **Description:** Returns students sorted by GPA in ascending order
     ## output

        -![Screenshot (976)](https://github.com/user-attachments/assets/8fa276fa-7c53-4b1b-885d-2e0237423918)
        -![Screenshot (977)](https://github.com/user-attachments/assets/52f53b39-0df9-4ba6-ac06-fd043fb74a5e)

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
