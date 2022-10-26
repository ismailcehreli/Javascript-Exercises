# 2. GÜN EGZERSİZLERİ

# Level 1

1- challenge adında bir değişken oluşturarak bu değişkene başlangıç değeri olarak '30 Days Of Javascript' değerini atayınız.

```js
let challenge = "30 Days Of JavaScript";
```

2- Tarayıcınızın konsolunda console.log() kullanarak bir string ifade yazdırınız.

Chrome tarayıcısı açtıktan sonra ctrl + shift + j kısayol tuş kombinasyonu ile konsol açılarak aşağıdaki komut satırı/satırları yazılır.

```js
console.log("Hello World!");
```

veya

```js
let string = "Hello World!";
console.log(string);
```

3- Tarayıcınızın konsolunda console.log kullanarak bir string ifadenin uzunluğunu yazdırınız.

Chrome tarayıcısı açtıktan sonra ctrl + shift + j kısayol tuş kombinasyonu ile konsol açılarak aşağıdaki komut satırı/satırları yazılır.

```js
console.log("Hello World!".length);
```

veya 


```js
let string = "Hello World!";
console.log(string.length);
```

4- toUpperCase() metodunu kullanarak tüm string karakterlerini büyük harf ile yazdır.

```js
console.log("hello world!".toUpperCase());
```

veya 

```js
let string = "hello world!);
console.log(string.toUpperCase());
```

5- toLowerCase() metodunu kullanarak tüm string karakterlerini küçük harf ile yazdır.

```js
console.log("HELLO WORLD!".toLowerCase());
```

veya 

```js
let string = ("HELLO WORLD!");
console.log(string.toLowerCase());
```

6- substr() veya substring() metodunu kullanarak string ifadede içerisindeki ilk kelimeyi keserek kalanı yazdırınız.

a) substr() metodu ile : 

```js
console.log = ("Hello World!".substr(6,11));
```

veya

```js
let string = "Hello World!";
console.log = (string.substr(6,11));
```

b) substring() metodu ile :

```js
console.log = ("Hello World!".substring(6,11));
```

veya

```js
let string = "Hello World!";
console.log = (string.substring(6,11));
```

7- Days Of JavaScript ifadesini 30 Days of JavaScript'ten ayırınız.

```js
let string ="30 Days Of JavaScript";
console.log(string.substr(0,2));
```

8- include() metodunu kullanarak string ifadenin içerisinde 'Script' kelimesinin var olup olmadığını kontrol ediniz.

```js
let string ="30 Days Of JavaScript";
console.log(string.includes("Script"));
```

9- split() metodunu kullananrak string ifadeyi diziye çeviriniz.

```js
let string ="30 Days Of JavaScript";
console.log(string.split());
```

10- '30 Days of JavaScript' string ifadesini split() metodunu kullanarak boşluklardan bölünüz.

```js
let string ="30 Days Of JavaScript";
console.log(string.split(" "));
```

11- 'Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon' string ifadesini split() metodu ile virgül'den bölerek dizi olarak yazdırınız.

```js
let string = "Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon";
console.log(string.split(","));
```

12- replace() metodunu kullanarak '30 Days of JavaScript' string ifadesini '30 Days of Python' olarak değiştiriniz.

```js
let string ="30 Days Of JavaScript";
console.log(string.replace("JavaScript","Python"));
```

13- charAt() metodunu kullanarak '30 Days Of JavaScript' string ifadesinin 15. indeksinin karakterini yazdırınız.

```js
let string ="30 Days Of JavaScript";
console.log(string.charAt(15));
```

14- charCodeAt() metodunu kullanarak '30 Days Of JavaScript' string ifadesinin içerisindeki J'nin unicode değerini yazdırınız.

```js
let string ="30 Days Of JavaScript";
console.log(string.charCodeAt("J"));
```


15- indexOf metodunu kullanarak 30 Days Of JavaScript string ifadesinin içerisinde geçen ilk "Of" ifadesinin index değerini yazdırınız. 

```js
let string ="30 Days Of JavaScript";
console.log(string.indexOf("Of"));
```

16- lastIndexOf metodunu kullanarak 30 Days Of JavaScript string ifadesinin içerisinde geçen son "Of" ifadesinin index değerini yazdırınız. 

```js
let string ="30 Days Of JavaScript";
console.log(string.lastIndexOf("Of"));
```

17- indexOf metodunu kullanarak 'You cannot end a sentence with because because because is a conjunction' cümlesi içerisindeki ilk "because" ifadesinin index değerini yazdırınız.

```js
let string = "You cannot end a sentence with because because because is a conjunction";
console.log(string.indexOf("because"));
```

