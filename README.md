# Objects

* The association between two terms, the key and the value.
```
{ key: value }
```
* The combination of the key and value represent a property.
* An object is a collection of key value pairs.
* Objects are used for modeling. We can model a user profile, personal accounts, and application data.
* Everything in JS is an object.
  * Functions are objects. Arrays are objects. Numbers, strings, etc. are all objects.

# Object Literals
```
let demo = {};
```
When defining JavaScript properties, the key is always a string. However, property keys don't require quotes (") like usual strings.

Property values can be any type.

You can also leave spaces between keys, values, and the colon to increase readability.
```
let demo = {
            firstname : "Mady",
            petowner: true
          };
```
Be sure to separate properties with commas.

# Objects and Dot Notation

Dot Notation allows us to access properties inside an object.
```
let animal = {
    name : "African bush elephant",
    scientificName : "Loxodonta africana",
    weight : 13000, //in pounds
    height : 11, //in feet
    speak: function(){
        console.log( "Trumpeting!!!" );
    }
};

console.log(animal.name);
```
Dot Notation allows us to add and edit properties inside an object.

**!!! You can accidentally change the type of a property value to another type if you aren't careful. !!!**
```
animal.speak = "I am an Elephant!!!";

animal.speak();
```
# Objects and Bracket Notation

Bracket notation allows us to access properties with strings. When using bracket notation, the property is wrapped in square brackets, [ "key value as a string" ], and the key is always a string.
```
console.log( cat[ "age" ] );
```
Use bracket notation when accessing a property with a variable.
```
let name = "African bush elephant";

animal.name => undefined

animal[name] => "African bush elephant"
```
# Arrays

* Use square brackets ```([ ])``` to define an array. You can start with an empty array or initialize an array with data.
```
let empty = [];

let movies = [ "Toy Story", "A Bug's Life", "Toy Story 2" ];
```
* An array is a zero-indexed JavaScript object that stores a list of values.

* Arrays provide a syntax so that all the items can be stored in one object and then accessed by their location (index) in the list.

* The first element in the array is index 0.
```
let pixarMovies = [ "Toy Story", "A Bug's Life", "Toy Story 2", "Monsters, Inc.", "Finding Nemo", "The Incredibles", "Ratatouille", "WALL-E", "Up", "Toy Story 3", "Cars 2", "Brave", Inside Out", "The Good Dinosaur", "Cars 3" ];

console.log(pixarMovies[3]);
```
* To assign a new value to an array, combine bracket notation with the assignment operator.
```
pixarMovies[3] = "Monsters University";
```
```Array.length```

The length property tells you how many elements are stored in the array.

```Array.push```

The push function will add a new element to the end of the array.

```Array.pop```

The pop function removes the last element from the end of the array and returns it.

```Array.unshift```

The unshift function adds a new element to the beginning of the array.

```Array.splice```

The splice function removes elements from an array using two numbers: the index from where elements should be removed and the number of elements to remove.
```
pixarMovies.splice(3, 2);

pixarMovies.splice(start with index 3, remove 2 elements);
```
