# Intermediate Assignment Week 9 - Simple Rest API Connected to MySQL Database
https://calm-fish-underclothes.cyclic.cloud

## Technologies Used

- Node.js: A JavaScript runtime that allows executing code on the server side.
- Express.js: A popular web application framework for Node.js that simplifies building APIs and web applications.
- TypeScript: A superset of JavaScript that adds static typing for enhanced code quality and maintainability.
- MySQL: An open-source relational database management system.

## SQL Query To Create Tables
1. Table User

`
CREATE TABLE User (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50),
    address VARCHAR(150)
) ENGINE = InnoDB DEFAULT CHARSET = utf8mb4 COLLATE = utf8mb4_0900_ai_ci;
`

2. Table Transactions

`
CREATE TABLE Transactions (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_id INT,
    type VARCHAR(10),
    amount DOUBLE
) ENGINE = InnoDB DEFAULT CHARSET = utf8mb4 COLLATE = utf8mb4_0900_ai_ci;
`

  
[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Z42oEjTh)
## API Contract
1. **GET** /user/:id
   
   As example, if input id = 2
   ![image](https://github.com/RevoU-FSSE-2/week-9-mfaisalkemal/assets/130155172/62c73490-3d29-4da8-b37e-af0718eae054)
2. **POST** /transaction
   
   As example, if input POST request like below
   
   `
   {
    "type": "income",
    "amount": 70000,
    "user_id": 1
   }
   `
   
   will get response
   ![image](https://github.com/RevoU-FSSE-2/week-9-mfaisalkemal/assets/130155172/bc04f693-7ad2-4731-9cee-cf8ee1201a55)
3. **PUT** /transaction/:id
   
   As example, if input request for PUT transactions id = 1 like below
   
   `
   {
    "type": "income",
    "amount": 60000,
    "user_id": 1
   }
   `

   will get response
   ![image](https://github.com/RevoU-FSSE-2/week-9-mfaisalkemal/assets/130155172/5d1ab5cd-f21e-4cc5-b8c2-55ecb9ef9391)

4. **DELETE** /transaction/:id
   
   As example, if input request for DELETE transactions id = 1 will get response
   
   ![image](https://github.com/RevoU-FSSE-2/week-9-mfaisalkemal/assets/130155172/fb5cbe57-2d29-4e5a-968c-da65c7a616dc)
