# Software 1 - Class Exercise 4
## Goals
- Use list functions

## Instructions

### Using List Functions
1. In the `ProductLogic` class, in the constructor where you are creating a new list of products, instead of having that list be empty, go ahead and add 2 or 3 products to it.  One of those products should have a quantity of 0.
1. Add the method `GetOnlyInStockProducts()` which will end up returning a list.
1. In the function definition of `GetOnlyInStockProducts()`, we are going to filter our product list to only return products with quantity greater than 0. We can the use the following example but you will need to change out `someListOfThings` with your product list. This will return a new list that contains only the products whose `Quantity` property is greater than zero.

    Example: `list(filter(lambda theThing: theThing.Quantity > 0, someListOfThings))`

    To explain the example a bit: We need to surround the `filter()` in `list()` so that it transform the filter result into a list. Additionally we are using a lambda as the first parameter of the `filter()` so it will execute the lambda on each item within `someListOfThings` similar to the behavior of a `for` loop. In our case it is checking the `Quantity` property of each item our list and evaluating whether it's greater than zero; if it is greater than zero than we are filtering that value. 
1. Let's take this a step further.  Let's say we would only want to return the names of the products.  We would do this by using the `map()` method. We will use this similarly to the `Select()` function which is found in C# and javascript. Even though python doesn't contain the `Select()` functions we can achieve the same behavior by using the `map()` function.
1. Use map so that we get only the list of names by doing: `list(map(lambda theThing: theThing.Name, ourProducts))`. 

    Explanation: The `map()` function is similar to `filter()` in that it will interact on every item of a given list. `map()` however will execute a certain function or expression on each item instead of `filter()`'s behavior.

    This is an example of using map to print each item in a list:
    `map(lambda element: print(element), myList)`
1. Finally, add a UI option to view in stock products only.