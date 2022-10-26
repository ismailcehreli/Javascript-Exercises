# 3. GÜN EGZERSİZLERİ

# Seviye 1

1- firstName, lastName, country, city, age, isMarried, year değişkenlerini oluşturun ve bunlara değer atayın. Farklı veri türlerini kontrol etmek için typeof operatörünü kullanın.

```js
const firstName = "İsmail";
const lastName = "Çehreli";
const country = "Türkiye";
const city = "İstanbul";
const age = 36;
const isMarried = true;
const year = 2022;

console.log(typeof firstName);
console.log(typeof lastName);
console.log(typeof country);
console.log(typeof city);
console.log(typeof age);
console.log(typeof isMarried);
console.log(typeof year);
```

2- '10' türünün 10'a eşit olup olmadığını kontrol edin.

```js
const a = "10";
const b = 10;
console.log(typeof parseInt(a) == typeof b);
```

3- parseInt('9.8')'in 10'a eşit olup olmadığını kontrol edin.

```js
console.log(parseInt(9.8) == 10);
```

4- Boolean değeri, doğru veya yanlıştır.

    1.  Doğruluk değeri sağlayan üç JavaScript ifadesi yazın.

    ```js
    let areYouReady = true;
    console.log(areYouReady ? "I am ready" : "No, please wait");

    let areYouHappy = true;
    console.log(areYouHappy ? "Yes I am" : "No I am not");

    let isItTrue = true;
    console.log(isItTrue ? "Yes It is" : "No It is not");
    ```

    2.  Yanlış değer sağlayan üç JavaScript ifadesi yazın.

```js
let areYouReady = false;
console.log(areYouReady ? "I am ready" : "No, please wait");

let areYouHappy = false;
console.log(areYouHappy ? "Yes I am" : "No I am not");

let isItTrue = false;
console.log(isItTrue ? "Yes It is" : "No It is not");
```

5. console.log() kullanmadan önce aşağıdaki karşılaştırma ifadesinin sonucunu bulun. Sonuca karar verdikten sonra console.log() kullanarak onaylayın.

   1. 4 > 3

   ```js
   let check = 4 > 3;
   console.log(check); // Sonuç true
   ```

   2. 4 >= 3

   ```js
   let check = 4 >= 3;
   console.log(check); // Sonuç false
   ```

   3. 4 < 3

   ```js
   let check = 4 < 3;
   console.log(check); // Sonuç false
   ```

   4. 4 <= 3

   ```js
   let check = 4 <= 3;
   console.log(check); // Sonuç false
   ```

   5. 4 == 4

   ```js
   let check = 4 == 4;
   console.log(check); // Sonuç true
   ```

   6. 4 === 4

   ```js
   let check = 4 === 4;
   console.log(check); // Sonuç true
   ```

   7. 4 != 4

   ```js
   let check = 4 != 4;
   console.log(check); // Sonuç false
   ```

   8. 4 !== 4

   ```js
   let check = 4 !== 4;
   console.log(check); // Sonuç false
   ```

   9. 4 != '4'

   ```js
   let check = 4 != "4";
   console.log(check); // Sonuç false
   ```

   10. 4 == '4'

   ```js
   let check = 4 == "4";
   console.log(check); // Sonuç true
   ```

   11. 4 === '4'

   ```js
   let check = 4 === "4";
   console.log(check); // Sonuç false
   ```

   12. Find the length of python and jargon and make a falsy comparison statement.

```js
const langFirst = "python";
const langSecond = "jargon";

console.log(langFirst.length);
console.log(langSecond.length);

let check = langFirst === langSecond;
console.log(check);
```

6. console.log() kullanmadan önce aşağıdaki ifadelerin sonucunu bulun. Sonuca karar verdikten sonra console.log() kullanarak onaylayın.

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

7. Aşağıdaki etkinlikleri yapmak için Date nesnesini kullanın.

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
  "Saturday",
];

