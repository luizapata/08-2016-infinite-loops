# Infinite Loops (Console-Driven-Development)

## Git Workflow

**Fork the Repository**

1. On Github's website, navigate to the [Infinite Loops Repository.](https://github.com/TelegraphPrep/04-2016-infinite-loops)
2. Click the "Fork" button near the top right part of the screen.
3. In the popup box, select your Github profile to copy the repository from the TelegraphPrep Github profile to your profile.

**Clone the Repository**

4. Once the repository is on your Github profile, navigate to your fork of that repository on Github's website.  
5. Click the "Copy to clipboard" button to copy the Git link for the repository.  
6. In your terminal, navigate to the folder you want to copy the repository into.  
7. In your terminal, type git clone [pasteTheLinkYouJustCopiedHere] then hit enter to clone the repository from Github to your local machine.  

**Open the Repository on Your Local Machine**

In your terminal, navigate to the repository.
View the location of that repository in your finder by typing open . into the terminal.  
To open the repository in Sublime, drag the repository folder over the Sublime icon in your Dock (at the bottom of the screen). All of the files within the repository should now be viewable in the sidebar in Sublime.

**More information on [Git Workflow](https://github.com/TelegraphPrep/PrepPlus-Wiki/blob/master/gitWorkflow.md)

## Pair Programming Dynamics
See the following document on [Pairing Dynamics Workflow](https://github.com/TelegraphPrep/PrepPlus-Wiki)

## About the Sprint

## CarFax.com Sprint

My friend is looking to buy a car this month and is excited to search CarFax.com. Unfortunately their search form is broken, and he has employed you to fix it for him so he can get on the road as soon as possible. Use your `loop` function to solve the next set of prompts. We have created a list of cars `sampleCarList` that you should investigate before starting. Each car object has corresponding properties that you will need to sift through to get what you want. Good luck!


```javascript

var sampleCarList = helpers.carFactory(helpers.carDatabase, helpers.carMaker, 100);
console.dir(sampleCarList);

```


### 1. findBlueCars
`findBlueCars` takes a `carList` array and returns an `array` containing each car object whose color is blue.
  * [ ] create an array, `allBlueCars`, to store your cars in.
  * [ ] use loop to loop through your `carList` array
  * [ ] each car is an object, so you'll want to loop through the objects as well
  * [ ] use a conditional to check whether the property is 'color', and the value is 'blue'
  * [ ] if so, push your corresponding car to the `allBlueCars` array.
  * [ ] when you're finished looping through, return the `allBlueCars` list.

### 2. findCarsByColor:
Let's expand our findBlueCars function to create an array of car objects whose color corresponds to what the user passes in.

  * [ ] add a second parameter, `color`, to your `findBlueCars` function
  * [ ] change your internal functionality to look for the color that the user specifies.

You'll notice that there aren't any directions for the next couple of exercises. We helped with the first 2 but it's your job to figure out how to build these out!

### 3. findCarsByYear:

`findCarsByYear` takes 2 parameters: `carList` and `year` and returns a collection of cars objects that were made in that year.

### 4. findCarsBetweenYears:
`findCarsBetweenYears` takes 3 parameters: `carList`, `startYear`, and `endYear` and returns a collection of cars objects that were made between those years.

### 5. indCarsByMake:
`findCarsByMake` takes 2 parameters: `carList` and `make` and returns a collection of car objects that have that make.

### 6. findCarsByMakeAndModel:
`findCarsByMakeAndModel` takes 3 parameters: `carList`, `make`, and `model` and returns a collection of car objects that have that make and model.

## EXTRA CREDIT:

### 7. Random Price Generator
`randomPriceGenerator` extends each `car object` to have a 'price' property with the value set to a random number between 15000 and 50000.

  ```javascript
  
  // Example:
  var carCollection = [{color: "black", make: "Ford", model:"Everest", year:1994}]
  randomPriceGenerator(carCollection);
  console.log(carCollection);

  // [{color: "black", make: "Ford", model:"Everest", year:1994, price: 27847}];
  
  ```
Create another function, `findByPrice` that takes a `price` parameter and a `list of cars` and returns a list of every car that falls under that price. If no cars fall under the price return "there are no cars below the price you entered."

  ```javascript
  
  // Example:  
  var carCollection = [{color: "black", make: "Ford", model:"Everest", year:1994, price: 27847}];
  console.log(findByPrice(28000, carCollection);
  // [{color: "black", make: "Ford", model:"Everest", year:1994, price: 27847}];
  
  ```

Extend your findByPrice function to take two parameters, a `lowEndPrice` and a `highEndPrice` and returns a list of cars that are between the two prices.

### 8. VerySpecificSearch

VerySpecificSearch allows the user to search using every specification: make, model, color, year, and between two prices. It returns a list containing each car that fulfills these VerySpecificSearch results. If there are no cars that fit the search terms, return "there are no cars that fit what you're looking for, try cars.com".

## EXTRA EXTRA CREDIT:
If there aren't any cars that fit the search term return "there are no cars that fit what you're looking for" and redirect their browser to Cars.com.
