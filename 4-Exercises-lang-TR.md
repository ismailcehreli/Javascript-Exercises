# 4. GÜN EGZERSİZLERİ

### Seviye 1

1. prompt(“Enter your age:”) ile kullanıcı girdisi alın. Kullanıcı 18 veya daha büyükse, geri bildirimde bulunun:'Sürecek kadar yaşlısınız', ancak 18 değilse, 18 yaşına girmesi gereken yıl sayısını beklemeye başlayarak başka bir geri bildirim verin.

   ```sh
   Enter your age: 30
   You are old enough to drive.

   Enter your age:15
   You are left with 3 years to drive.
   ```

   ```js
   let age = prompt("Can you please enter your age?");

   if (age >= 18){
   console.log(`You are old enough to drive`);
   } else {
   console.log(`You are left with ${18 - age} years to drive`);
   }
   ```

1. if… else kullanarak myAge ve yourAge değerlerini karşılaştırın. Karşılaştırmaya dayanarak ve sonucu kimin daha yaşlı olduğunu (ben veya siz) belirterek konsola kaydedin. Yaşı girdi olarak almak için komut prompt(“Enter your age:”) kullanın.

   ```sh
   Enter your age: 30
   You are 5 years older than me.
   ```

   ```js
   let myAge = 37;
   let yourAge = prompt("Can you please enter your age?");

   if (yourAge > myAge) {
   console.log(`You are ${yourAge - myAge} years older than me`);
   } else {
   console.log(`I am ${myAge - yourAge} years older than you`);
   }
   ```


1. a, b'den büyükse, 'a b'den büyüktür', aksi takdirde 'a, b'den küçüktür' döndürür. şekilde uygulamaya çalışın




    ```js
    let a = 4
    let b = 3
    ```

    ```sh
      4 is greater than 3
    ```

    - using if else

    ```js
    let a = 4
    let b = 3

    if (a > b){
    console.log(`${a} is greater than ${b}`);
    } else if (b > a) {
    console.log(`${b} is greater than ${a}`);
    } 
    ```

    - ternary operator.

    ```js
    let a = 4
    let b = 3
    
    console.log(a>b ? `${a} is greater than ${b}` : `${b} is greater than ${a}`);
         
    ```


1. Çift sayılar 2'ye tam bölünür kalan sıfırdır. Bir sayının çift olup olmadığını veya JavaScript kullanıp kullanmadığını nasıl kontrol edersiniz?

    ```sh
    Enter a number: 2
    2 is an even number

    Enter a number: 9
    9 is is an odd number.
    ```

    ```js
    let number = prompt("Please enter number");
    
    if (number % 2 == 0){
    console.log(`${number} is even number`);
    } else {
    console.log(`${number} is odd number`);
    }
    ```

### Seviye 2

1. Öğrencilere puanlarına göre not verebilecek bir kod yazın:
   - 80-100, A
   - 70-89, B
   - 60-69, C
   - 50-59, D
   - 0-49, F

   ```js
   let yourScore = prompt("Please enter your score");
   
   if (yourScore >= 80 & yourScore <= 100){
   console.log("Your letter grade is A");
   } else if (yourScore >= 70 & yourScore <= 89) {
   console.log("Your letter grade is B");
   } else if (yourScore >= 60 & yourScore <=69) {
   console.log("Your letter grade is C");
   } else if (yourScore >= 50 & yourScore <=59) {
   console.log("Your letter grade is D");
   } else if (yourScore >= 0 & yourScore <=49) {
   console.log("Your letter grade is F")
   } else {
   console.log("Invalid date. Please enter your score between 0 and 100");
   }
   ```

1. Mevsimin Sonbahar, Kış, İlkbahar veya Yaz olup olmadığını kontrol edin.
  Değerler :
    - Eylül, Ekim veya Kasım, mevsim sonbahardır.
    - Aralık, Ocak veya Şubat, mevsim kıştır.
    - Mart, Nisan veya Mayıs mevsimi bahardır
    - Haziran, Temmuz veya Ağustos, mevsim yazdır


   ```js
   let enterMonth = (prompt("Please enter month")).toLowerCase();
   let filterMonth = enterMonth[0].toUpperCase() + enterMonth.slice(1).toLowerCase();

   if (enterMonth == "september" || enterMonth == "october" || enterMonth =="november"){
   console.log(`It is ${filterMonth} and the season is Autumn`);
   } else if (enterMonth == "december" || enterMonth == "january" || enterMonth == "february") {
   console.log(`It is ${filterMonth} and the season is Winter`);
   } else if (enterMonth == "march" || enterMonth == "april" || enterMonth == "may") {
   console.log(`It is ${filterMonth} and the season is Spring`);
   } else if (enterMonth == "june" || enterMonth == "july" || enterMonth == "august") {
   console.log(`It is ${filterMonth} and the season is Summer`);
   } else {
   console.log(`${enterMonth} is invalid data. Please enter name of month.`);
   }
   ```
    
1. Bir günün hafta sonu mu yoksa iş günü mü olduğunu kontrol edin. Komut dosyanız girdi olarak gün alacaktır.

```sh
    What is the day  today? Saturday
    Saturday is a weekend.

    What is the day today? saturDaY
    Saturday is a weekend.

    What is the day today? Friday
    Friday is a working day.

    What is the day today? FrIDAy
    Friday is a working day.
  ```

  ```js
  const enterDay = prompt("What is the day today?");
  const filterDay = enterDay[0].toUpperCase() + enterDay.slice(1).toLowerCase();

  switch (filterDay) {
  case "Monday":
  case "Tuesday":
  case "Wednesday":
  case "Thursday":
  case "Friday":
  console.log(`${filterDay} is a working day.`);
  break;
  case "Saturday":
  case "Sunday":
  console.log(`${filterDay} is a weekend.`)
  break;
  default:
  console.log(`${filterDay} is invalid data. Please enter name of day.`);
  }
  ```

### Seviye 3

1. Bir aydaki gün sayısını söyleyen bir program yazın.

  ```sh
    Enter a month: January
    January has 31 days.

    Enter a month: JANUARY
    January has 31 day

    Enter a month: February
    February has 28 days.

    Enter a month: FEbruary
    February has 28 days.
  ```

  ```js
  let enterMonth = prompt("Please enter month");
  let enterYear = prompt("Please enter year");
  let filterMonth = enterMonth[0].toUpperCase() + enterMonth.slice(1).toLowerCase();
  
  if (filterMonth == "January") {
  let monthDays = new Date(`${enterYear}`,1, 0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "February") {
  let monthDays = new Date(`${enterYear}`,2, 0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (enterMonth == "March") {
  let monthDays = new Date(`${enterYear}`,3,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "April") {
  let monthDays = new Date(`${enterYear}`,4,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "May") {
  let monthDays = new Date(`${enterYear}`,5,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "June") {
  let monthDays = new Date(`${enterYear}`,6,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "July") {
  let monthDays = new Date(`${enterYear}`,7,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "August") {
  let monthDays = new Date(`${enterYear}`,8,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "September") {
  let monthDays = new Date(`${enterYear}`,9,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "October") {
  let monthDays = new Date(`${enterYear}`,10,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "November") {
  let monthDays = new Date(`${enterYear}`,11,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else if (filterMonth == "December") {
  let monthDays = new Date(`${enterYear}`,12,0).getDate();
  console.log(`${filterMonth} has ${monthDays} days.`);
  } else {
  console.log(`${enterMonth} or ${enterYear} are not valid data. Please enter name of month and year`);
  }
  ```