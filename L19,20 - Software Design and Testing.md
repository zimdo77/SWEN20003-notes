# Design principles
![Screenshot 2024-10-21 at 17.30.06](attachments/Screenshot%202024-10-21%20at%2017.30.06.png)
![Screenshot 2024-10-21 at 17.30.17](attachments/Screenshot%202024-10-21%20at%2017.30.17.png)
![Screenshot 2024-10-21 at 17.30.33](attachments/Screenshot%202024-10-21%20at%2017.30.33.png)
![Screenshot 2024-10-21 at 17.30.43](attachments/Screenshot%202024-10-21%20at%2017.30.43.png)![Screenshot 2024-10-21 at 17.30.58](attachments/Screenshot%202024-10-21%20at%2017.30.58.png)![Screenshot 2024-10-21 at 17.31.07](attachments/Screenshot%202024-10-21%20at%2017.31.07.png)
# Poor design symptoms
![Screenshot 2024-10-21 at 17.53.15](attachments/Screenshot%202024-10-21%20at%2017.53.15.png)
# Software testing (finding bugs)
Phases of software testing:
- **UNIT TESTING**: testing units/components independently before integrating (combining).
- **INTEGRATION AND SYSTEM TESTING**: integrating units to form the system and testing the system as a whole.
- **ACCEPTANCE TESTING**: validating if the system supports the functionality as per requirements (letting end-users test product and give feedback).
# Unit testing
![Screenshot 2024-10-21 at 18.02.41](attachments/Screenshot%202024-10-21%20at%2018.02.41.png)
NOTE: When generating test cases for a method, test the method for VALID and INVALID input.
# Creating units for unit testing
FROM:
![Screenshot 2024-10-21 at 19.00.50](attachments/Screenshot%202024-10-21%20at%2019.00.50.png)
TO:
![Screenshot 2024-10-21 at 19.01.16](attachments/Screenshot%202024-10-21%20at%2019.01.16.png)
This better abstracts the code, and makes for easier testing.
Now, all together:
![Screenshot 2024-10-21 at 19.02.17](attachments/Screenshot%202024-10-21%20at%2019.02.17.png)
# Unit testing in Java
![Screenshot 2024-10-21 at 19.03.04](attachments/Screenshot%202024-10-21%20at%2019.03.04.png)
# JUnit automated testing
![Screenshot 2024-10-22 at 15.35.14](attachments/Screenshot%202024-10-22%20at%2015.35.14.png)
# JUnit5 assertion methods
![Screenshot 2024-10-22 at 15.35.52](attachments/Screenshot%202024-10-22%20at%2015.35.52.png)
# JUnit5 tags
![Screenshot 2024-10-22 at 15.36.12](attachments/Screenshot%202024-10-22%20at%2015.36.12.png)
# TestCase Class
![Screenshot 2024-10-22 at 15.36.47](attachments/Screenshot%202024-10-22%20at%2015.36.47.png)
NOTE: There is a bug in the last test - the "r" needs to be an "R".
# JUnit advantages
![Screenshot 2024-10-22 at 15.42.49](attachments/Screenshot%202024-10-22%20at%2015.42.49.png)
# Examples
![Screenshot 2024-10-22 at 15.43.41](attachments/Screenshot%202024-10-22%20at%2015.43.41.png)
## Unit tests for `cellIsEmpty`
![Screenshot 2024-10-22 at 15.43.52](attachments/Screenshot%202024-10-22%20at%2015.43.52.png)
## Unit tests for `onBoard`
![Screenshot 2024-10-22 at 15.44.09](attachments/Screenshot%202024-10-22%20at%2015.44.09.png)
![Screenshot 2024-10-22 at 15.44.31](attachments/Screenshot%202024-10-22%20at%2015.44.31.png)
## Unit tests for `isValidMove`
![Screenshot 2024-10-22 at 15.44.55](attachments/Screenshot%202024-10-22%20at%2015.44.55.png)
![Screenshot 2024-10-22 at 15.45.04](attachments/Screenshot%202024-10-22%20at%2015.45.04.png)
## Unit tests for `attemptMove`
![Screenshot 2024-10-22 at 15.45.40](attachments/Screenshot%202024-10-22%20at%2015.45.40.png)
![Screenshot 2024-10-22 at 15.45.49](attachments/Screenshot%202024-10-22%20at%2015.45.49.png)
# What is examinable
![Screenshot 2024-10-22 at 13.20.35](attachments/Screenshot%202024-10-22%20at%2013.20.35.png)