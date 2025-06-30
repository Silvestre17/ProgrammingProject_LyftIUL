# 🚗 LyftIUL: A Python-based Carpooling Management System 🚗

<p align="center">
  <img src="./img/LyftIUL_logo.png" alt="LyftIUL Logo" width="200">
</p>

<p align="center"><b>Academic Year:</b> 2021/2022 <b>| 1st Semester | 1st Year</b></p>

<p align="center">
    <!-- Project Links -->
    <a href="https://github.com/Silvestre17/ProgrammingProject_LyftIUL"><img src="https://img.shields.io/badge/Project_Repo-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Repo"></a>
</p>

## 📝 Description

**LyftIUL** is a command-line application developed in Python that simulates a carpooling management platform for students at **ISCTE-IUL**. It allows users, acting as either **Drivers** or **Riders**, to manage their profiles, vehicles, and trips, facilitating ride-sharing between their homes and the university. The entire system is built on object-oriented principles.

## ✨ Objective

The main goal of this project was to apply object-oriented programming concepts to develop a robust, class-based system in Python capable of:
*   👤 Managing user and vehicle registrations.
*   🗺️ Scheduling and managing individual trips.
*   🤝 Handling passenger sign-ups for available rides.
*   📊 Providing key system statistics and activity analysis.

## 🎓 Project Context

This was an individual project developed for the **Programação** (*Programming*) course in the **[Licenciatura em Ciência de Dados](https://www.iscte-iul.pt/degree/code/0322/bachelor-degree-in-data-science)** (*Bachelor Degree in Data Science*) at **ISCTE-IUL**. The project was designed to demonstrate proficiency in *Python* programming, ***object-oriented design***, and basic data structures, since it was the first time we programmed in this course.

## ⚙️ Core Concepts

The platform is built around four main classes that model the real-world concepts of the carpooling system:

*   **`👤 User`**: Represents an ISCTE student. Key attributes include a unique student number, name, address, and contact information. A user can be a Driver or a Rider.
*   **`🚗 Vehicle`**: Represents a car owned by a Driver. Attributes include license plate, description, number of seats, and a counter for trips made.
*   **`🗺️ Trip`**: Represents a scheduled journey. It links a `Vehicle` to a specific date/time, route, number of available seats, and a list of registered passengers.
*   **`⚙️ Manager`**: The central class that orchestrates the entire system. It holds lists of all users, vehicles, and active trips, providing methods to manage the platform's operations.

## 🛠️ Technologies Used

This project was developed entirely in Python, using standard libraries and a few key packages for data analysis and visualization.

<p align="center">
    <a href="https://www.python.org/">
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    </a>
    <a href="https://numpy.org/">
        <img src="https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="Numpy" />
    </a>
    <a href="httpshttps://matplotlib.org/">
        <img src="https://img.shields.io/badge/Matplotlib-D3D3D3?style=for-the-badge&logo=matplotlib&logoColor=black" alt="Matplotlib" />
    </a>
</p>

## 📋 Project Breakdown & Key Tasks

The project was structured into five main implementation tasks (`T1` to `T5`), each focusing on a specific aspect of the system:

1.  **Task 1: User and Vehicle Classes (`T1`)**
    *   Implemented the `Utilizador` (User) and `Viatura` (Vehicle) classes with all required attributes (e.g., student number, address, license plate) and methods (e.g., getters, setters, `add_new_trip`). Ensured data integrity, such as making the student number immutable after creation.

2.  **Task 2: Trip Class (`T2`)**
    *   Developed the `Viagem` (Trip) class to manage individual journeys. This included properties to check if a trip is still active (`ativa`), calculate available seats (`boleias_disponiveis`), and methods to add passengers, preventing overbooking.

3.  **Task 3: Manager Class (`T3`)**
    *   Created the central `Gestor` (Manager) class to act as the system's brain. This class is responsible for managing lists of users, vehicles, and trips, preventing duplicates (e.g., users with the same number), and providing core system functionalities like listing entities, adding new trips, and cleaning up completed trips by archiving them to a `.csv` file.

4.  **Task 4: Main Program & CLI (`T4`)**
    *   Built a user-friendly, menu-driven command-line interface (CLI) to allow interaction with the system. The program runs in a loop, enabling users to perform operations like listing users, registering trips, and signing up for rides until they choose to exit.

5.  **Task 5: Statistical Analysis (`T5`)**
    *   Implemented a feature to analyze the trip history from the `historico.csv` file. This involved:
        *   Reading the historical data.
        *   Creating a **NumPy** matrix to aggregate the number of trips and rides per hour of the day.
        *   Visualizing this data with a **Matplotlib** plot to show peak activity hours.
        *   Calculating and displaying key metrics like average trips per hour and the busiest hour for rides.

## 🚀 How to Run

To run this application, follow these steps:

1.  **Prerequisites:**
    *   Ensure you have Python 3.x installed.
    *   Install the required libraries:
        ```bash
        pip install numpy matplotlib
        ```

2.  **Execution:**
    *   Navigate to the project's root directory in your terminal.
    *   Run the main script:
        ```bash
        python ProjetoProgramação_AndréSilvestre_CDA1_Nº104532.py
        ```
    *(Note: Replace `ProjetoProgramação_AndréSilvestre_CDA1_Nº104532.py` with the actual name of your main executable script.)*

3.  **Interaction:**
    *   The program will display a menu of options. Enter the number corresponding to the action you wish to perform.

## 🇵🇹 Note

This project was developed using Portuguese from Portugal 🇵🇹.