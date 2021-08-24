## 1. Check prime number?

Algorithm :

step 1: Start the program.

step 2: Initialize the variable number and flag = true

step 3: Check the condition if given number is equal to 1 . then the number equal to 1 print it is `"prime number"` and go to step 9. If it is not equal to 1 go to next step.

step 4: Check else if condition the number greater than 1. If it is true then go to next step

step 5: Declare for loop initialize variable i with 2. Repeat the steps until i < number

step 6: Inside for loop give If condition of number remainder i equals to 0, if the condition is true then flag variable is set to false. and break the loop. go to next step.

step 7: Check if flag is equal to true print it is `"prime number"`. else print it is `"not a prime number"`.

step 8: The given number is not equal one and its not greater than 1 then print `"Give greater than 0"`.

step 9: stop the program.


Pseudocode :

	BEGIN
	INPUT number,flag=true;
	IF number === 1
	   PRINT "Prime Number"
	ELSE IF  number > 1
		FOR (let i=2;i<number;i++)
		   IF (number % i == 0) 
		        flag = false;
		          break;
		IF (flag)
		    PRINT "Prime Number"
		ELSE
		    PRINT "Not a Prime Number"   
	ELSE
		PRINT "Give greater than 0"		
	END

Source Code : 👉

## 2. What is difference between == and === with an example?

- ==  is used for comparing two variables, but it ignores the datatype of variable.
- === is used for comparing two variables, but this operator also checks datatype and compares two values.

Source Code : 👉

## 3. How would you reverse a string in JavaScript?

## Algorithm :

step 1: start the program.

step 2: Declare a function with the name of ReverseString with parameter.

step 3:	check three condition in if statement first check the input is present or not second check the string length must be greater than 2 and third check the input string is a type of string or not.

step 3: Inside function declare a empty string variable ReversedString. 

step 4: Declare For loop with initialize i value of string length -1, condition of for loop is until the string index goes zero and finaly with decrement one by i.

step 4.5: concatenating character in reverse order using addition assignment operator.


## Pseudocode :

	Declare a function with the name of ReverseString (string) 
	   if(!string AND string.length < 2 AND typeof string !== 'string') 
    		return "Not valid" 
	    let ReversedString = ""
	    FOR (let i = string.length - 1; i >= 0; i--) 
	        ReversedString += string[i]
	    PRINT ReversedString
	CALL the function with input parameter


Source Code : 👉

## 4. How would you reverse words in a sentence?

Algorithm :

step 1: start the program.

step 2: Declare a function with the name of ReverseWord with parameter.

step 3:	Inside function create a variable ReversedWord.

step 4: reverse a word using three methods i.e split(), reverse(), join(). Here, split method first seperate the string by space and form a array, In reverse() method reverse the string array and join() method concatenating all of the strings in an array.

step 5: print the reversed word in a sentence.

step 6: call the function with input parameter of sentence.

step 7: stop the program.

Pseudocode :

	Declare a function with the name of ReverseWord (string) 
		let ReversedWord;
		ReversedWord = console.log(string.split(" ").reverse().join(""));
		return ReversedWord
	CALL the function with input parameter(sentence)


Source Code : 👉

## 5. How will you verify a word as a palindrome?

## Algorithm :

step 1: start the program.

step 2: Declare a function with the name of Palindrome with parameter.

step 4:	check three condition in if statement first check the input is present or not and second check the input string is a type of string or not.

step 5: Inside function Convert lowercase and remove the special characters using replace() method.

step 6: Get the length of the string and stored it in a length variable.

step 7: Declare For loop with initialize value i is 0, condition i < length/2 and i is increment by 1.

step 7.1: Create If statement and check the first character is equal to last character and looply. if the character does not matches then return `Not a Palindrome`

step 9: After the for loop print "Palindrome". because the for loop if statement for only check the unmatched character is found or not. if none of the character is mismatched then print "palindrome".

step 10: call the function with input parameter.

step 11: stop the program.



## Pseudocode :

	Declare a function with the name of Palindrome (string) 
		if(!string AND typeof string !== 'string') 
    		RETURN "Not valid" 
		PerfectString = string.toLowerCase().replace(/[^A-Za-z0-9]/g, '');
		var length = PerfectString.length;
		FOR (let i = 0; i < length/2; i++) 
			IF (str[i] !== str[length - 1 - i]) 
			   RETURN 'not palindrome';
		RETURN 'palindrome';
		}
	CALL the function with input parameter(string)


Source Code : 👉

## 6. Write your own program to explain the difference between forEach and map?

`forEach :`

`map :`

Source Code : 👉

## 7. Generate a random number between 1 to 5?

The Math.random() function return random number by the random number generation algorithm. Based on browser engine it varies.

## 8. Remove duplicate from the following array?([1,2,9,4,5,8,3,5,1,4,5])

 

## 9. Write a program to calculate the sum of the first 10 natural numbers.

## Algorithm :

step 1: start the program.

step 2: declare a valiable sum and initialize to zero.

step 3: Declare for loop with initialize i value to 1, condition of less than equal to 10 and increment i by one.

step 3.4: adding sum value to looping i value and stored in variable sum.

