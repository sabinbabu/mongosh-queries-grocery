## 1. Create a new collection named 'department'

<code>db.createCollection('departments')</code>

![Create](https://i.postimg.cc/sXwpDdrG/Screenshot-2025-02-18-at-4-47-49-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/5yrLLBjx/Screenshot-2025-02-18-at-4-48-25-pm.png)

## 3. Insert one record to collection

<code>db.departments.insertOne({
"department_name": "Produce",
"manager_name": "Alice Johnson"
})</code>

![Create](https://i.postimg.cc/7Z00JT4k/Screenshot-2025-02-18-at-4-51-07-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/hGnxLP47/Screenshot-2025-02-18-at-4-51-17-pm.png)

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

![Create](https://i.postimg.cc/W4sFDWSG/Screenshot-2025-02-18-at-4-52-36-pm.png)

## 6. Find name of all departments as array

<code>db.departments.distinct("department_name")</code>

![Read](https://i.postimg.cc/mDDPjPvh/Screenshot-2025-02-18-at-4-54-23-pm.png)

## 7. Update a record with manager name 'Alice Johnson' and add manager_start_date field to record.

<code>db.departments.updateOne({manager_name:'Alice Johnson'},{$set:{ "manager_start_date": "2022-03-15"}})</code>

![Update](https://i.postimg.cc/dDMDJ4LT/Screenshot-2025-02-18-at-4-57-00-pm.png)

## 8. Find department with name 'Alice Johnson'

<code>db.departments.find({manager_name:'Alice Johnson'})
</code>

![Read](https://i.postimg.cc/SQHGX49c/Screenshot-2025-02-18-at-4-57-34-pm.png)

## 9. Delete record with a specific key

<code>db.departments.deleteOne({department_name:'Meat'})</code>

![Delete](https://i.postimg.cc/kgvNhtpy/Screenshot-2025-02-18-at-5-00-09-pm.png)

## 10. Insert one record to collection

<code>db.departments.insertOne({"department_name": "Frozen Foods",
"manager_name": "Emily Clark",
"manager_start_date": "2023-01-20"
})</code>

![Create](https://i.postimg.cc/6qZnV7Zn/Screenshot-2025-02-18-at-5-00-51-pm.png)
