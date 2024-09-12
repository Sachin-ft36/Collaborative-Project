# Collaborative-Project
Reebok Style Product Grid Layout
This project replicates the grid-style product layout similar to the Reebok website, featuring products with images, titles, pricing, and a "favorite" button in the top-right corner. It also includes a badge ("I AM THE NEW") in the top-left corner of each product.

Features
Responsive product grid layout
Image display for each product
Customizable title, price, and product category
Favorite icon toggle on the top-right
Labeling of new products with a custom badge
Preview

Technologies Used
HTML5: Structure of the page.
CSS3: Styling of the product grid and responsiveness.
FontAwesome: For icons such as the favorite heart.
Flexbox: For product grid layout.
Folder Structure
markdown
root
│   README.md
│   index.html
│   style.css
│
└─── assets
    │   product-image1.jpg
    │   product-image2.jpg
    │   product-image3.jpg
    │   product-image4.jpg
    │   v-hicon-similar.svg
Installation
Clone the repository:
bash
git clone https://github.com/your-username/reebok-product-layout.git
Navigate into the project folder:
bash
Copy code
cd reebok-product-layout
Open index.html in your preferred browser.
HTML Structure
html

<div class="container">
    <img src="path-to-product-image" alt="Product Name">
    <div class="top-left">I AM THE NEW</div>
    <span class="top-right"><i class="fa-regular fa-heart"></i></span>
    <div class="description">
        <p><span>PRODUCT CATEGORY</span></p>
        <img class="small-icon-description" src="v-hicon-similar.svg" alt="">
        <h3>Product Name</h3>
        <p>Price</p>
    </div>
</div>
container: The main wrapper for each product.
top-left: Badge that displays on the top-left corner to label new products.
top-right: Favorite heart icon positioned in the top-right corner.
description: Contains the product category, name, and price.
small-icon-description: Icon that appears inside the description box.
CSS Styling
css
.container {
    position: relative;
    text-align: center;
    width: 300px;
    border: 1px solid #ddd;
    border-radius: 10px;
    overflow: hidden;
    background-color: #fff;
    transition: transform 0.3s ease;
}

.container img {
    width: 100%;
    height: auto;
}

.top-left {
    position: absolute;
    top: 8px;
    left: 10px;
    font-size: 13px;
    background-color: rgb(44, 153, 153);
    padding: 5px 8px;
    border-radius: 4px;
    color: white;
}

.top-right {
    position: absolute;
    top: 8px;
    right: 10px;
    color: black;
}

.top-right i {
    font-size: 20px;
    color: red;
    cursor: pointer;
}

.description {
    padding: 15px;
    text-align: left;
    position: relative;
}

.small-icon-description {
    position: absolute;
    top: 0;
    right: 0;
    width: 16%;
    height: auto;
}

.description h3 {
    font-weight: bold;
    font-size: 16px;
    color: black;
    margin: 5px 0;
}

.description p {
    font-weight: bold;
    font-size: 14px;
    color: black;
}
How to Use
Replace the product images with your own by updating the src attribute in the img tags.
Modify the product name, category, and price inside the description div.
You can adjust the size and styling by modifying the CSS file.
FontAwesome Integration
The heart icon uses FontAwesome. Add the following <link> in your <head> section of index.html to include FontAwesome:

html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
Contribution
Feel free to fork the repository, make updates, and submit a pull request.
