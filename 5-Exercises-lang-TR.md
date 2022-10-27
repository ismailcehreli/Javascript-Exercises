# 5. GÜN EGZERSİZLERİ

  

### Seviye 1

  

```js

const  countries = [

'Albania',
'Bolivia',
'Canada',
'Denmark',
'Ethiopia',
'Finland',
'Germany',
'Hungary',
'Ireland',
'Japan',
'Kenya'
]

const  webTechs = [

'HTML',
'CSS',
'JavaScript',
'React',
'Redux',
'Node',
'MongoDB'
]

```

1. _boş_ bir dizi yaratın;

```js
const emptyArr = [];
```

2. Eleman sayısı 5'ten fazla olan bir dizi yaratın.

```js
const arr = [1,2,3,4,5,6];
```

3. Yarattığınız dizinin uzunluğunu bulun ( length ).

```js
const arr = [1,2,3,4,5,6];

console.log(arr.length);
```

4. Dizinizdeki ilk elemanı, ortadaki elemanı ve sondaki elemanı bulun.

```js
const arr = [1,2,3,4,5,6];

console.log("Dizinin ilk elemanı " + arr[0]);

console.log("Dizinin ortanca elemanı " + arr[arr.length / 2]);

console.log("Dizinin ortanca elemanı " + arr[arr.length - 1]);

```

5.  _mixedDataTypes_ adında bir dizi yaratın,dizinin içine farklı veri tiplerinde elemanlar koyun ve bu dizinin uzunluğunu bulun. Dizinin uzunluğu 5'ten büyük olmalıdır.

```js
const mixedDataType = ["Adidas", 1, 3.12, true, { skills: ["HTML","CSS","Javascript"]}, "Istanbul"];
console.log(mixedDataType);
console.log(mixedDataType.length);
```

6. ItCompanies adlı bir dizi değişkeni oluşturun ve Facebook, Google, Microsoft, Apple, IBM, Oracle ve Amazon'a başlangıç değerleri atayın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];
```

7. _console.log()_ kullanarak dizinizi yazdırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];
console.log(itCompanies)
```

8. Dizinin içindeki şirketlerin sayısın yazdırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];
console.log(`Number of companies in array is ${itCompanies.length}`);
```

9. Dizinin içindeki ilk, ortadaki ve son elemanı yazdırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

console.log(`First company in Array is ${itCompanies[0]}`);

console.log(`Middle company in Array is ${itCompanies[(itCompanies.length - 1)/2]}`);

console.log(`Last company in Array is ${itCompanies[itCompanies.length-1]}`);
```

10. Dizideki her şirketi yazdırın.

  1. Tümünü tek seferde yazdırma : 

 ```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

 console.log(itCompanies)
 ```

 2. Tek tek yazdırma :

 ```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

 console.log(itCompanies[0]);
 console.log(itCompanies[1]);
 console.log(itCompanies[2]);
 console.log(itCompanies[3]);
 console.log(itCompanies[4]);
 console.log(itCompanies[5]);
 console.log(itCompanies[6]);
 ```

11. Her bir şirketin adını tek tek büyük harfleri ile değişterin ( ör: facebook -> FACEBOOK) ve her birini yazdırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

console.log(itCompanies[0].toUpperCase());
console.log(itCompanies[1].toUpperCase());
console.log(itCompanies[2].toUpperCase());
console.log(itCompanies[3].toUpperCase());
console.log(itCompanies[4].toUpperCase());
console.log(itCompanies[5].toUpperCase());
console.log(itCompanies[6].toUpperCase());
```

12. Diziyi bir cümle gibi yazdırın: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

const lastIndex = itCompanies[6]; 
itCompanies.pop();
console.log(`${(itCompanies.join(", ")).toString()} and ${lastIndex} are big IT companies.`);
```

13. itCompanies dizisinde belirli bir şirketin olup olmadığını kontrol edin.  Varsa şirketi geri döndürün, aksi takdirde _not found_ geri döndürün.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

if (itCompanies == "Amazon"){
    console.log("A company is not found in the itCompanies array");
} else {
    console.log("Company exists in the itCompanies array")
}
```

14. Birden fazla 'o' harfi içeren şirketleri filter metodunu kullanmadan filtreleyin.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];


```

15.  _sort()_ metodunu kullanarak diziyi sıralayın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompanies.sort();
console.log(itCompanies);

```

16.  _reverse()_ metodunu kullanarak diziyi tersine çevirin.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompanies.reverse();
console.log(itCompanies);
```

