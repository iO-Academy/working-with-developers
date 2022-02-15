# Working with developers

What do you want to get out of today? Specific things to learn?

What is programming?
- Commands to a computer
- Storing, manipulating, displaying data
- input and output

How?
All programming languages use the same basic concepts
- Statements
- Data types (booleans, strings, ints, floats, arrays, objects)
- Variables
- Functions
	- Internal functions (PHP has ~5600)
        - User-defined functions
- Loops

Exercises: 'Hello World' program  
Tell students to Fork this: https://replit.com/@MikeOram/Working-with-developers#index.js

<details>
  <summary>Exercise Steps</summary>
  
  ```javascript
	
	// step 1
	output('hello world, how are you?');

	// step 2
	var rand = Math.random() * 1000;
	output('hello world, how are you?');
	output(rand);

	
	// step 3
	var rand = Math.random() * 1000;
	if (rand > 500) {
		output('hello world, how are you?');
	} else {
		output('hello mike, how are you?');
	}

	
	// step 4
	function sayHello(target) {
		output('hello ' + target + ', how are you?');
	}

	var rand = Math.random() * 1000;
	if (rand > 500) {
		sayHello('world');
	} else {
		sayHello('mike');
	}

	
	// step 5
	function sayHello(target) {
		output('hello ' + target + ', how are you?');
	}

	var rand = Math.random() * 1000;
	var name = 'mike';
	if (rand > 500) {
		name = 'world';
	}
	sayHello(name);


	// step 6
	function sayHello(target) {
		return 'hello ' + target + ', how are you?';
	}

	var rand = Math.random() * 1000;
	var name = 'mike';
	if (rand > 500) {
		name = 'world';
	}
	output(sayHello(name));

	
	// step 7 - second feature
	function sayHello(target, greeting = 'hello') {	
		return greeting + ' ' + target + ', how are you?';
	}

	var rand = Math.random() * 1000;
	var name = 'mike';
	if (rand > 500) {
		name = 'world';
	}
	output(sayHello(name));
	// somewhere else in your application
	output(sayHello('bob', 'hi'));// technical debt!


	// step 8 - tests in the console
	function sayHello(target, greeting = 'hello') {	
		return greeting + ' ' + target + ', how are you?';
	}

	var result = sayHello('mike');
	test('hello mike, how are you?', result)

	var result2 = sayHello('mike', 'hi');
	test('hi mike, how are you?', result2)
	
  ```
</details>

- Looking at code
	- Cyclomatic complexity

How does the internet work?
- User
- Browser
- HTTP Request
- DNS Lookup
- IP Address
- Server
- Apache/Nginx
- PHP -> Runs your program
- returns some text (string)
- HTTP Response
- Browser
- DOM

- Show browser developer tools

Technology stack (add to drawing)
- HTML & CSS
- JavaScript
- PHP
- MySQL

Advanced concepts:
Testing (Unit, Integration, Acceptance)
TDD

