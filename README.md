# Fizzbuzz JavaScript Challange

- Question 1. Explain what the following lines of code do:
~~~
let  fizzBuzz = fs.readFileSync('./src/js/fizz-buzz.js');
eval( fizzBuzz + `\nexports.FizzBuzz = FizzBuzz;`)
~~~

- Question 2. Explain why we are placing the
~~~
let fizzBuzz = new FizzBuzz
~~~
outside the ```it``` block?

- Question 3. Explain the difference between using === and == in JS?

- Question 4. Explain why we are moving (number % 5 === 0) to the top?
A: There is no reason for this. The important thing is that the conditional for checking divisibility with 15 is declared first, since both 3 and 5 are factors of 15. If a number is not divisible by 15 all that is left is to check if it is either divisible by 3 or if it is divisible by 5. These two remaining cases are mutually exclusive and can thus be checked in any order.

- Question 5. Explain the difference between feature and unit test?
A:

- Question 6. Eplain what expectations in the context of testing are?
A:

Question 7: Write a line to line explanation of what is happening in this code:
~~~
<script src="src/js/fizz-buzz.js"></script> //Loads javascript file containing the FizzBuzz-function
    <script>
        document.addEventListener('DOMContentLoaded', () => { //Adds an event listner that fires when the page has been loaded
            let button = document.getElementById('button') //puts the button-element into a variable called 'button
            let displayDiv = document.getElementById('display_answer') //puts the display_answer div into a variable called 'displayDiv'
            button.addEventListener('click', () =>{  /adds an eventlistener to the button element that fires on the click event
                let value = document.getElementById('value').value // Get the value from input field and put it in a variable called value
                let fizzBuzz = new FizzBuzz // Create an instance of FizzBuzz
                let result = fizzBuzz.check(value) // calls the check function in fizzbuzz and passes in the value we got from the input field. Put the result in a variable called 'result'
                displayDiv.innerHTML = result; // Enters the result into the inner html of the displayDiv element.
            })
        })
    </script>
~~~

- Question 8: Explain what a CDN (Content Delivery Network) is?
A: A network of servers and data centers that are sprea out geographically so that it can deliver its services with high performance, low latency and a high degree of availiablity. It prioritizes servers/data centers closest to the client to deliver the content. Mostly used for delivery of web content.
