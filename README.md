[queries.sql.txt](https://github.com/user-attachments/files/17049227/queries.sql.txt)![photo_2024![photo_2024-09-18_18-26-47](https://github.com/user-attachments/assets/74a4cce3-022d-4b45-add0-0a8ff58cd0b7)
-09-18_21-16-21](https://github.com/user-attachments/assets/34f00643-a423-464f-921d-0e1dbf9e8217)
![photo_2024-09-18_18-27-01](https://github.com/user-attachments/assets/ba53160a-9998-4a9a-abc6-c6635f1caaec)
![photo_2024-09-18_18-27-12](https://github.com/user-attachments/assets/1782e324-7839-4b44-a837-12619f3a1706)

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

