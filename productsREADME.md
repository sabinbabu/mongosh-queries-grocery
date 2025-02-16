<code>db.createCollection('products')</code>

<code>show collections</code>

<code>db.products.find()</code>

<code>db.products.insertMany([{name:'Lindt Lindor Assorted Chocolate Box',price:13.00,quantity:10},{name:'Magnum Mini Classic Frozen Dessert Sticks 6 Pack',price:6.00,quantity:20}])</code>

<code>db.products.distinct('name')</code>

<code>db.products.updateOne({name:'Cavendish Banana'},{$set:{price:6.00,quantity:30}})</code>
