# Node.js-MySQL
Homework 10 - Bamazon

Overview

In this activity, you'll be creating an Amazon-like storefront with the MySQL skills you learned this week. The app will take in orders from customers and deplete stock from the store's inventory. 

Make sure you save and require the MySQL and Inquirer npm packages in your homework files--your app will need them for data input and storage.
Submission Guide

Make sure you use the normal GitHub. Because this is a CLI App, there will be no need to deploy it to Heroku. This time, though, you need to include screenshots, a gif, and/or a video showing us that you got the app working with no bugs. You can include these screenshots or a link to a video in a README.md file.
Include screenshots (or a video) of typical user flows through your application (for the customer and if relevant the manager/supervisor). This includes views of the prompts and the responses after their selection (for the different selection options).
Include any other screenshots you deem necessary to help someone who has never been introduced to your application understand the purpose and function of it. This is how you will communicate to potential employers/other developers in the future what you built and why, and to show how it works.
Because screenshots (and well-written READMEs) are extremely important in the context of GitHub, this will be part of the grading.
If you haven't written a markdown file yet, click here for a rundown, or just take a look at the raw file of these instructions.
Instructions

Challenge #1: Customer View (Minimum Requirement)

Create a MySQL Database called Bamazon.
Then create a Table inside of that database called products.
The products table should have each of the following columns:
item_id (unique id for each product)
product_name (Name of product)
department_name
price (cost to customer)
stock_quantity (how much of the product is available in stores)
Populate this database with around 10 different products. (i.e. Insert "mock" data rows into this database and table).
Then create a Node application called bamazonCustomer.js. Running this application will first display all of the items available for sale. Include the ids, names, and prices of products for sale.
The app should then prompt users with two messages.
The first should ask them the ID of the product they would like to buy.
The second message should ask how many units of the product they would like to buy.
Once the customer has placed the order, your application should check if your store has enough of the product to meet the customer's request.
If not, the app should log a phrase like Insufficient quantity!, and then prevent the order from going through.
However, if your store does have enough of the product, you should fulfill the customer's order.
This means updating the SQL database to reflect the remaining quantity.
Once the update goes through, show the customer the total cost of their purchase.
If this activity took you between 8-10 hours, then you've put enough time into this assignment. Feel free to stop here -- unless you want to take on the next challenge.


## Walkthrough

### Customer

1) Opening, running, and editing the app requires terminal, node, MySQL, inquirer and mysql npm. 

2) Enter in 'cd' + the folder location. Then run node bamazonCustomer.js

3) The terminal inquirer will ask you what is the item ID of the item you'd like to buy and also the amount of that item you want to purchase.

4) Upon completion. You will get a confirmation message that the purchase was made. Then you will see the updated inventory and the amount of money spent.

#### Video example

![Output sample](https://github.com/Ana-ACLA/Node.js-MySQL/raw/master/bamazon.gif)
