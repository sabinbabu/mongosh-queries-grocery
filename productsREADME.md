## 1. Create a new collection named 'products;

<code>db.createCollection('products')</code>

![Create](https://i.postimg.cc/905jhgm5/Screenshot-2025-02-16-at-7-35-50-pm.png)

## 2. Show list of available collections in database

<code>show collections</code>

![Collections](https://i.postimg.cc/139sXdpy/Screenshot-2025-02-16-at-7-34-41-pm.png)

## 3. Insert one record to collection

<code>db.products.insertOne({name:'Cavendish Banana'})</code>

![Create](https://i.postimg.cc/6379wGCR/Screenshot-2025-02-16-at-7-33-49-pm.png)

## 4. Read all available records in document

<code>db.products.find()</code>

![Read](https://i.postimg.cc/W41NWy35/Screenshot-2025-02-16-at-7-32-44-pm.png)

## 5. Insert multiple records to collection

<code>db.products.insertMany([{name:'Lindt Lindor Assorted Chocolate Box',price:13.00,quantity:10},{name:'Magnum Mini Classic Frozen Dessert Sticks 6 Pack',price:6.00,quantity:20}])</code>

![Create](https://i.postimg.cc/MKB89SY6/Screenshot-2025-02-16-at-7-30-18-pm.png)

## 6. Return array of keys from records with key 'name'

<code>db.products.distinct('name')</code>

![Read](https://i.postimg.cc/5yYMdddm/Screenshot-2025-02-16-at-7-29-08-pm.png)

## 7. Update a record with name 'Cavendish Banana', added price and quantity field to record.

<code>db.products.updateOne({name:'Cavendish Banana'},{$set:{price:6.00,quantity:30}})</code>

![Update](https://i.postimg.cc/BZVqhN9g/Screenshot-2025-02-16-at-7-27-42-pm.png)

## 8. Find product with name 'Cavendish Banana'

<code>db.products.findOne({name:'Cavendish Banana'})</code>

![Read](https://i.postimg.cc/gJ40kP7F/Screenshot-2025-02-16-at-7-25-06-pm.png)

## 9. Find products with quantity amount less than 5.

<code>db.products.find({quantity:{$lt:5}})</code>

![Read](https://i.postimg.cc/cHcvg3rz/Screenshot-2025-02-16-at-7-22-42-pm.png)

## 10. Delete record with a specific key

<code>db.products.deleteOne({name:'Tamar Valley Dairy Kids Greek Yoghurt Pouch Vanilla'})</code>

![Delete](https://i.postimg.cc/HnB8KMmM/Screenshot-2025-02-16-at-7-20-24-pm.png)
