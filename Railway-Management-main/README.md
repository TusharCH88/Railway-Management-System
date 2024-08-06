# Railway Management System

## Overview

The Railway Management System is a Java-based application that provides a graphical user interface (GUI) for managing railway operations, including booking tickets, searching for trains, and viewing train schedules. The system is designed using Object-Oriented Programming (OOP) principles to ensure modularity, scalability, and maintainability.

## Features

- **Login System**: Login functionality to access the system.
- **Train Search**: Search for trains between two stations for a specified date.
- **Booking System**: Book tickets by providing passenger details, seat preferences, and payment information.
- **Train Schedules**: View detailed train schedules, including departure and arrival times.

## OOP Concepts

The Railway Management System leverages several key Object-Oriented Programming concepts:

### 1. Classes and Objects

- **Station**: Represents a railway station with a name and a list of tracks connected to it.
- **Track**: Represents a track between two stations with a specified distance.
- **Train**: Represents a train with an ID, name, schedule, and delay information.
- **Booking**: Represents a booking with details like train, stations, date, passenger name, seat, and payment info.

### 2. Encapsulation

Encapsulation is used to bundle the data (attributes) and methods (functions) that operate on the data within a single unit or class. This helps in protecting the internal state of an object from unintended modifications.

- Each class has private fields and public methods to access and modify those fields.
- Example: The `Station` class has private attributes and methods to manage tracks.

### 3. Inheritance

Inheritance allows one class to inherit the fields and methods of another class. Although this project does not have an explicit inheritance hierarchy, it could be extended to have more specialized types of trains or stations.

### 4. Polymorphism

Polymorphism allows objects to be treated as instances of their parent class rather than their actual class. This can simplify the code and enhance flexibility.

### 5. Abstraction

Abstraction involves hiding the complex implementation details and showing only the necessary features of an object. The GUI components (like buttons, labels, and frames) interact with the backend logic without exposing the complex details.

## Code Structure

### Classes

- **Station**: 
  - Attributes: `name`, `tracks`
  - Methods: Constructor, methods to manage tracks

- **Track**:
  - Attributes: `from`, `to`, `distance`
  - Methods: Constructor

- **Train**:
  - Attributes: `id`, `name`, `schedule`, `delay`
  - Methods: Constructor

- **Booking**:
  - Attributes: `train`, `from`, `to`, `date`, `passengerName`, `seat`, `paymentInfo`
  - Methods: Constructor

### GUI Components

- **Main**: The main class initializes the data and creates the GUI windows.
  - `setupData()`: Initializes stations, tracks, and trains.
  - `createWelcomePage()`: Creates the welcome screen.
  - `createLoginPage()`: Creates the login screen.
  - `createSearchPage()`: Creates the train search screen.
  - `createTrainListPage()`: Displays the list of available trains.
  - `createBookingPage()`: Creates the booking details screen.
  - `createThankYouPage()`: Displays the booking confirmation.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) installed on your machine.
- An IDE or text editor for Java development (e.g., IntelliJ IDEA, Eclipse, VS Code).

### Running the Application

1. Clone the repository to your local machine.
2. Open the project in your preferred IDE.
3. Compile and run the `Main` class.
4. Follow the GUI prompts to use the Railway Management System.
