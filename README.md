# Javascript



## Setting up environment in local machine for javascript


- Create a new folder on the desktop
- Open your editor for the folder 
- Create a file test.js
- Now in test.js write console.log(“hello”);
- Go to the node website and download node

- Step : 1
   - Open VS code and go to view and open terminal and type node -v (for checking the node is successfully installed or not)
   - Now in terminal to run any file write node file_name.js


- Step : 2
  - Go to Github
  - Create a new repository
  - In repo go to code -> codespace 
  - Click on file -> go to view -> command palette -> write container -> add dev container configuration file -> search node -> search all definition -> nodejs & javascript -> ok
  - Save the work 
  - Go the fourth icon of the editor (SOURCE CONTROL FLOW) -> click on the + on that files where the changes occurs -> write a message -> commit
  - Click on the triple dots -> push.
  - 

## Write in Javascript

console.log(“hello”);

console.table([variableName])


## Let , const and var

**Constant** : Variable that cannot be changed and it is declared by the (const variableName) 
	    : Changes not allowed here

**Let** : use for scope.

**Var** : cause issue for block scope and functional scope.

If you declare scope in javascript and does not give any value then it will automatically take undefined.



## DataTypes:

**Use Strict** :  treat all js code as newer version. ( “use strict”; )

**alert()** : example – alert(“hello”);

Let name - “abc” // string

Let age = 18 // number 

Let isLoggedIn = false //boolean

Let state = null // null

Let state; // undefined


**<ins>Primitive Datatypes</ins>**

**Number** : 2 to power 53
  : bigint

**String** : “”

**Boolean** : true/false

**Null** : stand alone value // it’s type is object

**Undefined** : not defined value

**Symbol** : uniqueness


**Typeof _ or typeof()** : to define what type of value does it contain
	: eg console.log(typeof “abc”);


## Conversion and Operation


**<ins>Number</ins>**

Let score = “ 33 “ 

It will give the type string.

And if we want to convert it into number then .

Let valueInNumber = Number(score);

