# FA 5 UPDATED FLOWCHART AND PSEUDOCODE

---

## Pseudocode
    START
    LOAD students.json
    CONNECT TO Firebase

    WHILE True:

        DISPLAY:

        '''
        ===== STUDENT DATABASE MENU =====
        1. Display Students
        2. Add Student
        3. Update Student
        4. Delete Student
        5. Features
        6. Exit
        '''

        INPUT choice

        IF choice == "1":
            DISPLAY "Student List:"
            DISPLAY DATA

        ELIF choice == "2":
            INPUT id

            IF id already exists:
                DISPLAY "Student already exists!"
                CONTINUE

            INPUT name
            INPUT section
            INPUT math2
            INPUT math3
            INPUT bio
            INPUT chem
            INPUT physics
            INPUT cs
            INPUT pehm
            INPUT ve
            INPUT ss
            INPUT eng
            INPUT fili

            SET INPUT
            DISPLAY "Student added successfully!"

        ELIF choice == "3":
            INPUT id

            IF id does not exist:
                DISPLAY "Student does not exist!"
                CONTINUE

            INPUT name
            INPUT section
            INPUT math2
            INPUT math3
            INPUT bio
            INPUT chem
            INPUT physics
            INPUT cs
            INPUT pehm
            INPUT ve
            INPUT ss
            INPUT eng
            INPUT fili

            UPDATE DATA
            DISPLAY "Student updated successfully!"

            IF item is None:
                DISPLAY "Student not found."

        ELIF choice == "4":
            INPUT id

            IF id does not exist:
                DISPLAY "Student does not exist!"
                CONTINUE

            DELETE INFO MATCHING id
            DISPLAY "Student deleted successfully!"

        ELIF choice == "5":

            WHILE True:

                DISPLAY:

                '''
                ===== STUDENT DATABASE FEATURES =====
                1. Compute the General Average of One Student.
                2. List the Subjects Where the Student Scored 2.5 or Better.
                3. List the Subjects Where the Student Scored 2.75 or Worse.
                4. List the Students Who Have a Substandard General Average or Worse.
                5. List the Students Who Have Qualified for a Director's List in Their General Average.
                6. Back to Main Menu.
                '''

                INPUT choice

                MATCH choice:

                    CASE "1":
                        INPUT id

                        IF id does not exist:
                            DISPLAY "Student not found."
                            CONTINUE

                        CALCULATE SUM OF GRADES
                        CALCULATE COUNT
                        CALCULATE AVG

                        DISPLAY f"The general average of {NAME} is {AVG:.2f}!"

                    CASE "2":
                        INPUT id

                        IF id does not exist:
                            DISPLAY "Student not found."
                            CONTINUE

                        DISPLAY SUBJECTS WHERE grade <= 2.5

                    CASE "3":
                        INPUT id

                        IF id does not exist:
                            DISPLAY "Student not found."
                            CONTINUE

                        DISPLAY SUBJECTS WHERE grade >= 2.75

                    CASE "4":
                        CALCULATE SUM OF GRADES
                        CALCULATE COUNT
                        CALCULATE AVG

                        DISPLAY STUDENTS WHERE AVG >= 2.75

                    CASE "5":
                        CALCULATE SUM OF GRADES
                        CALCULATE COUNT
                        CALCULATE AVG

                        DISPLAY STUDENTS WHERE AVG <= 1.5

                    CASE "6":
                        BREAK

        ELIF choice == "6":
            DISPLAY "Exiting Program..."
            BREAK

    END

## Flowchart
![image alt](https://github.com/JanAPandes/Final-Project-CS2/blob/eac75060ae16df20401e0f782b58caf2ccaba11c/Project_Template_ComputerScience2-main/docs/CS%20FA%205%20FLOWCHART.png)