step 4: print sum.

step 5: stop the program.

## Pseudocode :
	
	let sum = 0
	FOR (let i=1; i<=10; i++)
		sum += i;
	RETURN sum

## 10. Write a program to print the sum of the even and odd numbers for a given number?
(100)
 
## Algorithm :

step 1: start the program.

step 2: Declare the variable odd,eve and Number with initialize value of 20.

step 3: Declare For loop with initialize value of i is 0, condition i less than or equal to given number and increment i by one;.

step 3.4: Write If statement and check i modulus 2 equal to 0. if the condition true then sum the number with even variable else the number addon with odd variable.

step 4: print odd and even data.

step 5: stop the program.

## Pseudocode :

	let odd,even,Number = 20;
	FOR (let i=0;i<= Number; i++)
		IF (i % 2 ==0)
			even += i
		ELSE
			odd += i
	RETURN odd,even 

## 11. Write a program to merge two arrays? ([1,2,9,3,5,1,4,5], [11,54,70,40])

We have two merge action 

- `unmutable merge :` the merge result is stored in a new array.
	- ...spread method
	- concat() method
- `Mutable merge :`this method merge into an array without creating a new array.
	- push() method


## 12. Remove duplicate from an array of an object by id and name?
a. [{id: 1, name: ‘Stephen covey’ }, {id: 2, name: ‘Robin Sharma’ }, {id: 3, name:
‘Tolstoy’}, {id: 3, name: ‘Tolstoy’}, {id: 5, name: ‘James clear’}]

## 13. Compare two objects, If all properties are equal return true or return false?
a. ({id: 1, name: “edison”}, {id: 1, name: “edison”})
b. ({id: 1, name: “edison”}, {id: 2, name: “edison”})

## Algorithm :

step 1: start the program.

step 2: Declare a function with the name of compare with object parameter.

step 3:	Inside a function first get  property name of objects in both objects.

step 4: Declare if statement and check the object key length value is equal or not. If it is not then return false.

step 5: Declare For of loop for object iteration.

step 5.1: Declare If statement for check the value of object1 is equal to value of object2. If it is true then return true else return false

step 6: stop the program.

## Pseudocode :

	Declare a function with the name of compare (object1,object2) 
		const object1_key = Object.keys(object1)
		const object2_key = Object.keys(object2)
		if (object1_key.length !== object2_key.length) 
			return "false";
		for (let key of keys1) 
			if (object1[key] !== object2[key]) 
			  	return false;
	return true;



## 14. Take a multidimensional array and flat the array?[1,4,2,3,[10,20,20], [100,500,700,600],
[2000,1000]]

	The flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.

Source Code : 👉

## 15. Group by the id of the following array of objects using the Array.reduce method?
[{id: 1, name: ‘edison’ }, {id: 2, name: ‘Annand’ }, {id: 3, name: ‘Vasnath’}]

## 16. Write a program in Javascript to display the pattern like right angle triangle using an asterisk.The pattern like :
*
**
***
****
*****

	The function* declaration ( function keyword followed by an asterisk) defines a generator function, which returns a Generator object

Source Code : 👉

## 17. Write a program in Javascript to make such a pattern like right angle triangle with number increased by 
1
2 3
4 5 6
7 8 9 10

## Algorithm :

step 1: start the program.

step 2: Top initialize variables data set to 0 and DataFormation variable set to empty string.

step 3: for loop with initialize value i is 1 followed by condition is i<5 and i incremented by one.

step 3.1: Nested for loop with initialize value j is 0, condition of j<1 and j incremented by one.

step 3.1.1: increment data by one i.e data++

step 3.1.2: store the incremented data into DataFormation variable to concatenate it.

step 3.1.3: concatenate with space into DataFormation variable.

step 3.2: give new line.

step 4: return DataFormation variable. Because the triangle formation is stored in DataFormation variable.

## Pseudocode :

	let data = 0, DataFormation = ""
		FOR (let i = 1; i<5; i++) 
			FOR (let j = 0;j < i;j++) 
			   data++
			   DataFormation+= data
			   DataFormation +=" "
			DataFormation +="\n"
	RETURN DataFormation


Source Code : 👉

## 18. Write a program in Javascript to make such a pattern like a pyramid with numbers
increased by 1

		1
	   2 3
	  4 5 6
	 7 8 9 10

## Algorithm

step 1: start the program.

step 2: Top initialize variables data set to 0 and DataFormation variable set to empty string.

step 3: Declare a for loop with initialize value i become 1, condition of i<5 and i incremented by 1.

step 3.1: Declare nested for loop with initialize value j become 5, condition of `j<i` and j decremented by 1. Inside loop give space for center the data.

step 3.2: Add another for loop with initialize value k become 0, condition of `k < 2*i-i` and k incremented by 1.

step 3.2.1: increment data by one and concatenate the data to DataFormation variable finally concatenate with space.

step 4: give new line using '\n'.

step 5 return DataFormation.

step 6: stop the program.

