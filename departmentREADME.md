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

![Create](https://i.postimg.cc/k4PRSB28/Screenshot-2025-02-17-at-2-23-58-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/L5HqywB8/Screenshot-2025-02-17-at-2-24-23-pm.png)

## 5. Insert multiple records to collection

<code>db.departments.insertMany([ {
"department_name": "Deli",
"manager_name": "Mark Smith",
"manager_start_date": "2020-08-01"
},
{
"department_name": "Bakery",
"manager_name": "Sarah Lee",
"manager_start_date": "2021-06-10"
},
{
"department_name": "Meat",
"manager_name": "John Davis",
"manager_start_date": "2019-11-05"
}])</code>

![Create](https://i.postimg.cc/CMNnZMSB/Screenshot-2025-02-17-at-2-32-39-pm.png)

## 6. Find name of all departments as array

<code>db.departments.distinct("department_name")</code>

![Read](https://i.postimg.cc/FsHd0tHP/Screenshot-2025-02-17-at-2-46-02-pm.png)

## 7. Update a record with manager name 'Alice Johnson' and add manager_start_date field to record.

<code>db.departments.updateOne({manager_name:'Alice Johnson'},{$set:{ "manager_start_date": "2022-03-15"}})</code>

![Update](https://i.postimg.cc/13g8Yp6w/Screenshot-2025-02-17-at-2-47-58-pm.png)

## 8. Find department with name 'Alice Johnson'

<code>db.departments.find({manager_name:'Alice Johnson'})
</code>

![Read](https://i.postimg.cc/HkfrGV4K/Screenshot-2025-02-17-at-2-49-04-pm.png)

## 10. Delete record with a specific key

<code>db.departments.deleteOne({department_name:'Meat'})</code>

![Delete](https://i.postimg.cc/d0kGdb4M/Screenshot-2025-02-17-at-2-50-58-pm.png)

## 11. Insert one record to collection

<code>db.customers.insertOne({
"name": "Ava Davis",
"phone": "+61 419 654 987",
"money_spent": 560.60,
"address": "876 Perth Lane, Perth, WA 6000",
"join_date": "2024-01-10"
})</code>

![Create](https://i.postimg.cc/y8rFD1hX/Screenshot-2025-02-17-at-2-51-46-pm.png)