18- lastIndexOf metodunu kullanarak 'You cannot end a sentence with because because because is a conjunction' cümlesi içerisindeki son "because" ifadesinin index değerini yazdırınız.

```js
let string = "You cannot end a sentence with because because because is a conjunction";
console.log(string.lastIndexOf("because"));
```

19- search metodunu kullanarak 'You cannot end a sentence with because because because is a conjunction' cümlesi içerisindeki ilk "because" ifadesinin index değerini yazdırınız.

```js
let string = "You cannot end a sentence with because because because is a conjunction";
console.log(string.search("because"));
```

20- Bir string ifadenin başındaki ve sonundaki boşlukları trim() metodu ile kaldırınız. Örn string ifade ' 30 Days Of JavaScript '.

```js
let string = " 30 Days Of JavaScript ";
console.log(string.trim());
```

21- 30 Days Of JavaScript string ifadesinde startsWith() metodunu kullanarak sonucu true dönmesini sağlayınız.

```js
let string = "30 Days Of JavaScript";
console.log(string.startsWith("30"));
```

22- 30 Days Of JavaScript string ifadesinde endsWith() metodunu kullanarak sonucu true dönmesini sağlayınız.

```js
let string = "30 Days Of JavaScript";
console.log(string.endsWith("JavaScript"));
```

23- 30 Days Of JavaScript string ifadesinin içerisindeki tüm a'ları match() metodunu kullanarak bulunuz.

```js
let string = "30 Days Of JavaScript";
console.log(string.match(/a/g));
```

24- concat() metodunu kullanarak '30 Days of' string ifadesi ile 'JavaScript' string ifadesini tek bir string ifadesi olacak şekilde ('30 Days Of JavaScript') birleştiriniz. 

```js
let string = "30 Days Of";
console.log(string.concat(" Javascript"));
```

25- 30 Days Of JavaScript string ifadesini repeat() metodunu kullanarak iki kere yazdırınız.

```js
let string = "30 Days Of JavaScript";
console.log(string.repeat(2));
```


# Level 2

1- console.log() metodunu kullanarak aşağıdaki cümleyi yazdırınız.

The quote 'There is no exercise better for the heart than reaching down and lifting people up.' by John Holmes teaches us to help one another.

```js
console.log(`The quote 'There is no exercise better for the heart than reaching down and lifting people up.' by John Holmes teaches us to help one another`);
```

veya

```js
console.log('The quote \'There is no exercise better for the heart than reaching down and lifting people up.\' by John Holmes teaches us to help one another');
```

veya

```js
console.log("The quote 'There is no exercise better for the heart than reaching down and lifting people up.' by John Holmes teaches us to help one another.");
```

2- console.log() metodunu kullanarak rahibe Teresa'nın alıntısını yazdırınız.

```js
console.log("\"Love is not patronizing and charity isn't about pity, it is about love. Charity and love are the same -- with charity you give love, so don't just give money but reach out your hand instead.\"");
```

veya

```js
console.log('"Love is not patronizing and charity isn\'t about pity, it is about love. Charity and love are the same -- with charity you give love, so don\'t just give money but reach out your hand instead."');
```

veya 

```js
console.log(`"Love is not patronizing and charity isn't about pity, it is about love. Charity and love are the same -- with charity you give love, so don't just give money but reach out your hand instead."`);
```

3- '10' ile 10 değerini typeof metodu ile eşit olup olmadığını kontrol ediniz. Eğer eşit değilse her iki değeri birbirine eşitleyiniz.

```js
string = +"10";
number = 10;
console.log(typeof string == typeof number);
```

veya

```js
string = parseInt("10"); 
number = 10;
console.log(typeof string == typeof number);
```

veya

```js
string = Number("10"); 
number = 10;
console.log(typeof string == typeof number);
```

4- parseFloat('9.8') değerinin 10 ile eşitliğini kontrol ediniz. Şayet eşit değilse iki değeri birbirine eşitleyiniz.

```js
num1 = (Math.round(parseFloat('9.8'))); //round methodu ile tam sayı olacak şekilde yukarı yuvarladık.
num2 = 10;
console.log(num1 == num2);
```

5- "python and jargon" string değeri içerisinde "on" ifadesinin olup olmadığını kontrol ediniz.

```js
let string = "python and jargon";
console.log(string.includes("on"));
```

6- "I hope this course is not full of jargon." cümlesinde jargon ifadesinin olup olmadığını kontrol ediniz.

```js
let string = "I hope this course is not full of jargon.";
console.log(string.includes("jargon"));
```

7- 0 ve 100 dahil olmak üzere iki sayı arasında rastgele sayı oluşturunuz.

