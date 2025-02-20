## 1. Create a new collection named 'suppliers'

<code>db.createCollection('suppliers')</code>

![Create](https://i.postimg.cc/0ykPH1hh/Screenshot-2025-02-20-at-1-11-51-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/zfMNBb31/Screenshot-2025-02-20-at-1-12-07-pm.png)

## 3. Insert one record to collection

<code>db.suppliers.insertOne({"supplier_name": "Aussie Produce Supplies",
"email": "contact@aussieproduce.com.au",
"phone": "+61 2 9123 4567",
"address": "123 Green Valley Rd, Sydney, NSW 2000"})</code>

![Create](https://i.postimg.cc/Y0Bw651n/Screenshot-2025-02-20-at-1-12-48-pm.png)

## 4. Read all available records in document

<code>db.customers.find()</code>

![Read](https://i.postimg.cc/SxJtKZ9J/Screenshot-2025-02-20-at-1-13-09-pm.png)

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

![Create](https://i.postimg.cc/PJXSnKhf/Screenshot-2025-02-20-at-1-14-03-pm.png)

## 6. Find suppliers whose supply product are eggs

<code>db.suppliers.find({supply_product: /eggs/i})</code>

![Read](https://i.postimg.cc/44P8QCbY/Screenshot-2025-02-20-at-1-16-02-pm.png)

## 7. Update a record with name 'Aussie Produce Supplies' and add supply_product field to record.

<code>db.suppliers.updateOne({supplier_name:'Aussie Produce Supplies'},{$set:{"supply_product": ["Fresh Vegetables", "Fruits", "Herbs"]}})</code>

![Update](https://i.postimg.cc/7YQmjgRD/Screenshot-2025-02-20-at-1-17-20-pm.png)

## 8. Find supplier with name 'Aussie Produce Supplies'

<code>db.suppliers.findOne({supplier_name:'Aussie Produce Supplies'})</code>

![Read](https://i.postimg.cc/1zDBgb35/Screenshot-2025-02-20-at-1-19-24-pm.png)

## 9. Delete record with a specific key

<code>db.suppliers.deleteOne({name:'Aussie Produce Supplies'})</code>

![Delete](https://i.postimg.cc/ZRcLH3NG/Screenshot-2025-02-20-at-1-20-15-pm.png)

## 10. Insert one record to collection

<code>db.suppliers.insertOne({ "supplier_name": "Down Under Grocery Wholesale",
"email": "wholesale@downundergrocery.com.au",
"phone": "+61 4 5678 1234",
"address": "101 Central Blvd, Adelaide, SA 5000",
"supply_product": ["Canned Goods", "Spices", "Beverages"]})
</code>

![Create](https://i.postimg.cc/jdCh6DS1/Screenshot-2025-02-20-at-1-20-43-pm.png)
