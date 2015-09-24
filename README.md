# Assignment
Given a small online store where a user can buy products for events. An event can have many products. Given an event, the user can buy any number of products in the store. When buying a product, a service fee is to be added to the total. Service fees can be configured on both event and product level. When no override is present for a product, the event fee applies.

Constraints:
- Events and products should at least have a 'name' property.
- A service fee consists of a currency and an amount.
- For simplicity, assume products themselves cost nothing.

Tasks:
- Design a small system that expresses these events, products and service fees in a database. Please provide the SQL schema for the database tables.
- Then, write an application that calculates the total service fee given an event and a list of products and quantities. A command line interface to the program is sufficient. The application should be written in Python.


# Usage

  - Clone the repository using ssh:

```sh
$ git clone git@github.com:BakanovKirill/Assignment.git
$ cd Assignment/
```
  - Deploy the project using buildout:

```sh
$ python bootstrap-buildout.py && bin/buildout
```
  - Load some test data into the Sqlite database. Test 

```sh
$ bin/django loaddata users.json
$ bin/django loaddata data.json
```
  - Run the project
```sh
$ bin/django runserver
```
  - Open the project in browser on **http://127.0.0.1:8000/**.
  - Access Django admin to view data **http://127.0.0.1:8000/admin**. 
  - Login: **tester** Password: **123456**

To test the project you can also run

```sh
$ bin/django test assignment
```
