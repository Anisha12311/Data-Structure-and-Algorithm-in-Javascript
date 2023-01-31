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
           
      

   



