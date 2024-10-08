### ১. জাভাস্ক্রিপ্টের পরিচিতি

#### জাভাস্ক্রিপ্ট কী?
জাভাস্ক্রিপ্ট হল একটি প্রোগ্রামিং ভাষা যা প্রধানত ওয়েব পেজে ইন্টারঅ্যাকটিভ উপাদান তৈরি করতে ব্যবহৃত হয়। এটি ক্লায়েন্ট-সাইড স্ক্রিপ্টিং ভাষা হিসেবে কাজ করে এবং ইউজার ইন্টারফেস উন্নত করতে সাহায্য করে। এছাড়া, সার্ভার-সাইড স্ক্রিপ্টিংয়ের জন্য Node.js ব্যবহার করা হয়।

#### জাভাস্ক্রিপ্টের ইতিহাস
জাভাস্ক্রিপ্ট ১৯৯৫ সালে নেটস্কেপের ব্রেন্ডান আইক দ্বারা তৈরি হয়েছিল। প্রথমে এটি "LiveScript" নামে পরিচিত ছিল, কিন্তু জাভা ভাষার জনপ্রিয়তার কারণে নাম পরিবর্তন করে "JavaScript" রাখা হয়। এটি প্রথম প্রকাশিত হয়েছিল নেটস্কেপ ২.০ ব্রাউজারে।

#### ECMAScript এবং এর সংস্করণগুলি
ECMAScript (ES) হল জাভাস্ক্রিপ্টের একটি স্ট্যান্ডার্ড যা ভাষাটির বৈশিষ্ট্য এবং ফিচার নির্ধারণ করে। বিভিন্ন সংস্করণে এটি নতুন বৈশিষ্ট্য এবং আপডেট এনে দেয়:
- **ES3 (1999)**: নতুন স্ট্রিং মেথড, নিয়ন্ত্রণ স্ট্রাকচার ইত্যাদি।
- **ES5 (2009)**: Strict mode, JSON সাপোর্ট, new Array methods, এবং অন্যান্য উন্নতি।
- **ES6/ES2015**: ক্লাস, মডিউল, arrow functions, promises, template literals, `let` এবং `const` কিওয়ার্ড ইত্যাদি।
- **ES7/ES2016**: Exponential operator (**) এবং Array.prototype.includes।
- **ES8/ES2017**: async/await, Object.entries(), Object.values()।
- **ES9/ES2018**: Rest/Spread properties, Asynchronous iteration।
- **ES10/ES2019**: Array.flat(), String.trimStart(), String.trimEnd()।
- **ES11/ES2020**: BigInt, Dynamic import, Nullish coalescing operator (??)।
- **ES12/ES2021**: Logical assignment operators, String.replaceAll()।

#### ব্রাউজারে জাভাস্ক্রিপ্ট বনাম সার্ভার-সাইড (Node.js)
- **ব্রাউজারে জাভাস্ক্রিপ্ট**: 
  - DOM ম্যানিপুলেশন: HTML এলিমেন্ট পরিবর্তন বা আপডেট করতে পারে।
  - ইভেন্ট হ্যান্ডলার: ব্যবহারকারীর ইন্টারঅ্যাকশন (যেমন ক্লিক) ট্র্যাক করতে পারে।
  - অ্যাসিনক্রোনাস অপারেশন: AJAX বা Fetch API ব্যবহার করে সার্ভার থেকে ডেটা সংগ্রহ করতে পারে।

- **Node.js**: 
  - সার্ভার তৈরি এবং পরিচালনা করতে পারে।
  - ফাইল সিস্টেমের সাথে কাজ করতে পারে।
  - ডাটাবেস অপারেশন (যেমন MongoDB, MySQL) করতে পারে।

#### HTML-এ জাভাস্ক্রিপ্ট অন্তর্ভুক্ত করা (script ট্যাগ)
জাভাস্ক্রিপ্ট কোড HTML পেজে অন্তর্ভুক্ত করতে `<script>` ট্যাগ ব্যবহার করা হয়। এটি `<head>` বা `<body>` ট্যাগের মধ্যে রাখা যেতে পারে।
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <script>
        console.log("Hello, World!");
        alert("Welcome to the page!");
    </script>
</body>
</html>
```

#### কনসোল এবং ডিবাগিং টুল
- **Console**: জাভাস্ক্রিপ্টের বিভিন্ন ডিবাগিং কার্যক্রমের জন্য ব্যবহার করা হয়।
  - `console.log()`: সাধারণ তথ্য প্রদর্শন করে।
  - `console.error()`: ত্রুটি মেসেজ প্রদর্শন করে।
  - `console.warn()`: সতর্কবার্তা প্রদর্শন করে।
- **ডিবাগিং টুলস**: ব্রাউজারে ডেভেলপার টুলস (F12 বা Ctrl+Shift+I) ত্রুটি এবং কর্মক্ষমতা বিশ্লেষণ করতে ব্যবহৃত হয়। এই টুলসগুলি আপনাকে কোড ট্রেস, ব্রেকপয়েন্ট সেট এবং স্ট্যাক ট্রেস দেখতে সহায়তা করে।

#### বেসিক সিনট্যাক্স নিয়ম
- **কেস সেনসিটিভ**: জাভাস্ক্রিপ্ট কেস সেনসিটিভ, যা মানে `Variable` এবং `variable` ভিন্ন।
- **সেমিকোলন**: সাধারণভাবে স্টেটমেন্টের শেষে সেমিকোলন ব্যবহার করা হয়, তবে জাভাস্ক্রিপ্ট স্বয়ংক্রিয়ভাবে সেমিকোলন ইনসার্ট করতে পারে (ASI: Automatic Semicolon Insertion)।
  ```javascript
  let x = 10; // সেমিকোলন ব্যবহার করা হয়েছে
  let y = 20 // ASI সেমিকোলন স্বয়ংক্রিয়ভাবে যোগ করবে
  ```

#### স্টেটমেন্ট এবং এক্সপ্রেশন
- **স্টেটমেন্ট**: একটি প্রোগ্রামিং ভাষার নির্দেশ যা একটি কাজ সম্পাদন করে, যেমন:
  ```javascript
  let x = 5; // স্টেটমেন্ট
  ```
- **এক্সপ্রেশন**: একটি অংশ যা একটি মান প্রদান করে, যেমন:
  ```javascript
  5 + 3 // এক্সপ্রেশন, ফলস্বরূপ 8
  ```

#### মন্তব্য (সিঙ্গেল-লাইন এবং মাল্টিপল-লাইন)
- **সিঙ্গেল-লাইন মন্তব্য**: কোডের এক লাইনে মন্তব্য করার জন্য ব্যবহৃত হয়:
  ```javascript
  // This is a single-line comment
  ```
- **মাল্টিপল-লাইন মন্তব্য**: একাধিক লাইনের মন্তব্য করার জন্য ব্যবহৃত হয়:
  ```javascript
  /*
    This is a multi-line comment
    which spans several lines
  */
  ```

#### ভেরিয়েবল (ঘোষণা এবং ইনিশিয়ালাইজেশন)
- **ঘোষণা**: একটি ভেরিয়েবল তৈরি করা, কিন্তু এটি কোন মান প্রদান করা হয়নি:
  ```javascript
  let x; // ভেরিয়েবল ঘোষণা
  ```
- **ইনিশিয়ালাইজেশন**: একটি ভেরিয়েবলকে একটি মান দেওয়া:
  ```javascript
  x = 10; // ভেরিয়েবল ইনিশিয়ালাইজেশন
  ```
- **একসাথে ঘোষণা ও ইনিশিয়ালাইজেশন**:
  ```javascript
  let x = 10; // একসাথে ঘোষণা ও ইনিশিয়ালাইজেশন
  ```

#### ডেটা টাইপ ওভারভিউ
- **Number**: পূর্ণসংখ্যা এবং দশমিক সংখ্যা যেমন `5`, `3.14`।
- **String**: অক্ষরের সিকোয়েন্স, যেমন `"Hello, World!"`, `'JavaScript'`।
- **Boolean**: সত্য বা মিথ্যা, যেমন `true`, `false`।
- **Undefined**: কোন ভেরিয়েবল ঘোষণা করা হয়েছে কিন্তু কোন মান সেট করা হয়নি।
- **Null**: একটি স্পষ্টভাবে "কোনো মান নেই" বা "শূন্য" নির্দেশ করে।
- **Symbol** (ES6): ইউনিক এবং অপ্রকারিক মানের জন্য ব্যবহৃত হয়।
- **BigInt** (ES11): খুব বড় পূর্ণসংখ্যার জন্য ব্যবহৃত হয়।

#### বেসিক অপারেশনগুলির পরিচিতি
- **`console.log()`**: কনসোলে আউটপুট প্রদর্শন করে:
  ```javascript
  console.log("Hello, World!");
  ```
- **`window.alert()`**: একটি পপ-আপ অ্যালার্ট বক্স প্রদর্শন করে:
  ```javascript
  alert("Welcome to the site!");
  ```
- **`window.write()`**: একটি ডকুমেন্টে সরাসরি লেখা; সাধারণত ব্যবহৃত হয় না এবং অপ্রস্তাবিত:
  ```javascript
  document.write("Hello, World!");
  ```
- **`innerHTML`**: একটি HTML এলিমেন্টের ভিতরের HTML কন্টেন্ট পরিবর্তন করে:
  ```javascript
  document.getElementById("demo").innerHTML = "Hello, World!";
```



### ২. ডেটা টাইপস

#### প্রিমিটিভ বনাম রেফারেন্স ডেটা টাইপ
- **প্রিমিটিভ ডেটা টাইপ**: সরাসরি মান ধারণ করে এবং অ্যালক্যাট সঞ্চয় করে। এগুলি হল `Number`, `String`, `Boolean`, `undefined`, `null`, `Symbol`, এবং `BigInt`। 
- **রেফারেন্স ডেটা টাইপ**: অন্য ডেটা টাইপের রেফারেন্স ধারণ করে। এগুলি হল `Object`, `Array`, এবং `Function`। 

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
// প্রিমিটিভ ডেটা টাইপ
let number = 10; // Number
let name = "John"; // String
let isActive = true; // Boolean
let notDefined; // Undefined
let noValue = null; // Null

// রেফারেন্স ডেটা টাইপ
let person = { name: "John", age: 30 }; // Object
let numbers = [1, 2, 3, 4, 5]; // Array
function greet() { console.log("Hello!"); } // Function
```

#### সংখ্যা এবং সংখ্যাগত অপারেশন
- **যোগ**: দুইটি সংখ্যার যোগফল প্রদান করে।
- **বিয়োগ**: দুইটি সংখ্যার পার্থক্য প্রদান করে।
- **গুণ**: দুইটি সংখ্যার গুণফল প্রদান করে।
- **ভাগ**: এক সংখ্যাকে অন্য সংখ্যার দ্বারা ভাগ করে।
- **মডুলাস**: দুইটি সংখ্যার ভাগফল থেকে অবশিষ্টাংশ প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let a = 10;
let b = 5;

console.log(a + b); // 15 (যোগ)
console.log(a - b); // 5 (বিয়োগ)
console.log(a * b); // 50 (গুণ)
console.log(a / b); // 2 (ভাগ)
console.log(a % b); // 0 (মডুলাস)
```

#### স্ট্রিং এবং স্ট্রিং ম্যানিপুলেশন
- **সংযোজন**: দুইটি স্ট্রিং একত্রিত করা।
- **দৈর্ঘ্য**: স্ট্রিংয়ের দৈর্ঘ্য নির্ধারণ করা।
- **ইনডেক্সিং**: স্ট্রিংয়ের নির্দিষ্ট অবস্থানে অক্ষর প্রাপ্তি।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let str1 = "Hello";
let str2 = "World";

// সংযোজন
let combined = str1 + " " + str2; // "Hello World"

// দৈর্ঘ্য
console.log(combined.length); // 11

// ইনডেক্সিং
console.log(combined[0]); // "H"
console.log(combined.charAt(1)); // "e"
```

#### বুলিয়ান এবং যৌক্তিক অপারেশন
- **true** এবং **false**: বুলিয়ান মান।
- **AND** (&&): দুইটি শর্তই সত্য হলে সত্য।
- **OR** (||): যেকোনো এক শর্ত সত্য হলে সত্য।
- **NOT** (!): শর্তের বিপরীত মান প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let x = 10;
let y = 20;

console.log(x > 5 && y < 25); // true (AND)
console.log(x > 15 || y < 25); // true (OR)
console.log(!(x > 15)); // true (NOT)
```

#### Undefined এবং Null এর পার্থক্য
- **Undefined**: একটি ভেরিয়েবল ঘোষণা করা হয়েছে কিন্তু মান দেওয়া হয়নি।
- **Null**: একটি ভেরিয়েবলে স্পষ্টভাবে "কোন মান নেই" নির্দেশ করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let a; // undefined
let b = null; // null

console.log(a); // undefined
console.log(b); // null
```

#### Symbols (অদ্বিতীয় এবং অপরিবর্তনীয় ডেটা টাইপ)
**Symbol**: একান্তভাবে ইউনিক মান, যা পরিবর্তনযোগ্য নয় এবং প্রধানত অবজেক্টের কী হিসেবে ব্যবহৃত হয়।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let uniqueSymbol = Symbol("description");

let obj = {
  [uniqueSymbol]: "value"
};

console.log(obj[uniqueSymbol]); // "value"
```

#### BigInt (বড় সংখ্যার সাথে কাজ করা)
**BigInt**: খুব বড় পূর্ণসংখ্যা সংরক্ষণ এবং গণনা করতে ব্যবহৃত হয়।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let bigIntNumber = 123456789012345678901234567890n; // BigInt

console.log(bigIntNumber + 1n); // 123456789012345678901234567891n
```

#### অবজেক্ট (কী-ভ্যালু পেয়ার, অবজেক্ট তৈরি করা)
**Object**: কী-ভ্যালু পেয়ার ধারণ করে এবং জাভাস্ক্রিপ্টের প্রধান ডেটা স্ট্রাকচার।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let person = {
  name: "John",
  age: 30,
  greet: function() { console.log("Hello!"); }
};

console.log(person.name); // "John"
person.greet(); // "Hello!"
```

#### অ্যারে (তৈরি এবং উপাদানগুলিতে অ্যাক্সেস করা)
**Array**: একাধিক মান ধারণ করে এবং তাদের একটি নির্দিষ্ট ক্রমে সংরক্ষণ করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let fruits = ["Apple", "Banana", "Cherry"];

// অ্যারে উপাদান অ্যাক্সেস
console.log(fruits[0]); // "Apple"
console.log(fruits[1]); // "Banana"

// অ্যারে লুপ
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

#### ফাংশনগুলি প্রথম শ্রেণীর নাগরিক হিসেবে
ফাংশনগুলি ভেরিয়েবলে সংরক্ষণ, অন্য ফাংশনে পাস এবং ফেরত দেওয়া যেতে পারে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
function add(x, y) {
  return x + y;
}

let operation = add; // ফাংশনকে ভেরিয়েবলে সংরক্ষণ

console.log(operation(5, 3)); // 8

function execute(callback) {
  return callback();
}

execute(() => "Function executed"); // "Function executed"
```

#### টাইপ চেকিং (typeof অপারেটর)
**`typeof`**: একটি ভেরিয়েবলের ডেটা টাইপ নির্ধারণ করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let number = 42;
let name = "Alice";
let isActive = true;
let person = { name: "John", age: 30 };

console.log(typeof number); // "number"
console.log(typeof name); // "string"
console.log(typeof isActive); // "boolean"
console.log(typeof person); // "object"
console.log(typeof undefined); // "undefined"
```



### ৩. অপারেটরস

#### অ্যারিথমেটিক অপারেটর

অ্যারিথমেটিক অপারেটর গাণিতিক গাণনা করার জন্য ব্যবহৃত হয়:

- **যোগ (+)**: দুইটি সংখ্যার যোগফল প্রদান করে।
- **বিয়োগ (-)**: দুইটি সংখ্যার পার্থক্য প্রদান করে।
- **গুণ (*)**: দুইটি সংখ্যার গুণফল প্রদান করে।
- **ভাগ (/)**: একটি সংখ্যা দ্বারা অন্য সংখ্যা ভাগ করে।
- **মডুলাস (%)**: দুইটি সংখ্যার ভাগফল থেকে অবশিষ্টাংশ প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let a = 15;
let b = 4;

console.log(a + b); // 19 (যোগ)
console.log(a - b); // 11 (বিয়োগ)
console.log(a * b); // 60 (গুণ)
console.log(a / b); // 3.75 (ভাগ)
console.log(a % b); // 3 (মডুলাস)
```

#### কম্পারিজন অপারেটর

কম্পারিজন অপারেটর দুটি মান তুলনা করতে ব্যবহৃত হয়:

- **==**: সমান মান তুলনা করে, টাইপ পরিবর্তন করতে পারে।
- **===**: সমান মান এবং টাইপ তুলনা করে।
- **!=**: সমান না হলে সত্য।
- **!==**: সমান না হলে অথবা টাইপ না হলে সত্য।
- **>**: প্রথম মান দ্বিতীয় মানের চেয়ে বড় হলে সত্য।
- **<**: প্রথম মান দ্বিতীয় মানের চেয়ে ছোট হলে সত্য।
- **>=**: প্রথম মান দ্বিতীয় মানের চেয়ে বড় অথবা সমান হলে সত্য।
- **<=**: প্রথম মান দ্বিতীয় মানের চেয়ে ছোট অথবা সমান হলে সত্য।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let x = 10;
let y = 20;

console.log(x == y); // false (মান সমান নয়)
console.log(x === 10); // true (মান এবং টাইপ সমান)
console.log(x != y); // true (মান সমান নয়)
console.log(x !== '10'); // true (মান সমান নয় এবং টাইপও আলাদা)
console.log(x > y); // false (১০ বড় নয় ২০ এর চেয়ে)
console.log(x < y); // true (১০ ছোট ২০ এর চেয়ে)
console.log(x >= 10); // true (১০ বড় অথবা সমান ১০ এর চেয়ে)
console.log(x <= y); // true (১০ ছোট অথবা সমান ২০ এর চেয়ে)
```

#### লজিক্যাল অপারেটর

লজিক্যাল অপারেটর শর্ত বিশ্লেষণ করতে ব্যবহৃত হয়:

- **&&** (AND): দুইটি শর্তই সত্য হলে সত্য।
- **||** (OR): যেকোনো একটি শর্ত সত্য হলে সত্য।
- **!** (NOT): শর্তের বিপরীত মান প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let a = true;
let b = false;

console.log(a && b); // false (দুইটি শর্তই সত্য নয়)
console.log(a || b); // true (একটি শর্ত সত্য)
console.log(!a); // false (a এর বিপরীত)
```

#### অ্যাসাইনমেন্ট অপারেটর

অ্যাসাইনমেন্ট অপারেটর ভেরিয়েবলের মান নির্ধারণ করে:

- **=**: মান নির্ধারণ করে।
- **+=**: মান যোগ করে এবং নির্ধারণ করে।
- **-=**: মান বিয়োগ করে এবং নির্ধারণ করে।
- ***=**: মান গুণ করে এবং নির্ধারণ করে।
- **/=**: মান ভাগ করে এবং নির্ধারণ করে।
- **%=**: মান মডুলাস করে এবং নির্ধারণ করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let num = 10;

num += 5; // num = num + 5;  num এখন 15
console.log(num); // 15

num -= 3; // num = num - 3;  num এখন 12
console.log(num); // 12

num *= 2; // num = num * 2;  num এখন 24
console.log(num); // 24

num /= 4; // num = num / 4;  num এখন 6
console.log(num); // 6

num %= 2; // num = num % 2;  num এখন 0
console.log(num); // 0
```

#### ইনক্রিমেন্ট এবং ডিক্রিমেন্ট অপারেটর

ইনক্রিমেন্ট এবং ডিক্রিমেন্ট অপারেটর সংখ্যা বৃদ্ধি বা কমাতে ব্যবহৃত হয়:

- **++**: সংখ্যা এক বৃদ্ধি করে।
- **--**: সংখ্যা এক কমায়।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let count = 10;

count++; // count = count + 1;  count এখন 11
console.log(count); // 11

count--; // count = count - 1;  count এখন 10
console.log(count); // 10
```

#### বিটওয়াইজ অপারেটর

বিটওয়াইজ অপারেটর বিট লেভেলে গণনা করে:

- **&**: বিট লেভেলে AND।
- **|**: বিট লেভেলে OR।
- **^**: বিট লেভেলে XOR।
- **~**: বিট লেভেলে NOT।
- **<<**: বিট শিফট লেফট।
- **>>**: বিট শিফট রাইট।
- **>>>**: বিট শিফট রাইট (unsigned).

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let a = 5; // 0101 in binary
let b = 3; // 0011 in binary

console.log(a & b); // 1 (0001 in binary)
console.log(a | b); // 7 (0111 in binary)
console.log(a ^ b); // 6 (0110 in binary)
console.log(~a);    // -6 (bitwise NOT)
console.log(a << 1); // 10 (1010 in binary, left shift)
console.log(a >> 1); // 2 (0010 in binary, right shift)
console.log(a >>> 1); // 2 (unsigned right shift)
```

#### টার্নারি অপারেটর

টার্নারি অপারেটর একটি শর্টকাট শর্ত যাচাই করার জন্য:

- **`condition ? expr1 : expr2`**: শর্ত সত্য হলে `expr1`, অন্যথায় `expr2`।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let age = 18;
let canVote = (age >= 18) ? "Yes" : "No";

console.log(canVote); // "Yes"
```

#### typeof অপারেটর

**`typeof`** অপারেটর একটি ভেরিয়েবলের ডেটা টাইপ নির্ধারণ করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let name = "Alice";
let age = 25;

console.log(typeof name); // "string"
console.log(typeof age); // "number"
console.log(typeof true); // "boolean"
console.log(typeof {}); // "object"
console.log(typeof []); // "object"
```

#### instanceof অপারেটর

**`instanceof`** অপারেটর একটি অবজেক্টের টাইপ চেক করতে ব্যবহৃত হয়।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
class Person {}
let person = new Person();

console.log(person instanceof Person); // true
console.log(person instanceof Object); // true
```

#### ইউনারি অপারেটর

ইউনারি অপারেটর একটি একক অপার্যান্ড নিয়ে কাজ করে:

- **`+`**: সংখ্যা হতে স্ট্রিং কনভার্ট করে।
- **`-`**: একটি সংখ্যার নেতিবাচক মান প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
let numString = "20";
let num = +numString; // স্ট্রিং থেকে সংখ্যা তৈরি

console.log(num); // 20
console.log(-num); // -20
```

#### অ্যারে এবং অবজেক্টগুলির জন্য স্প্রেড অপারেটর

স্প্রেড অপারেটর একটি অ্যারে বা অবজেক্টের সব উপাদান পৃথক পৃথক মানে রূপান্তর করে।

**রিয়েল লাইফ কোড উদাহরণ:**
```javascript
// অ্যারে স্প্রেড
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5]; // arr1 এর সব উপাদান এবং নতুন উপাদান যুক্ত

console.log(arr2); // [1, 2, 3, 4, 5]

// অবজেক্ট স্প্রেড
let obj1 = { a: 1, b: 2 };
let obj2 = { ...obj1, c: 3 }; // obj1 এর সব কী-ভ্যালু পেয়ার এবং নতুন কী-ভ্যালু যুক্ত

console.log(obj2); // { a: 1, b: 2, c: 3 }


```

অবশ্যই, একটি ইকমার্স প্রোজেক্টের প্রেক্ষাপটে বিভিন্ন অপারেটরের উদাহরণ এখানে দেওয়া হলো:

### ৩. অপারেটরস

#### অ্যারিথমেটিক অপারেটর

**যোগ (+)**: দুইটি সংখ্যার যোগফল প্রদান করে।
**বিয়োগ (-)**: দুইটি সংখ্যার পার্থক্য প্রদান করে।
**গুণ (*)**: দুইটি সংখ্যার গুণফল প্রদান করে।
**ভাগ (/)**: একটি সংখ্যা দ্বারা অন্য সংখ্যা ভাগ করে।
**মডুলাস (%)**: দুইটি সংখ্যার ভাগফল থেকে অবশিষ্টাংশ প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
// প্রোডাক্টের মূল্য এবং ডিসকাউন্টের হিসাব
let productPrice = 100; // প্রোডাক্টের মূল্য
let discount = 15; // ডিসকাউন্ট শতাংশ

// ডিসকাউন্টের পর মূল্য
let discountedPrice = productPrice - (productPrice * (discount / 100));
console.log(`Discounted Price: $${discountedPrice}`); // Discounted Price: $85

// মোট মূল্য একাধিক প্রোডাক্টের জন্য
let quantity = 3; // প্রোডাক্টের পরিমাণ
let totalPrice = discountedPrice * quantity;
console.log(`Total Price: $${totalPrice}`); // Total Price: $255
```

