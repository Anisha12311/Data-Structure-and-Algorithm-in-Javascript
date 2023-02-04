# Data-Structure and Algorithm in Javascript

## Topics

* Fibonacci Series

      function fibonacci(num) {
            let a = 0, b = 1, temp;
            let fib = [];
            for (let i = 0; i < num; i++) {
              fib.push(a);
              temp = a;
              a = b;
              b = temp + b;
            }
          return fib;
      }
      
* Factorial of a number

       function factorial(num) {
           let result = 1;
           for(let i = 1; i<=num; i++) {
                result *= i;
           }
           return result 
       }
       
 * Prime number

        function isPrime(n) {
         if(n >= 1) return false;
         for(let i = 2; i< n ; i++){
            if(n % i === 0) return false;
         }
         return true;  
        }
           
 * Power of number
         
         function power(n) {
            if(n<1) return false;
            while(n>1) {
              if(n % 2 !== 0) return false;
               n = n/2
             }
             return true;
           }
           
 * Stack
 
        class Stack{
            constructor(){
              this.items = [];
            }

            add(element){
              return this.items.push(element)
            }
            pop(){
              if(this.items == 0) return "Underflow";
              return this.items.pop()
            }
            peek(){
              return this.items[this.items.length - 1];
            }

            isEmpty(){
              return this.items == 0;
            }
          }


            let stack = new Stack();
            stack.add(10);
            stack.add(20);
            stack.add(30);

            console.log(stack.items);
            console.log(stack.pop());
            console.log(stack.peek());
            console.log(stack.items);
       
       
 * Remove Duplicate Items from Array
 
          let a = [1,23,2,2,31,1,12,13,12,15,16,1];
          let b = a.reduce(function (acc, values){
                  if(acc.indexOf(values) === -1){
                  acc.push(values)
                  }
                  return acc;
                  },[])
          console.log(b)        
          
 * Calculate the Area of a Triangle
 
           // If we are known base or height
           
           let base = prompt("Enter the base of triangle ");
           let height = prompt("Enter the height of triangle ");
           
           let area = (base * height)/2
           console.log("The area of the triangle is " , area);
           
           //If we are known all sides of triangle
           
           let side1 = parseInt(prompt("Enter side1 "))
           let side2 = parseInt(prompt("Enter side2 "))
           let side3 = parseInt(prompt("Enter side3 "))
           //semi perimeter
           let s = (side1+side2+side3)/2
           let areaTri = Math.sqrt(s*(s-side1)*(s-side2)*(s-side3));
           console.log("The are of triangle is", areaTri);
           
 * Swap two variables
 
            let a = parseInt(prompt("Enter the first number "));
            let b = parseInt(prompt("Enter the second number "));
            a = a+b;
            b = a-b;
            a = a-b;

            console.log("First value after the swap ", a)
            console.log("Second value after the swap ",b)

* Convert kilometeres to miles

            let factors = 0.621;

            let kilometers = prompt("Enter the kilometers ");

            let miles = kilometers * factors;

            console.log("Miles ",miles)
   
* Convert Celsius to Fahrenheit

            //fahrenheit  = (celsius *1.8) + 32;
            //celsius = (fahrenheit - 32) / 1.8
            const celsius = prompt("Enter a celsius value ");

            const fahrenheit = (celsius * 1.8) + 32;

            console.log(fahrenheit)


