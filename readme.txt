Finding documents
We can find all our documents (Products) with a command like below.

1
Product.find({})
Find a document based on id

1
Product.findOne({ _id: <id> })
Updating
Update a single document

1
Product.updateOne({ name: 'Soda' }, { brand: 'newBrand' });
Update multiple documents

1
Product.updateMany({ brand: 'demoBrand' }, { quantity: 500 });
Delete Documents
Delete a single document

1
Product.deleteOne({ name: 'Soda' });
Delete multiple documents

1
Product.deleteMany({ quantity: { $gte: 100 } });