17. Diziden ilk 3 şirketi dilimleyin ( Slice edin ).

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompaniesSlice = itCompanies.slice(0,3);
console.log(itCompaniesSlice);
```

18. Diziden son 3 şirketi dilimleyin ( Slice edin ).

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompaniesSlice2 = itCompanies.slice(3,6);
console.log(itCompaniesSlice2);
```

19. Ortadaki IT şirketini ya da şirketlerini diziden dilimleyin ( Slice edin ).

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompaniesSlice3 = itCompanies.slice(3,4);
console.log(itCompaniesSlice3);
```

20. İlk IT şirketini diziden kaldırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompanies.shift();
console.log(itCompanies);
```

21. Ortadaki IT şirketini ya da şirketlerini diziden kaldırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

const itCompaniesLen = Math.floor(itCompanies.length / 2);
console.log(itCompanies[itCompaniesLen]);
```

22. Sondaki IT şirketini diziden kaldırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompanies.pop();
console.log(itCompanies);

```

23. Bütün IT şirketlerini kaldırın.

```js
const itCompanies = ["Facebook", "Google", "Microsoft", "Apple", "IBM", "Oracle", "Amazon"];

itCompanies.splice(0, itCompanies.length);
console.log(itCompanies);
```

  
### Seviye 2


1.Ayrı bir country.js dosyası oluşturun ve country dizisini bu dosyaya kaydedin, ayrı bir web_techs.js dosyası oluşturun ve webTechs dizisini bu dosyaya kaydedin. Daha sonra Main.js dosyasından her iki dosyaya da erişim sağlayın.

1. Önce bütün noktalama işaretlerini kaldırın ve ve string ifadeyi dizi olarak değiştirin ve dizideki kelime sayısını sayın.
  

```js

let  text =

'I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.'

console.log(words)

console.log(words.length)

```

  

```sh

["I", "love", "teaching", "and", "empowering", "people", "I", "teach", "HTML", "CSS", "JS", "React", "Python"]

13

```

  

1. Aşşağıdaki alışveriş sepetindeki elemanları ekleyin, silin , düzenleyin. 

  

```js

const  shoppingCart = ['Milk', 'Coffee', 'Tea', 'Honey']

```

  

- Eğer alışveriş sepetine zaten 'Meat' eklenmemişse en başa ekleyin.  

- Eğer alışveriş sepetine zaten 'Sugar' eklenmemişse en sona ekleyin.  

- Eğer bala alerjiniz varsa 'Honey' elemanını diziden silin.

- 'Tea' elemanını 'Green Tea' olarak güncelleyin.

1. countries dizisinde 'Ethiopia' olup olmadığını kontrol edin. Eğer varsa  'ETHIOPIA' yazdırın. eğer yoksa bunu countries dizisine ekleyin.

2. webTechs dizisinde Sass olup olmadığını kontrol edin eğer varsa 'Sass is a CSS preprocess' yazdırın.  Eğer yoksa diziye Sass elemanını ekleyip diziyi yazdırın

4. Aşağıdaki iki değişkeni birleştirin ve bir fullStack değişkeninde atayın.

  

```js

const  frontEnd = ['HTML', 'CSS', 'JS', 'React', 'Redux']

const  backEnd = ['Node','Express', 'MongoDB']

console.log(fullStack)

```

  

```sh

["HTML", "CSS", "JS", "React", "Redux", "Node", "Express", "MongoDB"]

```

  

### Seviye 3

  

1. Aşağıdaki dizide 10 öğrencinin yaşı vardır:

  

```js

const  ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]

```

  

- Diziyi sıralayın ve en küçük ve en büyük yaşı bulun

- Medyan yaşı bulun(dizinin ortasındaki eleman ama ortada iki eleman varsa  elemanlar ikiye bölünür)

- Ortalama yaşı bulun(tüm elemanlar eleman sayısına bölünür)

- Yaş aralığını bulun (maks - min)

- _abs()_ metodunu kullanarak (min - ortalama) ve (maks - ortalama) değerlerini karşılaştırın, 

1. [countries array](https://github.com/Asabeneh/30DaysOfJavaScript/tree/master/data/countries.js) dizisinden ilk 10 ülkeyi dilimleyin ( Slice edin )

1.  [countries array](https://github.com/Asabeneh/30DaysOfJavaScript/tree/master/data/countries.js) dizisinden ortadaki ülkeleri bulun.

2. countries dizisini çift ise iki eşit diziye bölün. countries dizisi çift değilse, ilk yarı için bir ülke fazla olarak bölün