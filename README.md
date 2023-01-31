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
   



