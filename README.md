# Assignment
Given a small online store where a user can buy products for events. An event can have many products. Given an event, the user can buy any number of products in the store. When buying a product, a service fee is to be added to the total. Service fees can be configured on both event and product level. When no override is present for a product, the event fee applies.

Constraints:
- Events and products should at least have a 'name' property.
- A service fee consists of a currency and an amount.
- For simplicity, assume products themselves cost nothing.

Tasks:
- Design a small system that expresses these events, products and service fees in a database. Please provide the SQL schema for the database tables.
- Then, write an application that calculates the total service fee given an event and a list of products and quantities. A command line interface to the program is sufficient. The application should be written in Python.
