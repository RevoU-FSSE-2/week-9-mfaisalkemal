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
