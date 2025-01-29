# -Product-Schema-Model-
const mongoose = require('mongoose');

// Define Product Schema
const ProductSchema = new mongoose.Schema({
    title: { type: String, required: true },
    price: { type: Number, required: true },
    category: { type: String, required: true },
    inStock: { type: Boolean, default: true }
});

// Create and Export Product Model
const Product = mongoose.model('Product', ProductSchema);
module.exports = Product;

npm install mongoose
const Product = require('./models/Product');
git init
git add .
git commit -m "Add Product schema and model"
git push -u origin master
