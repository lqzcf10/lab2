Lab2 Report
================================

Title:  Lab2 The ORM Magic

Author: 黄文心、朱彩凤、朱倩

Date: 2021/6/3

Inroduction
==================

In this experiment, we do dependency inversion and Manipulate database with SQLAlchemy’s ORM to create four database tables for EnglishPal, a web application for boosting the learner’s vocabulary.

# Materials and Methods

In this lab, we study the dependency inversion ,High level module should not rely on low level module, both of them should rely on its abstraction; Abstraction should not rely on details; Details should rely on abstraction.

Abstractions should not depend on details, details should depend on abstractions. In other words, programming for the interface, not for the implementation.

With object-relational mapper (ORM) provided by SQLAlchemy, we can map a class to a database table, and map an object of that class to a row in the databasetable and o create four database tables for EnglishPal. With SQLAlchemy’s ORM, we can avoid directly using any raw SQL statements,let ORM depend on the domain model,but not the other way around.

Use FOREIGN KEY  to understand the relationship between two tables. 

# Results

code:The modified model.docx

# Pros&Cons

- Pros:This project framework is clearly structured,code easy to analyze and maintain and improves functions properly
- Cons:Basic functions are fully determined, with low room for further innovation and many places hava to be improved



# Discussions

Use Sqlalchemy's ORM as a web application to improve learners' vocabulary. The abstraction of code does not depend on the type of database and the uniqueness of database itself. It provides powerful general statements and types. It doesn't need to consider the database you choose and its manufacturer's implementation. Sqlalchemy also allows you to transfer data logic from Oracle or PostgreSQL to the application's database. It standardizes and escapes the database before submitting operations to it. This avoids some common problems, such as database injection attacks.

There are three ways to transfer dependencies: interface transfer, construction method transfer and setter method transfer.
In the actual programming, we generally need to do the following three points:
(1) Low level modules should have abstract classes or interfaces, or both.
(2) The declaration type of variable should be abstract class or interface.
(3) The use of inheritance follows the Riemannian substitution principle.
The core of the dependency inversion principle is to program for interfaces.

# References

[1] [A Brief Guide How to Write a Computer Science Lab Report](https://thehackpost.com/a-brief-guide-how-to-write-a-computer-science-lab-report.html)

[2] [Read the Docs](https://readthedocs.org/ )`[]()