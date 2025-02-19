## 1. Create a new collection named 'employees'

<code>db.createCollection('employees')</code>

![Create](https://i.postimg.cc/Cxd8pyyZ/Screenshot-2025-02-17-at-2-19-58-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/k5btDxgq/Screenshot-2025-02-17-at-2-20-23-pm.png)

## 3. Insert one record to collection

<code>db.employees.insertOne({"employee_name": "John Williams",
"phone_number": "+61 412 345 678",
"salary": 75000,
"join_date": "2020-02-10"})</code>

![Create](https://i.postimg.cc/k4PRSB28/Screenshot-2025-02-17-at-2-23-58-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/L5HqywB8/Screenshot-2025-02-17-at-2-24-23-pm.png)

## 5. Insert multiple records to collection

<code>db.employees.insertMany([ {
"employee_name": "Sophie Brown",
"phone_number": "+61 408 123 456",
"salary": 82000,
"join_date": "2019-11-20",
"address": "42 Darling Road, Melbourne, VIC 3000, Australia"
},
{
"employee_name": "Liam Davis",
"phone_number": "+61 491 234 567",
"salary": 95000,
"join_date": "2021-06-15",
"address": "9 Queen Street, Brisbane, QLD 4000, Australia"
},
{
"employee_name": "Olivia Harris",
"phone_number": "+61 421 567 890",
"salary": 88000,
"join_date": "2018-07-05",
"address": "78 Murray Street, Perth, WA 6000, Australia"
},])</code>

![Create](https://i.postimg.cc/CMNnZMSB/Screenshot-2025-02-17-at-2-32-39-pm.png)

## 6. Find customers whose address is Perth

<code>db.employees.find({address : /Perth/i})</code>

<!-- ![Read](https://i.postimg.cc/FsHd0tHP/Screenshot-2025-02-17-at-2-46-02-pm.png)

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
