
# Question_5

Creating a simple website which allow users
to register or login.when user clicks on login,he should enter his credentials and validating it with existing UserID, Password. If successful,a new webpage pops out and displays, “Welcome To IIT Indore” 
along with all the courses available for a BTech,





## Installation

1.Clone the repository 

```bash
git clone https://github.com/VIKAS-047/a7_question_5.git
```

```bash
cd a7_question_5
```
2.Install Required Python Libraries

```bash
pip install Flask
```

```bash
pip install mysql-connector-python
```

3.Setting Up MySQL Database

```bask
CREATE DATABASE user_management;

USE user_management;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_id VARCHAR(50) NOT NULL,
    mobile_number VARCHAR(15) NOT NULL,
    password VARCHAR(255) NOT NULL
);

CREATE TABLE courses (
    course_name VARCHAR(100) NOT NULL PRIMARY KEY
);

INSERT INTO courses (course_name)
VALUES 
    ('Computer Science and Engineering'),
    ('Chemical Engineering'),
    ('Civil Engineering'),
    ('Electrical Engineering'),
    ('Engineering Physics'),
    ('Mechanical Engineering'),
    ('Mathematics and Computing'),
    ('Metallurgy'),
    ('Space Sciences and Engineering');

```

4.Update Database Credentials

```bash
import mysql.connector

db = mysql.connector.connect(
    host="localhost",
    user="your_mysql_username",
    password="your_mysql_password",
    database="user_registration"
)
```


## Running Tests

To run tests, run the following command

```bash
  python app.py
```


## Screenshots

![Screenshot (121)](https://github.com/user-attachments/assets/9e690408-b96d-4f5e-bca7-d716ee423c1e)

![Screenshot (122)](https://github.com/user-attachments/assets/cb239732-b142-40ff-99c9-0247a5c822c8)

![Screenshot (126)](https://github.com/user-attachments/assets/aa6c9486-c234-459b-a081-9746d3035631)


