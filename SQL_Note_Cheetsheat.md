#NOTE AND CHEATSHEET: SQL

THIS IS A CHEATSHEET/NOTE TO THE ONE OF THE MOST POWERFUL TOOL FOR DATA ANALYSING. This document will help you understand Basic SQL language.

# 1. WHAT IS SQL?

Structured Query Language: A Relational Database Language

Principle:
1. space as splits, no capital/lower difference ; as an end
2. Markdown: -- for single, /* */ for multiple 
3. DATA DEFINITION LANGUAGE:(DFL)
    1. CREATE: create table/database
    2. DROP: delete table/database
    3. ALTER: change table/database
5. DATA MANIPULATION LANGUAGE:(DML)
    1. INSERT
    2. SELECT
    3. UPDATE
    4. DELETE
7. DATA CONTROL LANGUAGE (DCL)
8. DATA TYPE:
  1. INTEGER: integer
  2. TEXT:
    1. VARCHAR
  4. FLOAT/REAL

# 2. DATA DEFINITION LANGUAGE
## CREATE
### Create a Database: CREATE DATABASE

**CREATE DATABASE IF NOT EXISTS 資料庫名稱 
COLLATE 編碼;**

` CREATE DATABASE IF NOT EXISTS demo_shop 
  COLLATE utf8mb4_unicode_ci;`


### Create a Table: CREATE TABLE

**CREATE TABLE 資料表名稱   
(欄位名稱 欄位屬性);**

*id 為主鍵，資料不可重複，整數型別，非 NOT NULL 值（不允許空值）  
VARCHAR(長度) 為可變字串資料型別  
INT 為整數*

`CREATE TABLE users (
    id INT PRIMARY KEY NOT NULL UNIQUE,  
    username VARCHAR(12) NOT NULL,  
    age INT,  
    gender VARCHAR(6)  
);`

## DROP
**DROP DATABASE/TABLE 資料庫/資料表名稱;**

## ALTER
**ALTER TABLE 資料表名稱 ADD/DROP 欄位名稱;**

# 3. DATA MANIPULATION LANGUAGE

## INSERT

**INSERT INTO 資料表名稱 VALUES (欄位名稱)  
(欄位資料1, 欄位資料2);**

`INSERT INTO users (id, username, age, gender) VALUES`   
   `(1, 'Jack', 20, 'Male'),`  
   `(2, 'Amy', 33, 'Female'),`  
   `(3, 'Tony', 55, 'Male')`  
`;`

`INSERT INTO users VALUES`   
    `(1, 'Jack', 20, 'Male'),`  
    `(2, 'Amy', 33, 'Female'),` 
    `(3, 'Tony', 55, 'Male')`  
`;`
