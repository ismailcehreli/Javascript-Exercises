#Level 1 - Exercises

1- Declare firstName, lastName, country, city, age, isMarried, year variable and assign value to it and use the typeof operator to check different data types.

```js
const firstName = "İsmail";
const lastName = "Çehreli";
const country = "Türkiye";
const city = "İstanbul";
const age = 36;
const isMarried = true;
const year = 2022;

console.log(typeof(firstName));
console.log(typeof(lastName));
console.log(typeof(country));
console.log(typeof(city));
console.log(typeof(age));
console.log(typeof(isMarried));
console.log(typeof(year));
```

2- Check if type of '10' is equal to 10

```js
const a = "10";
const b = 10;
console.log(typeof(parseInt(a))==typeof(b));
```

3- Check if parseInt('9.8') is equal to 10

```js
console.log(parseInt(9.8) == 10);
```

4- Boolean value is either true or false.

```js
let areYouReady = true;
console.log(areYouReady ? "I am ready" : "No, please wait");
```

5. Figure out the result of the following comparison expression first without using console.log(). After you decide the result confirm it using console.log()
   1. 4 > 3 
   ```js 
   let check = 4 > 3;
   console.log(check); // Result is true
   ```
   
   2. 4 >= 3 
   ```js
   let check = 4 >= 3;
   console.log(check); // Result is false
   ```
   
   3. 4 < 3
   
   ```js
   let check = 4 < 3; 
   console.log(check); // Result is false
   ```

   4. 4 <= 3
   
   ```js
   let check = 4 <= 3;
   console.log(check); // Result is false
   ```

   5. 4 == 4
   
   ```js
   let check = 4 == 4;
   console.log(check); // Result is true
   ```
   
   6. 4 === 4
   
   ```js
   let check = 4 === 4;
   console.log(check); // Result is true
   ```
      
   12. 4 != 4
   
   ```js
   let check = 4 != 4;
   console.log(check); // Result is false
   ```
   
   14. 4 !== 4
   
   ```js
   let check = 4 !== 4;
   console.log(check); // Result is false
   ```
   
   16. 4 != '4'
   
   ```js
   let check = 4 != '4';
   console.log(check); // Result is false
   ```

   18. 4 == '4'
   
   ```js
   let check = 4 == '4';
   console.log(check); // Result is true
   ```
   
   20. 4 === '4'
   
      ```js
   let check = 4 === '4';
   console.log(check); // Result is false
   ```
   
   22. Find the length of python and jargon and make a falsy comparison statement.
  
  ```js
   const langFirst  = "python";
   const langSecond = "jargon";
   
   console.log(langFirst.length);
   console.log(langSecond.length);
   
   let check = langFirst === langSecond;
   console.log(check);
   ```

6. Figure out the result of the following expressions first without using console.log(). After you decide the result confirm it by using console.log()
   1. 4 > 3 && 10 < 12
   2. 4 > 3 && 10 > 12
   3. 4 > 3 || 10 < 12
   4. 4 > 3 || 10 > 12
   5. !(4 > 3)
   6. !(4 < 3)
   7. !(false)
   8. !(4 > 3 && 10 < 12)
   9. !(4 > 3 && 10 > 12)
   10. !(4 === '4')
   11. There is no 'on' in both dragon and python

7. Use the Date object to do the following activities

   1. What is the year today?
   2. What is the month today as a number?
   3. What is the date today?
   4. What is the day today as a number?
   5. What is the hours now?
   6. What is the minutes now?
   7. Find out the numbers of seconds elapsed from January 1, 1970 to now.

```js
date = new Date();
console.log(date.getFullYear());
console.log(date.getMonth());

days = [
    "Sunday",
    "Monday",
    "Tuesday",
    "Wednesday",
    "Thursday",
    "Friday",
    "Saturday"
];

console.log(days[date.getDay()]);
console.log(date.getDay());
console.log(date.getHours());
console.log(date.getMinutes());
console.log(date.getTime());
```

### Exercises: Level 2

1. Write a script that prompt the user to enter base and height of the triangle and calculate an area of a triangle (area = 0.5 x b x h).

   ```sh
   Enter base: 20
   Enter height: 10
   The area of the triangle is 100
   ```
   
 ```js
let enterBase = parseInt(prompt("Please insert base","0"));
let enterHeight = parseInt(prompt("Please enter height","0"));
let area = enterBase * enterHeight * 0.5;
let result = `The area of the triangle is ${area}`;
console.log(result);
 ```

2. Write a script that prompt the user to enter side a, side b, and side c of the triangle and and calculate the perimeter of triangle (perimeter = a + b + c)

   ```sh
   Enter side a: 5
   Enter side b: 4
   Enter side c: 3
   The perimeter of the triangle is 12
   ```
   
```js
let enterA = parseInt(prompt("Please enter a side of the triangle.","0"));
let enterB = parseInt(prompt("Please enter b side of the triangle.","0"));
let enterC = parseInt(prompt("Please enter c side of the triangle.","0"));
let perimeter = enterA + enterB + enterC;
console.log(`The perimeter of the triangle is ${perimeter}`); 
```

