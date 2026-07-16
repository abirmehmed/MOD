# MOD

---

# 🟢 LEVEL 0: The Foundations (Beginner)
*Goal: Test basic syntax, vocabulary, and simple logic. Users should be able to read basic JS code.*

### **Module 1: Introduction & Basics**
* What is JavaScript? (Client-side vs Server-side)
* Linking JS to HTML (`<script>` tag, external files)
* Outputting data (`console.log()`, `alert()`)
* Comments (Single-line `//`, Multi-line `/* */`)
* *Target: 20 Questions*

### **Module 2: Variables & Data Types**
* Declaring variables (`var`, `let`, `const`)
* Primitive Data Types (String, Number, Boolean, Null, Undefined)
* The `typeof` operator
* Basic String methods (`.length`, `.toUpperCase()`, `.toLowerCase()`)
* *Target: 40 Questions*

### **Module 3: Operators & Expressions**
* Arithmetic Operators (`+`, `-`, `*`, `/`, `%`, `**`)
* Assignment Operators (`=`, `+=`, `-=`)
* Comparison Operators (`>`, `<`, `>=`, `<=`)
* Equality (`==` vs `===`)
* Logical Operators (`&&`, `||`, `!`)
* *Target: 40 Questions*

### **Module 4: Control Flow (Making Decisions)**
* `if`, `else if`, `else` statements
* The Ternary Operator (`condition ? true : false`)
* `switch` statements and `break`
* Truthy and Falsy values in JavaScript
* *Target: 30 Questions*

### **Module 5: Loops & Iteration**
* `for` loops
* `while` and `do...while` loops
* Loop control (`break` and `continue`)
* *Target: 30 Questions*

---

# 🟡 LEVEL 1: Core JavaScript & The DOM (Intermediate)
*Goal: Test practical application, ES6+ features, and how JS interacts with the web page.*

### **Module 6: Functions**
* Function Declarations vs. Function Expressions
* Parameters and Arguments
* Return statements
* Arrow Functions (Syntax and implicit returns)
* Scope (Global vs. Function vs. Block scope)
* *Target: 50 Questions*

### **Module 7: Arrays & Array Methods**
* Creating and accessing arrays (Zero-based indexing)
* Basic methods (`push`, `pop`, `shift`, `unshift`, `splice`, `slice`)
* Iteration methods (`forEach`, `map`, `filter`, `find`, `reduce`)
* *Target: 60 Questions (Array methods are heavily tested in interviews!)*

### **Module 8: Objects**
* Object literals and properties
* Dot notation vs. Bracket notation
* Adding, modifying, and deleting properties
* The `this` keyword (Basic usage in objects)
* *Target: 40 Questions*

### **Module 9: Modern JavaScript (ES6+ Features)**
* Template Literals (`` `Hello ${name}` ``)
* Destructuring (Arrays and Objects)
* Spread and Rest operators (`...`)
* Default parameters
* *Target: 40 Questions*

### **Module 10: The DOM (Document Object Model)**
* Selecting elements (`getElementById`, `querySelector`, `querySelectorAll`)
* Manipulating content (`innerText`, `innerHTML`, `textContent`)
* Manipulating styles and classes (`style`, `classList.add/remove/toggle`)
* Creating and appending new elements
* *Target: 40 Questions*

### **Module 11: DOM Events**
* Event Listeners (`addEventListener`)
* The Event Object (`e.target`, `e.preventDefault()`)
* Mouse events, Keyboard events, Form submissions
* Event Bubbling and Capturing (Basic concept)
* *Target: 30 Questions*

---

# 🔴 LEVEL 2: Under the Hood (Advanced)
*Goal: Test deep understanding of how JavaScript works asynchronously, memory management, and complex patterns.*

### **Module 12: Asynchronous JavaScript**
* The Call Stack and the Event Loop (Macrotasks vs Microtasks)
* Callbacks and "Callback Hell"
* Promises (States: Pending, Fulfilled, Rejected)
* `.then()`, `.catch()`, `.finally()`
* `async` and `await` syntax
* The Fetch API
* *Target: 60 Questions*

### **Module 13: Advanced Functions & Scope**
* Closures (Lexical scoping)
* Hoisting (Variables vs Functions, Temporal Dead Zone)
* The `this` keyword in depth (Implicit, Explicit, Arrow functions)
* `call()`, `apply()`, and `bind()`
* IIFE (Immediately Invoked Function Expressions)
* *Target: 50 Questions*

### **Module 14: Object-Oriented JavaScript (OOP)**
* Prototypes and the Prototype Chain
* ES6 Classes (`class`, `constructor`, `extends`, `super`)
* Public vs. Private class fields (`#privateVar`)
* Static methods and properties
* *Target: 40 Questions*

### **Module 15: Advanced Object & Error Handling**
* `try...catch...finally` blocks
* Throwing custom errors
* Object methods (`Object.keys()`, `Object.values()`, `Object.entries()`)
* Optional Chaining (`?.`) and Nullish Coalescing (`??`)
* Shallow Copy vs. Deep Copy
* *Target: 40 Questions*

---

# 🟣 LEVEL 3: Expert & Niche (Bonus/Pro)
*Goal: For senior developers and JS enthusiasts. These are tricky, edge-case questions.*

### **Module 16: Web APIs & Storage**
* Local Storage vs. Session Storage vs. Cookies
* Timers (`setTimeout`, `setInterval`, `clearTimeout`)
* JSON (`JSON.stringify`, `JSON.parse`)
* *Target: 20 Questions*

### **Module 17: Memory & Performance**
* Garbage Collection (Mark and Sweep)
* Memory Leaks (How they happen and how to avoid them)
* Event Delegation (Optimizing event listeners)
* *Target: 20 Questions*

### **Module 18: Metaprogramming & Generators**
* Generators (`function*`, `yield`)
* Iterators and `Symbol.iterator`
* Proxies and Reflect API
* *Target: 20 Questions*

---

### 💡 How to use this Syllabus in your Database

To make your website use this syllabus, I recommend adding two new fields to your JSON structure: **`level`** (which you already have) and **`module_id`**.

Here is how your updated JSON structure should look:

```json
{
  "id": 104,
  "level": "intermediate",
  "module_id": "mod_07_arrays", 
  "module_name": "Arrays & Array Methods",
  "type": "code-fill-in-blank",
  "topic": "Array Methods",
  "question": "Complete the code to create a new array...",
  "code_snippet": "const doubled = numbers._______(num => num * 2);",
  "options": ["forEach", "map", "filter", "reduce"],
  "correct_answer": "map",
  "explanation": "map() creates a new array by applying a function to every element..."
}
```

### Why this structure is a game-changer for your website:

1. **Create "Learning Paths":** Your frontend can now have a dashboard that says: *"Level 0: 20% Complete. Next up: Module 4 Quiz!"*
2. **Targeted Practice:** If a user keeps failing questions about `map()` and `filter()`, your site can automatically generate a "Custom Quiz" pulling only from `module_id: "mod_07_arrays"`.
3. **Progress Tracking:** You can easily show a progress bar for each module (e.g., "You have answered 30 out of 60 questions correctly in Module 7").

If you follow this syllabus and aim for the "Target" question counts listed above, you will naturally hit **~830 high-quality questions**. Once you add a few variations of the code-snippet questions, you will easily cross the **1,000 question mark** with a perfectly balanced curriculum!
