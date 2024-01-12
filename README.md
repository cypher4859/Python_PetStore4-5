# Software 1 - Class Exercise 4
## Goals
- Use list functions

## Instructions

### Using List Functions
1. In the `ProductLogic` class, in the constructor where you are creating a new list of products, instead of having that list be empty, go ahead and add 2 or 3 products to it.  One of those products should have a quantity of 0.
1. Add the method `GetOnlyInStockProducts()` which will end up returning a list.
1. In the function definition, we are going to filter our product list to only return products with quantity greater than 0. We can the use the following example but you will need to change out `someListOfThings` with your product list. Example: `filter(lambda theThing: theThing.Quantity > 0, someListOfThings)
1. Let's take this a step further.  Let's say we would only want to return the names of the products.  We would do this by using the `map()` method. We will use this similarly to other languages `Select()` style function even though python doesn't contain the `Select()` functions.
1. Use map so that we get only the list of names by doing: `list(map(lambda theThing: theThing.Name, ourProducts))
1. Finally, add a UI option to view in stock products only.