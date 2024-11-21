# Activity 7: Robotics School Management System

## Project Name
Robotics School Management System

## Project Description
This project is a web-based management system designed for a small robotics school. The system allows for the management of users (students, teachers, and administrators), groups, courses, and robotics kits. 

### Features:
- **User Roles**: There are three user roles in the system – students, teachers, and administrators.
- **Courses**: Each course includes a title, a course cover image, content, and is associated with a robotics kit.
- **Groups**: Students are grouped into levels: beginner, intermediate, and advanced. More groups can be added in the future.
- **Robotics Kits**: Each course is associated with a specific robotics kit that is required for the students to complete the course.

### Entities in the System:
- **User**: Represents the people who can log in to the system, with roles such as student, teacher, or administrator.
- **Group**: Defines a learning level (beginner, intermediate, advanced) where students are grouped.
- **Course**: Contains the material for a subject along with the robotics kit required.
- **Robotics Kit**: Represents the educational kits used in each course.

## ER Diagram
![Captura de pantalla 2024-10-05 191537](https://github.com/user-attachments/assets/b57bb49c-d5ce-4e31-9aa2-4bdcc1d88234)


The ER diagram above represents the relationships between entities:
- **Users** can be students, teachers, or administrators.
- **Students** belong to **groups**, and each **group** is assigned to **courses**.
- **Courses** require a **robotics kit**, which is linked through a one-to-one relationship.

## Installation Instructions
1. Clone the repository.
2. Run `composer install` to install dependencies.
3. Configure the `.env` file with your database credentials.
4. Run `php artisan migrate` to set up the database.
5. Seed the database using `php artisan db:seed`.
6. Run `php artisan serve` to start the local development server.