#### কম্পারিজন অপারেটর

**==**: সমান মান তুলনা করে, টাইপ পরিবর্তন করতে পারে।
**===**: সমান মান এবং টাইপ তুলনা করে।
**!=**: সমান না হলে সত্য।
**!==**: সমান না হলে অথবা টাইপ না হলে সত্য।
**>**: প্রথম মান দ্বিতীয় মানের চেয়ে বড় হলে সত্য।
**<**: প্রথম মান দ্বিতীয় মানের চেয়ে ছোট হলে সত্য।
**>=**: প্রথম মান দ্বিতীয় মানের চেয়ে বড় অথবা সমান হলে সত্য।
**<=**: প্রথম মান দ্বিতীয় মানের চেয়ে ছোট অথবা সমান হলে সত্য।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let userCartTotal = 150;
let minimumFreeShipping = 100;

// ফ্রি শিপিং যোগ্য কিনা যাচাই করা
if (userCartTotal >= minimumFreeShipping) {
    console.log("Free shipping is available.");
} else {
    console.log("Add more items to your cart for free shipping.");
}

// মূল্য তুলনা
let itemPrice = 50;
let budget = 60;
console.log(itemPrice <= budget); // true (বাজেটের মধ্যে আছে)
```

#### লজিক্যাল অপারেটর

**&&** (AND): দুইটি শর্তই সত্য হলে সত্য।
**||** (OR): যেকোনো একটি শর্ত সত্য হলে সত্য।
**!** (NOT): শর্তের বিপরীত মান প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let isLoggedIn = true;
let hasItemsInCart = true;

// চেক করুন যদি ব্যবহারকারী লগড ইন এবং কার্টে আইটেম আছে
if (isLoggedIn && hasItemsInCart) {
    console.log("Proceed to checkout.");
} else {
    console.log("Please log in or add items to your cart.");
}

// ডিসকাউন্ট কুপন ব্যবহার করা
let hasDiscountCoupon = true;
let isHoliday = false;
console.log(hasDiscountCoupon || isHoliday); // true (একটি শর্ত সত্য)
```

#### অ্যাসাইনমেন্ট অপারেটর

**=**: মান নির্ধারণ করে।
**+=**: মান যোগ করে এবং নির্ধারণ করে।
**-=**: মান বিয়োগ করে এবং নির্ধারণ করে।
** *=**: মান গুণ করে এবং নির্ধারণ করে।
**/=**: মান ভাগ করে এবং নির্ধারণ করে।
**%=**: মান মডুলাস করে এবং নির্ধারণ করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let totalAmount = 200;

// প্রোডাক্ট যোগ করা
totalAmount += 50; // totalAmount এখন 250
console.log(`Total Amount: $${totalAmount}`);

// প্রোডাক্ট ফেরত দেয়া
totalAmount -= 30; // totalAmount এখন 220
console.log(`Total Amount after return: $${totalAmount}`);

// প্রোডাক্টে 10% ট্যাক্স যোগ করা
totalAmount *= 1.10; // totalAmount এখন 242
console.log(`Total Amount with tax: $${totalAmount}`);
```

#### ইনক্রিমেন্ট এবং ডিক্রিমেন্ট অপারেটর

**++**: সংখ্যা এক বৃদ্ধি করে।
**--**: সংখ্যা এক কমায়।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let cartItemCount = 5;

// কার্টে একটি আইটেম যোগ করা
cartItemCount++;
console.log(`Items in cart: ${cartItemCount}`); // 6

// কার্ট থেকে একটি আইটেম মুছে ফেলা
cartItemCount--;
console.log(`Items in cart after removal: ${cartItemCount}`); // 5
```

#### বিটওয়াইজ অপারেটর

**&**: বিট লেভেলে AND।
**|**: বিট লেভেলে OR।
**^**: বিট লেভেলে XOR।
**~**: বিট লেভেলে NOT।
**<<**: বিট শিফট লেফট।
**>>**: বিট শিফট রাইট।
**>>>**: বিট শিফট রাইট (unsigned).

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let itemFlags = 0b0011; // প্রাথমিক ফ্ল্যাগস

// ফ্ল্যাগ যোগ করা
let discountedFlag = 0b0100;
let updatedFlags = itemFlags | discountedFlag;
console.log(updatedFlags.toString(2)); // 0111 (ফ্ল্যাগ আপডেট করা)

```

#### টার্নারি অপারেটর

**`condition ? expr1 : expr2`**: শর্ত সত্য হলে `expr1`, অন্যথায় `expr2`।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let isMember = true;
let discountMessage = isMember ? "You get a 10% discount!" : "Join our membership for discounts.";

console.log(discountMessage); // "You get a 10% discount!"
```

#### typeof অপারেটর

**`typeof`** অপারেটর একটি ভেরিয়েবলের ডেটা টাইপ নির্ধারণ করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let productName = "Laptop";
let productPrice = 999.99;
let isAvailable = true;

console.log(typeof productName); // "string"
console.log(typeof productPrice); // "number"
console.log(typeof isAvailable); // "boolean"
console.log(typeof {}); // "object"
```

#### instanceof অপারেটর

**`instanceof`** অপারেটর একটি অবজেক্টের টাইপ চেক করতে ব্যবহৃত হয়।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
class Product {
    constructor(name, price) {
        this.name = name;
        this.price = price;
    }
}

let product = new Product("Smartphone", 299);

console.log(product instanceof Product); // true
console.log(product instanceof Object); // true
```

#### ইউনারি অপারেটর

**`+`**: সংখ্যা হতে স্ট্রিং কনভার্ট করে।
**`-`**: একটি সংখ্যার নেতিবাচক মান প্রদান করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
let productPriceStr = "129.99";
let productPrice = +productPriceStr; // স্ট্রিং থেকে সংখ্যা তৈরি

console.log(productPrice); // 129.99
console.log(-productPrice); // -129.99
```

#### অ্যারে এবং অবজেক্টগুলির জন্য স্প্রেড অপারেটর

স্প্রেড অপারেটর একটি অ্যারে বা অবজেক্টের সব উপাদান পৃথক পৃথক মানে রূপান্তর করে।

**রিয়েল লাইফ কোড উদাহরণ (ইকমার্স প্রোজেক্ট):**
```javascript
// অ্যারে স্প্রেড
let cartItems = ['Item1', 'Item2'];
let newItems = ['Item3', 'Item4'];
let allItems = [...cartItems, ...newItems];

console.log(allItems); // ['Item1', 'Item2', 'Item3', 'Item4']

// অবজেক্ট স্প্রেড
let productDetails = { name: "Laptop", price: 999.99 };
let additionalInfo = { warranty: "2 years", stock: 50 };
let completeProduct = { ...productDetails, ...additionalInfo };