3. Get length and width using prompt and calculate an area of rectangle (area = length x width and the perimeter of rectangle (perimeter = 2 x (length + width))

```js
let lenghtOfRectangle = parseInt(prompt("Please enter lenght of the rectangle.","0"));
let heightOfRectangle = parseInt(prompt("Please enter height of the rectangle.","0"));
let area = lenghtOfRectangle * heightOfRectangle;
console.log(`The area of the rectangle is ${area}`);
let perimeter = 2 * (lenghtOfRectangle + heightOfRectangle);
console.log(`The perimeter of the rectangle is ${perimeter}`);
```

4. Get radius using prompt and calculate the area of a circle (area = pi x r x r) and circumference of a circle(c = 2 x pi x r) where pi = 3.14.

```js
const pI = Math.PI;
let r = parseInt(prompt("Please enter radius.","0"));
let area = pI * r * r;
console.log(`The area of the circle is ${area}`);
let circumference = 2 * pI * r;
console.log((`Ht circumference of the circle is ${circumference}`));
```

5. Calculate the slope, x-intercept and y-intercept of y = 2x -2
6. Slope is m = (y<sub>2</sub>-y<sub>1</sub>)/(x<sub>2</sub>-x<sub>1</sub>). Find the slope between point (2, 2) and point(6,10)
7. Compare the slope of above two questions.
8. Calculate the value of y (y = x<sup>2</sup> + 6x + 9). Try to use different x values and figure out at what x value y is 0.
9. Writ a script that prompt a user to enter hours and rate per hour. Calculate pay of the person?

    ```sh
    Enter hours: 40
    Enter rate per hour: 28
    Your weekly earning is 1120
    ```

```js
const dayPerWeek = 7;

let hour = prompt("Please enter your working hour");
let rate = prompt("Please enter your rate hour");
let totalRate = hour * rate * dayPerWeek;

console.log(`Your weekly earning is $${totalRate}`);
```

10. If the length of your name is greater than 7 say, your name is long else say your name is short.
11. Compare your first name length and your family name length and you should get this output.

    ```js
    let firstName = 'Asabeneh'
    let lastName = 'Yetayeh'
    ```

    ```sh
    Your first name, Asabeneh is longer than your family name, Yetayeh
    ```
    
```js
let firstName = "Asabeneh";
let lastName = "Yetayeh";

if (firstName.length > lastName.length) {
console.log(`Your first name, ${firstName} is longer than your family name, ${lastName}`);
} else if (firstName.length === lastName.length) {
console.log(`Length of your first name, ${firstName} is equal than lenght of your family name, ${lastName}`);
} else {
console.log(`Your first name, ${firstName} is shorter than your family name, ${lastName}`);
}
```


12. Declare two variables _myAge_ and _yourAge_ and assign them initial values and myAge and yourAge.

   ```js
   let myAge = 250
   let yourAge = 25
   ```

   ```sh
   I am 225 years older than you.
   ```
   
```js
let myAge = 250
let yourAge = 25
let ageDifference = myAge -  yourAge;
console.log(`I am ${ageDifference} years older than you.`);
```
   

13. Using prompt get the year the user was born and if the user is 18 or above allow the user to drive if not tell the user to wait a certain amount of years.

    ```sh

    Enter birth year: 1995
    You are 25. You are old enough to drive

    Enter birth year: 2005
    You are 15. You will be allowed to drive after 3 years.
    ```
    
```js
let age = prompt("Please enter your age");
age >= 18
? console.log(`You are ${age}. You are old enough to drive`)
: console.log(`You are ${age}. You will be allowed to drive after ${18 - age} years.`);
```

14. Write a script that prompt the user to enter number of years. Calculate the number of seconds a person can live. Assume some one lives just hundred years

   ```sh
   Enter number of years you live: 100
   You lived 3153600000 seconds.
   ```
   
```js
const secondsPerMin = 60;
const minsPerHour = 60;
const hourPerDay = 24;
const daysPerYear = 365;

let yourAge = prompt(parseInt("Please enter your age."));

const calSecondPerHour  = secondsPerMin * minsPerHour;
const calSecondPerDay   = calSecondPerHour * hourPerDay;
const calSecondPerYear  = calSecondPerDay * daysPerYear;
const calSecondYourAge  = yourAge * calSecondPerYear;

console.log(`I have been alive for ${calSecondYourAge} seconds.`);
```

1. Create a human readable time format using the Date time object

   a. YYYY-MM-DD HH:mm
   
```java
const now = new(Date);

const year = now.getFullYear();
const month = now.getMonth();
const day = now.getDay();
const minute = now.getMinutes();
const hour = now.getHours();

const newDate = `${year}-${month}-${day} ${hour}:${minute}`;

console.log(newDate);
```
   
   b. DD-MM-YYYY HH:mm
   
```js
const now = new(Date);

const year = now.getFullYear();
const month = now.getMonth();
const day = now.getDay();
const minute = now.getMinutes();
const hour = now.getHours();

const newDate = `${day}-${month}-${year} ${hour}:${minute}`;

console.log(newDate);
```

   c. DD/MM/YYYY HH:mm

```js
const now = new(Date);

const year = now.getFullYear();
const month = now.getMonth();
const day = now.getDay();
const minute = now.getMinutes();
const hour = now.getHours();

const newDate = `${day}/${month}/${year} ${hour}:${minute}`;

console.log(newDate);
```


### Exercises: Level 3

1. Create a human readable time format using the Date time object. The hour and the minute should be all the time two digits(7 hours should be 07 and 5 minutes should be 05 )

   a. YYY-MM-DD HH:mm eg. 20120-01-02 07:05


```js
const now = new(Date);

const year = now.getFullYear();
const month = String(now.getMonth()).padStart(2,'0');
const day = String(now.getDay()).padStart(2,'0');
const minute = String(now.getMinutes()).padStart(2,'0');
const hour = String(now.getHours()).padStart(2,'0');

const newDate = `${year}-${month}-${day} ${hour}:${minute}`;
console.log(newDate);
```
