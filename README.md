# JavaScript-Notes

# **JavaScript for Website Development**

---

## **1. What JavaScript Is and Why It Is Used**

JavaScript is a **client-side programming language** used to add **logic, interactivity, and dynamic behavior** to websites. While HTML builds the structure and CSS styles the appearance, JavaScript controls **actions and responses**. It allows websites to react immediately to user inputs without reloading the page.

JavaScript is used in:

* Interactive forms
* Buttons and menus
* Image sliders
* Games and animations
* Online systems such as e-commerce and digital services

Modern websites **cannot function effectively without JavaScript**.

---

## **2. How to Run JavaScript Using VS Code**

### **Step-by-step process**

1. Open **VS Code**
2. Create a new folder (e.g. `myWebsite`)
3. Inside the folder, create:

   * `index.html`
   * `script.js`
4. Open `index.html` in a browser
5. Link JavaScript using the `<script>` tag

Example:

```html
<script src="script.js"></script>
```

### **Viewing Output**

* `alert()` → popup window
* `console.log()` → browser console (Press **F12** → Console tab)
* `document.write()` → webpage output

---

## **3. Ways of Adding JavaScript to HTML (With Examples)**

### **a) Inline JavaScript**

```html
<button onclick="alert('Clicked')">Click</button>
```

Other examples:

```html
<button onclick="alert('Welcome')">Welcome</button>
<input onchange="alert('Changed')">
<img onclick="alert('Image clicked')">
<a onclick="alert('Link clicked')">Link</a>
<div onclick="alert('Div clicked')">Box</div>
```

---

### **b) Internal JavaScript**

```html
<script>
  alert("Internal JS");
</script>
```

More examples:

```html
<script>console.log("Hello")</script>
<script>document.write("Text")</script>
<script>let x = 10;</script>
<script>if(true){alert("Yes")}</script>
<script>for(let i=1;i<=3;i++){console.log(i)}</script>
```

---

### **c) External JavaScript (Best Practice)**

HTML:

```html
<script src="script.js"></script>
```

JavaScript (`script.js`):

```javascript
alert("External JS");
```

More examples:

```javascript
console.log("Connected");
document.write("Loaded");
let age = 16;
alert(age);
function greet(){alert("Hi")}
```

---

## **4. JavaScript Comments**

### **Examples**

```javascript
// Single line comment
```

```javascript
/* Multi-line
   comment */
```

More examples:

```javascript
// Variable declaration
/* Loop example */
let x = 10; // store number
// alert("Hidden")
/* Function below */
```

---

## **5. Variables in JavaScript**

Variables store information.

### **Examples**

```javascript
let name = "Eric";
let age = 17;
let score = 85;
let isStudent = true;
let country = "Rwanda";
```

Other examples:

```javascript
let total = 10 + 5;
let price = 3000;
let status = false;
let grade = "A";
let year = 2026;
```

---

## **6. JavaScript Data Types**

### **Main data types**

Examples:

```javascript
let text = "Hello";      // String
let number = 10;        // Number
let active = true;      // Boolean
let empty = null;       // Null
let notSet;             // Undefined
```

More examples:

```javascript
let city = "Kigali";
let marks = 90;
let passed = false;
let data = null;
let x;
```

---

## **7. JavaScript Data Structures**

### **a) Arrays**

Arrays store multiple values.

```javascript
let fruits = ["Apple", "Banana", "Mango"];
```

More examples:

```javascript
let numbers = [1,2,3,4];
let names = ["John","Mary"];
let scores = [80,90,70];
let colors = ["Red","Blue"];
let days = ["Mon","Tue"];
```

Accessing arrays:

```javascript
console.log(fruits[0]);
```

---

### **b) Objects**

Objects store data in **key-value pairs**.

```javascript
let student = {
  name: "David",
  age: 16,
  grade: "G11"
};
```

More examples:

```javascript
let car = {brand:"Toyota",year:2020};
let user = {username:"admin",active:true};
let phone = {model:"Samsung",price:200};
let book = {title:"JS",pages:200};
let school = {name:"KDA",students:500};
```

---

## **8. JavaScript Operators**

Examples:

```javascript
let sum = 10 + 5;
let diff = 10 - 5;
let prod = 10 * 5;
let div = 10 / 5;
let rem = 10 % 3;
```

Comparison:

```javascript
10 == 10
10 != 5
10 > 5
10 < 20
```

---

## **9. Output Methods**

### **Examples**

```javascript
alert("Hello");
console.log("Testing");
document.write("Welcome");
```

More examples:

```javascript
alert(10);
console.log(5+5);
document.write("<h1>Title</h1>");
alert("Grade 11");
console.log("Done");
```

---

## **10. Conditional Statements**

### **Examples**

```javascript
if (age >= 18) {
  alert("Adult");
}
```

More examples:

```javascript
if (marks >= 50){alert("Pass")}
else{alert("Fail")}

if (x > y){console.log("Greater")}
if (loggedIn){alert("Welcome")}
if (score == 100){alert("Excellent")}
```

---

## **11. Loops**

### **For loop**

```javascript
for(let i=1;i<=5;i++){
  console.log(i);
}
```

