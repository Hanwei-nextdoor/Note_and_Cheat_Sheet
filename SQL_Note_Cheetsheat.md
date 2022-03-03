#NOTE AND CHEATSHEET: SQL

THIS IS A CHEATSHEET/NOTE TO THE ONE OF THE MOST POWERFUL TOOL FOR DATA ANALYSING. This document will help you understand Basic SQL language.

## 1. WHAT IS SQL?

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

Create a Database:

CREATE DATABASE IF NOT EXISTS 資料庫名稱 
COLLATE 編碼;

  CREATE DATABASE IF NOT EXISTS demo_shop 
  COLLATE utf8mb4_unicode_ci;


Create a Table: CREATE TABLE

CREATE TABLE 
