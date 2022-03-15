# Dev-Flower-Shop-

The Product Catalog has the information about available products, their respective codes and prices. It stored in a dictionary and it is shown to the customer as soon this code is executed.


items function:
* used to facilitate the customers to add items to the shopping cart,which is intially an empty list.
* asks the customer to input the number of items they wanted to purchase inorder to understand how many times it should ask for the product code, and it is stored in the count variable.
* A for loop is used to iterate as many times as the count, and adds the products to the cart(empty list) each time the user inputs a valid product code.
* used upper() inorder to make sure the code is taken as valid even if the user inputs lower case letters of the same code ( Assumption: Product codes are not case- sensitive)
* Returns a statement saying that the input is invalid for entering invalid values of number of items the user wanted to purchase and invalid product codes.
* In case of all valid inputs, returns the total cost of the products by calling the price function which in turn calls the delivery function. 

price function:
* takes cart(list of items) as an argument.
* counts the number of times a particular product/item is entered by the user.
* A loop with a conditional statement inside it is used to make sure that 'Buy one, get one at half price' is applied if there are even number of red flowers.
* Sums up the price of each item and returns the total cost of all the products/items added to cart.

delivery function:
*  used to preset the delivery charges for an order based on the total price of the cart.
*  called in the return statement of the price function to output the total price of the cart including delivery charges.

