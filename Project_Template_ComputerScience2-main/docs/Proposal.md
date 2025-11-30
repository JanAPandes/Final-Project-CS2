# 📌 Project Proposal, Group 1 8-Dahlia (Final Draft)

## 📝 Project Title  
The Student Manager: A Datalist of Student Grades

---

## 🔍 Problem Statement  
In many schools, teachers manually record, compute, and analyze student grades, which can be time-consuming and be prone to errors. This makes it difficult to quickly identify students who need help, generate class statistics, or give accurate feedback.
The process of calculating student grades is often done manually, which can lead to errors in computation, loss of data, and difficulty in tracking student performance. There is also lack of tools to analyze the overall class performance and identify struggling students.
This problem is worth solving because accurate and efficient grade management is essential for both the teachers and students. It allows the teachers to focus more on teaching and providing help to students who need it.
The problem directly affects how student grades are calculated, leading to errors and mistakes that could lead to inaccurate results that incorrectly reflects on a student's true performance.

---

## 🎯 Project Objectives  
- Objective 1: To analyze and summarize the data from the 'Student Grades' JSON Files.  
- Objective 2: To help users know different sets of data through the multi-branch selection structure.

---

## ⚙️ Planned Features  

- Feature 1: Compute the general average of one student.  
- Feature 2: List the subjects where the student scored 2.5 or better.
- Feature 3: List the subjects where the student scored 2.75 or worse.  
- Feature 4: List the students who have a substandard general average or worse.
- Feature 5: List the students who have qualified for a Director's List in their general average.

---

## ⌨️ Planned Inputs and Outputs  

- **Inputs**  
  - The user will choose between options on what they want to search. This is done through a multi-branch selection structure. The user shall choose between the following options, general average computation, scoring in subjects, and list of students based on general average. If "general average computation of one student" and "list the subjects where the student scored ___ or ____" are chosen by the user, it will then ask for the student's ID. If the user chooses a list of students, then it will get straight to the point and compute the general average of each student.

- **Outputs**  
  - The output would be the general average, list of subjects in which the grade fits a certain criteria, list of students who have a substandard general average or worse, or list of students who qualified for a Director's List. This highly depends though on what option the user chose.

---

## 🧠 Logic Plan
Describe your program’s logic:  

### Pseudocode  
    START

      LOAD JSON File
  
      INPUT x
  
      MATCH x
  
        CASE 1
  
          INPUT id
    
          FIND DICTIONARY
    
          DISPLAY DICTIONARY KEYS id, name, section
    
          CALCULATE AND DISPLAY AVERAGE OF subjects IN id
    
        CASE 2
  
          INPUT id
    
          FIND DICTIONARY
    
          DISPLAY DICTIONARY KEYS id, name, section
    
          DISPLAY ELEMENTS IN DICTIONARY KEY subjects <= 2.5
    
        CASE 3
  
          INPUT id
    
          FIND DICTIONARY
    
          DISPLAY DICTIONARY KEYS id, name, section
    
          DISPLAY ELEMENTS IN DICTIONARY KEY subjects >= 2.75
    
        CASE 4
  
          CALCULATE AVERAGE OF subjects IN ALL DICTIONARIES
    
          DISPLAY ALL DICTIONARY KEYS students IF
    
            ALL DICTIONARY KEYS subjects AVERAGE >= 2.75
      
        CASE 5
  
          CALCULATE AVERAGE OF subjects IN ALL DICTIONARIES
    
          DISPLAY ALL DICTIONARY KEYS students IF
    
            ALL DICTIONARY KEYS subjects AVERAGE <= 1.5
      
        CASE _
  
          DISPLAY "INVALID"
    
      REPEAT UNTIL USER EXITS PROGRAM
  
    END
  
### Flowchart  
Attach or draw a flowchart showing how the program will work.  

---

## 📂 GitHub Repository Link  
GitHub repository link:  
`https://github.com/JanAPandes/Final-Project-CS2`  

---
