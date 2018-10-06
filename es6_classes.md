// ES6 Classes use a constructor to map out the properties
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hi my name is ${this.name}`);
  }

}

/*
 If you want to extend a class to inherit its properties pass the inherited properties into its constructor.
 Call super within the constructor with the inherited properties in order to map them without retyping them.
*/

class Athlete extends Person {
  constructor(name, age, medals) {
    super(name, age);
    this.medals = medals;
  }

  brag() {
    console.log(`I have ${this.medals} bitches!`);
  }

}

const chloe = new Athlete('Chloe', 19, 5);
chloe.greet();
chloe.brag();