console.log(typeof(valueInNumber);

// “33” is easily converted in number

// “33abc” give number not completed converted in number

// true converted into value of 1


**<ins>Boolean</ins>**

Let isLoggedIn = 1;

Let booleanIsLoggedIn = Boolean(isLggedIn)
console.log(booleanIsLoggedIn);

// 1 ⇒ true

// 0 ⇒ false

// “ “ ⇒ false

// “hitesh” ⇒ true

**<ins>String</ins>**

Let someNumber = 33

Let stringNumber = String(someNumber)

console.log(stringNumber);



**<ins>OPERATION</ins>**
Let value = 3

Let negValue = -value

console.log(negValue);

Let str1 = “hello”

Let str2 = “new”

Let str3 = str1 + str2;

console.log(str3);



**Problem occur at** 

console.log(“1” + 2);// 12

console.log(1 + “2”); // 12

console.log(“1” + 2 + 2); // 122

console.log(1 + 2 + “2”); //32



## Comparison of DataTypes

console.log(2>1);

console.log(2 >= 1):

**Problem occur when you do not compare same datatype**
Like :- 
console.log(“2” > 1); //true

console.log(“02” > 1); //true

console.log(null > 0);   //false

console.log(null == 0); //false

console.log(null >= 0); //true

*The reason is that an equality check == and comparison > < >= <= work different*

*Comparisons convert null to a number , treating it as 0.*

*that’s why null >= 0 is true and null > 0 is false.*

console.log(undefined > 0);   //false

console.log(undefined == 0); //false

console.log(undefined >= 0); //false


**Strict check**

Mean ( === ) : I will not only check their values but also check their datatypes.
Like 
console.log(“2” === 0);

In this their type conversion doesnot happen instead it will check their datatype.


## Datatypes Summary

**Primitive**

**7 types : String, Number, Boolean, null, undefined, Symbol, BigInt**

const score = 100

const scoreValue = 100.3

const isLoggedIn = false

const outsideTemp = null

let userEmail;

const id = Symbol('123')

const anotherId = Symbol('123')

console.log(id === anotherId);

const bigNumber = 3456543576654356754n


**Reference (Non primitive)**

**Array, Objects, Functions**

const heros = ["shaktiman", "naagraj", "doga"];

let myObj = {
    name: "hitesh",
    age: 22,
}

const myFunction = function(){
    console.log("Hello world");
}

console.log(typeof anotherId);

// https://262.ecma-international.org/5.1/#sec-11.4.3




## Stack and Heap Memory

**Stack and  Heap memory** 

**Stack** is used in primitive type and heap memory is used in the non primitive type.

In stack the variable I described , we get a copy of that variable.

Let myName = “new” ;



In **Heap** , we get the reference of that variable.



## String

**String interpolation (backticks)**

Const name = “new”

Const repoCount = 50

console.log(name + repoCount); // this is not preferable so the string interpolation is used now a days.
```
console.log(`Hello my name is ${name.toUppercase} and my repo count is {repoCount}`);
```

**<ins>Another way to declare String</ins>**

Const gameName = new String(‘new-world’)


**<ins>Methods</ins>***

console.log(gameName[0]);

console.log(gameName.__proto__);

console.log(gameName.length);

console.log(gameName.toUpperCase());

console.log(gameName.chatAt(2)); // w

console.log(gameName.indexOf(‘w’); // 2

Const newString = gameName.substring(0,4)

console.log(newSring); //new-

Const anotherString = gamename.slice(0,4)

Const newString = “            new                   “;

console.log(newString);        //                new

console.log(newString.trim()); //new

Const url = “https://new.com/new%20choudhary” ;

console.log(url.replace(‘%20’ , ‘-’); // https://new.com/new-choudhary

console.log(gameName.split(‘-’));




## Numbers and Math

Const score = 400

Const balance = new Number(100)

console.log(balance); // [Number : 400]

console.log(balance.toString().length); //3

console.log(balance.toFixed(2)); //100.00

Const otherNumber = 23.8966

console.log(otherNumber.toPrecision(3)); //23.9 

Note: if there was 123.8966 then it will precise value will roundoff 124

Const hundreds = 1000000

console.log(hundreds.toLocaleString()); //1,000,000

console.log(hundreds.toLocaleString(‘en-IN’)); //10,00,000



**<ins>MATHS</ins>** 

console.log(Math);  //Object [Math] {}

console.log(Math.abs(-4)); 

console.log(Math.round(4.6));  //5

console.log(Math.ceil(4.2));  //5

console.log(Math.floor(4.6));  //4

console.log(Math.min(3,5,7,3);

console.log(Math.max(3,4,6,7);

console.log(Math.random());

Note :- it contain always between 0 and 1 if we want to get a particular range value in this 
So 

console.log((Math.random()*10) +1 );

console.logMath.floor(((Math.random()*10) +1 ));

Const min = 10

Const max = 20

console.log(Math.Floor(Math.random() * (max - min + 1) + min)); // 19 



## Dates 

Let myDate = new Date()

console.log(myDate);

Let myNewDate = new Date(2023, 0, 23)

console.log(myNewDate.toDateString()); // Mon Jan 23 2023

Let myNewDate = new Date(2023, 0, 23, 5, 3)

console.log(myNewDate.toLocaleString()); // 1/23/2023, 5:03:00 AM

Let myNewDate = new Date(“2023-01-14”)

console.log(myNewDate.toLocaleString()); // 1/14/2023, 12:00:00 AM

Let myTime = Date.now()

console.log(myTime); 

console.log(myTime.getTime()); 

console.log(Math.floor(Date.now()/1000));


Let newDate = new Date()

console.log(newDate.getMonth() + 1);

newDate.toLocaleString(‘default’ ,{

 	Weekday : “long”,
	
})



## Arrays

Const myArr = [0,1,2,3,4,5]

- Arrays always be written in the square brackets.
- In this array may contain the homogenous type of data or heterogenous type of data
- And the data contained by array are known as elements.
- Javascript arrays are resizeable (means it can dynamic in size)
- Arrays cannot be associative  arrays : array elements cannot be accessed using arbitrary strings as indexes.
- Like: console.log(myArr[0]); ///correct 
        console.log(myArr[“one”]); ///wrong
- Arrays are zero based indexing : array elements starts from the 0 th position 
- Array-copy-operation create shallow copies (object is a copy share the same reference (means if we change something it will directly change the original one)  ) rather than the deep- copies (object is copy whose properties do not share the same references (means if we change something it will not directly change the original one) )

  - Const myArr = [0,1,2,3,4,5]
  - Const myArr2 = [“new” , “world”]
  - Const myArr3 = new Array(1,2,3,4)

**<ins>Methods</ins>** 


myArr.push(6)

myArr.pop()

myArr.unshift(0)

myArr.shift()

myArr.includes(9)

myArr.indexOf(9)

myArr.slice[1,3]

myArr.splice[1,3]

Const marvel = [“thor” , “Ironman” ,”spiderman]

Const Dc = [“Superman” , “flash” , “batman”]

marvel.push(Dc)

**this will create a issue in which it can create array inside the error because in javascript in array we can pass the different types of data type.**

**<ins>Spread operator</ins>( … )**


Const all = [...marvel ,... Dc ]

condole.log(all);


Const another_array =[ 1, 2, 3,[ 4, 5, 6,] ,7 , [6 , 7, [4, 5]]

Const real_another_array = another_array.flat(Infinity)

console.log(real_another_array);


console.log(Array.isArray(“new”)); // check it is array or not

console.log(Array.from(“new”)); // convert this into array

console.log(Array.from({name: “new”}); //return empty array , and if we want an array we need to define it that we array with keys

Let score1 = 100

Let score = 200

Let score3 = 300

console.lof(Array.of(score1, score2, score 3); //  convert this into an array


## Object

**singleton object** 

**object literals**

```
Const JsUser = {
	Name : “sukhe”,
	Age: 20,
	Location : “Delhi”,
	Email : “sukhe@mail.com”,
	isLoggedIn : false ,
	lastLoginDays : [“Monday” , “Saturday”]
}
```

<ins>two ways to access the  objects</ins>

console.log(JsUser.email);

console.log(JsUser[“email”]);

Note :-  why we prefer the second method instead of the first one  because , Suppose an example in the JsUser “fullname”
```
		Const JsUser = {
			Name : “sukhe”,
			“Full name” : “sukhwinder singh”
			Age: 20,
			Location : “Delhi”,
			Email : “sukhe@mail.com”,
			isLoggedIn : false ,
			lastLoginDays : [“Monday” , “Saturday”]
		}
```

We cannot directly use it using the dot operator , so we need to use it by using the square bracket method.

// to add symbol in the object as a object 

Like
```
Const mySymbol = Symbol(“key1”)
Const JsUser = {
		Name : “sukhe”,
		“Full name” : “sukhwinder singh”,
		mySymbol : “key1”,  // wrong because if we use it , it will give type string
		[mySymbol] : “key1”, //correct way to pass symbol , using the square bracket 
		Age: 20,
		Location : “Delhi”,
		Email : “sukhe@mail.com”,
		isLoggedIn : false ,
		lastLoginDays : [“Monday” , “Saturday”]
}
```


JsUser.email = “new@mail.com” ;

Object.freeze(JsUser) ; // help not to propagate any changes.

jsUser.email = “new1111@mail.com” // this change is not propagated


**<ins>adding function in objects</ins>**

JsUser.greeting = function() {
	console.log(“Hello”);
}

console.log(JsUser.greeting); // function(anonymous)

console.log(JsUser.greeting()); //hello




Const newUser = new Object() // singleton object 

Const newUser1 = {} //non singleton object


newUser1.id = “123fr” 

newUser1.name = “Sammy”

newUser1.isLoggedIn = false  




**<ins>objects in object</ins>**
```
Const regularUser = {
	Email : new@gmail.com,
		Fullname : {
			Userfullname:{
 				firstname: “Sukhwinder”,
				Lastname: “Singh”
			}
		}
}

```

console.log(regularUser.fullname.Userfullname.firstname)

Const obj1 = {1 : “a” , 2 : “b”}

Const ob2 = {3 : “a” , 4 : “b”}

Const obj3 = Object.assign(obj1 , obj2);

Or 

Const obj3 = Object.assign({} , obj1 , obj2); 

Const obj3 = { ...obj1, ...obj2 }
```
Const user = [
	{
		Id : 1 ,
		Email : “s@gmail.com”
	},
	{
		Id : 2 ,
		Email : “u@gmail.com”
	},
	{
		Id : 3 ,
		Email : “k@gmail.com”
	},

]
```


**<ins>Method</ins>**

console.log(Object.keys(newUser));

console.log(Object.Values(newUser));

console.log(Object.entries(newUser));

console.log(newUser.hasOwnProperty(‘isLoggedIn’));


**<ins>Destructuring of Objects</ins>**
```
 Const course = {
	Coursename : “JS “,
	price : “999” ,
	courseInstructor: “Hitesh”
}
```

Const {courseInstructor} = course

console.log(courseInstructor);
 

/// we can also shorten the name in destructuring 

Const {courseInstructor : instructor} = course

console.log(instructor);




 

















 




















 




 






















 




 
