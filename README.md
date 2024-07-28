# Projects Overview

This repository contains various projects demonstrating different design patterns and practical implementations. Each project showcases a specific pattern or concept in software design. Below are the details for each project.

## 1. Weather Alert System

### Use Case Name
Weather Alert System

### Use Case Description
A weather alert system that sends notifications based on weather conditions. Users receive alerts for severe weather conditions like thunderstorms, high winds, or extreme temperatures.

### Logic of the Code
The system uses a strategy pattern to dynamically choose different alert strategies (e.g., email, SMS, push notifications) based on the weather conditions. It incorporates a `WeatherAlert` class that manages alerts and uses decorators to add additional features such as alert priorities or different notification methods.

### What It Solves
The system provides a flexible way to manage and deliver weather alerts. It allows easy addition of new alert methods and priorities without altering the core logic.

### Where It Is Used
This system can be used in weather apps, smart home systems, or any application requiring real-time weather notifications.

## 2. Lighting Control System

### Use Case Name
Adaptive Lighting Control System

### Use Case Description
An adaptive lighting control system that adjusts lighting based on different strategies. The system allows users to choose between different lighting strategies (e.g., bright, dim) based on their preferences or environmental conditions.

### Logic of the Code
The system employs the strategy pattern to switch between different lighting strategies dynamically. The `LightingStrategy` interface defines the lighting behavior, and concrete implementations like `BrightLightingStrategy` and `DimLightingStrategy` provide specific behaviors.

### What It Solves
This system provides flexibility in managing lighting conditions, allowing for adaptive responses to different needs and environments without modifying the core system.

### Where It Is Used
This system can be integrated into smart home automation systems, office environments, or any application requiring dynamic lighting adjustments.

## 3. Meal Builder System

### Use Case Name
Custom Meal Builder

### Use Case Description
A meal builder system that allows users to customize their meal by selecting various options such as size, bread type, toppings, and sauce.

### Logic of the Code
The system uses the builder pattern to construct a meal with various customizable options. The `MealBuilder` class provides methods to set different meal components, and the `CustomMealBuilder` class extends this to handle user inputs for meal customization.

### What It Solves
It allows users to build a meal according to their preferences, providing a flexible and user-friendly interface for meal customization.

### Where It Is Used
This system is ideal for fast-food restaurants, meal delivery services, and any application that requires custom meal preparation.

## 4. Smart Device Factory

### Use Case Name
Smart Device Factory

### Use Case Description
A factory system for creating smart devices like thermostats, lights, and cameras based on user specifications.

### Logic of the Code
The factory pattern is used to create instances of different smart devices. The `SmartDeviceFactory` class provides methods to create specific devices, encapsulating the creation logic and ensuring that devices are created according to the provided specifications.

### What It Solves
It simplifies the creation of various smart devices by centralizing the creation logic in one place, making the code more maintainable and extensible.

### Where It Is Used
This factory can be used in smart home systems, IoT applications, and any system that requires the creation of different types of smart devices.

## 5. Corporate Hierarchy System

### Use Case Name
Corporate Hierarchy Management

### Use Case Description
A system to manage corporate hierarchies, including employees and managers. The system allows users to add employees, assign them to managers, and view organizational details.

### Logic of the Code
The system employs composite and iterator patterns to manage and traverse a hierarchical structure of employees and managers. Classes like `Employee`, `Manager`, and `CorporateHierarchy` handle the hierarchical structure and operations.

### What It Solves
It provides a structured way to manage and view corporate hierarchies, making it easier to handle complex organizational structures and relationships.

### Where It Is Used
This system can be used in HR management software, organizational chart applications, and any application requiring management of employee hierarchies.

## 6. Smart Home Notification System

### Use Case Name
Customizable Notification System for Smart Home

### Use Case Description
A notification system for a smart home application that allows users to receive alerts through various channels like sound, email, or mobile app notifications.

### Logic of the Code
The decorator pattern is used to enhance the base notification system with additional features. The `Notification` class represents the core notification functionality, while decorators like `SoundAlertDecorator`, `EmailNotificationDecorator`, and `MobileAppNotificationDecorator` add specific features.

### What It Solves
It provides a flexible and extensible way to manage and enhance notifications, allowing users to customize how they receive alerts without modifying the core notification logic.

### Where It Is Used
This system can be used in smart home applications, alert management systems, and any application requiring customizable notification features.

# Virtual Classroom

## Use Case Name
Virtual Classroom

## Use Case Description
The Virtual Classroom application is a terminal-based system designed to manage classroom operations, including class scheduling, student enrollment, assignment management, and attendance tracking. The system provides an efficient and user-friendly way to handle various aspects of a classroom environment.

## Logic of the Code
### ClassroomManager Class
- **Singleton Pattern**: Ensures only one instance of the `ClassroomManager` exists.
- **Classroom Management**: Handles adding and removing classrooms, listing all available classrooms.
- **Student Management**: Manages student enrollment in classrooms.
- **Assignment Management**: Schedules and tracks assignments, handles submission of assignments.

### Entities
- **Classroom**: Represents a classroom with a name, a list of students, and assignments. Provides methods to add students, assign assignments, and retrieve student information.
- **Student**: Represents a student with an ID and methods to submit assignments.
- **Assignment**: Represents an assignment with details and status.

### Commands
- **AddClassroomCommand**: Adds a new classroom.
- **AddStudentCommand**: Enrolls a student in a classroom.
- **ScheduleAssignmentCommand**: Schedules an assignment for a classroom.
- **SubmitAssignmentCommand**: Allows a student to submit an assignment.
- **ListStudentsCommand**: Lists all students in a specific classroom.
- **RemoveClassroomCommand**: Removes a classroom from the system.

### Exception Handling
Custom exceptions are used to handle specific errors such as duplicate classrooms, non-existent classrooms, or unregistered students.

### Main Class
Provides a user interface through the terminal where commands are entered and processed.

## What It Solves
The Virtual Classroom application provides a structured way to manage classroom operations, making it easier for administrators and teachers to handle tasks such as scheduling, student management, and assignment tracking. It streamlines administrative tasks and ensures that all relevant data is organized and accessible.

## Where It Is Used
- **Educational Institutions**: To manage and monitor classroom activities, including student enrollments and assignment submissions.
- **Online Learning Platforms**: To provide administrative functionality for virtual classrooms.
- **Training Centers**: To handle scheduling, assignments, and student management for various training programs.

## How to Run the Application

1. **Compile the Code**:
   Ensure that you have Java Development Kit (JDK) installed. Use the following command to compile the code:

   ```sh
   javac -d bin src/main/java/com/example/virtualclassroom/*.java src/main/java/com/example/virtualclassroom/commands/*.java src/main/java/com/example/virtualclassroom/exceptions/*.java src/main/java/com/example/virtualclassroom/entities/*.java