More examples:

```javascript
for(let i=0;i<3;i++){alert(i)}
for(let i=10;i>=1;i--){console.log(i)}
for(let x=1;x<=10;x++){document.write(x)}
for(let i=0;i<names.length;i++){console.log(names[i])}
```

---

## **12. Functions**

### **Examples**

```javascript
function greet(){
  alert("Hello");
}
```

More examples:

```javascript
function add(){console.log(2+3)}
function showName(){alert("Eric")}
function welcome(){document.write("Welcome")}
function test(){console.log("Testing")}
function info(){alert("Info")}
```

---

## **13. Events in JavaScript**

Examples:

```html
<button onclick="greet()">Click</button>
```

Other examples:

```html
<button onclick="add()">Add</button>
<input onkeyup="alert('Typing')">
<img onclick="alert('Image')">
<div onclick="alert('Box')"></div>
<body onload="welcome()">
```

---

## **14. DOM Manipulation**

Examples:

```javascript
document.getElementById("demo").innerHTML = "Changed";
```

More examples:

```javascript
document.getElementById("title").style.color="red";
document.getElementById("box").style.display="none";
document.getElementById("msg").innerHTML="Hello";
document.getElementById("btn").disabled=true;
```

---

## **15. Form Validation**

Examples:

```javascript
if(name==""){alert("Required")}
```

More examples:

```javascript
if(age<18){alert("Too young")}
if(password.length<6){alert("Weak")}
if(email==""){alert("Enter email")}
if(score>100){alert("Invalid")}
```

---

## **16. JavaScript Keywords (Important)**

Common keywords students must know:

* `let`
* `var`
* `const`
* `if`
* `else`
* `for`
* `while`
* `function`
* `return`
* `break`
* `continue`
* `true`
* `false`
* `null`
* `undefined`
* `new`

---

## **17. Applications of JavaScript in Websites**

---

# **17. Applications of JavaScript in Websites (Extended)**

JavaScript is the core technology that makes modern websites interactive, responsive, and user-friendly. It allows websites to respond to user actions instantly, validate information, update content dynamically, and create engaging experiences without reloading the page. Below are the major applications of JavaScript in website development, explained in detail with multiple practical examples.

---

## **1. Login Systems**

JavaScript is widely used to control login systems by validating user input, checking credentials, and controlling access to pages. While secure authentication is usually handled on the server, JavaScript plays an important role in checking form fields, giving instant feedback, and improving user experience before data is sent.

Examples of JavaScript use in login systems:

* Checking if username and password fields are empty
* Displaying error messages when login fails
* Limiting login attempts
* Showing or hiding passwords
* Redirecting users after successful login

### **HTML–JavaScript Integration Examples**

**Example 1: Check empty login fields**

```html
<input id="user" placeholder="Username">
<input id="pass" type="password" placeholder="Password">
<button onclick="checkLogin()">Login</button>

<script>
function checkLogin(){
  if(user.value=="" || pass.value==""){
    alert("All fields required");
  }
}
</script>
```

**Example 2: Simple credential check**

```html
<button onclick="login()">Login</button>
<script>
function login(){
  if(user.value=="admin" && pass.value=="123"){
    alert("Login successful");
  }
}
</script>
```

**Example 3: Show password**

```html
<input type="checkbox" onclick="showPass()"> Show Password
<script>
function showPass(){
  pass.type="text";
}
</script>
```

**Example 4: Lock login after attempts**

```html
<script>
let tries=0;
function check(){
  tries++;
  if(tries>3){alert("Account locked")}
}
</script>
```

**Example 5: Redirect user**

```html
<script>
function success(){
  window.location="dashboard.html";
}
</script>
```

---

## **2. Online Forms**

JavaScript controls form behavior by validating input, preventing incorrect submissions, and improving usability. It ensures that users provide correct and complete data before submission.

Examples of JavaScript use in forms:

* Checking required fields
* Validating email format
* Limiting character length
* Displaying error messages
* Preventing submission when data is invalid

### **HTML–JavaScript Integration Examples**

**Example 1: Required field**

```html
<input id="name">
<button onclick="validate()">Submit</button>
<script>
function validate(){
  if(name.value==""){alert("Name required")}
}
</script>
```

**Example 2: Email validation**

```html
<script>
function checkEmail(){
  if(!email.value.includes("@")){alert("Invalid email")}
}
</script>
```

**Example 3: Limit characters**

```html
<script>
if(message.value.length>100){alert("Too long")}
</script>
```

**Example 4: Prevent submit**

```html
<form onsubmit="return false;">
```

**Example 5: Success message**

```html
<script>
alert("Form submitted successfully");
</script>
```

---

## **3. Pop-Up Messages**

Pop-ups are used to give users alerts, confirmations, warnings, or notifications. JavaScript creates pop-ups without reloading the page.

Examples of JavaScript pop-ups:

* Welcome messages
* Error alerts
* Confirmation dialogs
* Warning notifications
* Information pop-ups

### **HTML–JavaScript Integration Examples**

**Example 1: Welcome alert**

```html
<script>alert("Welcome to our website");</script>
```

**Example 2: Confirmation**

