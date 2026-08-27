# 🎓 Student Grade Management

A Windows desktop application for managing students, subjects, grades, and academic results.

The system provides a central menu from which users can maintain student records, manage subjects and their coefficients, enter grades, review results, and generate a results report. It was developed with **PC SOFT WinDev** and uses the **HyperFile** data format for local data storage.

This project demonstrates how a desktop information system can bring together data entry screens, persistent records, result consultation, and printable reporting in one application.

## 🎥 Demo

▶️ **Project demonstration:** Add a link to a project demonstration video here.

---

## 📌 Features

### 1. 🧭 Main Menu

The main menu provides access to the principal areas of the application:

* Student management
* Subject management
* Grade management
* Results consultation
* Results reporting

### 2. 👩‍🎓 Student Management

The student module stores the main information required to identify a student:

* Student ID
* First name
* Last name

### 3. 📚 Subject Management

Subjects can be maintained with the information used to organise and evaluate academic results:

* Subject ID
* Subject name
* Coefficient

### 4. 📝 Grade Management

The grade module associates grade records with the student and subject data. Grade records have their own automatically generated identifier and are stored persistently in the application database.

### 5. 📊 Results and Reporting

Users can open the results window to review academic results and use the dedicated results report to present or print the available information.

The project includes the report definition `RPT_Results.wde` alongside the results window `Results.wdw`.

---

## 🧠 Concepts Demonstrated

The project demonstrates practical desktop application and database concepts, including:

* Window-based user interface design
* Data entry and record management
* Relationships between students, subjects, and grades
* Persistent local data storage
* Automatic identifiers for records
* Report generation
* Separation of application screens, data analysis, and deployment files

---

## 🏗️ Data Model

The WinDev analysis defines the following main data entities.

### `Student`

Stores student identity information:

* `Student_ID`
* `First_name`
* `Last_name`

### `Subject`

Stores the subjects used by the system:

* `Subject_ID`
* `Name`
* `Coefficient`

### `Grade`

Stores grade records that connect students and subjects. The physical HyperFile file for this entity is named `Student_Subject_REAL.fic`, and `Grade_ID` is an automatic 8-byte identifier.

---

## 🔄 System Workflow

The normal workflow is:

```text
Open the application
	|
	v
Use the main menu
	|
	+--> Add or update students
	|
	+--> Add or update subjects and coefficients
	|
	+--> Enter and manage grades
	|
	v
Consult results
	|
	v
Generate or print the results report
```

---

## 🛠️ Technologies

* **Development environment:** PC SOFT WinDev
* **Project type:** Windows desktop application
* **Database technology:** HyperFile
* **Included package:** 32-bit Windows executable and installer
* **Project metadata:** WinDev project, analysis, windows, report, and deployment definitions

---

## 🚀 How to Run

### Option 1: Use the included installer

The repository includes a packaged installer in:

```text
Student_Grade_Management/Install_32-bit Windows executable/
```

Run `INSTALL.EXE` on a compatible Windows system and follow the installation steps.

### Option 2: Run the packaged application

The generated application files are available in:

```text
Student_Grade_Management/Exe/
```

Use the packaged executable on a compatible Windows system. The package is identified as a **32-bit Windows executable**, so compatibility with the target Windows environment should be checked before deployment.

### Option 3: Open the project in WinDev

Open the project file in a compatible WinDev installation:

```text
Student_Grade_Management/Student_Grade_Management.wdp
```

The project contains the application windows, report definition, analysis, and database mapping required for development or maintenance.

---

## 📂 Project Structure

```text
Student-Management/
|
|-- README.md
`-- Student_Grade_Management/
    |-- Student_Grade_Management.wdp   # WinDev project file
    |-- Menu.wdw                        # Main menu
    |-- Students.wdw                    # Student management window
    |-- Subjects.wdw                    # Subject management window
    |-- Grades.wdw                      # Grade management window
    |-- Results.wdw                     # Results window
    |-- RPT_Results.wde                 # Results report definition
    |-- Student_Grade_Management.xdd    # Database analysis definition
    |-- Student_Grade_Management.REP    # HyperFile database mapping
    |-- Exe/                             # Generated application and data files
    |-- Install_32-bit Windows executable/ # Windows installer package
    |-- Backup/                          # Project backup files
    `-- Student_Grade_Management.ana/   # Analysis and history files
```

---

## ⚙️ Current Limitations

This repository contains a WinDev project and compiled or proprietary project files rather than ordinary text-based source code. As a result:

* The application is designed for Windows.
* The included package targets 32-bit Windows.
* The project requires a compatible WinDev environment for source-level maintenance.
* HyperFile data files are local application files and are not documented here as a server-based database.
* Detailed validation rules, grading formulas, permissions, and business rules cannot be confirmed from the exported binary project files alone.
* The repository contains generated backups, analysis history, and deployment artifacts in addition to the main project files.

---

## 🔮 Possible Improvements

Future versions could include:

* A modern 64-bit build
* More detailed validation and error messages
* Authentication and role-based access
* Export of results to PDF, Excel, or CSV
* Configurable grading and pass/fail rules
* Search and filtering across students, subjects, and results
* Backup and restore tools for application data
* A clearer separation between development files and generated deployment files
* A web or cross-platform version of the system

---

## 🎯 Purpose of the Project

The purpose of this project is to provide a practical student information and grade management system. It combines structured data storage, desktop user interfaces, grade entry, result consultation, and report generation into a single WinDev application.

The project is also useful for demonstrating the main stages of a database-driven desktop application: defining an analysis, creating data-entry windows, connecting records, presenting results, and preparing an executable installation package.

---

## 👩‍💻 Author

**[Your Name]**

Replace this text with the author name, institution, and any other project details you would like to share.

---

⭐ Explore the WinDev project files and the included Windows installation package to learn more about the system.
