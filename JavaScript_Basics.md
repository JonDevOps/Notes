// Use the typeof operator to determine what data type a variable is holding.
/* Example: 

 let firstName = 'John';
 console.log(typeof firstName); // string
 
*/

// Use the ? operator to shorthand an if statement
/* Example: 

  let age = 21;
  age < 21 ? console.log('He is a kid') : console.log('He is an adult'); // 'He is an adult'
  
*/

// You can use a switch statement as an if and if else statement by setting the paramater to true
/* Example:

  let num = 8;
  
  switch(true) {
    case num < 10:
    console.log('The number is less than 10.');
    break;
    
    case num < 20:
    console.log('The number is less than 20');
    break;
    
    default:
    console.log('The number is greater than 20.');
  }
  
  */
  
// Truthy and Falsy values
// Truthy and False values are not true or false but will return true or false in an if  and if else statement.
// Falsy Values: undefined, NaN, 0, null, '';
// Truthy Values: Anything that is not a falsy value

// The two different types of functions are function statements and function expressions.
// function statements do not provide a value at the end. (you can call function statements before they are created)
// function expressions do provide a value at the end. (you cannot call a function expression before they are created.)

/* Example: 

add(2, 4); // This wil return 6
function add(num1, num2) {
  return num1 + num2;
}


substract(7, 1); // This will throw an error stating that the function is not existant
let substract = function() {
  return num1 - num2;
}

*/

// Use indexOf() method on an array to check the position of a value or if it exists at all.
/* Example: 

 let myArray = ['milk', 'eggs', 'chicken', 'butter'];
 indexOf('ham') // if the value does not exist in an array it returns -1
 if (indexOf('ham') === - 1) {
   console.log('That is not part of the array.');
 }
  
*/

// Use the keyword this to refer to a key in an object
/* Example:
  
  let john = {
    firstName: 'John',
    lastName: 'Smith',
    age: 38
    calcYear: function() {
      this.yearBorn = 2018 - this.age;
    }
  };

*/

// Use the instanceof keyword to return a boolean that checks if the variable is an instance of an function constructor

/* Example:

john instance of Person // returns true

*/

// You can use Object.create to inherit another object as a prototype
/* Example:

let personProto = {
  calcAge: function() {
    console.log(2018 - this.yearOfBirth);
  }
};

let jasmine = Object.create(personProto, {
  name: { value: 'Jasmine' },
  yearOfBirth: { value: 1990 },
  job: { value: 'Carpenter'}
});

// jasmine will inherit everything in the personProto as a prototype

*/
  
