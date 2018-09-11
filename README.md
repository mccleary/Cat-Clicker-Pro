# Cat Clicker Premium Pro

This is a continuation of the **Cat Clicker**. This repo includes the added functionality of the **Admin** button.

The JavaScript is now organized within a MVC (Model, View, Controller) architecture.

## To use this app
- Click on the name of the cat, on the left, that you would like to see and their picture will appear on the right.
- Click on the cat image as many times as you would like to increase the click count.
- Click on the "**Admin**" button and three input boxes will appear. These boxes allow you to change the name of the cat, the image, and number of clicks on each cats' image.
- Click the "**Save**" button to save your changes to the cat and the "**Cancel**" button to discard the changes.

## App script info for MVC setup
The cats' information is still stored in an array of objects, but within the object called model. Each cat is an object with name, number of clicks, and imageURL properties.

- Within the "view" objects is:
1. The for loop used to loop through the cat's arrays
2. The click event listeners for the buttons and cat names, created with an IIFE(Immediately-Invoked-Function-Expression)
3. The functions that change the cats' information when the "save" or "cancel" buttons are clicked.

 - The variables and functions within the model and view objects communicate with each other via the "octopus" object. The "octopus" object is the controller in the MVC architecture.