```html
<script>
confirm("Are you sure?");
</script>
```

**Example 3: Prompt input**

```html
<script>
let name=prompt("Enter your name");
</script>
```

**Example 4: Button pop-up**

```html
<button onclick="alert('Clicked')">Click</button>
```

**Example 5: Page load alert**

```html
<body onload="alert('Loaded')">
```

---

## **4. Sliders and Image Galleries**

JavaScript allows images to change automatically or when users click buttons. Sliders make websites more visual and interactive.

Examples of sliders:

* Automatic image slideshows
* Product image viewers
* Banner sliders
* Manual image navigation
* Portfolio galleries

### **HTML–JavaScript Integration Examples**

**Example 1: Change image**

```html
<img id="img" src="1.jpg">
<button onclick="change()">Next</button>
<script>
function change(){img.src="2.jpg";}
</script>
```

**Example 2: Auto slide**

```html
<script>
setInterval(change,2000);
</script>
```

**Example 3: Gallery click**

```html
<img onclick="img.src='pic2.jpg'">
```

**Example 4: Image toggle**

```html
<script>
img.style.display="none";
</script>
```

**Example 5: Thumbnail viewer**

```html
<img onclick="main.src=this.src">
```

---

## **5. Games**

JavaScript powers browser-based games by controlling logic, scoring, movement, and interaction.

Examples of JavaScript games:

* Number guessing game
* Quiz games
* Click-counter games
* Puzzle games
* Memory games

### **HTML–JavaScript Integration Examples**

**Example 1: Guessing game**

```html
<script>
if(guess==number){alert("Correct")}
</script>
```

**Example 2: Score counter**

```html
<script>
score++;
</script>
```

**Example 3: Click game**

```html
<button onclick="count++">Click</button>
```

**Example 4: Timer**

```html
<script>
setTimeout(end,5000);
</script>
```

**Example 5: Win message**

```html
alert("You win!");
```

---

## **6. Dashboards**

Dashboards display real-time data such as statistics, charts, and reports using JavaScript.

Examples:

* Student results dashboard
* Business analytics
* Attendance systems
* Financial reports
* Website statistics

### **HTML–JavaScript Integration Examples**

**Example 1: Display score**

```html
<script>
document.getElementById("score").innerHTML=85;
</script>
```

**Example 2: Update data**

```html
setInterval(update,1000);
```

**Example 3: Show/hide panel**

```html
panel.style.display="block";
```

**Example 4: Count users**

```html
users++;
```

**Example 5: Chart update**

```html
console.log("Chart updated");
```

---

## **7. Validation Systems**

JavaScript validation ensures data is correct before submission.

Examples:

* Password strength check
* Age validation
* Email format validation
* Phone number check
* Score limits

### **HTML–JavaScript Integration Examples**

**Example 1: Password length**

```html
if(pass.value.length<6){alert("Weak")}
```

**Example 2: Age check**

```html
if(age<18){alert("Not allowed")}
```

**Example 3: Score limit**

```html
if(score>100){alert("Invalid")}
```

**Example 4: Empty check**

```html
if(field==""){alert("Required")}
```

**Example 5: Match passwords**

```html
if(p1!=p2){alert("Mismatch")}
```

---

## **8. Interactive Menus**

JavaScript creates menus that open, close, or animate.

Examples:

* Dropdown menus
* Mobile menus
* Sidebar navigation
* Hover menus
* Expandable sections

### **HTML–JavaScript Integration Examples**

**Example 1: Toggle menu**

```html
menu.style.display="block";
```

**Example 2: Close menu**

```html
menu.style.display="none";
```

**Example 3: Button menu**

```html
<button onclick="openMenu()">Menu</button>
```

**Example 4: Hover menu**

```html
<div onmouseover="show()">Menu</div>
```

**Example 5: Sidebar toggle**

```html
sidebar.classList.toggle("active");
```

---

## **9. Chat Systems**

JavaScript enables messaging systems by sending and displaying messages instantly.

Examples:

* Live chat boxes
* Chatbots
* Customer support chats
* Messaging panels
* Notification alerts

### **HTML–JavaScript Integration Examples**

**Example 1: Send message**

```html
document.getElementById("chat").innerHTML+=msg;
```

**Example 2: Input message**

```html
let msg=input.value;
```

**Example 3: Clear chat**

```html
chat.innerHTML="";
```

**Example 4: Auto scroll**

```html
chat.scrollTop=chat.scrollHeight;
```

**Example 5: Chat alert**

```html
alert("New message");
```

---

## **10. Online Services (e.g. Irembo-style Systems)**

JavaScript enables complex online platforms that deliver services digitally.

Examples:

* Service request forms
* Payment confirmations
* Status tracking
* Appointment booking
* Notification systems

### **HTML–JavaScript Integration Examples**

**Example 1: Service request**

```html
alert("Request submitted");
```

**Example 2: Status update**

```html
status.innerHTML="Approved";
```

**Example 3: Booking system**

```html
if(date==""){alert("Select date")}
```

**Example 4: Payment message**

```html
alert("Payment successful");
```

**Example 5: Progress tracker**

```html
progress.value=80;
```

---