console.log(completeProduct); // { name: "Laptop", price: 999.99, warranty: "2 years", stock: 50 }
```




নিয়ন্ত্রণ প্রবাহের ধারণাগুলি নিম্নলিখিতভাবে বর্ণনা করা হয়েছে, তাদের ফর্ম্যাট এবং বাস্তব কোড উদাহরণের সাথে:

### ৪. নিয়ন্ত্রণ প্রবাহ

#### ১. if স্টেটমেন্ট

**বর্ণনা:** `if` স্টেটমেন্ট একটি নির্দিষ্ট শর্ত পূরণ হলে কোড ব্লক এক্সিকিউট করে। 

**ফর্ম্যাট:**
```javascript
if (condition) {
    // কোড ব্লক
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
let cartTotal = 320;

// যদি কার্টের মোট মূল্য $300 এর বেশি হয়
if (cartTotal > 300) {
    console.log("You qualify for a premium membership discount.");
}
```

#### ২. else if এবং else স্টেটমেন্ট

**বর্ণনা:** `else if` এবং `else` স্টেটমেন্টগুলি `if` স্টেটমেন্টের পরে ব্যবহৃত হয় একাধিক শর্ত যাচাই করার জন্য।

**ফর্ম্যাট:**
```javascript
if (condition1) {
    // কোড ব্লক 1
} else if (condition2) {
    // কোড ব্লক 2
} else {
    // কোড ব্লক 3
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
let cartTotal = 150;

// ডিসকাউন্টের জন্য বিভিন্ন শর্ত নির্ধারণ
if (cartTotal > 300) {
    console.log("You get a 20% discount on your order.");
} else if (cartTotal > 200) {
    console.log("You get a 10% discount on your order.");
} else if (cartTotal > 100) {
    console.log("You get a 5% discount on your order.");
} else {
    console.log("Add more items to get a discount.");
}
```

#### ৩. switch স্টেটমেন্ট

**বর্ণনা:** `switch` স্টেটমেন্ট একাধিক কেসের মধ্যে শর্তের ভিত্তিতে কোড ব্লক কার্যকর করে।

**ফর্ম্যাট:**
```javascript
switch (expression) {
    case value1:
        // কোড ব্লক 1
        break;
    case value2:
        // কোড ব্লক 2
        break;
    default:
        // ডিফল্ট কোড ব্লক
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
let orderStatus = "shipped";

switch (orderStatus) {
    case "pending":
        console.log("Your order is being processed.");
        break;
    case "shipped":
        console.log("Your order has been shipped.");
        break;
    case "delivered":
        console.log("Your order has been delivered.");
        break;
    case "canceled":
        console.log("Your order has been canceled.");
        break;
    default:
        console.log("Unknown status.");
}
```

#### ৪. নেস্টেড if স্টেটমেন্ট

**বর্ণনা:** `if` স্টেটমেন্টের মধ্যে অন্য `if` স্টেটমেন্ট থাকে, যা আরও বিস্তারিত শর্ত যাচাই করে।

**ফর্ম্যাট:**
```javascript
if (condition1) {
    if (condition2) {
        // কোড ব্লক
    }
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
let cartTotal = 350;
let isLoyalCustomer = true;

// লয়াল কাস্টমার হলে অতিরিক্ত ডিসকাউন্ট প্রদান
if (cartTotal > 300) {
    if (isLoyalCustomer) {
        console.log("You get a 30% discount as a loyal customer.");
    } else {
        console.log("You get a 15% discount on your order.");
    }
} else {
    console.log("No special discounts available.");
}
```

#### ৫. টার্নারি অপারেটর

**বর্ণনা:** টার্নারি অপারেটর একটি সহজ শর্তমূলক এক্সপ্রেশন যা একটি শর্তের ভিত্তিতে দুটি ভিন্ন মান প্রদান করে।

**ফর্ম্যাট:**
```javascript
condition ? expr1 : expr2
```

**বাস্তব কোড উদাহরণ:**
```javascript
let cartTotal = 250;
let discount = cartTotal > 200 ? "20% discount" : "No discount";
console.log(`Discount: ${discount}`); // "Discount: 20% discount"
```

#### ৬. শর্ট-সার্কিট মূল্যায়ন (&&, ||)

**বর্ণনা:** `&&` এবং `||` অপারেটরগুলি একটি শর্ত সত্য বা মিথ্যা হলে অন্যান্য শর্তগুলির মূল্যায়ন সংক্ষিপ্ত করে।

**ফর্ম্যাট:**
```javascript
condition1 && condition2
condition1 || condition2
```

**বাস্তব কোড উদাহরণ:**
```javascript
let isLoggedIn = true;
let hasItemsInCart = false;

// যদি লগড ইন থাকে এবং কার্টে আইটেম থাকে
if (isLoggedIn && hasItemsInCart) {
    console.log("Proceed to checkout.");
} else {
    console.log("Please log in or add items to your cart.");
}

// কার্টের মোট মূল্য $200 এর বেশি হলে ফ্রি শিপিং, অন্যথায় এক্সপ্রেশন
let cartTotal = 150;
let shippingMessage = cartTotal > 200 || "Add more items to get free shipping.";
console.log(shippingMessage); // "Add more items to get free shipping."
```

#### ৭. শর্তমূলক অ্যাসাইনমেন্ট (টার্নারি এবং যৌক্তিক অপারেটর ব্যবহার করে)

**বর্ণনা:** টার্নারি অপারেটর এবং যৌক্তিক অপারেটর ব্যবহার করে একটি ভেরিয়েবলে শর্ত অনুযায়ী মান অ্যাসাইন করা হয়।

**ফর্ম্যাট:**
```javascript
variable = condition ? expr1 : expr2
```

**বাস্তব কোড উদাহরণ:**
```javascript
let userRole = "guest";
let discount = userRole === "member" ? 20 : 5; // সদস্য হলে 20% ডিসকাউন্ট, অন্যথায় 5%

console.log(`Discount: ${discount}%`);
```

#### ৮. Truthy এবং Falsy মানগুলি

**বর্ণনা:** কিছু মান `falsy` হিসাবে বিবেচিত হয় এবং অন্যান্য সব মান `truthy` হয়। 

**ফর্ম্যাট:**
```javascript
if (value) {
    // কোড ব্লক যদি value truthy হয়
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
let cartItems = []; // খালি অ্যারে, falsy মান

// যদি কার্টে আইটেম থাকে
if (cartItems.length) {
    console.log("Your cart has items.");
} else {
    console.log("Your cart is empty.");
}
```

#### ৯. Nullish কোয়ালেসিং অপারেটর (??)

**বর্ণনা:** **`??`** অপারেটরটি `null` অথবা `undefined` মানের ক্ষেত্রে একটি ডিফল্ট মান প্রদান করে।

**ফর্ম্যাট:**
```javascript
variable = value ?? defaultValue
```

**বাস্তব কোড উদাহরণ:**
```javascript
let couponCode = null;
let defaultCoupon = "No Coupon";

// যদি couponCode `null` অথবা `undefined` হয় তবে defaultCoupon ব্যবহার হবে
let appliedCoupon = couponCode ?? defaultCoupon;
console.log(`Applied Coupon: ${appliedCoupon}`); // "Applied Coupon: No Coupon"
```

#### ১০. ঐচ্ছিক চেইনিং (?.)

**বর্ণনা:** **`?.`** অপারেটরটি একটি অবজেক্টের প্রপার্টি এক্সেস করার সময় অবজেক্টটি `null` অথবা `undefined` হলে ত্রুটি এড়াতে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
let value = object?.property;
```

**বাস্তব কোড উদাহরণ:**
```javascript
let userProfile = {
    address: {
        city: "Dhaka"
    }
};

// যদি address প্রপার্টি বিদ্যমান থাকে, তবে city প্রপার্টি এক্সেস করবে
let cityName = userProfile.address?.city;
console.log(`City: ${cityName}`); // "City: Dhaka"

// যদি address প্রপার্টি না থাকে, cityName হবে undefined
let countryName = userProfile.address?.country;
console.log(`Country: ${countryName}`); // "Country: undefined"
```

#### ১১. গার্ড ক্লজ

**বর্ণনা:** গার্ড ক্লজ একটি ফাংশন শুরু করার আগে কিছু শর্ত যাচাই করে, যা ভুল ইনপুট থেকে সুরক্ষা প্রদান করে।

**ফর্ম্যাট:**
```javascript
function someFunction(parameter) {
    if (!parameter) {
        throw new Error("Parameter is required.");
    }
    // ফাংশনের বাকি অংশ
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
function processOrder(order) {
    if (!order) {
        throw new Error("Order is required.");
    }
    // প্রক্রিয়া অব্যাহত
    console.log("Processing order:", order);
}

try {
    processOrder(null); // ত্রুটি হবে
} catch (error) {
    console.error(error.message); // "Order is required."
}
```

#### ১২. আর্লি রিটার্ন প্যাটার্নস

**বর্ণনা:** আর্লি রিটার্ন প্যাটার্ন ফ

াংশনের শুরুতেই শর্ত পূরণ হলে ফলাফল ফেরত দেয়, যা কোডের মূল অংশে পৌঁছানোর আগেই ফাংশন শেষ করে।

**ফর্ম্যাট:**
```javascript
function checkEligibility(age) {
    if (age < 18) {
        return "Not eligible.";
    }
    // অন্যান্য কোড
    return "Eligible.";
}
```

**বাস্তব কোড উদাহরণ:**
```javascript
function getDiscount(user) {
    if (!user.isActive) {
        return "No discount for inactive users.";
    }
    // একটিভ ইউজারদের জন্য ডিসকাউন্ট ক্যালকুলেশন
    return "You get a 10% discount.";
}

console.log(getDiscount({ isActive: false })); // "No discount for inactive users."
console.log(getDiscount({ isActive: true }));  // "You get a 10% discount."
```

প্রত্যেকটি প্রবাহ নিয়ন্ত্রণের ধারণা বাস্তব প্রোগ্রামিং পরিস্থিতিতে কীভাবে ব্যবহার করা যায় তা বুঝতে সাহায্য করবে।



### ৫. লুপস

লুপস হল প্রোগ্রামিং কনস্ট্রাক্ট যা আপনাকে একাধিকবার কোডের ব্লক এক্সিকিউট করতে সাহায্য করে। লুপের বিভিন্ন প্রকার এবং তাদের ব্যবহারগুলি নিচে বিস্তারিত বর্ণনা করা হয়েছে, ফর্ম্যাট ও বাস্তব উদাহরণের সাথে।

#### ১. for লুপ

**বর্ণনা:** `for` লুপ সাধারণত নির্দিষ্ট সংখ্যক বার পুনরাবৃত্তি করতে ব্যবহৃত হয়। এটি তিনটি অংশ নিয়ে গঠিত: ইনিশিয়ালাইজেশন, কন্ডিশন চেক, এবং ইনক্রিমেন্ট/ডিক্রিমেন্ট।

**ফর্ম্যাট:**
```javascript
for (initialization; condition; increment/decrement) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
// 1 থেকে 5 পর্যন্ত সংখ্যাগুলি কনসোলে প্রিন্ট করা
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
```

#### ২. while লুপ

**বর্ণনা:** `while` লুপ নির্দিষ্ট শর্ত পূরণ না হওয়া পর্যন্ত কোড ব্লক এক্সিকিউট করে।

**ফর্ম্যাট:**
```javascript
while (condition) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
let count = 1;

// 1 থেকে 5 পর্যন্ত সংখ্যাগুলি কনসোলে প্রিন্ট করা
while (count <= 5) {
    console.log(count);
    count++;
}
```

#### ৩. do...while লুপ

**বর্ণনা:** `do...while` লুপ প্রথমে কোড ব্লক এক্সিকিউট করে, তারপর শর্ত চেক করে। এটি কমপক্ষে একবার কোড ব্লক এক্সিকিউট হবে।

**ফর্ম্যাট:**
```javascript
do {
    // কোড ব্লক
} while (condition);
```

**বাস্তব উদাহরণ:**
```javascript
let count = 1;

// 1 থেকে 5 পর্যন্ত সংখ্যাগুলি কনসোলে প্রিন্ট করা
do {
    console.log(count);
    count++;
} while (count <= 5);
```

#### ৪. for...in লুপ

**বর্ণনা:** `for...in` লুপ একটি অবজেক্টের সমস্ত প্রপার্টির ওপর পুনরাবৃত্তি করে।

**ফর্ম্যাট:**
```javascript
for (let key in object) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
let product = {
    name: "Laptop",
    price: 1000,
    brand: "ABC"
};

// অবজেক্টের প্রপার্টি গুলির ওপর লুপ করা
for (let key in product) {
    console.log(`${key}: ${product[key]}`);
}
```

#### ৫. for...of লুপ

**বর্ণনা:** `for...of` লুপ একটি অ্যারে বা অন্যান্য iterable অবজেক্টের উপাদানগুলির ওপর পুনরাবৃত্তি করে।

**ফর্ম্যাট:**
```javascript
for (let element of iterable) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
let numbers = [10, 20, 30, 40, 50];

// অ্যারের উপাদানগুলির ওপর লুপ করা
for (let number of numbers) {
    console.log(number);
}
```

#### ৬. নেস্টেড লুপ

**বর্ণনা:** একটি লুপের ভিতরে অন্য একটি লুপ থাকে, যা একটি মাল্টি-ডাইমেনশনাল অ্যারে বা টেবিলের মতো স্ট্রাকচারগুলো হ্যান্ডল করতে সাহায্য করে।

**ফর্ম্যাট:**
```javascript
for (let i = 0; i < outerLimit; i++) {
    for (let j = 0; j < innerLimit; j++) {
        // কোড ব্লক
    }
}
```

**বাস্তব উদাহরণ:**
```javascript
// 2D ম্যাট্রিক্সের উপাদানগুলি প্রিন্ট করা
let matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

for (let row of matrix) {
    for (let cell of row) {
        console.log(cell);
    }
}
```

#### ৭. লুপ নিয়ন্ত্রণ (break, continue)

**বর্ণনা:** `break` লুপটি সম্পূর্ণভাবে বন্ধ করে দেয়, এবং `continue` লুপের বর্তমান ইটারেশন শেষ করে পরবর্তী ইটারেশনে চলে যায়।

**ফর্ম্যাট:**
```javascript
for (let i = 0; i < limit; i++) {
    if (conditionToBreak) {
        break;
    }
    if (conditionToContinue) {
        continue;
    }
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
for (let i = 1; i <= 10; i++) {
    if (i === 5) {
        break; // i 5 হলে লুপ বন্ধ হয়ে যাবে
    }
    console.log(i);
}

for (let i = 1; i <= 10; i++) {
    if (i % 2 === 0) {
        continue; // i যদি জোড় সংখ্যা হয় তবে এড়িয়ে যাবে
    }
    console.log(i); // কেবল একক সংখ্যাগুলি প্রিন্ট করবে
}
```

#### ৮. অ্যারেগুলির উপরে ইটারেশন

**বর্ণনা:** অ্যারে উপাদানগুলির ওপর লুপিং করতে ব্যবহৃত হয়, সাধারণত `for`, `for...of`, অথবা `forEach` মেথড ব্যবহার করে।

**ফর্ম্যাট:**
```javascript
let array = [1, 2, 3, 4, 5];
array.forEach(element => {
    // কোড ব্লক
});
```

**বাস্তব উদাহরণ:**
```javascript
let cartItems = ["item1", "item2", "item3"];

// অ্যারেগুলির উপরে ইটারেশন
cartItems.forEach(item => {
    console.log(`Item: ${item}`);
});
```

#### ৯. অবজেক্টগুলির উপরে ইটারেশননাm


**বর্ণনা:** অবজেক্টের প্রপার্টি বা কী-ভ্যালু পেয়ারগুলির ওপর লুপিং করতে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
for (let key in object) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
let user = {
    name: "Alice",
    age: 30,
    city: "New York"
};

// অবজেক্টের প্রপার্টি গুলির ওপর লুপ করা
for (let key in user) {
    console.log(`${key}: ${user[key]}`);
}
```

#### ১০. স্ট্রিংগুলির উপরে ইটারেশন

**বর্ণনা:** স্ট্রিংয়ের প্রতিটি চরিত্রের ওপর লুপিং করা।

**ফর্ম্যাট:**
```javascript
let str = "hello";
for (let char of str) {
    // কোড ব্লক
}
```

**বাস্তব উদাহরণ:**
```javascript
let message = "Hello";

// স্ট্রিংয়ের প্রতিটি চরিত্র প্রিন্ট করা
for (let char of message) {
    console.log(char);
}
```

#### ১১. ইনফিনিট লুপ এবং সেগুলি প্রতিরোধ করা

**বর্ণনা:** ইনফিনিট লুপ একটি লুপ যা কখনও শেষ হয় না। সেগুলি প্রতিরোধ করার জন্য শর্ত সঠিকভাবে নির্ধারণ করা প্রয়োজন।

**ফর্ম্যাট:**
```javascript
while (true) {
    // কোড ব্লক
    if (conditionToBreak) {
        break;
    }
}
```

**বাস্তব উদাহরণ:**
```javascript
let counter = 1;

while (true) {
    console.log(counter);
    if (counter >= 5) {
        break; // ইনফিনিট লুপ থেকে বের হওয়া
    }
    counter++;
}
```

#### ১২. লুপ কর্মক্ষমতা বিবেচনা

**বর্ণনা:** লুপের কর্মক্ষমতা একটি গুরুত্বপূর্ণ বিষয়, বিশেষ করে বড় ডেটাসেটের সাথে কাজ করার সময়। নেস্টেড লুপস এবং অতিরিক্ত প্রক্রিয়াকরণের কারণে কর্মক্ষমতা প্রভাবিত হতে পারে।

**ফর্ম্যাট:**
```javascript
// অপ্টিমাইজড লুপ উদাহরণ
for (let i = 0; i < array.length; i++) {
    // কোড ব্লক
}

// কমপ্লেক্স লজিক বা বড় ডেটা সেটস হ্যান্ডল করার সময় অপ্টিমাইজড লুপস ব্যবহার করুন।
```

**বাস্তব উদাহরণ:**
```javascript
// বিশাল অ্যারে প্রক্রিয়া করার জন্য অপ্টিমাইজড লুপ
let largeArray = new Array(10000).fill(0);

let sum = 0;
for (let i = 0; i < largeArray.length; i++) {
    sum += largeArray[i];
}

console.log(`Sum: ${sum}`);
```

এই উদাহরণগুলি আপনাকে JavaScript-এ বিভিন্ন লুপ প্র

কার এবং তাদের ব্যবহার বুঝতে সহায়ক হবে, এবং কিভাবে সেগুলি বাস্তব জীবনের সমস্যা সমাধানে কাজে লাগানো যায় তা দেখাবে।




### ৬. ফাংশনস

ফাংশনগুলি কোড পুনঃব্যবহারের জন্য গুরুত্বপূর্ণ। তারা নির্দিষ্ট কাজ সম্পাদন করার জন্য কোডের ব্লকগুলি সংজ্ঞায়িত করে। এখানে ফাংশন সম্পর্কিত বিভিন্ন ধারণা এবং তাদের ইকমার্স প্রজেক্টে বাস্তব উদাহরণ দেয়া হলো।

#### ১. ফাংশন ঘোষণা

**বর্ণনা:** ফাংশন ঘোষণা কোড ব্লকের নাম এবং এর কার্যকারিতা নির্ধারণ করে। এটি মূলত একটি পুনঃব্যবহারযোগ্য ব্লক যা কোনও নির্দিষ্ট কাজ সম্পাদন করে।

**ফর্ম্যাট:**
```javascript
function functionName(parameters) {
    // কোড ব্লক
    return result;
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// প্রোডাক্টের দাম হিসাব করার জন্য একটি ফাংশন
function calculatePrice(price, taxRate) {
    return price + (price * taxRate);
}

// ব্যবহার
let totalPrice = calculatePrice(100, 0.15);
console.log(`Total Price: $${totalPrice}`);
```

#### ২. ফাংশন এক্সপ্রেশন

**বর্ণনা:** ফাংশন এক্সপ্রেশন ফাংশনকে একটি ভেরিয়েবলে সংজ্ঞায়িত করে। এটি একটি অ্যানোনিমাস ফাংশনও হতে পারে।

**ফর্ম্যাট:**
```javascript
const functionName = function(parameters) {
    // কোড ব্লক
    return result;
};
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একটি ফাংশন এক্সপ্রেশন যা প্রোডাক্টের ডিসকাউন্ট প্রয়োগ করে
const applyDiscount = function(price, discount) {
    return price - (price * discount);
};

// ব্যবহার
let discountedPrice = applyDiscount(200, 0.1);
console.log(`Discounted Price: $${discountedPrice}`);
```

#### ৩. অ্যারো ফাংশন

**বর্ণনা:** অ্যারো ফাংশনগুলি একটি সংক্ষিপ্ত সিনট্যাক্স প্রদান করে। এগুলি `function` কীওয়ার্ডের পরিবর্তে `=>` ব্যবহার করে।

**ফর্ম্যাট:**
```javascript
const functionName = (parameters) => {
    // কোড ব্লক
    return result;
};
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// অ্যারো ফাংশন যা একটি প্রোডাক্টের ফাইনাল প্রাইস হিসাব করে
const getFinalPrice = (price, discount) => price - (price * discount);

// ব্যবহার
let finalPrice = getFinalPrice(150, 0.05);
console.log(`Final Price: $${finalPrice}`);
```

#### ৪. বেনামী ফাংশন

**বর্ণনা:** বেনামী ফাংশন কোন নাম ছাড়াই সংজ্ঞায়িত হয় এবং সাধারণত অন্য ফাংশনে প্যারামিটার হিসেবে ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
const result = (function() {
    // কোড ব্লক
    return value;
})();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// বেনামী ফাংশন যা একটি প্রোডাক্টের মোট মূল্য হিসাব করে
const total = (function(price, quantity) {
    return price * quantity;
})(20, 5);

console.log(`Total Value: $${total}`);
```

#### ৫. IIFE (ইমিডিয়েটলি ইনভোকড ফাংশন এক্সপ্রেশন)

**বর্ণনা:** IIFE একটি ফাংশন যা ডিক্লেয়ার হওয়ার সাথে সাথেই চালিত হয়। এটি একটি একক ইন্সট্যান্স তৈরি করতে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
(function() {
    // কোড ব্লক
})();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একটি IIFE যা ইনভেন্টরি আপডেট করে
(function() {
    const inventory = {
        'item1': 10,
        'item2': 20
    };

    inventory['item1'] -= 1;
    console.log(`Updated Inventory: ${JSON.stringify(inventory)}`);
})();
```

#### ৬. ফাংশন প্যারামিটার এবং আর্গুমেন্ট

**বর্ণনা:** ফাংশনের প্যারামিটারগুলি ফাংশনের মধ্যে ডেটা প্রেরণ করার জন্য ব্যবহৃত হয়, এবং আর্গুমেন্টগুলি সেই প্যারামিটারগুলির জন্য প্রেরিত মান।

**ফর্ম্যাট:**
```javascript
function functionName(param1, param2) {
    // কোড ব্লক
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// প্রোডাক্ট রিভিউ জমা দেওয়ার জন্য ফাংশন
function submitReview(productId, reviewText) {
    console.log(`Review for Product ${productId}: ${reviewText}`);
}

// ব্যবহার
submitReview(123, 'Great product!');
```

#### ৭. ডিফল্ট প্যারামিটার

**বর্ণনা:** ডিফল্ট প্যারামিটারগুলি ফাংশনের প্যারামিটারগুলির জন্য ডিফল্ট মান প্রদান করে।

**ফর্ম্যাট:**
```javascript
function functionName(param1 = defaultValue) {
    // কোড ব্লক
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// ডিফল্ট প্যারামিটার ব্যবহার করে প্রোডাক্টের মূল্য হিসাব করা
function calculateDiscountedPrice(price, discount = 0.1) {
    return price - (price * discount);
}

// ব্যবহার
let price1 = calculateDiscountedPrice(100); // discount ডিফল্ট মান হবে 0.1
let price2 = calculateDiscountedPrice(100, 0.2); // discount 0.2
console.log(`Price with default discount: $${price1}`);
console.log(`Price with custom discount: $${price2}`);
```

#### ৮. রেস্ট প্যারামিটার

**বর্ণনা:** রেস্ট প্যারামিটার একটি ফাংশনে একটি নির্দিষ্ট সংখ্যক আর্গুমেন্ট গ্রহণ করে এবং একটি অ্যারে হিসেবে একত্রিত করে।

**ফর্ম্যাট:**
```javascript
function functionName(...restParams) {
    // কোড ব্লক
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একাধিক প্রোডাক্ট আইডি সহ অর্ডার তৈরি করার জন্য ফাংশন
function createOrder(customerId, ...productIds) {
    console.log(`Order for Customer ${customerId} with Products: ${productIds.join(', ')}`);
}

// ব্যবহার
createOrder(456, 'prod1', 'prod2', 'prod3');
```

#### ৯. রিটার্ন স্টেটমেন্ট

**বর্ণনা:** রিটার্ন স্টেটমেন্ট ফাংশনের ফলাফল ফিরিয়ে দেয়।

**ফর্ম্যাট:**
```javascript
function functionName() {
    return result;
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একটি ফাংশন যা প্রোডাক্টের নাম প্রদান করে
function getProductName(productId) {
    const products = {
        1: 'Laptop',
        2: 'Smartphone',
        3: 'Tablet'
    };
    return products[productId] || 'Unknown Product';
}

// ব্যবহার
console.log(getProductName(1)); // Laptop
console.log(getProductName(4)); // Unknown Product
```

#### ১০. ফাংশন স্কোপ এবং ক্লোজার

**বর্ণনা:** স্কোপ হল ফাংশনের ভেতরের এবং বাইরের ভেরিয়েবলের দৃশ্যমানতা। ক্লোজার হল একটি ফাংশন যা তার স্কোপের পরিবর্তনশীল অ্যাক্সেস করতে পারে।

**ফর্ম্যাট:**
```javascript
function outerFunction() {
    let outerVar = 'I am outside!';
    
    function innerFunction() {
        console.log(outerVar); // innerFunction() ক্লোজার ব্যবহার করছে
    }
    
    return innerFunction;
}

const myFunction = outerFunction();
myFunction(); // 'I am outside!'
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একটি ফাংশন যা প্রোডাক্টের ডিসকাউন্ট ক্যালকুলেটর প্রদান করে
function createDiscountCalculator(discountRate) {
    return function(price) {
        return price - (price * discountRate);
    };
}

const seasonalDiscountCalculator = createDiscountCalculator(0.2);

let originalPrice = 100;
let discountedPrice = seasonalDiscountCalculator(originalPrice);
console.log(`Discounted Price: $${discountedPrice}`);
```

#### ১১. উচ্চতর ক্রমের ফাংশন

**বর্ণনা:** উচ্চতর ক্রমের ফাংশন এমন ফাংশন যা অন্যান্য ফাংশনকে আর্গুমেন্ট হিসেবে গ্রহণ করে অথবা একটি ফাংশন ফেরত দেয়।

**ফর্ম্যাট:**
```javascript
function higherOrderFunction(callback) {
    return callback();
}
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// একটি উচ্চতর ক্রমের ফাংশন যা অন্যান্য ফাংশনকে কল করে
function processOrder(orderId, callback) {
    console.log(`Processing Order ${orderId}`);
    callback();
}

processOrder(123, () => {
    console.log('Order Processed!');
});
```

#### ১২. ফাংশন বাইন্ডিং (bind, call, apply)

**বর্ণ

না:** `bind`, `call`, এবং `apply` ফাংশনের `this` প্রসঙ্গ পরিবর্তন করে। `bind` নতুন ফাংশন তৈরি করে, `call` এবং `apply` সরাসরি কল করে।

**ফর্ম্যাট:**
```javascript
function exampleFunction(arg1, arg2) {
    console.log(this, arg1, arg2);
}

const boundFunction = exampleFunction.bind(context, arg1);
boundFunction();

exampleFunction.call(context, arg1, arg2);
exampleFunction.apply(context, [arg1, arg2]);
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
// প্রোডাক্ট ডিসকাউন্ট ফাংশন যেটি 'this' প্রসঙ্গ ব্যবহার করে
const discountCalculator = {
    discountRate: 0.1,
    calculatePrice(price) {
        return price - (price * this.discountRate);
    }
};

const productPrice = 200;
console.log(`Discounted Price: $${discountCalculator.calculatePrice(productPrice)}`);
```

এই উদাহরণগুলি কোডের বিভিন্ন ফাংশনের কাজ বুঝতে সহায়ক হবে এবং বাস্তব জীবনের ইকমার্স প্রোজেক্টে কীভাবে ফাংশনগুলি ব্যবহার করা যায় তা প্রদর্শন করবে।




### ৭. স্কোপ

স্কোপ হচ্ছে ভেরিয়েবল এবং ফাংশনের দৃশ্যমানতা বা অ্যাক্সেসের পরিধি। এটি নির্ধারণ করে কোন ভেরিয়েবল কোথায় এবং কখন উপলব্ধ। এখানে স্কোপ সম্পর্কিত বিভিন্ন ধারণা এবং বাস্তব উদাহরণ দেয়া হলো।

#### ১. গ্লোবাল স্কোপ

**বর্ণনা:** গ্লোবাল স্কোপে ডিফাইন করা ভেরিয়েবল বা ফাংশন পুরো প্রোগ্রাম জুড়ে যে কোনো স্থানে অ্যাক্সেসযোগ্য।

**ফর্ম্যাট:**
```javascript
let globalVar = 'I am global';

function printGlobal() {
    console.log(globalVar); // অ্যাক্সেসযোগ্য
}

printGlobal();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
let cartItems = []; // গ্লোবাল ভেরিয়েবল

function addToCart(item) {
    cartItems.push(item);
}

addToCart('Laptop');
console.log(cartItems); // ['Laptop']
```

#### ২. লোকাল স্কোপ

**বর্ণনা:** লোকাল স্কোপে ডিফাইন করা ভেরিয়েবল বা ফাংশন শুধুমাত্র ঐ ব্লকের ভিতরেই অ্যাক্সেসযোগ্য।

**ফর্ম্যাট:**
```javascript
function localScopeExample() {
    let localVar = 'I am local';
    console.log(localVar); // অ্যাক্সেসযোগ্য
}

localScopeExample();
console.log(localVar); // Error: localVar is not defined
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function calculateDiscount(price) {
    let discount = 0.1; // লোকাল স্কোপ ভেরিয়েবল
    return price - (price * discount);
}

console.log(calculateDiscount(100)); // 90
console.log(discount); // Error: discount is not defined
```

#### ৩. ব্লক স্কোপ (let, const)

**বর্ণনা:** `let` এবং `const` ব্যবহার করে ডিফাইন করা ভেরিয়েবলগুলি ব্লক স্কোপের অধীনে থাকে, অর্থাৎ তারা শুধু তাদের ডিফাইন করা ব্লকেই অ্যাক্সেসযোগ্য।

**ফর্ম্যাট:**
```javascript
if (true) {
    let blockVar = 'I am block-scoped';
    console.log(blockVar); // অ্যাক্সেসযোগ্য
}

console.log(blockVar); // Error: blockVar is not defined
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function applyCoupon(coupon) {
    if (coupon) {
        const discount = 0.2; // ব্লক স্কোপ ভেরিয়েবল
        return discount;
    }
    return 0;
}

console.log(applyCoupon(true)); // 0.2
console.log(discount); // Error: discount is not defined
```

#### ৪. ফাংশন স্কোপ (var)

**বর্ণনা:** `var` দ্বারা ডিফাইন করা ভেরিয়েবলগুলি ফাংশন স্কোপের অধীনে থাকে। এটি একটি ফাংশনের ভিতরে ডিফাইন করা হলে, শুধু সেই ফাংশনের ভিতরে অ্যাক্সেসযোগ্য।

**ফর্ম্যাট:**
```javascript
function varScopeExample() {
    var functionVar = 'I am function-scoped';
    console.log(functionVar); // অ্যাক্সেসযোগ্য
}

varScopeExample();
console.log(functionVar); // Error: functionVar is not defined
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function processOrder() {
    var orderStatus = 'Processing'; // ফাংশন স্কোপ ভেরিয়েবল
    console.log(orderStatus); // Processing
}

processOrder();
console.log(orderStatus); // Error: orderStatus is not defined
```

#### ৫. স্কোপ চেইন

**বর্ণনা:** স্কোপ চেইন হল একটি ফাংশন কীভাবে তার প্যারেন্ট স্কোপ থেকে ভেরিয়েবল অ্যাক্সেস করে।

**ফর্ম্যাট:**
```javascript
function outerFunction() {
    let outerVar = 'I am outer';

    function innerFunction() {
        console.log(outerVar); // outerVar অ্যাক্সেসযোগ্য
    }

    innerFunction();
}

outerFunction();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
let globalDiscount = 0.05;

function applyDiscount(price) {
    let localDiscount = 0.1;

    function calculateFinalPrice() {
        return price - (price * localDiscount) - (price * globalDiscount);
    }

    return calculateFinalPrice();
}

console.log(applyDiscount(200)); // 155
```

#### ৬. লেক্সিক্যাল স্কোপিং

**বর্ণনা:** লেক্সিক্যাল স্কোপিং হল যেখানে একটি ফাংশনের স্কোপ তার বাইরের স্কোপ দ্বারা নির্ধারিত হয়।

**ফর্ম্যাট:**
```javascript
function outer() {
    let outerVar = 'I am outer';

    function inner() {
        console.log(outerVar); // outerVar লেক্সিক্যাল স্কোপিং দ্বারা অ্যাক্সেসযোগ্য
    }

    inner();
}

outer();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function createTaxCalculator(taxRate) {
    return function(price) {
        return price + (price * taxRate);
    };
}

const salesTaxCalculator = createTaxCalculator(0.07);
console.log(salesTaxCalculator(100)); // 107
```

#### ৭. শ্যাডোইং ভেরিয়েবল

**বর্ণনা:** শ্যাডোইং হল যখন একটি ভেরিয়েবল একটি বাইরের ভেরিয়েবলকে প্রতিস্থাপন করে একই নাম দিয়ে।

**ফর্ম্যাট:**
```javascript
let varName = 'Global';

function testShadowing() {
    let varName = 'Local';
    console.log(varName); // Local
}

testShadowing();
console.log(varName); // Global
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
let discount = 0.05; // গ্লোবাল ডিসকাউন্ট

function applyOrderDiscount(price) {
    let discount = 0.1; // লোকাল ডিসকাউন্ট
    return price - (price * discount);
}

console.log(applyOrderDiscount(200)); // 180
console.log(discount); // 0.05
```

#### ৮. ক্লোজার এবং এর ব্যবহার

**বর্ণনা:** ক্লোজার হল একটি ফাংশন যা তার বাইরের ফাংশনের স্কোপে ডিফাইন করা ভেরিয়েবলগুলিকে অ্যাক্সেস করতে পারে।

**ফর্ম্যাট:**
```javascript
function makeCounter() {
    let count = 0;

    return function() {
        count += 1;
        return count;
    };
}

const counter = makeCounter();
console.log(counter()); // 1
console.log(counter()); // 2
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function createCart() {
    let items = [];

    return {
        addItem(item) {
            items.push(item);
            console.log(`${item} added to cart.`);
        },
        getItems() {
            return items;
        }
    };
}

const cart = createCart();
cart.addItem('Smartphone');
console.log(cart.getItems()); // ['Smartphone']
```

#### ৯. ভেরিয়েবল হোইস্টিং বিভিন্ন স্কোপে

**বর্ণনা:** ভেরিয়েবল হোইস্টিং হল JavaScript-এ ভেরিয়েবলের ঘোষণা স্বয়ংক্রিয়ভাবে উপরের দিকে স্থানান্তরিত হয়।

**ফর্ম্যাট:**
```javascript
function hoistingExample() {
    console.log(hoistedVar); // undefined
    var hoistedVar = 'I am hoisted';
    console.log(hoistedVar); // I am hoisted
}

hoistingExample();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function checkOrderStatus() {
    console.log(status); // undefined
    var status = 'Pending';
    console.log(status); // Pending
}

checkOrderStatus();
```

#### ১০. স্ট্রিক্ট মোড এবং স্কোপ

**বর্ণনা:** স্ট্রিক্ট মোড কোডের কিছু ভুল বা অস্বাভাবিক আচরণকে প্রতিরোধ করে এবং ভেরিয়েবল ঘোষণা করার সময় স্কোপকে আরো কঠোরভাবে নিয়ন্ত্রণ করে।

**ফর্ম্যাট:**
```javascript
'use strict';

function strictModeExample() {
    // let এবং const ব্যবহারে কোনো ভুল হবে না
    let strictVar = 'Strict Mode';
    console.log(strictVar);
}

strictModeExample();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
'use strict';

function calculateTotal(price, quantity) {
    // `undeclaredVariable` ব্যবহার করা যাবে না
    let total = price * quantity;
    return total;
}

console.log(calculateTotal(100, 3)); // 300
```

#### ১১. অ্যারো ফাংশন বনাম নিয়মিত ফাংশনগুলিতে স্কোপ

**বর্ণনা:** অ্যারো ফাংশনগুলি তাদের প্যারেন্ট স্কোপের `this` ব্যবহার করে, নিয়মিত ফাংশনগুলি তাদের নিজস্ব `this` তৈরি করে।

**ফর্ম্যাট:**
```javascript
const regularFunction = function() {
    console.log(this); // ফাংশনের কল করার প্রেক্ষিতে `this` নির্ধারিত হবে
};

const arrowFunction = () => {
    console.log(this); // অ্যারো ফাংশ

ন প্যারেন্ট স্কোপের `this` ব্যবহার করে
};

regularFunction();
arrowFunction();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
const cart = {
    items: ['Laptop', 'Smartphone'],
    printItems: function() {
        this.items.forEach(function(item) {
            console.log(item); // `this` refers to `cart`
        });
    }
};

cart.printItems();

const cartArrow = {
    items: ['Tablet', 'Headphones'],
    printItems: function() {
        this.items.forEach(item => {
            console.log(item); // `this` refers to `cartArrow`
        });
    }
};

cartArrow.printItems();
```

#### ১২. টেম্পোরারি ডেড জোন (TDZ) let এবং const-এর সাথে

**বর্ণনা:** TDZ হল `let` এবং `const` দ্বারা ডিফাইন করা ভেরিয়েবলগুলি তাদের ঘোষণা করার আগে অ্যাক্সেসযোগ্য না হওয়া।

**ফর্ম্যাট:**
```javascript
function tdzExample() {
    console.log(tdzVar); // ReferenceError: Cannot access 'tdzVar' before initialization
    let tdzVar = 'In TDZ';
}

tdzExample();
```

**বাস্তব ইকমার্স উদাহরণ:**
```javascript
function calculateFinalPrice(price) {
    console.log(discount); // ReferenceError: Cannot access 'discount' before initialization
    let discount = 0.1;
    return price - (price * discount);
}

console.log(calculateFinalPrice(100));
```

এই ব্যাখ্যাগুলি এবং কোড উদাহরণগুলি স্কোপ সম্পর্কিত বিভিন্ন ধারণা এবং তাদের বাস্তব ব্যবহার বুঝতে সহায়ক হবে।



### ৮. হোইস্টিং

**হোইস্টিং** হল জাভাস্ক্রিপ্টের একটি আচরণ যেখানে ভেরিয়েবল এবং ফাংশনের ডিক্লারেশন তাদের স্কোপের শীর্ষে স্থানান্তরিত হয়, চায় সেগুলি কোডের যেকোনো স্থানে ডিক্লার করা হোক না কেন। এর ফলে কোডের কার্যকর হওয়ার আগে ডিক্লারেশনগুলি প্রথমেই প্রক্রিয়াকরণ হয়। তবে এটি শুধুমাত্র ডিক্লারেশনকে উপরে তোলে, না যে ভ্যালু অ্যাসাইনমেন্টকে।

#### ১. **ভেরিয়েবল হোইস্টিং** (var বনাম let/const)

- **var:** `var` দ্বারা ডিক্লার করা ভেরিয়েবলগুলোকে পুরো ফাংশন বা গ্লোবাল স্কোপের শীর্ষে হোইস্ট করা হয়। এটি অ্যাক্সেসযোগ্য হয়, কিন্তু ডিক্লার করার আগে এর মান হয় `undefined`।

**ফর্ম্যাট:** 
```javascript
console.log(hoistedVar); // undefined
var hoistedVar = 'I am hoisted';
console.log(hoistedVar); // I am hoisted
```

- **let/const:** `let` এবং `const` দ্বারা ডিক্লার করা ভেরিয়েবলগুলিও হোইস্ট করা হয়, কিন্তু তারা **টেম্পোরারি ডেড জোনে (TDZ)** অবস্থান করে এবং তাদের অ্যাক্সেস করা যায় না যতক্ষণ না তারা ডিক্লার হয়।

**ফর্ম্যাট:** 
```javascript
console.log(hoistedLet); // ReferenceError: Cannot access 'hoistedLet' before initialization
let hoistedLet = 'I am not hoisted';

console.log(hoistedConst); // ReferenceError: Cannot access 'hoistedConst' before initialization
const hoistedConst = 'I am not hoisted';
```

#### ২. **ফাংশন হোইস্টিং**

ফাংশন ডিক্লারেশন সম্পূর্ণরূপে হোইস্ট করা হয়, যার মানে আপনি ফাংশনটিকে ডিক্লার করার আগে কল করতে পারেন।

**ফর্ম্যাট:** 
```javascript
console.log(add(2, 3)); // 5

function add(a, b) {
    return a + b;
}
```

#### ৩. **হোইস্টিং অর্ডার**

হোইস্টিংয়ের অর্ডার সাধারণত নিচের মতো হয়:
1. প্রথমে **ফাংশন ডিক্লারেশন** হোইস্ট করা হয়।
2. তারপর **var ডিক্লারেশন** হোইস্ট করা হয়।
3. এরপর **let/const ডিক্লারেশন** হোইস্ট করা হয় কিন্তু তারা টেম্পোরারি ডেড জোনে থাকে।

#### ৪. **টেম্পোরারি ডেড জোন (TDZ) এবং let/const**

**TDZ** হল একটি অবস্থা যেখানে `let` এবং `const` দ্বারা ডিক্লার করা ভেরিয়েবলগুলো ডিক্লার হওয়ার আগে অ্যাক্সেসযোগ্য নয়। এর মানে হলো যে, স্ক্রিপ্টটি চলার আগে কোড ব্লকের মধ্যে তারা অকার্যকর অবস্থায় থাকে।

**ফর্ম্যাট:** 
```javascript
console.log(someLet); // ReferenceError: Cannot access 'someLet' before initialization
let someLet = 'TDZ Example';
```

#### ৫. **হোইস্টিংয়ের ব্যবহারিক উদাহরণ**

ব্যবহারিক উদাহরণে, হোইস্টিং কার্যকরী ফাংশনালিটি এবং ভুল ত্রুটি সম্পর্কে গভীর ধারণা দেয়।

**বাস্তব উদাহরণ:**
```javascript
// ফাংশন হোইস্টিংয়ের ব্যবহার
console.log(calculateTotal(100, 20)); // 120

function calculateTotal(price, tax) {
    return price + tax;
}

// var হোইস্টিংয়ের সমস্যা
console.log(item); // undefined
var item = 'Laptop';

// let/const হোইস্টিংয়ে TDZ
console.log(cart); // ReferenceError: Cannot access 'cart' before initialization
let cart = [];
```

#### ৬. **নেস্টেড স্কোপে হোইস্টিং**

হোইস্টিং নেস্টেড স্কোপে কাজ করে, তবে স্কোপ অনুযায়ী কাজ করে। অর্থাৎ, ভেতরের স্কোপের ভেরিয়েবল বাইরের স্কোপ থেকে আলাদা থাকে।

**ফর্ম্যাট:** 
```javascript
function outer() {
    var outerVar = 'Outer';

    function inner() {
        console.log(outerVar); // Outer
        var innerVar = 'Inner';
    }

    inner();
    console.log(innerVar); // Error: innerVar is not defined
}

outer();
```

#### ৭. **ফাংশন এক্সপ্রেশনগুলির সাথে হোইস্টিং**

ফাংশন এক্সপ্রেশন হোইস্ট করা হয় না। এটি শুধুমাত্র ডিক্লারেশনের পর অ্যাক্সেসযোগ্য হয়।

**ফর্ম্যাট:** 
```javascript
console.log(add); // undefined
var add = function(a, b) {
    return a + b;
};

console.log(add(2, 3)); // 5
```

#### ৮. **অ্যারো ফাংশনগুলির সাথে হোইস্টিং**

অ্যারো ফাংশনগুলিও ফাংশন এক্সপ্রেশনের মতো আচরণ করে এবং হোইস্ট হয় না।

**ফর্ম্যাট:** 
```javascript
console.log(multiply); // undefined
var multiply = (a, b) => a * b;

console.log(multiply(2, 3)); // 6
```

#### ৯. **সাধারণ সমস্যা এবং সমস্যা এড়ানো**

- **var ব্যবহার করলে:** ভেরিয়েবল হোইস্টিং থেকে এড়ানোর জন্য `let` এবং `const` ব্যবহার করা উচিৎ।
- **TDZ ইস্যু:** ভেরিয়েবল এবং ফাংশনগুলি সঠিক ক্রমে ডিক্লার করুন।

#### ১০. **হোইস্টিং সমস্যাগুলি ডিবাগ করা**

- **ReferenceError:** ভেরিয়েবলগুলো ডিক্লার করার আগেই অ্যাক্সেস করতে চাওয়া হলে এই সমস্যা হয়। 
- **undefined:** হোইস্টিংয়ের ফলে `var` ডিক্লারেশন আগে হলেও তার ভ্যালু `undefined` থাকে।

#### ১১. **হোইস্টিং সমস্যাগুলি কমানোর জন্য সেরা অনুশীলন**

- সবসময় ভেরিয়েবলগুলো ডিক্লারেশন ব্লকের উপরের দিকে রাখুন।
- `let` এবং `const` ব্যবহার করুন।
- ফাংশন এক্সপ্রেশনগুলির ক্ষেত্রে ফাংশনগুলো ডিক্লার করার পর ব্যবহার করুন।

#### ১২. **স্কোপ এবং হোইস্টিং পারস্পরিক ক্রিয়া বুঝা**

হোইস্টিং এবং স্কোপ পরস্পর যুক্ত। স্কোপের উপর নির্ভর করে ভেরিয়েবল এবং ফাংশনের হোইস্টিং কাজ করে। গ্লোবাল স্কোপে হোইস্টিং গ্লোবাল লেভেলে ঘটে এবং ফাংশন বা ব্লক স্কোপে হোইস্টিং স্থানীয়ভাবে ঘটে।

**ফর্ম্যাট:** 
```javascript
function hoistingExample() {
    var localVar = 'I am local';
    console.log(globalVar); // undefined (হোইস্টিংয়ের কারণে)
    var globalVar = 'I am global';
}

hoistingExample();
``` 

এই ব্যাখ্যা থেকে হোইস্টিংয়ের বিভিন্ন দিক এবং ব্যবহারিক উদাহরণ পরিষ্কারভাবে বোঝা যাবে।



### ৯. অ্যারেজ (Arrays)

**অ্যারে** হল জাভাস্ক্রিপ্টের একটি ডেটা স্ট্রাকচার যা একাধিক মানকে একটি তালিকায় সংরক্ষণ করতে ব্যবহার করা হয়। এতে ভিন্ন ধরনের ডেটা যেমন সংখ্যা, স্ট্রিং, বুলিয়ান ইত্যাদি রাখা যায়।

#### ১. **অ্যারে তৈরি করা**
অ্যারে তৈরি করতে দুটি উপায় আছে: `Array` কনস্ট্রাক্টর অথবা অ্যারে লিটারাল (`[]`) ব্যবহার করা।

**ফর্ম্যাট:**
```javascript
// Array literal
let arr = [1, 2, 3];

// Array constructor
let arr2 = new Array(4, 5, 6);
```

#### ২. **ইনডেক্স দ্বারা উপাদানগুলি অ্যাক্সেস করা**
অ্যারের উপাদানগুলি ইন্ডেক্স দ্বারা অ্যাক্সেস করা যায়। অ্যারের ইনডেক্স ০ থেকে শুরু হয়।

**ফর্ম্যাট:**
```javascript
let fruits = ['Apple', 'Banana', 'Mango'];
console.log(fruits[0]); // Apple
```

#### ৩. **উপাদানগুলি সংশোধন করা**
ইনডেক্স ব্যবহার করে অ্যারের উপাদানগুলিকে সহজেই সংশোধন করা যায়।

**ফর্ম্যাট:**
```javascript
fruits[1] = 'Orange';
console.log(fruits); // ['Apple', 'Orange', 'Mango']
```

#### ৪. **অ্যারে দৈর্ঘ্য প্রোপার্টি**
`length` প্রোপার্টির মাধ্যমে অ্যারের মোট উপাদান সংখ্যা জানা যায়।

**ফর্ম্যাট:**
```javascript
console.log(fruits.length); // 3
```

#### ৫. **উপাদানগুলি যোগ করা (push, unshift)**

- **push:** অ্যারের শেষে উপাদান যোগ করে।
- **unshift:** অ্যারের শুরুতে উপাদান যোগ করে।

**ফর্ম্যাট:**
```javascript
fruits.push('Grapes');
console.log(fruits); // ['Apple', 'Orange', 'Mango', 'Grapes']

fruits.unshift('Pineapple');
console.log(fruits); // ['Pineapple', 'Apple', 'Orange', 'Mango', 'Grapes']
```

#### ৬. **উপাদানগুলি সরানো (pop, shift)**

- **pop:** অ্যারের শেষ উপাদান সরিয়ে দেয়।
- **shift:** অ্যারের প্রথম উপাদান সরিয়ে দেয়।

**ফর্ম্যাট:**
```javascript
fruits.pop();
console.log(fruits); // ['Pineapple', 'Apple', 'Orange', 'Mango']

fruits.shift();
console.log(fruits); // ['Apple', 'Orange', 'Mango']
```

#### ৭. **অ্যারে স্লাইস করা (slice মেথড)**

`slice` মেথড নির্দিষ্ট ইনডেক্স থেকে একটি অংশ কপি করে নতুন অ্যারে তৈরি করে। এটি মূল অ্যারেকে পরিবর্তন করে না।

**ফর্ম্যাট:**
```javascript
let slicedFruits = fruits.slice(1, 3);
console.log(slicedFruits); // ['Orange', 'Mango']
```

#### ৮. **অ্যারে স্প্লাইস করা (splice মেথড)**

`splice` মেথড নির্দিষ্ট ইনডেক্স থেকে উপাদান মুছে ফেলে এবং চাইলে নতুন উপাদান যোগ করে। এটি মূল অ্যারেকে পরিবর্তন করে।

**ফর্ম্যাট:**
```javascript
fruits.splice(1, 1, 'Strawberry');
console.log(fruits); // ['Apple', 'Strawberry', 'Mango']
```

#### ৯. **উপাদানগুলি খুঁজে পাওয়া (indexOf, lastIndexOf, includes)**

- **indexOf:** প্রথম ম্যাচ করা ইনডেক্স প্রদান করে।
- **lastIndexOf:** শেষ ম্যাচ করা ইনডেক্স প্রদান করে।
- **includes:** উপাদানটি অ্যারেতে আছে কিনা তা বলে।

**ফর্ম্যাট:**
```javascript
console.log(fruits.indexOf('Mango')); // 2
console.log(fruits.lastIndexOf('Mango')); // 2
console.log(fruits.includes('Apple')); // true
```

#### ১০. **অ্যারের উপর ইটারেশন (for লুপ, forEach, map)**

- **for লুপ:** অ্যারের উপরে লুপ চালিয়ে উপাদানগুলি অ্যাক্সেস করা যায়।
- **forEach:** প্রতিটি উপাদানে কলব্যাক ফাংশন প্রয়োগ করে।
- **map:** প্রতিটি উপাদানের উপর কলব্যাক ফাংশন প্রয়োগ করে এবং একটি নতুন অ্যারে রিটার্ন করে।

**ফর্ম্যাট:**
```javascript
// for loop
for (let i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}

// forEach
fruits.forEach(function(fruit) {
    console.log(fruit);
});

// map
let upperFruits = fruits.map(fruit => fruit.toUpperCase());
console.log(upperFruits); // ['APPLE', 'STRAWBERRY', 'MANGO']
```

#### ১১. **অ্যারে ফিল্টারিং (filter মেথড)**

`filter` মেথড একটি শর্ত অনুযায়ী অ্যারের উপাদান ফিল্টার করে এবং একটি নতুন অ্যারে প্রদান করে।

**ফর্ম্যাট:**
```javascript
let numbers = [1, 2, 3, 4, 5];
let evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // [2, 4]
```

#### ১২. **অ্যারে রিডিউস করা (reduce মেথড)**

`reduce` মেথড একটি অ্যারের উপাদানগুলিকে একক মানে রিডিউস করে।

**ফর্ম্যাট:**
```javascript
let sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum); // 15
```

### বাস্তব উদাহরণ (ইকমার্স)
একটি ইকমার্স অ্যাপ্লিকেশনে অ্যারেগুলির ব্যবহার হতে পারে যেমন পণ্যগুলির একটি তালিকা পরিচালনা করা, কার্টে পণ্য যোগ করা বা সরানো ইত্যাদি।

**বাস্তব উদাহরণ:**
```javascript
let cart = [];

// পণ্য যোগ করা
function addToCart(product) {
    cart.push(product);
    console.log(`${product} added to cart`);
}

// পণ্য সরানো
function removeFromCart(product) {
    let index = cart.indexOf(product);
    if (index > -1) {
        cart.splice(index, 1);
        console.log(`${product} removed from cart`);
    } else {
        console.log(`${product} is not in the cart`);
    }
}

// কার্টে পণ্য যোগ এবং সরানোর উদাহরণ
addToCart('Laptop');
addToCart('Phone');
console.log(cart); // ['Laptop', 'Phone']

removeFromCart('Phone');
console.log(cart); // ['Laptop']
```

এই উদাহরণে, অ্যারে দিয়ে পণ্যের তালিকা ম্যানেজ করা হয়েছে। `push` মেথড দিয়ে পণ্য যোগ করা হয়েছে এবং `splice` মেথড দিয়ে সরানো হয়েছে।




### ১০. স্ট্রিংস (Strings)

**স্ট্রিং** জাভাস্ক্রিপ্টে এক বা একাধিক অক্ষরের একটি সিকোয়েন্স। স্ট্রিং ব্যবহার করে টেক্সট ম্যানিপুলেশন এবং প্রসেসিং করা যায়। স্ট্রিং একবার তৈরি হলে তা অপরিবর্তনীয় হয় (immutable)।

#### ১. **স্ট্রিং তৈরি করা (একক কোটস, ডবল কোটস, ব্যাকটিক্স)**

স্ট্রিং তৈরি করার জন্য তিনটি পদ্ধতি রয়েছে: একক কোটস, ডবল কোটস, এবং ব্যাকটিক্স।

**ফর্ম্যাট:**
```javascript
let singleQuoteStr = 'Hello, World!';
let doubleQuoteStr = "Hello, World!";
let backtickStr = `Hello, World!`; // Template literal
```

#### ২. **অক্ষরগুলি পালানো**

স্ট্রিংয়ের বিশেষ অক্ষরগুলি পালানোর জন্য ব্যাকস্ল্যাশ (`\`) ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let str = 'It\'s a beautiful day!'; // একক কোটস পালানো
let str2 = "He said, \"Hello!\""; // ডবল কোটস পালানো
```

#### ৩. **স্ট্রিং দৈর্ঘ্য প্রোপার্টি**

`length` প্রোপার্টি দিয়ে স্ট্রিংয়ের মোট অক্ষরের সংখ্যা জানা যায়।

**ফর্ম্যাট:**
```javascript
let message = "Hello, JavaScript!";
console.log(message.length); // 18
```

#### ৪. **ইনডেক্স দ্বারা অক্ষরগুলি অ্যাক্সেস করা**

স্ট্রিংয়ের প্রতিটি অক্ষরের ইন্ডেক্স থাকে, যা ০ থেকে শুরু হয়। ইন্ডেক্স ব্যবহার করে স্ট্রিংয়ের নির্দিষ্ট অক্ষর অ্যাক্সেস করা যায়।

**ফর্ম্যাট:**
```javascript
console.log(message[0]); // 'H'
console.log(message.charAt(1)); // 'e'
```

#### ৫. **স্ট্রিং মেথডগুলি (charAt, charCodeAt, fromCharCode)**

- **`charAt`**: একটি নির্দিষ্ট ইনডেক্সের অক্ষর প্রদান করে।
- **`charCodeAt`**: একটি নির্দিষ্ট ইনডেক্সের অক্ষরের ইউনিকোড মান প্রদান করে।
- **`fromCharCode`**: একটি ইউনিকোড মান থেকে একটি স্ট্রিং তৈরি করে।

**ফর্ম্যাট:**
```javascript
console.log(message.charAt(0)); // 'H'
console.log(message.charCodeAt(0)); // 72
console.log(String.fromCharCode(72)); // 'H'
```

#### ৬. **স্ট্রিং সংযোজন (concat, + অপারেটর)**

স্ট্রিং সংযোজনের জন্য দুটি পদ্ধতি রয়েছে:
- **concat()** মেথড
- **+** অপারেটর

**ফর্ম্যাট:**
```javascript
let str1 = "Hello";
let str2 = "World";

console.log(str1.concat(", ", str2, "!")); // 'Hello, World!'
console.log(str1 + ", " + str2 + "!"); // 'Hello, World!'
```

#### ৭. **স্ট্রিং স্লাইস করা (slice, substring, substr)**

স্ট্রিংয়ের অংশ বের করার জন্য বিভিন্ন মেথড রয়েছে:
- **slice(start, end)**: নির্দিষ্ট অংশ বের করে, কিন্তু মূল স্ট্রিং পরিবর্তন করে না।
- **substring(start, end)**: স্ট্রিংয়ের অংশ বের করে, তবে নেগেটিভ ইনডেক্স সমর্থন করে না।
- **substr(start, length)**: নির্দিষ্ট অংশ নির্দিষ্ট দৈর্ঘ্যের জন্য বের করে।

**ফর্ম্যাট:**
```javascript
let text = "JavaScript Programming";
console.log(text.slice(0, 10)); // 'JavaScript'
console.log(text.substring(11, 22)); // 'Programming'
console.log(text.substr(0, 4)); // 'Java'
```

#### ৮. **স্ট্রিংয়ের মধ্যে অনুসন্ধান করা (indexOf, lastIndexOf, includes)**

- **indexOf**: নির্দিষ্ট অক্ষরের প্রথম উপস্থিতির ইনডেক্স প্রদান করে।
- **lastIndexOf**: নির্দিষ্ট অক্ষরের শেষ উপস্থিতির ইনডেক্স প্রদান করে।
- **includes**: নির্দিষ্ট অক্ষর বা স্ট্রিংটি আছে কিনা তা যাচাই করে।

**ফর্ম্যাট:**
```javascript
console.log(text.indexOf('Script')); // 4
console.log(text.lastIndexOf('a')); // 3
console.log(text.includes('Java')); // true
```

#### ৯. **স্ট্রিং অংশগুলি প্রতিস্থাপন করা (replace, replaceAll)**

- **replace()**: প্রথম ম্যাচ করা অংশটি প্রতিস্থাপন করে।
- **replaceAll()**: স্ট্রিংয়ের সব ম্যাচ করা অংশ প্রতিস্থাপন করে।

**ফর্ম্যাট:**
```javascript
let sentence = "I love programming. Programming is fun.";
console.log(sentence.replace('Programming', 'JavaScript')); // 'I love programming. JavaScript is fun.'
console.log(sentence.replaceAll('Programming', 'JavaScript')); // 'I love JavaScript. JavaScript is fun.'
```

#### ১০. **কেস পরিবর্তন করা (toUpperCase, toLowerCase)**

- **toUpperCase()**: স্ট্রিংয়ের সব অক্ষর বড় হাতের করে দেয়।
- **toLowerCase()**: স্ট্রিংয়ের সব অক্ষর ছোট হাতের করে দেয়।

**ফর্ম্যাট:**
```javascript
console.log(text.toUpperCase()); // 'JAVASCRIPT PROGRAMMING'
console.log(text.toLowerCase()); // 'javascript programming'
```

#### ১১. **স্ট্রিং স্প্লিট করা (split মেথড)**

`split()` মেথড স্ট্রিংটিকে নির্দিষ্ট বিভাজকের মাধ্যমে একটি অ্যারেতে ভাগ করে।

**ফর্ম্যাট:**
```javascript
let sentence2 = "I, love, programming";
let words = sentence2.split(', ');
console.log(words); // ['I', 'love', 'programming']
```

#### ১২. **টেম্পলেট লিটারেলস এবং ইন্টারপোলেশন**

টেম্পলেট লিটারেলস ব্যবহার করে স্ট্রিংয়ের মধ্যে ভেরিয়েবল এবং এক্সপ্রেশনকে সহজেই ইন্টারপোলেট করা যায়। এটি ব্যাকটিক্স (``) ব্যবহার করে তৈরি করা হয়।

**ফর্ম্যাট:**
```javascript
let name = 'John';
let age = 25;
let sentence3 = `My name is ${name} and I am ${age} years old.`;

console.log(sentence3); // 'My name is John and I am 25 years old.'
```

### বাস্তব উদাহরণ (ইকমার্স):

একটি ইকমার্স সাইটে পণ্যের বিবরণ, মূল্য, এবং নামের মত তথ্য প্রক্রিয়া করার জন্য স্ট্রিং ব্যাপকভাবে ব্যবহার করা হয়।

**বাস্তব উদাহরণ:**
```javascript
let productName = "Wireless Mouse";
let productPrice = 25.99;

// টেম্পলেট লিটারেল ব্যবহার করে বিবরণ তৈরি করা
let productDescription = `Product: ${productName}, Price: $${productPrice}`;
console.log(productDescription); // 'Product: Wireless Mouse, Price: $25.99'

// স্ট্রিং ম্যানিপুলেশন
let newDescription = productDescription.replace('Wireless', 'Bluetooth');
console.log(newDescription); // 'Product: Bluetooth Mouse, Price: $25.99'

// স্ট্রিং স্প্লিট এবং ইন্টারপোলেশন ব্যবহার করে
let features = "Lightweight, Durable, Long Battery Life";
let featuresList = features.split(', ');
console.log(`Features of ${productName}: ${featuresList.join(', ')}`);
// 'Features of Wireless Mouse: Lightweight, Durable, Long Battery Life'
``` 

এই উদাহরণে, স্ট্রিং ব্যবহার করে পণ্যের নাম, মূল্য এবং বিবরণ তৈরি করা হয়েছে। `replace`, `split`, এবং টেম্পলেট লিটারেল ব্যবহার করে স্ট্রিং ম্যানিপুলেশন করা হয়েছে।




### ১১. **অবজেক্টস (Objects)**

জাভাস্ক্রিপ্টে **অবজেক্ট** একটি ডেটা স্ট্রাকচার যা কী-মান (key-value) জোড়া আকারে ডেটা সংরক্ষণ করে। অবজেক্টের কী একটি স্ট্রিং বা সিম্বল হতে পারে, আর মান যেকোনো ধরনের ডেটা টাইপ হতে পারে, যেমন: সংখ্যা, স্ট্রিং, ফাংশন, বা এমনকি অন্য অবজেক্ট।

#### ১. **অবজেক্ট তৈরি করা (অবজেক্ট লিটারেলস, new Object)**

অবজেক্ট তৈরি করার দুটি প্রধান উপায় আছে:
- **অবজেক্ট লিটারেলস**: সরাসরি `{}` সিম্বল ব্যবহার করে।
- **new Object()**: জাভাস্ক্রিপ্টের বিল্ট-ইন কন্সট্রাক্টর ব্যবহার করে।

**ফর্ম্যাট:**
```javascript
// অবজেক্ট লিটারেল
let person = {
  name: 'John',
  age: 30,
  job: 'Developer'
};

// new Object() ব্যবহার করে
let car = new Object();
car.brand = 'Toyota';
car.model = 'Corolla';
car.year = 2020;
```

#### ২. **প্রোপার্টিগুলি অ্যাক্সেস করা (ডট নোটেশন, ব্র্যাকেট নোটেশন)**

অবজেক্টের প্রোপার্টি দুটি উপায়ে অ্যাক্সেস করা যায়:
- **ডট নোটেশন**: প্রোপার্টির নাম সরাসরি ব্যবহার করা হয়।
- **ব্র্যাকেট নোটেশন**: প্রোপার্টির নাম একটি স্ট্রিং হিসেবে ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
// ডট নোটেশন
console.log(person.name); // 'John'

// ব্র্যাকেট নোটেশন
console.log(person['job']); // 'Developer'
```

#### ৩. **প্রোপার্টিগুলি সংশোধন করা**

প্রোপার্টির মান পরিবর্তন করতে ডট বা ব্র্যাকেট নোটেশন ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
person.age = 35; // ডট নোটেশন
person['job'] = 'Senior Developer'; // ব্র্যাকেট নোটেশন
console.log(person); // {name: 'John', age: 35, job: 'Senior Developer'}
```

#### ৪. **নতুন প্রোপার্টি যোগ করা**

অবজেক্টে নতুন প্রোপার্টি যোগ করার জন্যও একই ডট বা ব্র্যাকেট নোটেশন ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
person.country = 'USA'; // নতুন প্রোপার্টি যোগ করা
console.log(person.country); // 'USA'
```

#### ৫. **প্রোপার্টি মুছে ফেলা**

`delete` অপারেটর ব্যবহার করে অবজেক্ট থেকে প্রোপার্টি মুছে ফেলা যায়।

**ফর্ম্যাট:**
```javascript
delete person.job; // 'job' প্রোপার্টি মুছে ফেলা
console.log(person); // {name: 'John', age: 35, country: 'USA'}
```

#### ৬. **অবজেক্টের মধ্যে মেথড (ফাংশন প্রোপার্টি)**

অবজেক্টের প্রোপার্টি হিসেবে ফাংশন রাখা যেতে পারে, যা মেথড হিসেবে কাজ করে।

**ফর্ম্যাট:**
```javascript
let user = {
  name: 'Alice',
  greet: function() {
    console.log(`Hello, my name is ${this.name}`);
  }
};

user.greet(); // 'Hello, my name is Alice'
```

#### ৭. **অবজেক্ট মেথডে this কীওয়ার্ড**

অবজেক্টের মেথডের ভেতরে **this** কীওয়ার্ড অবজেক্টটিকে রেফার করে। এটি ব্যবহার করে অবজেক্টের অন্যান্য প্রোপার্টি অ্যাক্সেস করা যায়।

**ফর্ম্যাট:**
```javascript
let employee = {
  name: 'Bob',
  position: 'Manager',
  details: function() {
    return `${this.name} works as a ${this.position}`;
  }
};

console.log(employee.details()); // 'Bob works as a Manager'
```

#### ৮. **অবজেক্ট প্রোপার্টিগুলির উপর ইটারেশন (for...in লুপ, Object.keys, Object.values)**

অবজেক্টের প্রোপার্টির উপর ইটারেট করার জন্য বিভিন্ন পদ্ধতি রয়েছে:
- **for...in** লুপ
- **Object.keys()**: প্রোপার্টির কীসমূহ অ্যারের মধ্যে দেয়।
- **Object.values()**: প্রোপার্টির মানসমূহ অ্যারের মধ্যে দেয়।

**ফর্ম্যাট:**
```javascript
for (let key in person) {
  console.log(key + ": " + person[key]);
}

// Object.keys() এবং Object.values() ব্যবহার করে
console.log(Object.keys(person)); // ['name', 'age', 'country']
console.log(Object.values(person)); // ['John', 35, 'USA']
```

#### ৯. **নেস্টেড অবজেক্ট**

অবজেক্টের ভেতরে আরেকটি অবজেক্ট রাখা যায়, যা নেস্টেড অবজেক্ট হিসেবে পরিচিত।

**ফর্ম্যাট:**
```javascript
let student = {
  name: 'David',
  marks: {
    math: 90,
    science: 85
  }
};

console.log(student.marks.math); // 90
```

#### ১০. **অবজেক্টগুলি কপি করা (Object.assign, স্প্রেড অপারেটর)**

অবজেক্ট কপি করার জন্য দুটি পদ্ধতি:
- **Object.assign()**
- **স্প্রেড অপারেটর**

**ফর্ম্যাট:**
```javascript
let original = {a: 1, b: 2};

// Object.assign() দিয়ে কপি
let copy1 = Object.assign({}, original);

// স্প্রেড অপারেটর দিয়ে কপি
let copy2 = {...original};

console.log(copy1); // {a: 1, b: 2}
console.log(copy2); // {a: 1, b: 2}
```

#### ১১. **অবজেক্ট তুলনা করা**

অবজেক্ট তুলনা করার সময় শুধু তাদের রেফারেন্স তুলনা করা হয়, মান নয়। তাই দুই অবজেক্টের রেফারেন্স সমান হলে তবেই তারা সমান হিসেবে বিবেচিত হবে।

**ফর্ম্যাট:**
```javascript
let obj1 = {a: 1};
let obj2 = {a: 1};
let obj3 = obj1;

console.log(obj1 === obj2); // false, কারণ রেফারেন্স আলাদা
console.log(obj1 === obj3); // true, কারণ রেফারেন্স একই
```

#### ১২. **অবজেক্ট ডিস্ট্রাকচারিং**

অবজেক্ট থেকে নির্দিষ্ট প্রোপার্টি বের করে আনতে **ডিস্ট্রাকচারিং** ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let book = { title: 'JavaScript Guide', author: 'John Doe', year: 2021 };

// ডিস্ট্রাকচারিং
let { title, author } = book;

console.log(title); // 'JavaScript Guide'
console.log(author); // 'John Doe'
```

### বাস্তব উদাহরণ (ই-কমার্স সাইট):

একটি ই-কমার্স সাইটে পণ্যের তথ্য সংরক্ষণ এবং প্রক্রিয়াকরণের জন্য অবজেক্ট ব্যবহার করা যেতে পারে।

**বাস্তব উদাহরণ:**
```javascript
let product = {
  name: 'Laptop',
  price: 1200,
  details: {
    brand: 'Dell',
    model: 'Inspiron 15'
  },
  showDetails: function() {
    console.log(`${this.name} by ${this.details.brand}, Model: ${this.details.model}, Price: $${this.price}`);
  }
};

// প্রোপার্টি অ্যাক্সেস করা
console.log(product.name); // 'Laptop'

// মেথড কল করা
product.showDetails(); // 'Laptop by Dell, Model: Inspiron 15, Price: $1200'

// নতুন প্রোপার্টি যোগ করা
product.stock = 30;
console.log(product.stock); // 30

// অবজেক্ট ডিস্ট্রাকচারিং
let { name, price } = product;
console.log(name, price); // 'Laptop', 1200
``` 

এই উদাহরণে, `product` অবজেক্টের মধ্যে পণ্যের তথ্য সংরক্ষণ করা হয়েছে। মেথড ব্যবহার করে পণ্যের বিবরণ প্রদর্শন করা হয়েছে এবং ডিস্ট্রাকচারিংয়ের মাধ্যমে পণ্যের নির্দিষ্ট তথ্য আলাদা করা হয়েছে।



### ১২. **অবজেক্ট মেথডস (Object Methods)**

জাভাস্ক্রিপ্টে **অবজেক্ট মেথড** হল কিছু বিল্ট-ইন ফাংশন যা অবজেক্টের সাথে কাজ করতে সাহায্য করে, যেমন কপি করা, অবজেক্টের প্রোপার্টিগুলি অ্যাক্সেস করা, বা অবজেক্টের প্রোটোটাইপ সেট করা ইত্যাদি। এখানে বিভিন্ন অবজেক্ট মেথড সম্পর্কে বিস্তারিত আলোচনা করা হয়েছে।

---

#### ১. **Object.assign() মেথড**
`Object.assign()` মেথড ব্যবহার করে একটি বা একাধিক উৎস অবজেক্ট থেকে প্রোপার্টিগুলি একটি টার্গেট অবজেক্টে কপি করা যায়।

**ফর্ম্যাট:**
```javascript
let target = {a: 1};
let source = {b: 2, c: 3};
let result = Object.assign(target, source);
console.log(result); // {a: 1, b: 2, c: 3}
```

---

#### ২. **Object.create() মেথড**
`Object.create()` মেথড ব্যবহার করে একটি নতুন অবজেক্ট তৈরি করা হয়, যা একটি নির্দিষ্ট প্রোটোটাইপ অবজেক্টকে ইনহেরিট করে।

**ফর্ম্যাট:**
```javascript
let proto = {greet: function() { console.log('Hello!'); }};
let newObj = Object.create(proto);
newObj.greet(); // 'Hello!'
```

---

#### ৩. **Object.keys() মেথড**
`Object.keys()` মেথড একটি অবজেক্টের সমস্ত enumerable প্রোপার্টির নাম (key) গুলোকে একটি অ্যারের মধ্যে প্রদান করে।

**ফর্ম্যাট:**
```javascript
let obj = {a: 1, b: 2, c: 3};
let keys = Object.keys(obj);
console.log(keys); // ['a', 'b', 'c']
```

---

#### ৪. **Object.values() মেথড**
`Object.values()` মেথড অবজেক্টের প্রোপার্টিগুলির মানগুলোকে একটি অ্যারের মধ্যে প্রদান করে।

**ফর্ম্যাট:**
```javascript
let obj = {a: 1, b: 2, c: 3};
let values = Object.values(obj);
console.log(values); // [1, 2, 3]
```

---

#### ৫. **Object.entries() মেথড**
`Object.entries()` মেথড অবজেক্টের কী-মান জোড়াগুলোকে (key-value pairs) একটি অ্যারের মধ্যে প্রদান করে। প্রতিটি জোড়া একটি অ্যারের মধ্যে থাকে।

**ফর্ম্যাট:**
```javascript
let obj = {a: 1, b: 2, c: 3};
let entries = Object.entries(obj);
console.log(entries); // [['a', 1], ['b', 2], ['c', 3]]
```

---

#### ৬. **Object.freeze() মেথড**
`Object.freeze()` মেথড একটি অবজেক্টকে ফ্রিজ করে দেয়, যার ফলে অবজেক্টের প্রোপার্টিগুলি আর পরিবর্তন করা যায় না (অর্থাৎ, অবজেক্ট Immutable হয়ে যায়)।

**ফর্ম্যাট:**
```javascript
let obj = {a: 1};
Object.freeze(obj);
obj.a = 2; // পরিবর্তন হবে না
console.log(obj.a); // 1
```

---

#### ৭. **Object.seal() মেথড**
`Object.seal()` মেথড একটি অবজেক্টকে সিল করে দেয়, যার ফলে নতুন প্রোপার্টি যোগ করা বা মুছে ফেলা যায় না, কিন্তু প্রোপার্টির মান পরিবর্তন করা যায়।

**ফর্ম্যাট:**
```javascript
let obj = {a: 1};
Object.seal(obj);
obj.a = 2; // পরিবর্তন হবে
delete obj.a; // মুছে ফেলা যাবে না
console.log(obj.a); // 2
```

---

#### ৮. **Object.defineProperty() মেথড**
`Object.defineProperty()` মেথড ব্যবহার করে অবজেক্টের একটি প্রোপার্টি নির্ধারণ বা সংশোধন করা যায় এবং এর জন্য কনফিগারেবল, এনিউমারেবল, এবং লেখারযোগ্য (writable) প্রোপার্টি সেট করা যায়।

**ফর্ম্যাট:**
```javascript
let obj = {};
Object.defineProperty(obj, 'name', {
  value: 'John',
  writable: false,
  enumerable: true
});
console.log(obj.name); // 'John'
obj.name = 'Doe'; // পরিবর্তন হবে না কারণ writable: false
console.log(obj.name); // 'John'
```

---

#### ৯. **Object.defineProperties() মেথড**
`Object.defineProperties()` মেথড ব্যবহার করে একাধিক প্রোপার্টি একই সময়ে নির্ধারণ করা যায়।

**ফর্ম্যাট:**
```javascript
let obj = {};
Object.defineProperties(obj, {
  name: {
    value: 'John',
    writable: false
  },
  age: {
    value: 30,
    writable: true
  }
});
console.log(obj.name); // 'John'
console.log(obj.age); // 30
```

---

#### ১০. **Object.getOwnPropertyDescriptor() মেথড**
`Object.getOwnPropertyDescriptor()` মেথড একটি নির্দিষ্ট প্রোপার্টির **descriptor** প্রদান করে, যা প্রোপার্টির কনফিগারেবল, এনিউমারেবল, writable, এবং value সম্পর্কে তথ্য প্রদান করে।

**ফর্ম্যাট:**
```javascript
let obj = {name: 'Alice'};
let descriptor = Object.getOwnPropertyDescriptor(obj, 'name');
console.log(descriptor);
/* 
{
  value: 'Alice',
  writable: true,
  enumerable: true,
  configurable: true
}
*/
```

---

#### ১১. **Object.getPrototypeOf() মেথড**
`Object.getPrototypeOf()` মেথড ব্যবহার করে একটি অবজেক্টের প্রোটোটাইপ পাওয়া যায়।

**ফর্ম্যাট:**
```javascript
let obj = {};
let proto = Object.getPrototypeOf(obj);
console.log(proto); // {constructor: ƒ, ...} (অবজেক্টের প্রোটোটাইপ)
```

---

#### ১২. **Object.setPrototypeOf() মেথড**
`Object.setPrototypeOf()` মেথড ব্যবহার করে একটি অবজেক্টের প্রোটোটাইপ সেট করা যায়।

**ফর্ম্যাট:**
```javascript
let proto = {greet: function() { console.log('Hello!'); }};
let obj = {};
Object.setPrototypeOf(obj, proto);
obj.greet(); // 'Hello!'
```

---

### বাস্তব উদাহরণ (ইউজার অবজেক্ট):
```javascript
let user = {
  name: 'David',
  age: 25
};

// Object.assign() দিয়ে নতুন অবজেক্ট তৈরি
let newUser = Object.assign({}, user, {location: 'USA'});
console.log(newUser); // {name: 'David', age: 25, location: 'USA'}

// Object.freeze() দিয়ে অবজেক্ট ফ্রিজ করা
Object.freeze(user);
user.age = 30; // পরিবর্তন হবে না
console.log(user.age); // 25

// Object.entries() দিয়ে কী-মান জোড়া দেখা
console.log(Object.entries(newUser)); 
// [['name', 'David'], ['age', 25], ['location', 'USA']]
``` 

এই কোডে **অবজেক্ট মেথড** এর বিভিন্ন কার্যকলাপ দেখা যায়, যা ব্যবহার করে অবজেক্ট ম্যানেজ করা যায়।




### ১৩. **ডিস্ট্রাকচারিং (Destructuring)**

ডিস্ট্রাকচারিং হলো একটি সুবিধাজনক সিনট্যাক্স যা ব্যবহার করে অ্যারে বা অবজেক্টের মানগুলোকে দ্রুত ভেরিয়েবলে অ্যাসাইন করা যায়। এটি কোডকে আরো সংক্ষিপ্ত ও পড়তে সহজ করে।

#### ১. **অ্যারে ডিস্ট্রাকচারিং (Array Destructuring)**

অ্যারে থেকে মানগুলো আলাদা ভেরিয়েবলে অ্যাসাইন করা যায় সহজেই।

**ফর্ম্যাট:**
```javascript
let numbers = [10, 20, 30];
let [first, second, third] = numbers;
console.log(first); // 10
console.log(second); // 20
console.log(third); // 30
```

---

#### ২. **অবজেক্ট ডিস্ট্রাকচারিং (Object Destructuring)**

অবজেক্ট থেকে প্রোপার্টির মানগুলো ভেরিয়েবলে অ্যাসাইন করা যায়।

**ফর্ম্যাট:**
```javascript
let person = {name: 'John', age: 25};
let {name, age} = person;
console.log(name); // 'John'
console.log(age); // 25
```

---

#### ৩. **ডিফল্ট মান ডিস্ট্রাকচারিংয়ে (Default Values in Destructuring)**

কোনো প্রোপার্টি বা আইটেম না থাকলে ডিফল্ট মান সেট করা যায়।

**ফর্ম্যাট:**
```javascript
let [a = 5, b = 10] = [7];
console.log(a); // 7
console.log(b); // 10

let {x = 100, y = 200} = {x: 50};
console.log(x); // 50
console.log(y); // 200
```

---

#### ৪. **নেস্টেড ডিস্ট্রাকচারিং (Nested Destructuring)**

নেস্টেড অবজেক্ট বা অ্যারে ডিস্ট্রাকচার করা যায় সহজেই।

**ফর্ম্যাট:**
```javascript
let user = {
  name: 'Alice',
  address: {
    city: 'Wonderland',
    country: 'Imagination'
  }
};
let {name, address: {city, country}} = user;
console.log(name); // 'Alice'
console.log(city); // 'Wonderland'
console.log(country); // 'Imagination'
```

---

#### ৫. **ডিস্ট্রাকচারিংয়ে ভেরিয়েবল পুনঃনামকরণ (Renaming Variables in Destructuring)**

ডিস্ট্রাকচারিংয়ের সময় ভেরিয়েবলের নাম পরিবর্তন করা যায়।

**ফর্ম্যাট:**
```javascript
let user = {name: 'Bob', age: 30};
let {name: userName, age: userAge} = user;
console.log(userName); // 'Bob'
console.log(userAge); // 30
```

---

#### ৬. **ফাংশন প্যারামিটারে ডিস্ট্রাকচারিং (Destructuring in Function Parameters)**

ফাংশনের প্যারামিটারে ডিস্ট্রাকচারিং ব্যবহার করা যায়।

**ফর্ম্যাট:**
```javascript
function display({name, age}) {
  console.log(`Name: ${name}, Age: ${age}`);
}

let person = {name: 'Charlie', age: 22};
display(person); // 'Name: Charlie, Age: 22'
```

---

#### ৭. **ডিস্ট্রাকচারিং ব্যবহার করে ভেরিয়েবল সুইচ করা (Switching Variables Using Destructuring)**

ডিস্ট্রাকচারিং ব্যবহার করে ভেরিয়েবলগুলো সহজেই সুইচ করা যায়।

**ফর্ম্যাট:**
```javascript
let a = 1, b = 2;
[a, b] = [b, a];
console.log(a); // 2
console.log(b); // 1
```

---

#### ৮. **অ্যারে ডিস্ট্রাকচারিংয়ে আইটেমগুলি স্কিপ করা (Skipping Items in Array Destructuring)**

অ্যারের নির্দিষ্ট আইটেমগুলো স্কিপ করা যায় ডিস্ট্রাকচারিংয়ের সময়।

**ফর্ম্যাট:**
```javascript
let numbers = [10, 20, 30, 40];
let [first, , third] = numbers;
console.log(first); // 10
console.log(third); // 30
```

---

#### ৯. **ডিস্ট্রাকচারিংয়ের সাথে রেস্ট অপারেটর মেশানো (Combining Rest Operator with Destructuring)**

`rest` অপারেটর ব্যবহার করে বাকি আইটেমগুলো একটি অ্যারেতে সংগ্রহ করা যায়।

**ফর্ম্যাট:**
```javascript
let [first, second, ...rest] = [1, 2, 3, 4, 5];
console.log(first); // 1
console.log(second); // 2
console.log(rest); // [3, 4, 5]
```

---

#### ১০. **ডিস্ট্রাকচারিংয়ের ব্যবহারিক উদাহরণ (Practical Example of Destructuring)**

ডিস্ট্রাকচারিং বাস্তব কোডে প্রায়ই ব্যবহার হয়। নিচে একটি উদাহরণ:

**ফর্ম্যাট:**
```javascript
let response = {
  status: 'success',
  data: {
    user: {
      name: 'David',
      age: 28
    }
  }
};

let {status, data: {user: {name, age}}} = response;
console.log(status); // 'success'
console.log(name); // 'David'
console.log(age); // 28
```

---

#### ১১. **লুপে ডিস্ট্রাকচারিং (Destructuring in Loops)**

লুপের মধ্যে ডিস্ট্রাকচারিং ব্যবহার করে অ্যারের আইটেমগুলো সহজে অ্যাক্সেস করা যায়।

**ফর্ম্যাট:**
```javascript
let users = [
  {name: 'John', age: 25},
  {name: 'Jane', age: 22},
  {name: 'Doe', age: 30}
];

for (let {name, age} of users) {
  console.log(`${name} is ${age} years old.`);
}
// 'John is 25 years old.'
// 'Jane is 22 years old.'
// 'Doe is 30 years old.'
```

---

#### ১২. **এক্সপ্রেশনে ডিস্ট্রাকচারিং অ্যাসাইনমেন্ট (Destructuring Assignment in Expressions)**

এক্সপ্রেশনের ভিতরেও ডিস্ট্রাকচারিং ব্যবহার করা যায়।

**ফর্ম্যাট:**
```javascript
let x, y;
({x, y} = {x: 10, y: 20});
console.log(x); // 10
console.log(y); // 20
```

---

### সারসংক্ষেপ:
ডিস্ট্রাকচারিং ব্যবহার করে আমরা খুব সহজেই অ্যারে ও অবজেক্ট থেকে ভেরিয়েবলে মান অ্যাসাইন করতে পারি, ফাংশনে প্যারামিটার পাস করতে পারি, এবং আরও অনেক কিছু করতে পারি। এটি জাভাস্ক্রিপ্টে কোডকে সংক্ষিপ্ত ও পরিষ্কার করে তুলতে গুরুত্বপূর্ণ ভূমিকা পালন করে।




### ১৫. **জেসন (JSON)**

#### ১. **JSON কী?**
JSON (JavaScript Object Notation) হলো ডেটা বিনিময়ের জন্য হালকা এবং মানব-পাঠযোগ্য একটি ফরম্যাট। এটি মূলত জাভাস্ক্রিপ্ট অবজেক্ট লিটারেলের উপর ভিত্তি করে তৈরি করা হয়েছে এবং অন্যান্য প্রোগ্রামিং ভাষায়ও সমর্থিত।

#### ২. **JSON সিনট্যাক্স নিয়ম**

- JSON-এ ডেটা কী এবং ভ্যালুর আকারে থাকে (key/value pair)।
- কী সর্বদা ডাবল কোট ("") এর মধ্যে থাকে।
- ভ্যালু সংখ্যা, স্ট্রিং, বুলিয়ান, অ্যারে, অবজেক্ট বা `null` হতে পারে।
- অবজেক্ট `{}` দ্বারা সীমাবদ্ধ এবং অ্যারে `[]` দ্বারা সীমাবদ্ধ।

**ফর্ম্যাট:**
```json
{
  "name": "John",
  "age": 30,
  "isStudent": false,
  "courses": ["Math", "Science"],
  "address": {
    "city": "New York",
    "zip": "10001"
  }
}
```

---

#### ৩. **JSON.parse দিয়ে JSON পার্সিং**

JSON স্ট্রিংকে জাভাস্ক্রিপ্ট অবজেক্টে রূপান্তর করার জন্য `JSON.parse()` মেথডটি ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
let jsonString = '{"name": "John", "age": 30}';
let obj = JSON.parse(jsonString);
console.log(obj.name); // "John"
console.log(obj.age);  // 30
```

---

#### ৪. **JSON.stringify দিয়ে JSON স্ট্রিংফাইং**

জাভাস্ক্রিপ্ট অবজেক্টকে JSON স্ট্রিংয়ে রূপান্তর করার জন্য `JSON.stringify()` মেথডটি ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
let person = {name: "John", age: 30};
let jsonString = JSON.stringify(person);
console.log(jsonString); // '{"name":"John","age":30}'
```

---

#### ৫. **JSON এর সাধারণ ব্যবহার**

JSON সাধারণত API থেকে ডেটা পাঠানোর জন্য বা ডেটা স্টোর করার জন্য ব্যবহৃত হয়। এটি ডেটার বিনিময়ে দ্রুত এবং সহজ।

**ফর্ম্যাট:**
```javascript
let data = {
  name: "John",
  age: 30,
  hobbies: ["Reading", "Gaming"]
};

let jsonData = JSON.stringify(data); // সার্ভারে পাঠানোর জন্য
let parsedData = JSON.parse(jsonData); // সার্ভার থেকে প্রাপ্ত ডেটা পার্স করার জন্য
```

---

#### ৬. **নেস্টেড JSON অবজেক্ট**

নেস্টেড JSON অবজেক্টে অবজেক্টের ভিতরে অবজেক্ট বা অ্যারে থাকতে পারে।

**ফর্ম্যাট:**
```json
{
  "name": "John",
  "age": 30,
  "address": {
    "street": "123 Main St",
    "city": "New York"
  },
  "hobbies": ["Reading", "Swimming"]
}
```

---

#### ৭. **JSON বনাম জাভাস্ক্রিপ্ট অবজেক্ট**

- JSON ডেটা ফরম্যাট এবং জাভাস্ক্রিপ্ট অবজেক্ট প্রোগ্রামিং স্ট্রাকচার।
- JSON শুধুমাত্র স্ট্রিং ফরম্যাটে থাকে, কিন্তু জাভাস্ক্রিপ্ট অবজেক্ট ভিন্ন ধরনের ডেটা রাখে এবং মেথড থাকে।
  
**ফর্ম্যাট:**
```javascript
// জাভাস্ক্রিপ্ট অবজেক্ট
let person = {name: "John", age: 30};

// JSON স্ট্রিং
let jsonPerson = '{"name": "John", "age": 30}';
```

---

#### ৮. **JSON পার্সিংয়ে ত্রুটি পরিচালনা**

JSON পার্সিংয়ে কোনো সমস্যা থাকলে `try...catch` ব্যবহার করে তা হ্যান্ডেল করা যায়।

**ফর্ম্যাট:**
```javascript
let invalidJson = '{"name": "John", "age": 30,'; // ভুল JSON

try {
  let person = JSON.parse(invalidJson);
} catch (error) {
  console.error("Invalid JSON:", error);
}
```

---

#### ৯. **গভীর কপি অবজেক্টের জন্য JSON মেথড**

গভীর কপি তৈরির জন্য JSON.stringify() এবং JSON.parse() এর সমন্বয় ব্যবহার করা যেতে পারে।

**ফর্ম্যাট:**
```javascript
let obj = {name: "John", address: {city: "New York"}};
let deepCopy = JSON.parse(JSON.stringify(obj));

deepCopy.address.city = "Boston";
console.log(obj.address.city); // "New York"
console.log(deepCopy.address.city); // "Boston"
```

---

#### ১০. **API থেকে JSON ডেটার সাথে কাজ করা**

API থেকে প্রাপ্ত JSON ডেটা প্রায়শই `fetch()` মেথডের মাধ্যমে প্রাপ্ত হয় এবং JSON.parse দিয়ে অবজেক্টে রূপান্তর করা হয়।

**ফর্ম্যাট:**
```javascript
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => {
    console.log(data);
  })
  .catch(error => console.error('Error:', error));
```

---

#### ১১. **জটিল জাভাস্ক্রিপ্ট অবজেক্টগুলি JSON-এ রূপান্তর করা**

জটিল অবজেক্ট, যেমন ফাংশন বা undefined প্রোপার্টি যুক্ত থাকলে JSON.stringify() ব্যবহার করে তা JSON এ রূপান্তর করা যাবে না।

**ফর্ম্যাট:**
```javascript
let complexObj = {
  name: "John",
  age: undefined, // JSON-এ এটি অন্তর্ভুক্ত হবে না
  greet: function() { console.log("Hello!"); } // ফাংশন অন্তর্ভুক্ত হবে না
};

let jsonStr = JSON.stringify(complexObj);
console.log(jsonStr); // '{"name":"John"}'
```

---

#### ১২. **JSON ব্যবহারের ব্যবহারিক উদাহরণ**

JSON প্রায়ই কনফিগারেশন ফাইল, API ডেটা ট্রান্সমিশন এবং স্থানীয় ডেটা স্টোরেজে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
// লোকাল স্টোরেজে JSON ডেটা সংরক্ষণ
let user = {name: "Alice", age: 25};
localStorage.setItem("user", JSON.stringify(user));

// লোকাল স্টোরেজ থেকে JSON ডেটা পুনরুদ্ধার
let storedUser = JSON.parse(localStorage.getItem("user"));
console.log(storedUser.name); // "Alice"
```

---

### সারসংক্ষেপ:
JSON হলো ডেটা বিনিময়ের জন্য একটি প্রমিত ফরম্যাট, যা সহজেই জাভাস্ক্রিপ্ট এবং অন্যান্য প্রোগ্রামিং ভাষার সাথে ব্যবহার করা যায়। `JSON.parse()` এবং `JSON.stringify()` এর মাধ্যমে জাভাস্ক্রিপ্ট অবজেক্ট এবং JSON স্ট্রিং এর মধ্যে পরিবর্তন করা যায়।



### ১৬. **তারিখ এবং সময়**

#### ১. **Date অবজেক্ট তৈরি করা**

JavaScript-এ তারিখ এবং সময় পরিচালনা করার জন্য `Date` অবজেক্ট ব্যবহৃত হয়। নতুন `Date` অবজেক্ট তৈরি করার জন্য `Date` কনস্ট্রাক্টর ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
// বর্তমান তারিখ ও সময়
let now = new Date();
console.log(now); // যেমন: 2024-09-06T12:00:00.000Z

// নির্দিষ্ট তারিখ ও সময়
let specificDate = new Date('2024-09-06T12:00:00');
console.log(specificDate); // 2024-09-06T12:00:00.000Z

// নির্দিষ্ট বছর, মাস, দিন, ঘন্টা, মিনিট, সেকেন্ড
let dateFromComponents = new Date(2024, 8, 6, 12, 0, 0); // মাস 0 থেকে শুরু হয়
console.log(dateFromComponents); // 2024-09-06T12:00:00.000Z
```

---

#### ২. **বর্তমান তারিখ এবং সময় প্রাপ্তি**

বর্তমান তারিখ ও সময় প্রাপ্তি খুবই সহজ।

**ফর্ম্যাট:**
```javascript
let now = new Date();
console.log(now); // যেমন: 2024-09-06T12:00:00.000Z
```

---

#### ৩. **individual তারিখ উপাদান প্রাপ্তি (বছর, মাস, দিন, ইত্যাদি)**

`Date` অবজেক্ট থেকে নির্দিষ্ট তারিখ উপাদানগুলি প্রাপ্তি।

**ফর্ম্যাট:**
```javascript
let now = new Date();

let year = now.getFullYear();   // 2024
let month = now.getMonth();     // 8 (সেপ্টেম্বর, 0 থেকে শুরু হয়)
let day = now.getDate();        // 6
let hours = now.getHours();     // 12
let minutes = now.getMinutes(); // 0
let seconds = now.getSeconds(); // 0

console.log(`Year: ${year}, Month: ${month + 1}, Day: ${day}, Hours: ${hours}, Minutes: ${minutes}, Seconds: ${seconds}`);
```

---

#### ৪. **individual তারিখ উপাদান সেট করা**

তারিখ উপাদানগুলি সেট করার জন্য `set` মেথড ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let date = new Date();
date.setFullYear(2025);
date.setMonth(11); // ডিসেম্বার
date.setDate(25);

console.log(date); // 2025-12-25T00:00:00.000Z
```

---

#### ৫. **তারিখ ফরম্যাটিং (toDateString, toISOString, ইত্যাদি)**

`Date` অবজেক্টের বিভিন্ন ফরম্যাটিং মেথড ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let date = new Date();

console.log(date.toDateString());  // "Fri Sep 06 2024"
console.log(date.toISOString());    // "2024-09-06T12:00:00.000Z"
console.log(date.toLocaleDateString()); // "9/6/2024" (লোকাল কনফিগারেশন অনুযায়ী)
```

---

#### ৬. **তারিখ স্ট্রিং পার্স করা**

স্ট্রিং থেকে তারিখ অবজেক্ট তৈরি করার জন্য `Date` কনস্ট্রাক্টর ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let dateString = '2024-09-06T12:00:00';
let date = new Date(dateString);
console.log(date); // 2024-09-06T12:00:00.000Z
```

---

#### ৭. **তারিখ তুলনা**

তারিখ তুলনা করতে সাধারণত দুইটি `Date` অবজেক্টের তুলনা করা হয়।

**ফর্ম্যাট:**
```javascript
let date1 = new Date('2024-09-06');
let date2 = new Date('2024-09-07');

if (date1 < date2) {
  console.log("date1 is before date2");
} else if (date1 > date2) {
  console.log("date1 is after date2");
} else {
  console.log("date1 is the same as date2");
}
```

---

#### ৮. **তারিখ গাণিতিক (দিন যোগ/বিয়োগ, ইত্যাদি)**

দিন যোগ বা বিয়োগ করার জন্য `setDate` এবং `getDate` মেথড ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let date = new Date();

// 10 দিন যোগ করা
date.setDate(date.getDate() + 10);
console.log(date); // 2024-09-16T00:00:00.000Z

// 5 দিন বিয়োগ করা
date.setDate(date.getDate() - 5);
console.log(date); // 2024-09-11T00:00:00.000Z
```

---

#### ৯. **টাইমস্ট্যাম্প থেকে তারিখ রূপান্তর**

টাইমস্ট্যাম্পকে `Date` অবজেক্টে রূপান্তর করার জন্য `Date` কনস্ট্রাক্টর ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let timestamp = 1693992000000; // টাইমস্ট্যাম্প (মিলি সেকেন্ড)
let date = new Date(timestamp);
console.log(date); // 2024-09-06T12:00:00.000Z
```

---

#### ১০. **সময় অঞ্চল পরিচালনা**

সময় অঞ্চল ব্যবস্থাপনার জন্য `Intl.DateTimeFormat` ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let date = new Date();
let formatter = new Intl.DateTimeFormat('en-US', {
  timeZone: 'America/New_York',
  year: 'numeric',
  month: '2-digit',
  day: '2-digit',
  hour: '2-digit',
  minute: '2-digit'
});
console.log(formatter.format(date)); // 09/06/2024, 08:00 AM (এটি লোকাল টাইম জোন অনুযায়ী পরিবর্তিত হবে)
```

---

#### ১১. **তারিখ মেথড ওভারভিউ (getTime, setTime, ইত্যাদি)**

**`getTime()`**: `Date` অবজেক্টের টাইমস্ট্যাম্প (মিলি সেকেন্ডে) প্রদান করে।
**`setTime()`**: টাইমস্ট্যাম্প থেকে `Date` অবজেক্ট সেট করে।

**ফর্ম্যাট:**
```javascript
let date = new Date();

// টাইমস্ট্যাম্প প্রাপ্তি
let timestamp = date.getTime();
console.log(timestamp); // যেমন: 1693992000000

// টাইমস্ট্যাম্প সেট করা
let newDate = new Date();
newDate.setTime(timestamp);
console.log(newDate); // পূর্ববর্তী তারিখ
```

---

#### ১২. **তারিখ ম্যানিপুলেশনের ব্যবহারিক উদাহরণ**

**ফর্ম্যাট:**
```javascript
// তারিখের মধ্যে দিন যোগ করা
function addDays(date, days) {
  let result = new Date(date);
  result.setDate(result.getDate() + days);
  return result;
}

let today = new Date();
let futureDate = addDays(today, 30);
console.log(`Today: ${today.toDateString()}, Future Date: ${futureDate.toDateString()}`);

// দুটি তারিখের মধ্যে দিন গোনা
function daysBetween(date1, date2) {
  const oneDay = 24 * 60 * 60 * 1000; // একদিনের মিলি সেকেন্ড
  const diffInTime = date2.getTime() - date1.getTime();
  return Math.round(diffInTime / oneDay);
}

let startDate = new Date('2024-09-01');
let endDate = new Date('2024-09-06');
let diffDays = daysBetween(startDate, endDate);
console.log(`Days between ${startDate.toDateString()} and ${endDate.toDateString()}: ${diffDays} days`);
```

---

### সারসংক্ষেপ:
JavaScript-এ তারিখ এবং সময় পরিচালনা করা একটি মৌলিক এবং গুরুত্বপূর্ণ কাজ। `Date` অবজেক্ট বিভিন্ন মেথড প্রদান করে যা তারিখের উপাদান প্রাপ্তি, সেট করা, ফরম্যাটিং, তুলনা, এবং গাণিতিক অপারেশন করা সম্ভব করে তোলে। `Intl.DateTimeFormat` ব্যবহার করে সময় অঞ্চল পরিচালনা করা যায় এবং টাইমস্ট্যাম্প ব্যবহার করে তারিখ তৈরি করা যায়।



### ১৭. **ত্রুটি পরিচালনা**

ত্রুটি পরিচালনা জাভাস্ক্রিপ্টে গুরুত্বপূর্ণ কারণ এটি আপনার কোডের ভুল বা ব্যতিক্রমী পরিস্থিতি পরিচালনার জন্য ব্যবহৃত হয়। এটি নিশ্চিত করে যে কোডের ত্রুটিগুলি আপনার অ্যাপ্লিকেশনকে ব্যাহত না করে এবং আপনি সঠিকভাবে ত্রুটির মোকাবিলা করতে পারেন।

#### ১. **try...catch স্টেটমেন্ট**

`try...catch` ব্লক একটি কোড ব্লকের মধ্যে ত্রুটি ধরতে এবং পরিচালনা করতে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
try {
    // কোড যা ত্রুটি সৃষ্টি করতে পারে
    let result = someFunction();
    console.log(result);
} catch (error) {
    // ত্রুটি পরিচালনা
    console.error('Error occurred:', error.message);
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
try {
    let num = 10;
    let result = num / 0; // সম্ভাব্য ত্রুটি
    console.log(result);
} catch (error) {
    console.error('Error occurred:', error.message);
}
```

---

#### ২. **throw স্টেটমেন্ট**

`throw` স্টেটমেন্ট ব্যবহার করে আপনি নিজস্ব ত্রুটি তৈরি করতে পারেন।

**ফর্ম্যাট:**
```javascript
function checkNumber(num) {
    if (num < 0) {
        throw new Error('Negative number not allowed');
    }
    return num;
}

try {
    checkNumber(-1);
} catch (error) {
    console.error('Error occurred:', error.message);
}
```

---

#### ৩. **finally ক্লজ**

`finally` ক্লজ ব্যবহার করা হয় যা `try` এবং `catch` ব্লকের পরে রান হয়, এটি ত্রুটি ঘটুক বা না ঘটুক।

**ফর্ম্যাট:**
```javascript
try {
    // কোড যা ত্রুটি সৃষ্টি করতে পারে
    let result = someFunction();
    console.log(result);
} catch (error) {
    // ত্রুটি পরিচালনা
    console.error('Error occurred:', error.message);
} finally {
    // এই ব্লক সবসময় রান হয়
    console.log('Cleanup code runs regardless of error');
}
```

---

#### ৪. **কাস্টম ত্রুটির বার্তা**

`Error` অবজেক্টে কাস্টম বার্তা সেট করা যায়।

**ফর্ম্যাট:**
```javascript
try {
    throw new Error('This is a custom error message');
} catch (error) {
    console.error('Error occurred:', error.message);
}
```

---

#### ৫. **ত্রুটি অবজেক্ট প্রোপার্টি (name, message, stack)**

ত্রুটি অবজেক্টে বিভিন্ন প্রোপার্টি থাকে:

- **name**: ত্রুটির প্রকার।
- **message**: ত্রুটির বার্তা।
- **stack**: ত্রুটির স্ট্যাক ট্রেস।

**ফর্ম্যাট:**
```javascript
try {
    throw new Error('Custom error');
} catch (error) {
    console.log('Error Name:', error.name);
    console.log('Error Message:', error.message);
    console.log('Stack Trace:', error.stack);
}
```

---

#### ৬. **কাস্টম ত্রুটি ক্লাস তৈরি করা**

নিজস্ব ত্রুটি ক্লাস তৈরি করার জন্য `class` ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
class CustomError extends Error {
    constructor(message) {
        super(message);
        this.name = 'CustomError';
    }
}

try {
    throw new CustomError('Something went wrong');
} catch (error) {
    console.error(`${error.name}: ${error.message}`);
}
```

---

#### ৭. **নেস্টেড try...catch ব্লক**

`try...catch` ব্লক গুলো একটি অপরের মধ্যে রাখা যেতে পারে।

**ফর্ম্যাট:**
```javascript
try {
    try {
        let result = JSON.parse('invalid JSON');
    } catch (innerError) {
        console.error('Inner catch:', innerError.message);
    }
} catch (outerError) {
    console.error('Outer catch:', outerError.message);
}
```

---

#### ৮. **অ্যাসিঙ্ক্রোনাস ত্রুটি পরিচালনা**

অ্যাসিঙ্ক্রোনাস কোডে `try...catch` ব্লক ব্যবহার করা যায় `async/await` এর সাথে।

**ফর্ম্যাট:**
```javascript
async function fetchData() {
    try {
        let response = await fetch('https://api.example.com/data');
        let data = await response.json();
        console.log(data);
    } catch (error) {
        console.error('Fetch error:', error.message);
    }
}

fetchData();
```

---

#### ৯. **ত্রুটি পরিচালনার জন্য সেরা অনুশীলন**

- **স্পষ্ট ত্রুটি বার্তা**: ব্যবহারকারীর জন্য বোঝা সহজ হওয়া উচিত।
- **ত্রুটি লগিং**: ত্রুটির লগ রাখা গুরুত্বপূর্ণ ডিবাগিং এর জন্য।
- **ত্রুটির প্রকার**: বিভিন্ন ধরনের ত্রুটি জন্য আলাদা ত্রুটি ক্লাস ব্যবহার করুন।
- **বৈধ ইনপুট**: ইনপুট ভ্যালিডেশন করে ত্রুটি প্রতিরোধ করুন।

---

#### ১০. **ত্রুটি পরিচালনা দিয়ে ডিবাগিং**

ত্রুটি লগিং ও স্ট্যাক ট্রেস বিশ্লেষণ করে কোডের ত্রুটি সনাক্ত করুন। 

**ফর্ম্যাট:**
```javascript
try {
    // কিছু কোড
} catch (error) {
    console.error('Error stack trace:', error.stack);
}
```

---

#### ১১. **ত্রুটির লগিংয়ের জন্য console.error ব্যবহার**

`console.error` ত্রুটির বার্তা লগ করার জন্য ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
try {
    throw new Error('An error occurred');
} catch (error) {
    console.error('Error:', error.message);
}
```

---

#### ১২. **প্রতিশ্রুতির ত্রুটি পরিচালনা (catch মেথড)**

প্রতিশ্রুতির ত্রুটি পরিচালনার জন্য `catch` মেথড ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
fetch('https://api.example.com/data')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Promise error:', error.message));
```

---

### সারসংক্ষেপ:

ত্রুটি পরিচালনা জাভাস্ক্রিপ্টে কোডের স্থায়িত্ব নিশ্চিত করতে গুরুত্বপূর্ণ। `try...catch` ব্লক, `throw` স্টেটমেন্ট, এবং `finally` ক্লজ ব্যবহার করে ত্রুটি হ্যান্ডলিং করা হয়। কাস্টম ত্রুটি ক্লাস তৈরি করা, নেস্টেড `try...catch` ব্লক ব্যবহৃত হয় ত্রুটি পরিচালনার উন্নতি করার জন্য। অ্যাসিঙ্ক্রোনাস অপারেশন, ডিবাগিং, লগিং, এবং প্রতিশ্রুতির ত্রুটি পরিচালনা প্রক্রিয়া উন্নত করতে সাহায্য করে।




### ১৮. **অ্যাসিঙ্ক্রোনাস জাভাস্ক্রিপ্ট**

অ্যাসিঙ্ক্রোনাস জাভাস্ক্রিপ্ট এমনভাবে কোড লেখার একটি পদ্ধতি যা কোড কার্যক্রম একসাথে নির্বাহ করতে সাহায্য করে, যেমন নেটওয়ার্ক অনুরোধ, টাইমআউট, বা অন্যান্য দীর্ঘ-running অপারেশন। এটি ব্যবহারকারী অভিজ্ঞতা উন্নত করতে সহায়ক কারণ এটি UI ব্লক করতে দেয় না।

#### ১. **অ্যাসিঙ্ক্রোনাস আচরণ বোঝা**

অ্যাসিঙ্ক্রোনাস কোড সাধারণত `callback` ফাংশন, `Promise`, এবং `async/await` দ্বারা পরিচালিত হয়। এটি দীর্ঘ-running অপারেশন চলাকালীন অন্যান্য কোড ব্লক করতে দেয় না।

---

#### ২. **কলব্যাক এবং কলব্যাক ফাংশন**

কলব্যাক ফাংশন হল একটি ফাংশন যা অন্য একটি ফাংশনের প্যারামিটার হিসাবে পাস করা হয় এবং তা পরে কল হয়।

**ফর্ম্যাট:**
```javascript
function fetchData(callback) {
    setTimeout(() => {
        callback('Data received');
    }, 1000);
}

fetchData((data) => {
    console.log(data);
});
```

**ব্যবহারিক উদাহরণ:**
```javascript
function loadScript(url, callback) {
    const script = document.createElement('script');
    script.src = url;
    script.onload = () => callback(null, 'Script loaded successfully');
    script.onerror = () => callback(new Error('Script loading failed'));
    document.head.append(script);
}

loadScript('script.js', (error, message) => {
    if (error) {
        console.error(error);
    } else {
        console.log(message);
    }
});
```

---

#### ৩. **কলব্যাক হেল এবং কীভাবে তা এড়ানো যায়**

কলব্যাক হেল হলো একাধিক নেস্টেড কলব্যাকগুলির সমস্যাযুক্ত অবস্থা যা কোডের পড়তে এবং পরিচালনা করতে অসুবিধা করে। এটি এড়াতে আপনি `Promise` বা `async/await` ব্যবহার করতে পারেন।

**ফর্ম্যাট:**
```javascript
// কলব্যাক হেল উদাহরণ
doSomething(function (result) {
    doSomethingElse(result, function (result2) {
        doAnotherThing(result2, function (result3) {
            console.log(result3);
        });
    });
});
```

**ব্যবহারিক উদাহরণ:**
```javascript
// কলব্যাক হেল থেকে মুক্তি
function doSomething() {
    return new Promise((resolve, reject) => {
        // কিছু অ্যাসিঙ্ক্রোনাস কাজ
        resolve('result');
    });
}

doSomething()
    .then(result => doSomethingElse(result))
    .then(result2 => doAnotherThing(result2))
    .then(result3 => console.log(result3))
    .catch(error => console.error(error));
```

---

#### ৪. **প্রতিশ্রুতি (Promise)**

প্রতিশ্রুতি একটি অবজেক্ট যা একটি অ্যাসিঙ্ক্রোনাস অপারেশনের ফলাফল প্রতিনিধিত্ব করে এবং এটি সফল (resolve) বা ব্যর্থ (reject) হতে পারে।

**ফর্ম্যাট:**
```javascript
let promise = new Promise((resolve, reject) => {
    // কিছু অ্যাসিঙ্ক্রোনাস কাজ
    if (success) {
        resolve('Success!');
    } else {
        reject('Error!');
    }
});
```

**ব্যবহারিক উদাহরণ:**
```javascript
let promise = new Promise((resolve, reject) => {
    setTimeout(() => resolve('Data received'), 1000);
});

promise.then(result => console.log(result))
       .catch(error => console.error(error));
```

---

#### ৫. **প্রতিশ্রুতি শৃঙ্খল**

প্রতিশ্রুতির শৃঙ্খল একটি প্রতিশ্রুতি থেকে আরেকটি প্রতিশ্রুতির সাথে সংযোগ স্থাপন করে।

**ফর্ম্যাট:**
```javascript
fetchData()
    .then(result => process(result))
    .then(result2 => moreProcessing(result2))
    .catch(error => console.error(error));
```

**ব্যবহারিক উদাহরণ:**
```javascript
function getData() {
    return new Promise((resolve) => {
        setTimeout(() => resolve('Data'), 1000);
    });
}

function processData(data) {
    return new Promise((resolve) => {
        setTimeout(() => resolve(data + ' processed'), 1000);
    });
}

getData()
    .then(data => processData(data))
    .then(result => console.log(result))
    .catch(error => console.error(error));
```

---

#### ৬. **প্রতিশ্রুতি ত্রুটি পরিচালনা (catch মেথড)**

`catch` মেথড প্রতিশ্রুতির কোনো ত্রুটি হ্যান্ডল করতে ব্যবহৃত হয়।

**ফর্ম্যাট:**
```javascript
let promise = new Promise((resolve, reject) => {
    reject('Error');
});

promise
    .then(result => console.log(result))
    .catch(error => console.error('Caught error:', error));
```

---

#### ৭. **async ফাংশন**

`async` ফাংশন একটি ফাংশন যা একটি প্রতিশ্রুতি ফেরত দেয় এবং এর ভিতরে `await` ব্যবহার করা যায়।

**ফর্ম্যাট:**
```javascript
async function fetchData() {
    return 'Data';
}

fetchData().then(data => console.log(data));
```

**ব্যবহারিক উদাহরণ:**
```javascript
async function getData() {
    let response = await fetch('https://api.example.com/data');
    let data = await response.json();
    return data;
}

getData().then(data => console.log(data)).catch(error => console.error(error));
```

---

#### ৮. **await কীওয়ার্ড**

`await` কীওয়ার্ড একটি প্রতিশ্রুতি সম্পূর্ণ হওয়া পর্যন্ত অপেক্ষা করে এবং প্রতিশ্রুতির ফলাফল সরাসরি ফেরত দেয়।

**ফর্ম্যাট:**
```javascript
async function example() {
    let result = await someAsyncFunction();
    console.log(result);
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
async function fetchData() {
    try {
        let response = await fetch('https://api.example.com/data');
        let data = await response.json();
        console.log(data);
    } catch (error) {
        console.error('Error:', error);
    }
}

fetchData();
```

---

#### ৯. **try...catch সহ async/await মিশ্রিত করা**

`async/await` এর সাথে `try...catch` ব্লক ব্যবহার করে ত্রুটি পরিচালনা করা হয়।

**ফর্ম্যাট:**
```javascript
async function fetchData() {
    try {
        let response = await fetch('https://api.example.com/data');
        let data = await response.json();
        console.log(data);
    } catch (error) {
        console.error('Error:', error);
    }
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
async function getUserData() {
    try {
        let response = await fetch('https://api.example.com/user');
        if (!response.ok) throw new Error('Network response was not ok');
        let user = await response.json();
        console.log(user);
    } catch (error) {
        console.error('Failed to fetch user:', error);
    }
}

getUserData();
```

---

#### ১০. **কলব্যাক থেকে প্রতিশ্রুতি রূপান্তর**

কলব্যাক ভিত্তিক API গুলোকে প্রতিশ্রুতিতে রূপান্তর করা।

**ফর্ম্যাট:**
```javascript
function asyncOperation() {
    return new Promise((resolve, reject) => {
        oldApiCall((error, result) => {
            if (error) reject(error);
            else resolve(result);
        });
    });
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
function getDataUsingCallback(callback) {
    setTimeout(() => callback(null, 'Data'), 1000);
}

function getData() {
    return new Promise((resolve, reject) => {
        getDataUsingCallback((error, result) => {
            if (error) reject(error);
            else resolve(result);
        });
    });
}

getData().then(data => console.log(data)).catch(error => console.error(error));
```

---

#### ১১. **async/await এর ব্যবহারিক উদাহরণ**

**ফর্ম্যাট:**
```javascript
async function processData() {
    let data = await fetchData();
    // আরো কাজ
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
async function fetchDataFromApi() {
    try {
        let response = await fetch('https://api.example.com/data');
        let data = await response.json();
        console.log('Fetched Data:', data);
    } catch (error) {
        console.error('Fetch Error:', error);
    }
}

fetchDataFromApi();
```

---

#### ১২. **fetch API সহ async/await ব্যবহার**

`fetch` API ব্যবহার করে `async/await` এর সাথে ডেটা আহরণ।

**ফর্ম্যাট:**
```javascript
async function fetchData() {
    let response = await fetch('url');
    let data = await response.json();
    return data;
}
```

**ব্যবহারিক উদাহরণ:**
```javascript
async function getWeather() {
    try {
        let response = await fetch('https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY&q=London

');
        let weatherData = await response.json();
        console.log('Weather Data:', weatherData);
    } catch (error) {
        console.error('Failed to fetch weather data:', error);
    }
}

getWeather();
```

---

### সারসংক্ষেপ:

অ্যাসিঙ্ক্রোনাস জাভাস্ক্রিপ্ট ব্যবহারের মাধ্যমে দীর্ঘ-running অপারেশনগুলি সম্পন্ন করা হয় যাতে প্রোগ্রাম চালু থাকে। কলব্যাক, প্রতিশ্রুতি, এবং `async/await` ব্যবহারের মাধ্যমে অ্যাসিঙ্ক্রোনাস আচরণ সহজে পরিচালনা করা যায়। কলব্যাক হেল থেকে মুক্তি, প্রতিশ্রুতি শৃঙ্খল, এবং ত্রুটি পরিচালনা কৌশলগুলো অ্যাসিঙ্ক্রোনাস কোডের কার্যকারিতা উন্নত করতে সাহায্য করে।




### ১৯. **ডম ম্যানিপুলেশন**

ডম (Document Object Model) ম্যানিপুলেশন হল একটি ওয়েব পৃষ্ঠার HTML ডকুমেন্টের উপাদানগুলির সাথে কাজ করার প্রক্রিয়া। এটি ডাইনামিক ওয়েব পৃষ্ঠার তৈরি, পরিবর্তন, এবং ইন্টারঅ্যাকশন সম্ভব করে।

#### ১. **এলিমেন্ট নির্বাচন করা**

**ফর্ম্যাট:**
- `document.getElementById(id)`: একটি নির্দিষ্ট আইডি সহ এলিমেন্ট নির্বাচন করে।
- `document.querySelector(selector)`: CSS সিলেক্টর ব্যবহার করে প্রথম ম্যাচ করা এলিমেন্ট নির্বাচন করে।
- `document.querySelectorAll(selector)`: CSS সিলেক্টর ব্যবহার করে সমস্ত ম্যাচ করা এলিমেন্ট নির্বাচন করে।

**ব্যবহারিক উদাহরণ:**
```javascript
// আইডি দ্বারা নির্বাচন
let elementById = document.getElementById('myId');

// CSS সিলেক্টর দ্বারা প্রথম এলিমেন্ট নির্বাচন
let firstElement = document.querySelector('.myClass');

// CSS সিলেক্টর দ্বারা সমস্ত এলিমেন্ট নির্বাচন
let allElements = document.querySelectorAll('p');
```

---

#### ২. **ডম ট্র্যাভার্সিং**

ডম ট্র্যাভার্সিং ব্যবহার করে এলিমেন্টের প্যারেন্ট, চাইল্ড, এবং সিস্টার এলিমেন্টগুলির সাথে কাজ করা হয়।

**ফর্ম্যাট:**
- `parentNode`: প্যারেন্ট এলিমেন্ট রিটার্ন করে।
- `childNodes`: চাইল্ড এলিমেন্টগুলির একটি নোড লিস্ট রিটার্ন করে।
- `nextSibling`: বর্তমান এলিমেন্টের পরবর্তী সিস্টার এলিমেন্ট রিটার্ন করে।
- `previousSibling`: বর্তমান এলিমেন্টের পূর্ববর্তী সিস্টার এলিমেন্ট রিটার্ন করে।

**ব্যবহারিক উদাহরণ:**
```javascript
let child = document.getElementById('myId');
let parent = child.parentNode;
let children = child.childNodes;
let next = child.nextSibling;
let previous = child.previousSibling;
```

---

#### ৩. **নতুন এলিমেন্ট তৈরি করা**

নতুন এলিমেন্ট তৈরি করতে `createElement` ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let newElement = document.createElement('div');
```

**ব্যবহারিক উদাহরণ:**
```javascript
let newDiv = document.createElement('div');
newDiv.textContent = 'This is a new div';
document.body.appendChild(newDiv);
```

---

#### ৪. **এলিমেন্ট কন্টেন্ট সংশোধন**

এলিমেন্টের কন্টেন্ট পরিবর্তন করতে `textContent` এবং `innerHTML` ব্যবহার করা হয়।

**ফর্ম্যাট:**
- `textContent`: এলিমেন্টের টেক্সট কন্টেন্ট সেট বা রিটার্ন করে।
- `innerHTML`: এলিমেন্টের HTML কন্টেন্ট সেট বা রিটার্ন করে।

**ব্যবহারিক উদাহরণ:**
```javascript
let element = document.getElementById('myId');
element.textContent = 'New text content';
element.innerHTML = '<p>New HTML content</p>';
```

---

#### ৫. **এলিমেন্ট অ্যাট্রিবিউট সংশোধন**

এলিমেন্টের অ্যাট্রিবিউট সংশোধন করতে `setAttribute`, `getAttribute`, এবং `removeAttribute` ব্যবহার করা হয়।

**ফর্ম্যাট:**
- `setAttribute(name, value)`: একটি অ্যাট্রিবিউট সেট করে।
- `getAttribute(name)`: একটি অ্যাট্রিবিউটের মান রিটার্ন করে।
- `removeAttribute(name)`: একটি অ্যাট্রিবিউট মুছে ফেলে।

**ব্যবহারিক উদাহরণ:**
```javascript
let link = document.getElementById('myLink');
link.setAttribute('href', 'https://www.example.com');
let href = link.getAttribute('href');
link.removeAttribute('href');
```

---

#### ৬. **এলিমেন্ট স্টাইল সংশোধন**

এলিমেন্টের স্টাইল পরিবর্তন করতে `style` প্রোপার্টি ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
element.style.property = 'value';
```

**ব্যবহারিক উদাহরণ:**
```javascript
let element = document.getElementById('myId');
element.style.backgroundColor = 'blue';
element.style.color = 'white';
```

---

#### ৭. **ক্লাস যোগ এবং সরানো**

ক্লাস যোগ করতে এবং সরাতে `classList` ব্যবহার করা হয়।

**ফর্ম্যাট:**
- `classList.add(className)`: একটি ক্লাস যোগ করে।
- `classList.remove(className)`: একটি ক্লাস সরিয়ে ফেলে।
- `classList.toggle(className)`: ক্লাসটি থাকলে সরিয়ে ফেলে, না থাকলে যোগ করে।
- `classList.contains(className)`: ক্লাসটি আছে কিনা চেক করে।

**ব্যবহারিক উদাহরণ:**
```javascript
let element = document.getElementById('myId');
element.classList.add('new-class');
element.classList.remove('old-class');
element.classList.toggle('toggle-class');
let hasClass = element.classList.contains('check-class');
```

---

#### ৮. **ইভেন্ট হ্যান্ডলিং**

ইভেন্ট হ্যান্ডল করতে `addEventListener` এবং `removeEventListener` ব্যবহার করা হয়।

**ফর্ম্যাট:**
- `addEventListener(type, listener)`: একটি ইভেন্ট লিসনার যোগ করে।
- `removeEventListener(type, listener)`: একটি ইভেন্ট লিসনার সরিয়ে ফেলে।

**ব্যবহারিক উদাহরণ:**
```javascript
let button = document.getElementById('myButton');

function handleClick() {
    alert('Button clicked!');
}

button.addEventListener('click', handleClick);
button.removeEventListener('click', handleClick);
```

---

#### ৯. **ইভেন্ট ডেলিগেশন**

ইভেন্ট ডেলিগেশন হল একটি পদ্ধতি যেখানে একটি প্যারেন্ট এলিমেন্টে ইভেন্ট লিসনার যোগ করা হয় এবং এর চাইল্ড এলিমেন্টের ইভেন্টগুলি হ্যান্ডল করা হয়।

**ফর্ম্যাট:**
```javascript
parentElement.addEventListener('click', function(event) {
    if (event.target && event.target.matches('selector')) {
        // ইভেন্ট হ্যান্ডলিং কোড
    }
});
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('parentElement').addEventListener('click', function(event) {
    if (event.target && event.target.matches('button')) {
        alert('Button clicked!');
    }
});
```

---

#### ১০. **ফর্ম এবং ফর্ম এলিমেন্টগুলির সাথে কাজ করা**

ফর্ম এবং ফর্ম এলিমেন্টগুলির মান পেতে এবং সেট করতে `value` প্রোপার্টি ব্যবহার করা হয়।

**ফর্ম্যাট:**
```javascript
let formElement = document.getElementById('myForm');
let inputValue = formElement.elements['inputName'].value;
```

**ব্যবহারিক উদাহরণ:**
```javascript
let form = document.getElementById('myForm');
form.addEventListener('submit', function(event) {
    event.preventDefault(); // ফর্ম সাবমিট প্রতিরোধ করে

    let name = form.elements['name'].value;
    let email = form.elements['email'].value;

    console.log('Name:', name);
    console.log('Email:', email);
});
```

---

#### ১১. **এলিমেন্ট ক্লোন এবং মুছে ফেলা**

**ফর্ম্যাট:**
- `cloneNode(deep)`: একটি এলিমেন্টের ক্লোন তৈরি করে। `deep` `true` হলে, চাইল্ড এলিমেন্টগুলোও ক্লোন হবে।
- `remove()`: এলিমেন্ট মুছে ফেলে।

**ব্যবহারিক উদাহরণ:**
```javascript
let element = document.getElementById('myId');

// ক্লোন করা
let clonedElement = element.cloneNode(true);
document.body.appendChild(clonedElement);

// মুছে ফেলা
element.remove();
```

---

#### ১২. **DOMContentLoaded ইভেন্ট**

`DOMContentLoaded` ইভেন্ট তখন ট্রিগার হয় যখন পুরো HTML ডকুমেন্ট লোড হয়, কিন্তু সমস্ত CSS এবং ইমেজ সম্পূর্ণ লোড হওয়ার আগেই।

**ফর্ম্যাট:**
```javascript
document.addEventListener('DOMContentLoaded', function() {
    // কোড এখানে চলে
});
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.addEventListener('DOMContentLoaded', function() {
    console.log('Document is fully loaded and parsed');
});
```

---

### সারসংক্ষেপ:

ডম ম্যানিপুলেশন জাভাস্ক্রিপ্টের মাধ্যমে ওয়েব পৃষ্ঠার এলিমেন্টগুলি তৈরি, পরিবর্তন, এবং সরাতে সহায়ক। এটি এলিমেন্ট নির্বাচন, স্টাইল আপডেট, ক্লাস পরিচালনা, ইভেন্ট হ্যান্ডলিং এবং ডম ট্র্যাভার্সিং সহ বিভিন্ন কার্যাবলী অন্তর্ভুক্ত করে। এই ম্যানিপুলেশনগুলি ব্যবহারকারীর অভিজ্ঞতাকে উন্নত করতে এবং ডাইনামিক কনটেন্ট প্রস্তাব করতে সাহায্য করে।





### ২০. **ইভেন্ট হ্যান্ডলিং**

ইভেন্ট হ্যান্ডলিং ওয়েব পৃষ্ঠার ইন্টারঅ্যাকটিভিটি ব্যবস্থাপনার একটি গুরুত্বপূর্ণ অংশ। এটি ব্যবহারকারীর ক্রিয়া যেমন ক্লিক, টাইপিং, মাউস মুভমেন্ট, ইত্যাদির প্রতি প্রতিক্রিয়া জানাতে সাহায্য করে।

#### ১. **EventListener যোগ করা**

**ফর্ম্যাট:**
```javascript
element.addEventListener(eventType, eventHandler);
```

**ব্যবহারিক উদাহরণ:**
```javascript
let button = document.getElementById('myButton');

function handleClick() {
    alert('Button clicked!');
}

button.addEventListener('click', handleClick);
```

---

#### ২. **EventListener সরানো**

**ফর্ম্যাট:**
```javascript
element.removeEventListener(eventType, eventHandler);
```

**ব্যবহারিক উদাহরণ:**
```javascript
let button = document.getElementById('myButton');

function handleClick() {
    alert('Button clicked!');
}

// যোগ করা
button.addEventListener('click', handleClick);

// সরানো
button.removeEventListener('click', handleClick);
```

---

#### ৩. **সাধারণ ইভেন্ট**

**ইভেন্ট টাইপ:**
- `click`: এলিমেন্টে ক্লিক করা।
- `submit`: ফর্ম সাবমিট করা।
- `mouseover`: মাউস এলিমেন্টের উপর রাখা।

**ব্যবহারিক উদাহরণ:**
```javascript
// Click event
document.getElementById('myButton').addEventListener('click', function() {
    console.log('Button clicked!');
});

// Submit event
document.getElementById('myForm').addEventListener('submit', function(event) {
    event.preventDefault(); // ফর্ম সাবমিট প্রতিরোধ করে
    console.log('Form submitted!');
});

// Mouseover event
document.getElementById('myElement').addEventListener('mouseover', function() {
    console.log('Mouse over the element!');
});
```

---

#### ৪. **ইভেন্ট অবজেক্ট প্রোপার্টি**

**প্রোপার্টি:**
- `event.target`: ইভেন্ট ঘটানো এলিমেন্ট।
- `event.currentTarget`: ইভেন্ট হ্যান্ডলার যোগ করা এলিমেন্ট।
- `event.type`: ইভেন্টের টাইপ (যেমন 'click', 'submit')।

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('myButton').addEventListener('click', function(event) {
    console.log('Target:', event.target);
    console.log('Current Target:', event.currentTarget);
    console.log('Event Type:', event.type);
});
```

---

#### ৫. **ইভেন্ট প্রোপাগেশন (বাবলিং এবং ক্যাপচারিং)**

**বাবলিং:** ইভেন্ট প্রপাগেট করে প্যারেন্ট থেকে চাইল্ডে।
**ক্যাপচারিং:** ইভেন্ট প্রপাগেট করে চাইল্ড থেকে প্যারেন্টে।

**ফর্ম্যাট:**
```javascript
element.addEventListener(eventType, eventHandler, { capture: true }); // ক্যাপচারিং
element.addEventListener(eventType, eventHandler); // বাবলিং
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('parent').addEventListener('click', function() {
    console.log('Parent clicked!');
}, { capture: true });

document.getElementById('child').addEventListener('click', function() {
    console.log('Child clicked!');
});
```

---

#### ৬. **ডিফল্ট আচরণ প্রতিরোধ করা (preventDefault)**

**ফর্ম্যাট:**
```javascript
event.preventDefault();
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('myForm').addEventListener('submit', function(event) {
    event.preventDefault(); // ফর্ম সাবমিট প্রতিরোধ করে
    console.log('Form submission prevented!');
});
```

---

#### ৭. **প্রোপাগেশন থামানো (stopPropagation)**

**ফর্ম্যাট:**
```javascript
event.stopPropagation();
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('child').addEventListener('click', function(event) {
    event.stopPropagation(); // ইভেন্ট প্রোপাগেশন থামায়
    console.log('Child clicked!');
});

document.getElementById('parent').addEventListener('click', function() {
    console.log('Parent clicked!');
});
```

---

#### ৮. **ইভেন্ট ডিবাউন্সিং এবং থ্রোটলিং**

**ডিবাউন্সিং:** নির্দিষ্ট সময়ের মধ্যে একাধিক ইভেন্ট ঘটে এমন সিচুয়েশন সামলাতে সাহায্য করে। সাধারণত ব্যবহার হয় ইনপুট ফিল্ডের জন্য।

**থ্রোটলিং:** একটি নির্দিষ্ট সময়সীমার মধ্যে কতবার ইভেন্ট কার্যকর হবে তা সীমিত করে।

**ব্যবহারিক উদাহরণ (ডিবাউন্সিং):**
```javascript
let debounceTimeout;
function debounce(func, delay) {
    return function() {
        clearTimeout(debounceTimeout);
        debounceTimeout = setTimeout(func, delay);
    };
}

document.getElementById('myInput').addEventListener('input', debounce(function() {
    console.log('Input changed!');
}, 300));
```

**ব্যবহারিক উদাহরণ (থ্রোটলিং):**
```javascript
function throttle(func, limit) {
    let lastFunc;
    let lastRan;
    return function() {
        const context = this;
        const now = Date.now();
        if (!lastRan) {
            func.apply(context, arguments);
            lastRan = now;
        } else {
            clearTimeout(lastFunc);
            lastFunc = setTimeout(function() {
                if (now - lastRan >= limit) {
                    func.apply(context, arguments);
                    lastRan = now;
                }
            }, limit - (now - lastRan));
        }
    };
}

document.getElementById('myButton').addEventListener('click', throttle(function() {
    console.log('Button clicked!');
}, 2000));
```

---

#### ৯. **কাস্টম ইভেন্ট**

**ফর্ম্যাট:**
```javascript
let event = new CustomEvent('myEvent', { detail: { key: 'value' } });
element.dispatchEvent(event);
```

**ব্যবহারিক উদাহরণ:**
```javascript
let element = document.getElementById('myElement');

element.addEventListener('myEvent', function(event) {
    console.log('Custom event triggered with detail:', event.detail);
});

let customEvent = new CustomEvent('myEvent', { detail: { message: 'Hello World' } });
element.dispatchEvent(customEvent);
```

---

#### ১০. **কীবোর্ড ইভেন্ট হ্যান্ডলিং**

**ইভেন্ট টাইপ:**
- `keydown`: কীবোর্ড কি প্রেস করার সময়।
- `keyup`: কীবোর্ড কি মুক্ত করার সময়।
- `keypress`: কীবোর্ড কি প্রেস করার সময় (শুধুমাত্র চরিত্র কীগুলির জন্য)।

**ব্যবহারিক উদাহরণ:**
```javascript
document.addEventListener('keydown', function(event) {
    console.log('Key pressed:', event.key);
});

document.addEventListener('keyup', function(event) {
    console.log('Key released:', event.key);
});
```

---

#### ১১. **মাউস ইভেন্ট হ্যান্ডলিং**

**ইভেন্ট টাইপ:**
- `click`: মাউস ক্লিক।
- `dblclick`: ডাবল ক্লিক।
- `mouseover`: মাউস এলিমেন্টের উপর রাখা।
- `mouseout`: মাউস এলিমেন্টের বাইরে চলে যাওয়া।
- `mousemove`: মাউস মুভমেন্ট।

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('myElement').addEventListener('click', function(event) {
    console.log('Element clicked!');
});

document.getElementById('myElement').addEventListener('mousemove', function(event) {
    console.log('Mouse moved:', event.clientX, event.clientY);
});
```

---

#### ১২. **ইভেন্ট ডেলিগেশন সেরা অনুশীলন**

ইভেন্ট ডেলিগেশন হল একটি প্যারেন্ট এলিমেন্টে ইভেন্ট লিসনার যোগ করে এবং তার চাইল্ড এলিমেন্টগুলির ইভেন্ট হ্যান্ডলিং করা। এটি প্রায়ই অনেক এলিমেন্টের ইভেন্ট হ্যান্ডল করার জন্য ব্যবহৃত হয়।

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('parentElement').addEventListener('click', function(event) {
    if (event.target && event.target.matches('button')) {
        console.log('Button clicked:', event.target.textContent);
    }
});
```

---

### সারসংক্ষেপ:

ইভেন্ট হ্যান্ডলিং হল ওয়েব পৃষ্ঠার ইন্টারঅ্যাকটিভিটি ব্যবস্থাপনার একটি মূল অংশ। এটি ইভেন্ট লিসনার যোগ করা, সরানো, সাধারণ ইভেন্ট হ্যান্ডলিং, ইভেন্ট প্রোপার্টি, প্রোপাগেশন, ডিফল্ট আচরণ প্রতিরোধ, কাস্টম ইভেন্ট তৈরি, এবং কীবোর্ড ও মাউস ইভেন্ট হ্যান্ডলিং অন্তর্ভুক্ত করে। এই কৌশলগুলি ব্যবহারের মাধ্যমে আপনি ব্যবহারকারীর ইন্টারঅ্যাকশনকে কার্যকরভাবে পরিচালনা করতে পারেন।






### ২১. **ফর্ম এবং ফর্ম ভ্যালিডেশন**

ফর্ম এবং ফর্ম ভ্যালিডেশন ওয়েব পৃষ্ঠায় ব্যবহারকারীর ইনপুট সংগ্রহ এবং যাচাই করার জন্য অত্যন্ত গুরুত্বপূর্ণ। এটি ডেটার সঠিকতা এবং সম্পূর্ণতা নিশ্চিত করতে সাহায্য করে।

#### ১. **ফর্ম এলিমেন্টগুলি অ্যাক্সেস করা**

ফর্মের বিভিন্ন এলিমেন্ট যেমন `input`, `select`, `textarea` সহজেই অ্যাক্সেস করা যায়:

**ব্যবহারিক উদাহরণ:**
```javascript
let inputElement = document.getElementById('myInput');
let selectElement = document.getElementById('mySelect');
let textareaElement = document.getElementById('myTextarea');
```

---

#### ২. **ফর্ম জমা দেওয়ার ইভেন্ট**

**ফর্ম্যাট:**
```javascript
formElement.addEventListener('submit', eventHandler);
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('myForm').addEventListener('submit', function(event) {
    console.log('Form submitted!');
});
```

---

#### ৩. **ফর্ম জমা প্রতিরোধ করা**

**ফর্ম্যাট:**
```javascript
event.preventDefault();
```

**ব্যবহারিক উদাহরণ:**
```javascript
document.getElementById('myForm').addEventListener('submit', function(event) {
    event.preventDefault(); // ফর্ম জমা প্রতিরোধ করে
    console.log('Form submission prevented!');
});
```

---

#### ৪. **ফর্ম মানগুলি পাওয়া এবং সেট করা**

**মান পাওয়া:**
```javascript
let inputValue = document.getElementById('myInput').value;
```

**মান সেট করা:**
```javascript
document.getElementById('myInput').value = 'New value';
```

**ব্যবহারিক উদাহরণ:**
```javascript
let inputElement = document.getElementById('myInput');
let inputValue = inputElement.value;
console.log('Current value:', inputValue);

inputElement.value = 'Updated value';
```

---

#### ৫. **ফর্ম ইনপুট ভ্যালিডেশন**

**HTML5 ভ্যালিডেশন এট্রিবিউট:**
```html
<input type="text" required minlength="5" pattern="[A-Za-z]+" />
```

**ব্যবহারিক উদাহরণ:**
```html
<form id="myForm">
    <input type="text" id="myInput" required minlength="5" />
    <input type="submit" value="Submit" />
</form>
```

---

#### ৬. **কাস্টম ভ্যালিডেশন**

**ফর্ম্যাট:**
```javascript
inputElement.setCustomValidity('Custom error message');
```

**ব্যবহারিক উদাহরণ:**
```javascript
let inputElement = document.getElementById('myInput');
inputElement.addEventListener('input', function() {
    if (inputElement.value.length < 5) {
        inputElement.setCustomValidity('Input must be at least 5 characters long.');
    } else {
        inputElement.setCustomValidity('');
    }
});
```

---

#### ৭. **ভ্যালিডেশন মেসেজ প্রদর্শন**

ভ্যালিডেশন মেসেজগুলি ব্যবহারকারীর ইনপুট ত্রুটির জন্য স্বয়ংক্রিয়ভাবে প্রদর্শিত হয় যদি আপনি HTML5 ভ্যালিডেশন এট্রিবিউট ব্যবহার করেন।

**ব্যবহারিক উদাহরণ:**
```html
<form id="myForm">
    <input type="text" id="myInput" required minlength="5" />
    <input type="submit" value="Submit" />
</form>
```

---

#### ৮. **Constraint Validation API ব্যবহার করা**

**ফর্ম্যাট:**
```javascript
inputElement.checkValidity();
inputElement.validationMessage;
```

**ব্যবহারিক উদাহরণ:**
```javascript
let inputElement = document.getElementById('myInput');
if (!inputElement.checkValidity()) {
    console.log('Validation error:', inputElement.validationMessage);
}
```

---

#### ৯. **বিভিন্ন ইনপুট টাইপ পরিচালনা**

**ইনপুট টাইপ:**
- `text`
- `email`
- `password`

**ব্যবহারিক উদাহরণ:**
```html
<form id="myForm">
    <input type="text" id="textInput" placeholder="Text input" />
    <input type="email" id="emailInput" placeholder="Email input" />
    <input type="password" id="passwordInput" placeholder="Password input" />
    <input type="submit" value="Submit" />
</form>
```

---

#### ১০. **চেকবক্স এবং রেডিও বাটন পরিচালনা**

**চেকবক্স:**
```html
<input type="checkbox" id="myCheckbox" />
```

**রেডিও বাটন:**
```html
<input type="radio" name="myRadio" id="radio1" />
<input type="radio" name="myRadio" id="radio2" />
```

**ব্যবহারিক উদাহরণ:**
```javascript
let checkbox = document.getElementById('myCheckbox');
checkbox.addEventListener('change', function() {
    if (checkbox.checked) {
        console.log('Checkbox is checked');
    } else {
        console.log('Checkbox is unchecked');
    }
});

let radios = document.querySelectorAll('input[name="myRadio"]');
radios.forEach(radio => {
    radio.addEventListener('change', function() {
        console.log('Selected radio:', this.id);
    });
});
```

---

#### ১১. **ফাইল ইনপুট পরিচালনা**

**ফর্ম্যাট:**
```javascript
let fileInput = document.getElementById('fileInput');
fileInput.addEventListener('change', function() {
    let files = fileInput.files;
    console.log('Selected files:', files);
});
```

**ব্যবহারিক উদাহরণ:**
```html
<input type="file" id="fileInput" />
```

---

#### ১২. **FormData API সহ ফর্ম ডেটা**

**ফর্ম্যাট:**
```javascript
let formData = new FormData(formElement);
```

**ব্যবহারিক উদাহরণ:**
```javascript
let form = document.getElementById('myForm');
let formData = new FormData(form);

formData.forEach((value, key) => {
    console.log(key, value);
});
```

**সারসংক্ষেপ:**

ফর্ম এবং ফর্ম ভ্যালিডেশন ব্যবহারকারীর ইনপুট সংগ্রহ এবং যাচাই করতে সাহায্য করে। এটি ফর্ম এলিমেন্টে অ্যাক্সেস করা, ফর্ম জমা দেওয়ার ইভেন্ট পরিচালনা করা, ইনপুট ভ্যালিডেশন, কাস্টম ভ্যালিডেশন, Constraint Validation API ব্যবহার, বিভিন্ন ইনপুট টাইপ পরিচালনা, চেকবক্স ও রেডিও বাটন, ফাইল ইনপুট, এবং FormData API অন্তর্ভুক্ত করে। এসব কৌশল ব্যবহার করে আপনি ব্যবহারকারীর ইনপুটকে সঠিকভাবে পরিচালনা এবং যাচাই করতে পারেন।






### ২২. **লোকাল স্টোরেজ এবং সেশন স্টোরেজ**

ওয়েব স্টোরেজ API দুটি মূল অংশে বিভক্ত: `localStorage` এবং `sessionStorage`। এরা ক্লায়েন্ট-সাইড স্টোরেজের জন্য ব্যবহৃত হয় যা ব্রাউজারে ডেটা সংরক্ষণ করে। এই স্টোরেজ দুইটি বিভিন্ন সময়সীমার জন্য ডেটা সংরক্ষণ করে।

#### ১. **ওয়েব স্টোরেজের পরিচিতি**

ওয়েব স্টোরেজ API দুইটি সঞ্চয় ব্যবস্থা প্রদান করে:
- **`localStorage`**: ব্রাউজার বন্ধ করার পরও ডেটা সংরক্ষণ করে।
- **`sessionStorage`**: ব্রাউজার সেশন চলাকালীন ডেটা সংরক্ষণ করে; ব্রাউজার বা ট্যাব বন্ধ করলে ডেটা মুছে যায়।

---

#### ২. **localStorage API ওভারভিউ**

**`localStorage`** ক্লায়েন্ট-সাইড স্টোরেজের জন্য ব্যবহার করা হয় এবং ডেটা সার্ভার থেকে পাঠানো হয় না।

**ব্যবহারিক উদাহরণ:**
```javascript
// আইটেম সেট করা
localStorage.setItem('key', 'value');

// আইটেম পাওয়া
let value = localStorage.getItem('key');
console.log(value); // 'value'

// আইটেম মুছে ফেলা
localStorage.removeItem('key');

// সমস্ত স্টোরেজ পরিষ্কার করা
localStorage.clear();
```

---

#### ৩. **sessionStorage API ওভারভিউ**

**`sessionStorage`** শুধুমাত্র বর্তমান ব্রাউজার সেশনের জন্য ডেটা সংরক্ষণ করে এবং ব্রাউজার বন্ধ হলে ডেটা মুছে যায়।

**ব্যবহারিক উদাহরণ:**
```javascript
// আইটেম সেট করা
sessionStorage.setItem('sessionKey', 'sessionValue');

// আইটেম পাওয়া
let sessionValue = sessionStorage.getItem('sessionKey');
console.log(sessionValue); // 'sessionValue'

// আইটেম মুছে ফেলা
sessionStorage.removeItem('sessionKey');

// সমস্ত স্টোরেজ পরিষ্কার করা
sessionStorage.clear();
```

---

#### ৪. **আইটেম সেট এবং পেতে**

**আইটেম সেট করা:**
```javascript
localStorage.setItem('username', 'JohnDoe');
```

**আইটেম পাওয়া:**
```javascript
let username = localStorage.getItem('username');
console.log(username); // 'JohnDoe'
```

---

#### ৫. **আইটেম মুছে ফেলা**

**আইটেম মুছে ফেলা:**
```javascript
localStorage.removeItem('username');
```

---

#### ৬. **স্টোরেজ পরিষ্কার করা**

**স্টোরেজ পরিষ্কার করা:**
```javascript
localStorage.clear(); // localStorage পরিষ্কার করা
sessionStorage.clear(); // sessionStorage পরিষ্কার করা
```

---

#### ৭. **অবজেক্ট এবং অ্যারে সংরক্ষণ (JSON.stringify)**

**অবজেক্ট সংরক্ষণ:**
```javascript
let user = { name: 'John', age: 30 };
localStorage.setItem('user', JSON.stringify(user));
```

**অ্যারে সংরক্ষণ:**
```javascript
let colors = ['red', 'green', 'blue'];
localStorage.setItem('colors', JSON.stringify(colors));
```

---

#### ৮. **অবজেক্ট এবং অ্যারে পুনরুদ্ধার (JSON.parse)**

**অবজেক্ট পুনরুদ্ধার:**
```javascript
let user = JSON.parse(localStorage.getItem('user'));
console.log(user.name); // 'John'
```

**অ্যারে পুনরুদ্ধার:**
```javascript
let colors = JSON.parse(localStorage.getItem('colors'));
console.log(colors[0]); // 'red'
```

---

#### ৯. **স্টোরেজ ইভেন্টগুলি**

স্টোরেজ ইভেন্ট ব্যবহারকারী যখন একটি স্টোরেজ পদ্ধতিতে পরিবর্তন করে তখন ট্রিগার হয়।

**ব্যবহারিক উদাহরণ:**
```javascript
window.addEventListener('storage', function(event) {
    console.log('Storage key changed:', event.key);
    console.log('New value:', event.newValue);
});
```

---

#### ১০. **localStorage এর ব্যবহার**

**ব্যবহারিক উদাহরণ:**
```javascript
localStorage.setItem('theme', 'dark');
let theme = localStorage.getItem('theme');
console.log('Current theme:', theme);
```

---

#### ১১. **sessionStorage এর ব্যবহার**

**ব্যবহারিক উদাহরণ:**
```javascript
sessionStorage.setItem('sessionData', 'data');
let sessionData = sessionStorage.getItem('sessionData');
console.log('Session data:', sessionData);
```

---

#### ১২. **ওয়েব স্টোরেজে নিরাপত্তার বিবেচনা**

ওয়েব স্টোরেজে সংরক্ষিত ডেটা ক্লায়েন্ট-সাইডে থাকে এবং এক্সেস করা সহজ। sensitive তথ্য যেমন পাসওয়ার্ড বা ক্রেডেনশিয়াল সংরক্ষণ করা উচিত নয়।

---

#### ১৩. **ওয়েব স্টোরেজে কর্মক্ষমতা বিবেচনা**

ওয়েব স্টোরেজের ডেটার আকার বড় হলে ব্রাউজারের কর্মক্ষমতায় প্রভাব ফেলতে পারে। কিছু ব্রাউজার সীমিত সংখ্যক আইটেম বা মোট আকারে সীমাবদ্ধতা রাখে।

---

**সারসংক্ষেপ:**

লোকাল স্টোরেজ এবং সেশন স্টোরেজ ওয়েব পৃষ্ঠায় ডেটা সংরক্ষণ ও পরিচালনা করার জন্য ব্যবহৃত হয়। `localStorage` দীর্ঘমেয়াদী ডেটা সংরক্ষণ করে, আর `sessionStorage` শুধুমাত্র বর্তমান সেশনের জন্য ডেটা সংরক্ষণ করে। JSON.stringify এবং JSON.parse ব্যবহার করে অবজেক্ট ও অ্যারে সংরক্ষণ এবং পুনরুদ্ধার করা যায়। স্টোরেজ ইভেন্ট এবং নিরাপত্তা বিবেচনা করার মাধ্যমে এদের কার্যকারিতা উন্নত করা যায়।







### ২৩. **মডিউলস**

মডিউলস হল কোডের অংশ যা পৃথকভাবে তৈরি, রক্ষণাবেক্ষণ, এবং পুনরায় ব্যবহারযোগ্য হয়। মডিউল সিস্টেম কোডের গঠন এবং পুনঃব্যবহারযোগ্যতা উন্নত করে। JavaScript এ মডিউল ব্যবহারের জন্য ES6 (ECMAScript 2015) নতুন মডিউল সিস্টেম এনেছে।

---

#### ১. **মডিউলের পরিচিতি**

মডিউল হল কোডের একটি ব্লক যা নির্দিষ্ট কার্যকলাপ সম্পাদন করে এবং অন্য মডিউল বা স্ক্রিপ্ট দ্বারা পুনরায় ব্যবহার করা যেতে পারে। ES6 মডিউল সিস্টেম মডিউলগুলোকে পৃথক ফাইল হিসেবে সংজ্ঞায়িত করে।

---

#### ২. **ES6 মডিউল সিনট্যাক্স (import এবং export)**

ES6 মডিউলস `import` এবং `export` কিওয়ার্ড ব্যবহার করে কোড ভাগ করে নেয়।

**এক্সপোর্ট করা:**
```javascript
// myModule.js
export const pi = 3.14;
export function calculateArea(radius) {
    return pi * radius * radius;
}
```

**ইমপোর্ট করা:**
```javascript
// main.js
import { pi, calculateArea } from './myModule.js';
console.log(pi); // 3.14
console.log(calculateArea(5)); // 78.5
```

---

#### ৩. **ডিফল্ট এক্সপোর্ট**

একটি মডিউল শুধুমাত্র একটি ডিফল্ট এক্সপোর্ট থাকতে পারে। এটি প্রাথমিক এক্সপোর্ট যা সরাসরি ইমপোর্ট করা হয়।

**ডিফল্ট এক্সপোর্ট:**
```javascript
// myDefaultModule.js
const greeting = 'Hello, world!';
export default greeting;
```

**ডিফল্ট এক্সপোর্ট ইমপোর্ট করা:**
```javascript
// main.js
import greeting from './myDefaultModule.js';
console.log(greeting); // Hello, world!
```

---

#### ৪. **নামযুক্ত এক্সপোর্ট**

একাধিক নামযুক্ত এক্সপোর্ট একসাথে ব্যবহার করা যেতে পারে।

**নামযুক্ত এক্সপোর্ট:**
```javascript
// myNamedModule.js
export const name = 'John';
export const age = 30;
```

**নামযুক্ত এক্সপোর্ট ইমপোর্ট করা:**
```javascript
// main.js
import { name, age } from './myNamedModule.js';
console.log(name); // John
console.log(age); // 30
```

---

#### ৫. **মডিউল ইমপোর্ট**

মডিউল ফাইল থেকে একাধিক উপাদান ইমপোর্ট করা যায়।

**ইমপোর্ট উদাহরণ:**
```javascript
// anotherModule.js
export function multiply(a, b) {
    return a * b;
}
export function divide(a, b) {
    return a / b;
}
```

**মডিউল ইমপোর্ট করা:**
```javascript
// main.js
import { multiply, divide } from './anotherModule.js';
console.log(multiply(2, 3)); // 6
console.log(divide(6, 2)); // 3
```

---

#### ৬. **সমস্ত এক্সপোর্ট একটি অবজেক্ট হিসাবে ইমপোর্ট করা**

**মডিউল এক্সপোর্ট:**
```javascript
// allExports.js
export const name = 'Alice';
export const age = 25;
export function greet() {
    return 'Hello!';
}
```

**সব এক্সপোর্ট একটি অবজেক্ট হিসাবে ইমপোর্ট করা:**
```javascript
// main.js
import * as all from './allExports.js';
console.log(all.name); // Alice
console.log(all.age); // 25
console.log(all.greet()); // Hello!
```

---

#### ৭. **ডাইনামিক ইমপোর্ট**

**ডাইনামিক ইমপোর্ট ব্যবহার:**
```javascript
// main.js
async function loadModule() {
    const module = await import('./myDynamicModule.js');
    console.log(module.default);
}
loadModule();
```

---

#### ৮. **একাধিক ফাইল থেকে এক্সপোর্ট করা**

একাধিক ফাইল থেকে এক্সপোর্ট করতে মডিউলগুলিকে একত্রিত করা যায়।

**ফাইল ১:**
```javascript
// file1.js
export const value1 = 'Value from file 1';
```

**ফাইল ২:**
```javascript
// file2.js
export const value2 = 'Value from file 2';
```

**একত্রিত করা:**
```javascript
// combined.js
export * from './file1.js';
export * from './file2.js';
```

**ইমপোর্ট করা:**
```javascript
// main.js
import { value1, value2 } from './combined.js';
console.log(value1); // Value from file 1
console.log(value2); // Value from file 2
```

---

#### ৯. **মডিউল স্কোপ**

মডিউলগুলির মধ্যে পরিবর্তনশীলগুলি শুধুমাত্র সেই মডিউলের অভ্যন্তরীণ স্কোপে দেখা যায়, যা মডিউল স্কোপের কারণে অন্যান্য মডিউল থেকে এক্সেস করা যায় না।

**মডিউল স্কোপ উদাহরণ:**
```javascript
// moduleA.js
const secret = 'This is a secret';
export const publicData = 'This is public data';
```

```javascript
// moduleB.js
import { publicData } from './moduleA.js';
console.log(publicData); // This is public data
console.log(secret); // ReferenceError: secret is not defined
```

---

#### ১০. **মডিউল পুনরায় এক্সপোর্ট করা**

মডিউল পুনরায় এক্সপোর্ট করতে `export` কিওয়ার্ড ব্যবহার করা হয়।

**মডিউল পুনরায় এক্সপোর্ট করা:**
```javascript
// utilities.js
export { functionA, functionB } from './moduleA.js';
```

---

#### ১১. **মডিউল ব্যবহারের ব্যবহারিক উদাহরণ**

মডিউল ব্যবহার করে বিভিন্ন কাজ সহজে সংগঠিত করা যায়, কোড পুনঃব্যবহার করা যায় এবং প্রকল্পের গঠন উন্নত করা যায়।

**ব্যবহারিক উদাহরণ:**
```javascript
// dataModule.js
export const data = [1, 2, 3, 4, 5];

// processData.js
import { data } from './dataModule.js';

export function processData(arr) {
    return arr.map(item => item * 2);
}

// main.js
import { processData } from './processData.js';
import { data } from './dataModule.js';

const result = processData(data);
console.log(result); // [2, 4, 6, 8, 10]
```

---

#### ১২. **Webpack এর মতো টুলগুলির সাথে মডিউল বান্ডলিং**

Webpack এবং অন্যান্য বান্ডলার টুল ব্যবহার করে মডিউলগুলিকে একত্রিত করা যায় এবং প্রোডাকশন ব্যবহারের জন্য প্রস্তুত করা যায়। 

**Webpack কনফিগারেশন উদাহরণ:**
```javascript
// webpack.config.js
const path = require('path');

module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'bundle.js',
        path: path.resolve(__dirname, 'dist')
    },
    module: {
        rules: [
            {
                test: /\.js$/,
                exclude: /node_modules/,
                use: {
                    loader: 'babel-loader',
                    options: {
                        presets: ['@babel/preset-env']
                    }
                }
            }
        ]
    }
};
```

**নোট:** Webpack এর সাহায্যে কোড বিভক্তি, লোডারস, প্লাগিনস ইত্যাদি ব্যবহার করে উন্নত ফিচারগুলির সাথে বান্ডলিং করা যায়।

---

**সারসংক্ষেপ:**

মডিউলস কোডের সংগঠন এবং পুনরায় ব্যবহারযোগ্যতা উন্নত করে। ES6 মডিউল সিনট্যাক্স `import` এবং `export` কিওয়ার্ড ব্যবহার করে মডিউলগুলির মধ্যে কোড ভাগ করা হয়। ডিফল্ট এক্সপোর্ট, নামযুক্ত এক্সপোর্ট, ডাইনামিক ইমপোর্ট, এবং মডিউল স্কোপের সাথে কাজ করা হয়। Webpack এর মতো টুলগুলির সাহায্যে মডিউল বান্ডলিংয়ের মাধ্যমে কোড ম্যানেজমেন্ট সহজ হয়।





### ২৪. **ফেচ API**

**Fetch API** হলো একটি আধুনিক ব্রাউজার API যা HTTP রিকোয়েস্ট এবং রেসপন্স পরিচালনা করতে ব্যবহৃত হয়। এটি `XMLHttpRequest` (XHR) এর একটি আধুনিক প্রতিস্থাপক, এবং এটি একটি প্রমিস-ভিত্তিক ইন্টারফেস প্রদান করে যা কোডের জন্য বেশি পরিষ্কার এবং সহজ পড়তে।

---

#### ১. **Fetch API পরিচিতি**

Fetch API হল একটি নতুন ইন্টারফেস যা একটি প্রমিস-ভিত্তিক উপায়ে HTTP রিকোয়েস্ট করতে এবং রেসপন্স গ্রহণ করতে সহায়তা করে। এটি ব্রাউজারের `window` অবজেক্টের অংশ এবং এটি আসিনক্রোনাস অপারেশনের জন্য প্রমিস ব্যবহার করে।

---

#### ২. **GET রিকোয়েস্ট করা**

**GET রিকোয়েস্ট** হলো একটি HTTP মেথড যা সার্ভার থেকে ডেটা প্রাপ্তির জন্য ব্যবহৃত হয়।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

---

#### ৩. **রেসপন্স ডেটা পরিচালনা**

**ফেচ API** তে রেসপন্স একটি প্রমিস প্রদান করে যা `.json()`, `.text()`, বা `.blob()` মেথড ব্যবহার করে প্রসেস করা যেতে পারে।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
    .then(response => response.json()) // JSON ডেটা রূপান্তর
    .then(data => {
        console.log(data);
        // ডেটা ব্যবহার
    })
    .catch(error => console.error('Error:', error));
```

---

#### ৪. **ফেচ-এ ত্রুটি পরিচালনা**

Fetch API শুধুমাত্র নেটওয়ার্ক ত্রুটির জন্য প্রমিস প্রত্যাখ্যান করবে, HTTP স্ট্যাটাস কোড 200-299 ছাড়া।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts/9999')
    .then(response => {
        if (!response.ok) {
            throw new Error('Network response was not ok ' + response.statusText);
        }
        return response.json();
    })
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

---

#### ৫. **POST রিকোয়েস্ট করা**

**POST রিকোয়েস্ট** নতুন ডেটা সার্ভারে পাঠানোর জন্য ব্যবহৃত হয়।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json'
    },
    body: JSON.stringify({
        title: 'foo',
        body: 'bar',
        userId: 1
    })
})
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

---

#### ৬. **রিকোয়েস্ট হেডার সেট করা**

রিকোয়েস্ট হেডার সেট করার জন্য `headers` প্রপার্টি ব্যবহার করা হয়।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts', {
    method: 'GET',
    headers: {
        'Authorization': 'Bearer your-token',
        'Accept': 'application/json'
    }
})
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

---

#### ৭. **JSON রেসপন্স সহ কাজ করা**

রেসপন্স JSON ডেটা রূপান্তর করতে `.json()` মেথড ব্যবহার করুন।

**কোড উদাহরণ:**
```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
    .then(response => response.json()) // JSON ডেটা রূপান্তর
    .then(data => console.log(data)) // JSON ডেটা লগ
    .catch(error => console.error('Error:', error));
```

---

#### ৮. **async/await সহ ডেটা অ্যাসিঙ্ক্রোনাসলি ফেচ করা**

`async` এবং `await` ব্যবহার করে কোডকে আরও ক্লিন এবং পড়তে সহজ করা যায়।

**কোড উদাহরণ:**
```javascript
async function fetchData() {
    try {
        const response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
        if (!response.ok) {
            throw new Error('Network response was not ok ' + response.statusText);
        }
        const data = await response.json();
        console.log(data);
    } catch (error) {
        console.error('Error:', error);
    }
}

fetchData();
```

---

#### ৯. **ফেচ রিকোয়েস্ট অ্যাবোর্ট করা**

ফেচ রিকোয়েস্ট অ্যাবোর্ট করার জন্য `AbortController` ব্যবহার করা হয়।

**কোড উদাহরণ:**
```javascript
const controller = new AbortController();
const signal = controller.signal;

fetch('https://jsonplaceholder.typicode.com/posts/1', { signal })
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => {
        if (error.name === 'AbortError') {
            console.log('Fetch request was aborted');
        } else {
            console.error('Error:', error);
        }
    });

// অ্যাবোর্ট রিকোয়েস্ট
controller.abort();
```

---

#### ১০. **CORS সহ ফেচ ব্যবহার**

CORS (Cross-Origin Resource Sharing) ব্যবহারের জন্য কিছু হেডার যুক্ত করা প্রয়োজন হতে পারে।

**কোড উদাহরণ:**
```javascript
fetch('https://api.example.com/data', {
    method: 'GET',
    headers: {
        'Authorization': 'Bearer your-token',
        'Content-Type': 'application/json'
    }
})
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error('Error:', error));
```

---

#### ১১. **ফেচ ব্যবহারের ব্যবহারিক উদাহরণ**

প্র্যাকটিক্যাল উদাহরণ হিসেবে ফেচ API ব্যবহারের সাথে একটি ফর্ম ডেটা জমা দেওয়ার উদাহরণ:

**ফর্ম ডেটা সাবমিট উদাহরণ:**
```javascript
document.querySelector('form').addEventListener('submit', async (event) => {
    event.preventDefault();

    const formData = new FormData(event.target);

    try {
        const response = await fetch('https://jsonplaceholder.typicode.com/posts', {
            method: 'POST',
            body: JSON.stringify(Object.fromEntries(formData.entries())),
            headers: {
                'Content-Type': 'application/json'
            }
        });

        if (!response.ok) {
            throw new Error('Network response was not ok ' + response.statusText);
        }

        const data = await response.json();
        console.log(data);
    } catch (error) {
        console.error('Error:', error);
    }
});
```

---

#### ১২. **অন্যান্য মেথডের সাথে ফেচ তুলনা করা (XHR, Axios)**

- **XHR (XMLHttpRequest)**: পুরানো পদ্ধতি যা ফেচ API এর তুলনায় বেশ জটিল এবং প্রমিস-ভিত্তিক নয়। কোড সাধারণত বেশি বর্গাকার এবং বিভ্রান্তিকর।

- **Axios**: একটি জনপ্রিয় থার্ড-পার্টি লাইব্রেরি যা প্রমিস-ভিত্তিক এবং XHR এর তুলনায় ব্যবহার সহজ।

**Axios উদাহরণ:**
```javascript
axios.get('https://jsonplaceholder.typicode.com/posts/1')
    .then(response => console.log(response.data))
    .catch(error => console.error('Error:', error));
```

**ফেচ API** আধুনিক ব্রাউজারসের জন্য সহজ এবং প্রমিস-ভিত্তিক সমাধান প্রদান করে, তবে প্রয়োজনে Axios বা XHR ব্যবহার করা যেতে পারে।