console.log(days[date.getDay()]);
console.log(date.getDay());
console.log(date.getHours());
console.log(date.getMinutes());
console.log(date.getTime());
```

# Seviye 2

1. Kullanıcıdan üçgenin tabanını ve yüksekliğini girmesini ve bir üçgenin alanını hesaplamasını isteyen bir komut dosyası yazın (alan = 0,5 x b x h).

   ```sh
   Enter base: 20
   Enter height: 10
   The area of the triangle is 100
   ```

```js
let enterBase = parseInt(prompt("Please insert base", "0"));
let enterHeight = parseInt(prompt("Please enter height", "0"));
let area = enterBase * enterHeight * 0.5;
let result = `The area of the triangle is ${area}`;
console.log(result);
```

2. Kullanıcıdan üçgenin a kenarını, b kenarını ve c kenarını girmesini ve üçgenin çevresini hesaplamasını isteyen bir komut dosyası yazın (çevre = a + b + c).

   ```sh
   Enter side a: 5
   Enter side b: 4
   Enter side c: 3
   The perimeter of the triangle is 12
   ```

```js
let enterA = parseInt(prompt("Please enter a side of the triangle.", "0"));
let enterB = parseInt(prompt("Please enter b side of the triangle.", "0"));
let enterC = parseInt(prompt("Please enter c side of the triangle.", "0"));
let perimeter = enterA + enterB + enterC;
console.log(`The perimeter of the triangle is ${perimeter}`);
```

3. Komut istemini kullanarak uzunluk ve genişliği alın ve bir dikdörtgenin alanını hesaplayın (alan = uzunluk x genişlik ve dikdörtgenin çevresi (çevre = 2 x (uzunluk + genişlik)).

```js
let lenghtOfRectangle = parseInt(
  prompt("Please enter lenght of the rectangle.", "0")
);
let heightOfRectangle = parseInt(
  prompt("Please enter height of the rectangle.", "0")
);
let area = lenghtOfRectangle * heightOfRectangle;
console.log(`The area of the rectangle is ${area}`);
let perimeter = 2 * (lenghtOfRectangle + heightOfRectangle);
console.log(`The perimeter of the rectangle is ${perimeter}`);
```

4. Komut istemini kullanarak yarıçapı alın ve bir dairenin alanını (alan = pi x r x r) ve bir dairenin çevresini (c = 2 x pi x r) hesaplayın, burada pi = 3.14.

```js
const pI = Math.PI;
let r = parseInt(prompt("Please enter radius.", "0"));
let area = pI * r * r;
console.log(`The area of the circle is ${area}`);
let circumference = 2 * pI * r;
console.log(`Ht circumference of the circle is ${circumference}`);
```

5. y = 2x -2'nin eğimini, x kesme noktasını ve y kesme noktasını hesaplayın.
6. Eğim m = (y<sub>2</sub>-y<sub>1</sub>)/(x<sub>2</sub>-x<sub>1</sub>). (2, 2) noktası ile (6,10) noktası arasındaki eğimi bulun.
7. Yukarıdaki iki sorunun eğimini karşılaştırın.
8. y'nin değerini hesaplayın (y = x<sup>2</sup> + 6x + 9). Farklı x değerleri kullanmayı deneyin ve y'nin hangi x değerinin 0 olduğunu bulun.
9. Kullanıcıdan saat ve saat başına oran girmesini isteyen bir komut dosyası yazın. Kişinin ücretini hesapla?

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

10. Adınızın uzunluğu 7'den büyükse, adınız uzun, yoksa adınızın kısa olduğunu söyleyin.
11. Adınızın uzunluğunu ve soyadınızın uzunluğunu karşılaştırın ve bu çıktıyı almalısınız.

```js
let firstName = "Asabeneh";
let lastName = "Yetayeh";
```

```sh
Your first name, Asabeneh is longer than your family name, Yetayeh
```

```js
let firstName = "Asabeneh";
let lastName = "Yetayeh";

if (firstName.length > lastName.length) {
  console.log(
    `Your first name, ${firstName} is longer than your family name, ${lastName}`
  );
} else if (firstName.length === lastName.length) {
  console.log(
    `Length of your first name, ${firstName} is equal than lenght of your family name, ${lastName}`
  );
} else {
  console.log(
    `Your first name, ${firstName} is shorter than your family name, ${lastName}`
  );
}
```

12. İki değişken _myAge_ ve _yourAge_ bildirin ve bunlara başlangıç değerleri ile myAge ve yourAge atayın.

```js
let myAge = 250;
let yourAge = 25;
```

```sh
I am 225 years older than you.
```

```js
let myAge = 250;
let yourAge = 25;
let ageDifference = myAge - yourAge;
console.log(`I am ${ageDifference} years older than you.`);
```

13. İstemi kullanarak, kullanıcının doğduğu yılı alır ve kullanıcı 18 veya daha büyükse, kullanıcıya belirli bir süre beklemesini söylemediği takdirde, kullanıcının araba kullanmasına izin verir.

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
  : console.log(
      `You are ${age}. You will be allowed to drive after ${18 - age} years.`
    );
```

14. Kullanıcıdan yıl sayısını girmesini isteyen bir komut dosyası yazın. Bir kişinin yaşayabileceği saniye sayısını hesaplayın. Birinin sadece yüz yıl yaşadığını varsayalım.

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

const calSecondPerHour = secondsPerMin * minsPerHour;
const calSecondPerDay = calSecondPerHour * hourPerDay;
const calSecondPerYear = calSecondPerDay * daysPerYear;
const calSecondYourAge = yourAge * calSecondPerYear;

console.log(`I have been alive for ${calSecondYourAge} seconds.`);
```

15. Tarih saat nesnesini kullanarak insan tarafından okunabilir bir saat biçimi oluşturun.

    1. YYYY-MM-DD HH:mm

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

    2.  DD-MM-YYYY HH:mm

```js
const now = new Date();

const year = now.getFullYear();
const month = now.getMonth();
const day = now.getDay();
const minute = now.getMinutes();
const hour = now.getHours();

const newDate = `${day}-${month}-${year} ${hour}:${minute}`;

console.log(newDate);
```

    3.  DD/MM/YYYY HH:mm

```js
const now = new Date();

const year = now.getFullYear();
const month = now.getMonth();
const day = now.getDay();
const minute = now.getMinutes();
const hour = now.getHours();

const newDate = `${day}/${month}/${year} ${hour}:${minute}`;

console.log(newDate);
```

# Seviye 3

1. Tarih saat nesnesini kullanarak insan tarafından okunabilir bir saat biçimi oluşturun. Saat ve dakika her zaman iki basamaklı olmalıdır (7 saat 07 ve 5 dakika 05 olmalıdır)

   1. YYY-MM-DD HH:mm eg. 2020-01-02 07:05

```js
const now = new Date();

const year = now.getFullYear();
const month = String(now.getMonth()).padStart(2, "0");
const day = String(now.getDay()).padStart(2, "0");
const minute = String(now.getMinutes()).padStart(2, "0");
const hour = String(now.getHours()).padStart(2, "0");

const newDate = `${year}-${month}-${day} ${hour}:${minute}`;
console.log(newDate);
```
