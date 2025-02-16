## 1. Create a new collection named 'products

<code>db.createCollection('products')</code>

## 2. Show list of available collections in database

<code>show collections</code>

## 3. Insert one record to collection

<code>db.products.insertOne({name:'Cavendish Banana'})</code>

## 4. Read all available records in document

<code>db.products.find()</code>

## 5. Insert multiple records to collection

<code>db.products.insertMany([{name:'Lindt Lindor Assorted Chocolate Box',price:13.00,quantity:10},{name:'Magnum Mini Classic Frozen Dessert Sticks 6 Pack',price:6.00,quantity:20}])</code>

## 6. Return array of keys from records with key 'name'

<code>db.products.distinct('name')</code>

## 7. Update a record with name 'Cavendish Banana', added price and quantity field to record.

<code>db.products.updateOne({name:'Cavendish Banana'},{$set:{price:6.00,quantity:30}})</code>

## 8. Find product with name 'Cavendish Banana'

<code>db.products.findOne({name:'Cavendish Banana'})</code>

## 9. Find products with quantity amount less than 5.

<code>db.products.find({quantity:{$lt:5}})</code>

## 10. Delete record with a specific key

<code>db.products.deleteOne({name:'Tamar Valley Dairy Kids Greek Yoghurt Pouch Vanilla'})</code>
