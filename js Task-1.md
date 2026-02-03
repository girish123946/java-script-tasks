js Task-1

 
 1.)	Difference between var, let, and const ? 

var is function-scoped, allows redeclaration, and allows reinitialization, which can sometimes cause unexpected behavior.

let is block-scoped, does not allow redeclaration in the same scope, but allows reinitialization.

const is block-scoped, does not allow redeclaration or reinitialization, and is used for values that should remain constant.

 2.)Which keyword allows redeclaration and why? 

 Answer: Var allows redeclaration 
Reason: var is function-scoped, so JavaScript allows redeclaring the same variable within the same scope. 
 
3.)	Which keyword allows reinitialization? 
Answer: var and let allow reinitialization 
Reason: They are designed to allow value changes after declaration

4.)	Which keyword does not allow redeclaration and reinitialization? 
Answer: Const  Keyword does not allow both redeclaration and reinitialization 
Reason: const creates a constant reference that cannot be changed or redeclared

5.)	Why should const be used for fixed values? 
     Answer:  
Prevents accidental reassignment 
Makes code safer and predictable 
Improves readability 
Helps JavaScript engine optimize code 
 
6.)	What error occurs when redeclaring a let variable? 
Answer: Syntax Error 
Reason: let is block-scoped and redeclaration is not allowed in the same scope. 

7.)	What error occurs when reassigning a const variable? 
Answer: TypeError 
Reason: const variables cannot be reassigned once initialized. 
 

8.)	Which keyword is preferred in modern JavaScript and why?  
Answer: let and const are preferred 
Reason:  
  Block-scoped (avoids bugs)   No accidental redeclaration   const ensures immutability 
  Cleaner and safer code 
 
 
9.)	Can const be declared without initialization? Explain. 
Answer: NO 
Reason: const must be initialized at the time of declaration because its value cannot be changed later

10.)When should var be avoided? 
•	Writing modern JavaScript (ES6+) 
•	Working inside blocks (if, for, while) 
•	Preventing hoisting-related bugs 
•	Building large or secure application 
 
Section B: code-based questions. 
 
11.)Predict the output? 
var a=10;
a=20;
var a =30;
console.log(a);
output :30
Reason: var allows redeclaration and reassignment, so the last value (30) is printed. 

12.)Predict the output? 
let b=5;
b=15;
console.log(b);
output: 15
Reason: let allows reinitialization (reassignment) but not redeclaration 
 
13.)Identify the error? 
let x=10;
let x=20; 
output: syntaxError Identifier ‘x’ has already been declared 
Reason: let does not allow redeclaration in the same scope 
 
14.)Identify the error? 
const y = 50; 
y =100;
output :TypeError:Assignment to constant varaiable
Reason: const does not allow reassignment. 
 
15.)Program using var to show redeclaration? 
var name ="Girish";
var name ="kumar";
console.log(name);
output :Kumar
Reason: var allows redeclaration 
 
16.)Program using let to show reinitialization? 
let age = 21; 
age = 22; 
console.log(age);  
ouput:22 
Reason : let allows reassignment but not redeclaration 
 
17.)Program using const and explanation? 
const maxScore = 100; 
console.log(maxScore); 
output : 100 
Explanation 
•	const variables must be assigned a value when declared 
•	The value cannot be changed later 
 
18.)Convert var to let where applicable? 
var count = 10; 
count = 20; 
let count = 10; 
count = 20; 
Reason : No redeclaration needed 
 
19.)Convert var to const where applicable? 
var country = "India"; 
const country = "India"; 
Reason : Value never changes use const 
 
20.) Write your own example for var, let, and const? 
Example for var 
var name = "Girish"; 
var name = "Kumar";   // Redeclaration allowed 
name = "HS Girish";   // Reassignment allowed 
console.log(name);  
output : H.S Girish 
Explanation : Var allows redeclaration and reassignment 
  
 Example for let  
 let age = 21; 
 age = 22;   // Reassignment allowed 
 console.log(age); 
 output : 22 
Explanation: let allows reassignment and does not allow redeclaration 
 
Example for const 
Const country =”India”; 
Country =”USA”; // Reassignment not allowed 
Ouput : Error 
Explanation : const does not allow redeclaration and reassignment . The value is fixed. 
 
 
 
 
 
 

