# Plan for Recipe Book Project

### Object Oriented Design 

Abstract Class (polymorphism):
- Recipe

Subclass:
- DinnerRecipe
- DrinkRecipe
(Each subclass will have unique attributes.)

Attributes:
- name (String) → name of the recipe
- cookingTime (int) → preparation/cooking time in minutes
- calories (double) → calorie count of the recipe

Abstract method:
- displayRecipe() → prints details about the recipe (polymorphism: implemented differently by subclasses)

Dinner(subclass) attributes:
- cuisineType (String: Jamaican, Asian, etc.)
- mainCourseType (String: meat, fish, vegan- friendly, etc.)
- sideDishPairing (String: rice and peas, breadfruit, etc.)

Drink(subclass) attributes:
- fruitType (String: Mango, Strawberry, etc.)
- nutritionalValue (String: Rich in Iron, Vitamin C, etc.)
- isFreshlyMade (boolean: true/false)

### Data Management 
- Store recipes in an ArrayList<Recipe>.
- The program will provide options to:
- Add new recipes (Dinner or Drink)
- Sort recipes by: Name (String) , Cooking time (int) , Calories (double)
- Display all recipes

### Functions and Interactions Menu-driven interface (Scanner + loop):
Polymorphism:
Calling displayRecipe() on a Recipe reference will automatically use the correct subclass implementation (DinnerRecipe or DrinkRecipe).
- Add Dinner Recipe
- Add Drink Recipe
- Display All Recipes

Sorting:
Sorting will be implemented using Comparator and Collections.sort(). which will sort based on the custom rules user provide.
- Sort Recipes by Name
- Sort Recipes by Cooking Time
- Sort Recipes by Calories

### Data Types 
- String (recipe name, cuisine type, fruit type, nutritional value, etc.)
- int (cooking time)(mins)
- double (calories)
- Boolean(whether the drink is freshly made)

### Output and Formatting 
- Nicely formatted in each subclass.
- Each recipe will be displayed with neat formatting.
- Examples
