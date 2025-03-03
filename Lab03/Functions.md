# This Lab includes the step-by-step instructions to create and export functions in Node.js

## 📋 Table of Contents
1. [Create a New Node.js Project]
2. [Initialize the Project]
3. [Create a JavaScript File]
4. [ Write Functions in the Functions.js]
5. [Create index JS File]
6. [Run Your index.js]

### 1️⃣ 🗂️ Create a New Node.js Project
  - First, make sure you have Node.js installed. Then, create a new project directory and navigate into it.

---
### 2️⃣ 📦 Initialize the Project
 - Initialize a new Index.js project with **npm**:

         npm init -y
   
- This will create a **package.json** file in your project directory.

---
### 3️⃣ ✏️ Create a JavaScript File
  - Create a new JavaScript file named as **Functions.js**

### 4️⃣ 📝 Write Functions in the Functions.js
      
      // functions.js

     // A simple function to add two numbers
     function add(a, b) {
        return a + b;
     }

    // A function to subtract two numbers
    function subtract(a, b) {
        return a - b;
     }

    // Export the functions
    module.exports = { add, subtract };

---
### 5️⃣ 🖥️ Create Another JS File (index.js) to Use the Functions

  - Open index.js and import the functions from functions.js, then use them:
     
           // Import the functions from functions.js
           const { add, subtract } = require('./functions');

          // Use the functions
          const sum = add(5, 3);
          const difference = subtract(5, 3);

          console.log(`Sum: ${sum}`); // Output: Sum: 8
          console.log(`Difference: ${difference}`); // Output: Difference: 2

--- 

### 6️⃣ 🚀 Run Your index.js
  - At terminal :

          node index.js
    
  - Output

          Sum: 8
          Difference: 2

---







