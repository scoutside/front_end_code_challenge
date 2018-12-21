
Scoutside Front End Engineer Code/Design Challenge
=======================

Hello!

We're excited that you're interested in joining the [Scoutside](https://scoutside.com) team.  In the past, we have
brought potential engineering candidates into our office for a full-day
technical interview.  This interview would include whiteboard programming
exercises, code reviews, and other thought exercises.  Unfortunately, onsite technical interviews are often biased against people who are not comfortable being put on the spot.  Not to mention, who _actually_ codes on a whiteboard in real life?  In short,  we realized that we
were evaluating candidates in an unusual situation.

So instead, we've come up with this relatively open-ended programming/design
challenge that will allow you to demonstrate your skills from the comfort
of your own workspace.  In addition, we know your time is valuable, so please
feel free to use your completed work as a portfolio piece.

We wish you the best of luck and can't wait to see what you create!

Thanks,  
Team Scoutside

--------------------------------------------------------------
## Overview

This is a blank canvas. Tooling and Frameworks are left up to you, though we have a preference towards [Vue.js](https://vuejs.org/). We are equal parts Design and Development at Scoutside and one of 


##### Product Data
We can handle this several ways:

- Create a mock_data.js file and access contents as a module

** **Extra Credit:** Use the ruby script to generate dummy data based on shopify. (You'll need to convert the .csv to json. Feel free to use an external library to handle this.)

Make sure you have the Faker gem installed:

    gem install faker

Run the script with an argument specifying how many products you want:

    ruby faker_script.rb 15

The shopify_data.csv file will be generated in the project root directory.

** **Extra Extra Credit:**
- Sign up for a Shopify Partner Account.
- Create a Development Store.
- Navigate to https://[your-dev-store].myshopify.com/admin/products and find the import button. Then select the generated file and boom - Your store now has dummy data.
- Create a [Private App](https://help.shopify.com/en/api/getting-started/authentication/private-authentication) API Key.
- Utilize the Shopify [Product API](https://help.shopify.com/en/api/reference/products/product) to fetch the generated data.

### Create an MV* app split into three parts

- 1. A form to add new products to a "shop"

- 2. A list that represents products in the shop

- 3. A subset list of selected items from the shop


#### Add an Item Form


The form can be very simple - the title of a product, the price (in $) and a numeric value representing quantity of stock to add. When submitted, the product appears in a list of all products added (we'll call this the Inventory List). Bonus points for validation if all fields are not complete (or invalid format).


#### Inventory List


The Inventory List will list all products added through the form, with the ability to add an item to the Shopping Basket with an Add button next to each product. Multiple quantities of each item can be added to the shopping basket, and when no more stock is available for a particular item, that item will be displayed in a disabled state.


#### Shopping Basket


The Shopping Basket will display a subset of products added from the Inventory List. Each row will include the product title, the quantity and a button to remove all items of that product from the basket. When removed, the product is removed from the shopping basket and the quantity of the Inventory List is updated accordingly.



Our main areas of interest are code structure, commenting, HTML/CSS implementation, architecture of each of the components and flow of data between each, and the implementation of validation (if created). Code can be submitted as a ZIP file, but preferred as a link to GitHub / BitBucket etc. If running locally, we'll need instructions for installation and execution, or alternatively a URL to the demo is great too. 