## Pyramid Pseudocode :

	 let DataFormation = "",data=0;
	  FOR (let i = 1;i<5;i++) 
			FOR (let j=5;j>i;j--) 
		     DataFormation += " ";
		  FOR (let k = 0; k < 2*i-i ; k++) 
		     data++;
		     DataFormation += data;
		     DataFormation += " ";
	  DataFormation += "\n";
	  console.log(DataFormation);


Source Code : 👉

## 19. Write a program in Javascript to display the pattern like a diamond

	*
	***
	*****
	*******
	*********
	*******
	*****
	***
	*



## Algorithm

step 1: start the program. first the dimond pattern is combination of pyramid and reciprocal of pyramid.

step 2: Create two for loop one is for pyramid and another for loop for reciprocal of pyramid concept

step 3: top initialization of variable DataFormation set to empty string.

step 4: In first for loop is similiar to [Pyramid Pseudocode](#Pyramid-Pseudocode).

step 5: Declare Second for loop with the similiar logic of looping based on length of row.

step 5.1: Declare nested for loop with initial value j euqal to 0,condition `j < i` , j incremented by 1.

step 5.1.1: concatenate space with DataFormation variable using addition assignment operator.

step 5.2: declare another nested for loop with initial value `k euqal to (5-i)*2-1` , condition k > 0 and k decremented by 1.

step 5.2.1: concatenate * with variable DataFormation.

step 6: give new line using '\n'.

step 7: stop the program.

## Pseudocode :

	let DataFormation = "";
	FOR (let i = 1;i<=5;i++) 
		FOR (let j=5;j>i;j--) 
		   DataFormation += " ";
		FOR (let k=0;k<i*2-1;k++) 
		   DataFormation += "*";
		DataFormation += "\n";
	FOR (let i=1;i<=5-1;i++) 
		FOR (let j=0;j<i;j++) 
		   DataFormation += " ";
		FOR (let k=(5-i)*2-1;k>0;k--) 
		   DataFormation += "*";
		DataFormation += "\n";
	console.log(DataFormation);


Source Code : 👉

## 20. Explain following terms
a. console.log :
This Api used to give the output message in browser console. It's a string or object whaterver it is.

	let obj = {name:"javascript",age:12};
	let arr = [1,2,3,4];
	let string = "Hi";
	console.log(obj,arr,string);				// {name: "javascript", age: 12} (4) [1, 2, 3, 4] "Hi"

b. console.dir :
If you want to look at all the object’s properties and methods,you can use console.dir method. then you can see the contents of child objects too.

	let object = { property1 : 1, property1 : 2, method : function(){} };
    console.dir(object);
    Output : 👇
    > Object
        >method: ƒ ()
         property1: 2
        >[[Prototype]]: Object

c. console.count :
- This Api is gives the number of times it get called.
- If we did not called with parameter of label then it was called with the "default" label.

		function check() {
			console.count();
		console.log("javascript");
		}
		check();
		check();
		console.count();

    	Output : 👇
			default: 1
			VM60:4 javascript
			VM60:3 default: 2
			VM60:4 javascript
			VM60:8 default: 3
d. console.table :
- This Api method display the data in table format. In this method, one argument is mandatory. the argument is array of object. 
- The table label format may differ based on formation of array and object.

		console.table(["Javascript", "React js", "node js"]);
		let lang = [["c", "c++"], ["c#", "Dot net"], ["js", "node js"]];
		console.table(lang);

e. console.time/timeLog/timeEnd :

The `console.time()` method starts a timer you can use to track how long an operation takes. You give each timer a unique name, and may have up to `10,000 timers running` on a given page. When you call `console.timeEnd()` with the same name, the browser will output the time, in `milliseconds`, that elapsed since the timer was started.

You can track the amount of time between function calls. This can be helpful

	function obj() {
		let arr = Array(1000);
		for(let i=0; i<arr.length; i++) {
		    arr[i] = new Object();
		}
	}
	console.time();
		obj();
	console.timeEnd(); 								// default: 0.508056640625 ms


f. console.trace :
The console.trace() method outputs a stack trace to the Web console.

	function check() {
	  function nested() {
	    console.trace();
	  }
	  nested();
	}
	check();

	Output : 👇
		VM49:3 console.trace
		nested @ VM49:3
		check @ VM49:5
		(anonymous) @ VM49:7

g. console.group/groupEnd

This method creates a new inline group in the Web console log

	console.log("This is the outer level");
	console.group();
	console.log("Level 2");
	console.group();
	console.log("Level 3");
	console.warn("More of level 3");
	console.groupEnd();
	console.log("Back to level 2");
	console.groupEnd();
	console.log("Back to the outer level");

    Output : 👇
    This is the outer level
    console.group
		VM39:3 Level 2
		VM39:4 console.group
			VM39:5 Level 3
			VM39:6 More of level 3
			(anonymous) @ VM39:6
		VM39:8 Back to level 2
	VM39:10 Back to the outer level

h. console.assert

This method writes an error message to the console if the assertion is false. If the assertion is true, nothing happens.

	console.assert(false, 'the word is %s', 'foo');		//show error message
	console.assert(false, 'the word is %s', 'foo');		// nothing happen
	let data = 10;
	console.assert(data % 10 === 0, {number: data, errorMsg: "Not divisible by 10"});
	