```js
let num = Math.random() * 101; 
console.log(Math.floor(num));
```

8- 50 ve 100 dahil olmak üzere iki sayı arasında rastgele sayı oluşturunuz.

```js
let num = (Math.random() * 51) + 50; 
console.log(Math.floor(num));
```

9- 0 ve 255 dahil olmak üzere iki sayı arasında rastgele sayı oluşturunuz.

```js
let num = (Math.random() * 256 );
console.log(Math.floor(num));
```

10- Rastgele sayı kullanarak "Javascript" string karakterlerine ulaşınız.

```js
let string = "Javascript";
let indexNo = Math.floor(Math.random() * (string.length - 1)); 
console.log(string[indexNo]);
```

11- Aşağıdaki deseni yazdırmak için console.log() ve kaçış karakterlerini kullanınız.

```js
1 1 1 1 1
2 1 2 4 8
3 1 3 9 27
4 1 4 16 64
5 1 5 25 125
```

```js
console.log("1 1 1 1 1\n2 1 2 4 8\n3 1 3 9 27\n4 1 4 16 64\n5 1 5 25 125");
```

12- substr() metodunu kullanarak 'You cannot end a sentence with because because because a conjunction' ifadesinden because because because 

```js
let string = "You cannot end a sentence with because because because a conjunction.";
let newString = string.substr(0,30) + string.substr(54,15);
console.log(newString);
```

# Level 3

1- 'Love is the best thing in this world. Some found their love and some are still looking for their love.' Bu cümledeki love kelimesinin sayısını yazdırınız.

```js
let string = "Love is the best thing in this world. Some found their love and some are still looking for their love.";
console.log(string.match(/love/gi));
```

2- match() metodunu kullanarak 'You cannot end a sentence with because because because is a conjunction' cümlesinde geçen because kelimesinin sayısını yazdırınız.

```js
let string = "You cannot end a sentence with because because because is a conjunction";
console.log(string.match(/because/gi));
```

3- Aşağıdaki cümleyi temizleyin ve en çok kullanılan kelimeyi bulunuz.

Karakterleri temizleme : 

```js
let string = '%I $am@% a %tea@cher%, &and& I lo%#ve %te@a@ching%;. The@re $is no@th@ing; &as& mo@re rewarding as educa@ting &and& @emp%o@weri@ng peo@ple. ;I found tea@ching m%o@re interesting tha@n any ot#her %jo@bs. %Do@es thi%s mo@tiv#ate yo@u to be a tea@cher!? %Th#is 30#Days&OfJavaScript &is al@so $the $resu@lt of &love& of tea&ching';

let newString = string.replace(/%|\$|@|&|#|;/gi,"");

console.log(newString);
```

En çok kullanılan kelimeyi bulma : 

```js
let string = "I am a teacher, and I love teaching. There is nothing as more rewarding as educating and empowering people. I found teaching more interesting than any other jobs. Does this motivate you to be a teacher!? This 30DaysOfJavaScript is also the result of love of teaching";

function findMostFrequentWord(string) 
{ 
  let words = string.match(/\w+/g);
  let chars = {}; 
  for (let word of words) { 
    if (chars[word]) { 
      chars[word]++; 
    } 
    else { 
      chars[word] = 1; 
    } 
  } 

  let max = 0; 
  let MostFrequentWord = ''; 
  for (let word of words) { 
    if (chars[word] > max) { 
      max = chars[word]; MostFrequentWord = word; 
    } 
  } 
  return MostFrequentWord; 
}

console.log("Most frequent word is : " + findMostFrequentWord(string));
```

4- Aşağıdaki metinden sayıları çıkararak kişinin yıllık toplam gelirini hesaplayınız. 

'He earns 5000 euro from salary per month, 10000 euro annual bonus, 15000 euro online courses per month.

```js
let string = "He earns 5000 euro from salary per month, 10000 euro annual bonus, 15000 euro online courses per month.";

let salaryPerMonth= +(string.substr(9,4));
let annualBonus= +(string.substr(42,4));
let coursesPerMonth= +(string.substr(67,5));

console.log(`Salary per month : ${salaryPerMonth} Euro`);
console.log(`Courses per month : ${coursesPerMonth} Euro`);
console.log(`Annual Bonus = ${annualBonus} Euro`);

let months = 12;
let annualSalary = salaryPerMonth * months;
let annualCourses = coursesPerMonth * months;

console.log(`Annual Salary : ${annualSalary} Euro`);
console.log(`Annual Courses : ${annualCourses} Euro`);

totalSalary = annualBonus + annualCourses + annualSalary;

console.log(`Annual Total Salary : ${totalSalary}`);
```
