# Sales Management System using Python and SQLite
A sales management system using Python to provide user interface and SQLite to manage data, developed for the course CT60A4304 Basics of database systems of LUT University, Finland.<br>
It enables users to efficiently track relations between orders, items and customers. Important information includes items, customers, and shipments. The database also stores information on customers’ delivery address and contact details. If a new customer is ordering a product, the customer’s information (name, age, address, phone number and email) is entered into the database. Then the customer could choose to order a variety of items and the order is finalized by recording the details of the order to a join table. In case the items requested are not available, then they should be added to the database.<br>
Possible database users: Sales employee, managers, delivery/postal services. Sales employees enter the information mentioned above to the database. Managers check the information and make necessary changes. Postmen or couriers could see the contact details and address, but could not add, delete or change any data. Some queries are implemented as follow:
- Select a table and view all the information stored in it
- Select a table and insert a new row
- Select a table and delete a row
- Select a table and update a row
- Create a chart displaying number of times each item was ordered
- List all items each customer has ordered
## Modeling
Concept model:<br>
![image](https://user-images.githubusercontent.com/68151686/203984591-6582a40e-f357-4ccc-8330-69b5fbc5ef1e.png)<br>
Relational model:<br>
![image](https://user-images.githubusercontent.com/68151686/203984700-e8b14f27-e76b-4fae-9e71-5228b3da8df2.png)

## Example
```
+----------------------------------------------+--------+
|                    Option                    | Number |
+----------------------------------------------+--------+
|                  View Table                  |   1    |
|                  Insert Row                  |   2    |
|                  Delete Row                  |   3    |
|                  Update Row                  |   4    |
| Chart: Number of times each item was ordered |   5    |
|     List items each customer has ordered     |   6    |
|                     Quit                     |   7    |
+----------------------------------------------+--------+
Select option: 1
+----------+--------+
|  Option  | Number |
+----------+--------+
| Customer |   1    |
| Address  |   2    |
| Country  |   3    |
| Contact  |   4    |
| Shipment |   5    |
|   Item   |   6    |
+----------+--------+
Select table to view: 1
+------------+----------------------+-----+
| CustomerID |         Name         | Age |
+------------+----------------------+-----+
|   10001    |    Tomasz Gorczyca   |  23 |
|   10002    |    Leon Kulikowski   |  36 |
|   10003    |      Artur Nowak     |  32 |
|   10004    |     Iwa Cegielska    |  28 |
|   10005    |   Adriana Polkowska  |  31 |
|   10006    |  Patrycja Ptaszynska |  29 |
+------------+----------------------+-----+

Press ENTER to return to main menu...
```
