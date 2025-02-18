## 1. Create a new collection named 'department'

<code>db.createCollection('departments')</code>

![Create](https://i.postimg.cc/Cxd8pyyZ/Screenshot-2025-02-17-at-2-19-58-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/k5btDxgq/Screenshot-2025-02-17-at-2-20-23-pm.png)

## 3. Insert one record to collection

<code>db.departments.insertOne({
"department_name": "Produce",
"manager_name": "Alice Johnson"
})</code>

<!-- ![Create](https://i.postimg.cc/k4PRSB28/Screenshot-2025-02-17-at-2-23-58-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/L5HqywB8/Screenshot-2025-02-17-at-2-24-23-pm.png)

## 5. Insert multiple records to collection

<code>db.customers.insertMany([ {
"name": "Liam Williams",
"phone": "+61 418 654 321",
"money_spent": 220.50,
"address": "789 Melbourne Street, Melbourne, VIC 3000",
"join_date": "2022-10-05"
},
{
"name": "Olivia Brown",
"phone": "+61 407 987 654",
"money_spent": 415.90,
"address": "456 Adelaide Avenue, Adelaide, SA 5000",
"join_date": "2021-12-01"
},
{
"name": "Ethan Smith",
"phone": "+61 413 123 789",
"money_spent": 128.30,
"address": "321 Brisbane Drive, Brisbane, QLD 4000",
"join_date": "2020-04-25"
}])</code>

![Create](https://i.postimg.cc/CMNnZMSB/Screenshot-2025-02-17-at-2-32-39-pm.png)

## 6. Find customers whose address is Sydney

<code>db.customers.find({"address": /Sydney/i})</code>

![Read](https://i.postimg.cc/FsHd0tHP/Screenshot-2025-02-17-at-2-46-02-pm.png)

## 7. Update a record with name 'Emily Johnson' and add join_date field to record.

<code>db.customers.updateOne({name:'Emily Johnson'},{$set:{"join_date": "2023-08-15"}})</code>

![Update](https://i.postimg.cc/13g8Yp6w/Screenshot-2025-02-17-at-2-47-58-pm.png)

## 8. Find customer with name 'Emily Johnson'

<code>db.customers.findOne(name:'Emily Johnson')</code>

![Read](https://i.postimg.cc/HkfrGV4K/Screenshot-2025-02-17-at-2-49-04-pm.png)

## 9. Find customers with money_spent greater than 300.

<code>db.customers.find({money_spent:{$gt:300.00}})</code>

![Read](https://i.postimg.cc/xdMc9n6d/Screenshot-2025-02-17-at-2-50-03-pm.png)

## 10. Delete record with a specific key

<code>db.customers.deleteOne({name:'Olivia Brown'})</code>

![Delete](https://i.postimg.cc/d0kGdb4M/Screenshot-2025-02-17-at-2-50-58-pm.png)

## 11. Insert one record to collection

<code>db.customers.insertOne({
"name": "Ava Davis",
"phone": "+61 419 654 987",
"money_spent": 560.60,
"address": "876 Perth Lane, Perth, WA 6000",
"join_date": "2024-01-10"
})</code>

![Create](https://i.postimg.cc/y8rFD1hX/Screenshot-2025-02-17-at-2-51-46-pm.png) -->
