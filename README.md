![photo_2024-09-18_21-16-21](https://github.com/user-attachments/assets/0365ac5c-7730-4d83-a7a8-d7db2ab63622)

![photo_2024-09-18_18-26-47](https://github.com/user-attachments/assets/c8cbe951-b5b9-40bb-bc38-419fd6679663)

![photo_2024-09-18_18-27-01](https://github.com/user-attachments/assets/dcad403d-20cd-4977-a744-e71cbd67bc26)

![photo_2024-09-18_18-27-12](https://github.com/user-attachments/assets/c6076ea4-8379-47b8-83f3-8a78cfd45b4f)


[Upl-- Создание базы данных
CREATE DATABASE sales_database;

-- Использование базы данных
USE sales_database;

-- Создание таблицы
CREATE TABLE sales (
    id INT AUTO_INCREMENT PRIMARY KEY,
    product VARCHAR(255),
    price DECIMAL(10, 2),
    quantity INT
);

-- Вставка данных
INSERT INTO sales (product, price, quantity) 
VALUES ('Laptop', 1000, 5),
       ('Phone', 700, 3),
       ('Tablet', 500, 2),
       ('Printer', 300, 4);
       
SELECT * FROM sales;

SELECT * FROM sales
LIMIT 2;

SELECT SUM(price * quantity) AS total_value
FROM sales;

SELECT product, SUM(quantity) AS total_quantity, AVG(price) AS average_price
FROM sales
GROUP BY product;oading queries.sql.txt…]()

