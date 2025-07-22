// ==========================================================
// Project: js-code-16-dats
// Duration: 21/07/2025 to 21/10/2025
// Purpose: Learning JavaScript step-by-step from basics
// ==========================================================


// =========================
// 📘 1.0_days.js
// =========================

// 🔹 Basic Introduction to JavaScript & V8 Engine

// 🔹 Variable Declaration
// let → modern (block scope)
// var → old (function scope, avoid using)
// const → constant (cannot be changed)

let a;
var b;
const c = 5;

const hello = "Gopal Das";
console.log(hello); // Output: Gopal Das



// =========================
// 📘 1.1_days.js
// =========================

// 🔹 Variable Declaration and Data Types
let name = "Gopal Das";
console.log(name); // Output: Gopal Das

// 🔹 JavaScript Data Types

/* 
📌 Primitive Data Types:
- Number
- String
- Boolean
- BigInt
- Null
- Undefined
- Symbol
*/

/*
📌 Non-Primitive Data Types:
- Array
- Object
- Function
*/

// 🔹 typeof() - To check variable type
let balance = 12;
console.log(typeof(balance)); // Output: number

let name_passBook = name;
console.log(typeof(name_passBook)); // Output: string

// 🔹 Null vs Undefined
let bal = null;
console.log(typeof(bal)); // Output: object (JavaScript quirk)

let account;
console.log(typeof(account)); // Output: undefined

// 🔹 BigInt
let number = 8955489815459575775754n; // 'n' suffix makes it a BigInt
console.log(typeof(number)); // Output: bigint

// 🔹 Safe Integer Range in JS
console.log(Number.MAX_SAFE_INTEGER); // Output: 9007199254740991
console.log(Number.MIN_SAFE_INTEGER); // Output: -9007199254740991

//==================================================================
// 🔰 JavaScript Day 2 – Notes + Code
// ✅ Topic: Non-Primitive Data Types, Type Conversion, Operators

// --------------------
// 🧠 Non-Primitive Data Types
// --------------------

// ✅ Array - Can store different types of values
let arr = [20, 36, "Gopal Das", 7.5];
console.log(typeof arr); // Output: object

// ✅ Object - Key:Value format
let obj = {
    user_name: "Gopal",
    account: 645367437647,
    balance: 420
};
console.log(obj);

// ✅ Function - typeof is 'function'
let fun = function () {
    console.log("Hello, 2nd days class...");
};
fun();

// ✅ Another function declaration
function fun1() {
    console.log("kiya...");
}
fun1();

console.log(); // spacing
console.log();

// --------------------
// 🔁 Type Conversion
// --------------------

// ✅ String ➝ Number
let balance = "100";
let num = Number(balance);
console.log(typeof balance); // string
console.log(typeof num);     // number

// ✅ Boolean ➝ Number
let x = true;
console.log(Number(x));      // Output: 1
console.log(typeof x);       // boolean

// ✅ NaN Example - Invalid string to number
let srt = "100cs";
console.log(Number(srt));    // Output: NaN (Not a Number)

// ✅ null ➝ 0
let x1 = null;
console.log(Number(x1));     // Output: 0

// ✅ undefined ➝ NaN
let x2 = undefined;
console.log(Number(x2));     // Output: NaN

console.log();
console.log();

// --------------------
// ➕ Operators & Precedence
// --------------------
// Order of execution:
// 1. Brackets
// 2. Multiply / Divide (left to right)
// 3. Add / Subtract (left to right)

console.log(20 % 4); // Output: 0 (modulus operator)

// ✅ Assignment Operator
let a = 10;
a += 5; // same as a = a + 5
console.log(a); // Output: 15
//==================================================================
// 📁 File: 2.0_day.js
// 📅 Date: 22/07/2025
// 🔥 Topic: Comparison & Bitwise Operators

// ========== COMPARISON OPERATORS ==========

// 1. == vs ===
// == checks value only (performs type conversion)
let num = 10;
let str = "10";
console.log(num == str); // true → value is same, type auto-converted

// === checks value AND type
console.log(num === str); // false → number vs string

// 2. Relational comparison with type conversion
let a1 = 10;
let str1 = "30";
console.log(a1 < str1); // true → "30" is converted to 30

// 3. null and undefined comparison
console.log(null == undefined);  // true → loosely equal
console.log(null === undefined); // false → types differ

// 4. ⚠️ Avoid chained comparisons like this:
let a = 10;
let b = "10";
let c = 1;
console.log(a == b == c); // false (unexpected behavior)
// Explanation: (a == b) → true → becomes 1
// Then: 1 == c → true
// But JS evaluates left to right: (true == 1) → true

// ========== BITWISE OPERATORS ==========

// & → Bitwise AND
console.log(3 & 2); // 2 → 011 & 010 = 010

// | → Bitwise OR
console.log(4 | 5); // 5 → 100 | 101 = 101

// << → Left shift (multiply by 2^n)
console.log(5 << 3); // 40 → 5 * 2^3 = 40

// >> → Right shift (divide by 2^n)
console.log(20 >> 2); // 5 → 20 / 2^2 = 5

/* ========== QUICK SUMMARY ==========

==      : Equal value (type converts)
===     : Equal value and type (strict)
null == undefined  : true
null === undefined : false

&       : Bitwise AND
|       : Bitwise OR
<<      : Left shift (× 2^n)
>>      : Right shift (÷ 2^n)

Avoid a == b == c → gives unexpected results due to type coercion

*/
//==========================================================


// =========================
// ✅ End of Combined Learning File
// More topics will be added soon...
// =========================
