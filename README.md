1)a) and b)
class Movie {
  constructor(title,studio,rating){
    this.title = title;
    this.studio = studio;
    this.rating = rating;
    if(Movie.rating === "PG"){
        return Movie;
    }
  }
}

1)c) 
let getPG = (str3) => {
  str3 = [];
  for(let i=0;i<str2.length;i++){
    str3 = str2;
    if(str3[i].rating === "PG"){
       console.log(str3[i]);
    }
  }
  return str3;
}

c) and d)
var m1 = new Movie("Casino Royale","Eon Productions","PG13");
var m2 = new Movie("Vaaranam Aayiram","GVM","PG");
var m3 = new Movie("Velayudam","AVM","PG");
var m4 = new Movie("Vinaaithandi Varuvaaya","AVM","PG13");
var str2=[];
str2.push(m1);
str2.push(m2);
str2.push(m3);
str2.push(m4);

getPG(str2);

2)

script.js

var Circle = /** @class */ (function () {
    function Circle(radius, color) {
        this.radius = 1.0;
        this.color = "Red";
        if (typeof (radius) !== "undefined") {
            this.radius = radius;
        }
        if (typeof (color) !== "undefined") {
            this.color = color;
        }
    }
    Circle.prototype.getRadius = function () {
        return this.radius;
    };
    Circle.prototype.setRadius = function (radius) {
        this.radius = radius;
    };
    Circle.prototype.getColor = function () {
        return this.color;
    };
    Circle.prototype.setColor = function (color) {
        this.color = color;
    };
    Circle.prototype.toString = function () {
        return "Radius: " + this.radius + " Color: " + this.color;
    };
    Circle.prototype.getArea = function () {
        return (2 * (Math.PI) * this.radius);
    };
    Circle.prototype.getCircumference = function () {
        return (2 * this.radius);
    };
    return Circle;
}());
var c1 = new Circle();
console.log("Constructor with no params: " + c1.toString());
var c2 = new Circle(3.5);
console.log("Constructor with one param: " + c2.toString());
var c3 = new Circle(2.2, 'Yellow');
console.log("getRadius: " + c3.getRadius());
c3.setRadius(3.3);
console.log("Radius value after setRadius: " + c3.getRadius());
console.log("getColor: " + c3.getColor());
c3.setColor("Blue");
console.log("Color Value after setColor: " + c3.getColor());
console.log(c3.toString());
console.log("Area: " + c3.getArea());
console.log("Circumference: " + c3.getCircumference());

script.ts

type colorData = "Red" | "Yellow" | "Blue" | "Green"
class Circle{
    radius : number = 1.0
    color: colorData = "Red"

    constructor(radius?:number, color?:colorData){
        if(typeof(radius)!=="undefined") { this.radius = radius }
        if(typeof(color)!=="undefined") { this.color = color }
    }

    getRadius():number{
        return this.radius
    }

    setRadius(radius:number){
        this.radius = radius
    }
    getColor():colorData{
        return this.color
    }

    setColor(color:colorData){
        this.color = color
    }

    toString():String{
        return `Radius: ${this.radius} Color: ${this.color}`
    }

    getArea():number{
        return ((Math.PI)*this.radius*this.radius)
    }

    getCircumference():number{
        return (2*(Math.PI)*this.radius)
    }
}

let c1 = new Circle()
console.log("Constructor with no params: "+ c1.toString())

let c2 = new Circle(3.5)
console.log("Constructor with one param: "+ c2.toString())

let c3 = new Circle(2.2, 'Yellow')
console.log("getRadius: "+c3.getRadius())
c3.setRadius(3.3)
console.log("Radius value after setRadius: " +c3.getRadius())
console.log("getColor: "+c3.getColor())
c3.setColor("Blue")
console.log("Color Value after setColor: " + c3.getColor())
console.log(c3.toString())
console.log("Area: "+c3.getArea())
console.log("Circumference: "+c3.getCircumference())

3)

class person{
    constructor(firstName,lastName,DOB,age){
        this.firstName = firstName;
        this.lastName = lastName;
        this.DOB = DOB;
        this.age = age;
    }
}

var p1 = new person("Sundar","K","24/07/2000",23);
console.log(p1);

4)

class Uber{
    constructor(baseRate,estimatedRate,time,distance,demandPercentage){
        this.baseRate = baseRate;
        this.estimatedRate = estimatedRate;
        this.time = time;
        this.distance = distance;
        this.demandPercentage = demandPercentage;
        let finalRate = baseRate*(estimatedRate*(time+distance))*demandPercentage;
        console.log(finalRate);
    }
}

var u1 = new Uber(3,35,4,12,(0.75));
