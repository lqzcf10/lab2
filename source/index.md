Lab3 Report
================================

Title:  Lab3 The Service Layer

Author: 黄文心、朱彩凤、朱倩

Date: 2021/6/17

Introduction
==================

In this experiment , you are going to implement a service layer in services.py for EnglishPal, which provides a core service called read. This service would choose a suitable article for a user to read.and Practice Test-driven development 

# Materials and Methods

In this lab, we study the dependency inversion ,High level module should not rely on low level module, both of them should rely on its abstraction; Abstraction should not rely on details; Details should rely on abstraction.

With object-relational mapper (ORM) provided by SQLAlchemy, we can map a class to a database table, and map an object of that class to a row in the databasetable and o create four database tables for EnglishPal. With SQLAlchemy’s ORM, we can avoid directly using any raw SQL statements,let ORM depend on the domain model,but not the other way around.

Use FOREIGN KEY  to understand the relationship between two tables. 

On the basis of Experiment 2,implement a service layer in services.py for EnglishPal, which provides a core service called read, The function read takes user,user repo,article repo,session four arguments and returns an article ID if the user has been successfully assigned with an article to read.

By running pytest -v -s test services.py  command  make all the fifive test cases defifined in test services.py.Pytest is a very mature full-function Python testing framework, which has the following characteristics:Simple and flexible, easy to start,Support parameterization.It can support simple unit test and complex function test, and can also be used for automatic testing such as selenium/appium, and pytest + request Pytest has many third-party plug-ins, and can be customized for extension. It is better to use, such as pytest selenium (integrated selenium), pytest HTML (perfect HTML test report generation), pytest rerun failures (repeated execution of failure cases), pytest xdist (multi CPU distribution), etc
Skip and xfail processing of test cases.It's good to integrate with Jenkins
Report framework - allow also supports pytest.

# Results

The running results are in the file.

# Pros&Cons

- Pros:This project framework is clearly structured,code easy to analyze and maintain and improves functions properly
- Cons:Basic functions are fully determined, with low room for further innovation and many places hava to be improved



# Discussions

Use Sqlalchemy's ORM as a web application to improve learners' vocabulary. The abstraction of code does not depend on the type of database and the uniqueness of database itself. It provides powerful general statements and types. It doesn't need to consider the database you choose and its manufacturer's implementation. Sqlalchemy also allows you to transfer data logic from Oracle or PostgreSQL to the application's database. It standardizes and escapes the database before submitting operations to it. This avoids some common problems, such as database injection attacks.

Try running cases again
When we do interface testing, we will encounter 503 or short-term network fluctuations, which will lead to the failure of case operation, which is not the expected result. At this time, we can solve it by retrying to run cases.
Install pytest rerun failures:
pip install -U pytest-rerunfailures
Operation mode:
pytest test_ se.py --reruns NUM
Num fills in the number of retries.



# References

[1] [A Brief Guide How to Write a Computer Science Lab Report](https://thehackpost.com/a-brief-guide-how-to-write-a-computer-science-lab-report.html)

[2] [Read the Docs](https://readthedocs.org/ )`[]()