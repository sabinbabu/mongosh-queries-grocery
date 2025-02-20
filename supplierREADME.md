## 1. Create a new collection named 'suppliers'

<code>db.createCollection('suppliers')</code>

![Create](https://i.postimg.cc/Cxd8pyyZ/Screenshot-2025-02-17-at-2-19-58-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/k5btDxgq/Screenshot-2025-02-17-at-2-20-23-pm.png)

## 3. Insert one record to collection

<code>db.suppliers.insertOne({"supplier_name": "Aussie Produce Supplies",
"email": "contact@aussieproduce.com.au",
"phone": "+61 2 9123 4567",
"address": "123 Green Valley Rd, Sydney, NSW 2000"})</code>

![Create](https://i.postimg.cc/k4PRSB28/Screenshot-2025-02-17-at-2-23-58-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/L5HqywB8/Screenshot-2025-02-17-at-2-24-23-pm.png)

## 5. Insert multiple records to collection

<code>db.suppliers.insertMany([{
"supplier_name": "Outback Foods",
"email": "sales@outbackfoods.com.au",
"phone": "+61 3 9876 5432",
"address": "45 Bushland Ave, Melbourne, VIC 3000",
"supply_product": ["Organic Snacks", "Grains", "Dried Fruits"]
},
{
"supplier_name": "Coastal Seafoods",
"email": "info@coastalseafoods.com.au",
"phone": "+61 8 5647 2389",
"address": "78 Marine Drive, Perth, WA 6000",
"supply_product": ["Fresh Seafood", "Frozen Fish", "Seafood Sauces"]
},
{
"supplier_name": "Farm Fresh Foods",
"email": "orders@farmfresh.com.au",
"phone": "+61 7 3345 7788",
"address": "29 Country Lane, Brisbane, QLD 4000",
"supply_product": ["Dairy Products", "Eggs", "Fresh Meats"]
}])</code>

![Create](https://i.postimg.cc/CMNnZMSB/Screenshot-2025-02-17-at-2-32-39-pm.png)

## 6. Find suppliers whose supply product are eggs

<code>db.suppliers.find({supply_product: /eggs/i})</code>

![Read](https://i.postimg.cc/FsHd0tHP/Screenshot-2025-02-17-at-2-46-02-pm.png)

## 7. Update a record with name 'Aussie Produce Supplies' and add supply_product field to record.

<code>db.suppliers.updateOne({supplier_name:'Aussie Produce Supplies'},{$set:{"supply_product": ["Fresh Vegetables", "Fruits", "Herbs"]}})</code>

![Update](https://i.postimg.cc/13g8Yp6w/Screenshot-2025-02-17-at-2-47-58-pm.png)

## 8. Find supplier with name 'Aussie Produce Supplies'

<code>db.suppliers.findOne({supplier_name:'Aussie Produce Supplies'})</code>

<!-- ![Read](https://i.postimg.cc/HkfrGV4K/Screenshot-2025-02-17-at-2-49-04-pm.png)

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
