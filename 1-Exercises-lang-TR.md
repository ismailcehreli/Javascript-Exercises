# 1. Gün Egzersizleri

1. "Yorumlar, kodu daha okunabilir kılar" yazan tek satırlık bir yorum yazın.

```js
// Yorumlar, kodu daha okunabilir kılar
```

2. "30 Günde Javascript" yazan bir başka yorum yazın.

```js
// 30 Günde Javascript
```

3.  "Yorumlar, kodu daha okunabilir kılar, yeniden kullanmayı kolaylaştırır ve bilgilendiricidir." yazan çok satırlı bir yorum yazın.

```js
/*
  Yorumlar, kodu daha okunablir kılar,
  yeniden kullanmayı kolaylaştırır
  ve bilgilendiricidir.
*/
```

4. `variable.js` adında bir javascript dosyası oluşturun ve `string`, `boolean`, `undefined` ve `null` veri türünde değişkenler tanımlayın.

```js
// variable.js
let repo = "30 günde javascript";
let isForked = false;
let test; // değer atanmamışsa undefined olarak belirlenir
let isOkay = null;
```

5. `datatypes.js` adında bir javascript dosyası oluşturun ve yukarıdaki değişkenlerin veri türlerini `typeof` kullanarak kontrol edin.

```js
let repo = "30 günde javascript";
let isForked = false;
let test; // değer atanmamışsa undefined olarak belirlenir
let isOkay = null;

console.log(typeof repo);
console.log(typeof isForked);
console.log(typeof test);
console.log(typeof isOkay);
```

6. Değer atamadan dört farklı değişken tanımlayın.

```js
let variable1;
let variable2;
let varitable3;
let variable4;
```

7. Değer atayarak dört farklı değişken tanımlayın.

```js
let variable1 = "değer 1";
let variable2 = 15;
let variable3 = false;
let variable4 = null;
```

8. Adınızı, soyadınızı, medeni durumunuzu, ülkenizi ve yaşınnızı tek tek değişken oluşturarak tanımlayın.

```js
let name = "İsmail";
let surname = "Çehreli";
let mariage = false;
let country = "Türkiye";
let age = 29;
```

9. Adınızı, soyadınızı, medeni durumunuzu, ülkenizi ve yaşınnızı tek seferde değişken oluşturarak tanımlayın.

```js
let name = "İsmail",
  surname = "Çehreli",
  mariage = false,
  country = "Türkiye",
  age = 37;
```

10. `myAge` ve `yourAge` adında iki değişken tanımlayıp değerlerini belirleyin ve aşağıdaki şekilde konsola log basın.

I am 25 years old.
You are 30 years old.

```js
let myAge = 25;
let yourAge = 30;
console.log(`I am ${myAge} years old.
You are ${yourAge} years old.`);
```
