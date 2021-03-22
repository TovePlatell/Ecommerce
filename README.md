# Ecommerce
API


DROP DATABASE IF EXISTS Ecommerce; CREATE DATABASE Ecommerce;
DROP TABLE IF EXISTS cart; DROP DATABASE IF EXISTS products; DROP DATABASE IF EXISTS users;
CREATE TABLE users(user_id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, user_name VARCHAR(50) NOT NULL, user_password VARCHAR(50) NOT NULL, user_email VARCHAR(100)) ENGINE = INNODB; CREATE TABLE products(product_id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, product_name VARCHAR(50) NOT NULL, product_desc VARCHAR(500) NOT NULL, price INT) ENGINE = INNODB; CREATE TABLE cart(cart_id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, product_id INT NOT NULL, CONSTRAINT FKproductsId FOREIGN KEY(product_id) REFERENCES products(product_id)) ENGINE = INNODB;
![image](https://user-images.githubusercontent.com/72736333/112003513-4142a380-8b21-11eb-85ad-ecae46c58468.png)
