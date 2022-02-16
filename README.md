# Working with developers

[Use these slides](https://docs.google.com/presentation/d/1io0OSH00rFhvylfgk_PnqqhXQ60sbO08JNYn_adyhBs/edit#slide=id.g10e8e37efd6_0_3)

What do you want to get out of today? Specific things to learn?

#### What is programming?
- Commands to a computer
- Storing, manipulating, displaying data
- input and output

#### How?
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

#### Looking at code
	- Cyclomatic complexity
	- Average size system looks like:
		- 6TB of data
		- 1TB updated daily
		- 2.4GB of logs (~82.5 million)
		- 60 Virtual machines

#### How does the internet work?
- Show diagrams in slides
- Show browser developer tools
	- show network requests happening on a website load

#### Tips for talking to developers

- Dont make assumptions
- Schedule time with developers
	- Don't seagull
	- Don't secret squirrel
	- On average it takes 15 minutes to return to previous point when interupted
- Use images, flow charts, decision tables
- Use examples! 
- Ensure all the information required is provided:
```
1 reward point for every £1 you spend
100 points can be exchanged for £10
20% VAT is not included
```
- Write good stories!
	- Give problems, not solutions
	- Don't dictate tech
	- https://www.romanpichler.com/blog/10-tips-writing-good-user-stories/

Advanced concepts:
Testing (Unit, Integration, Acceptance)
TDD

