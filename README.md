# 203J1A0505FSAssignments
// 1. Basic Types
let num: number = 10;
let str: string = "Hello";
let bool: boolean = true;
let numArray: number[] = [1, 2, 3, 4, 5];
let tuple: [string, number] = ["John", 30];

enum DaysOfWeek {
  Monday,
  Tuesday,
  Wednesday,
  Thursday,
  Friday,
  Saturday,
  Sunday
}

// 2. Functions
function add(x: number, y: number): number {
  return x + y;
}

function capitalize(str: string): string {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

// 3. Interfaces
interface Person {
  name: string;
  age: number;
  email: string;
}

let user: Person = {
  name: "John Doe",
  age: 25,
  email: "john@example.com"
};

// 4. Classes
class Car {
  make: string;
  model: string;
  year: number;

  constructor(make: string, model: string, year: number) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  displayInfo(): void {
    console.log(`Car: ${this.year} ${this.make} ${this.model}`);
  }
}

// 5. Generics
function reverseArray<T>(arr: T[]): T[] {
  return arr.reverse();
}

// Testing
console.log(num);
console.log(str);
console.log(bool);
console.log(numArray);
console.log(tuple);
console.log(DaysOfWeek.Monday);
console.log(add(5, 3));
console.log(capitalize("hello"));
console.log(user);
let myCar = new Car("Toyota", "Camry", 2020);
myCar.displayInfo();
console.log(reverseArray([1, 2, 3, 4, 5]));
console.log(reverseArray(["a", "b", "c", "d", "e"]));
