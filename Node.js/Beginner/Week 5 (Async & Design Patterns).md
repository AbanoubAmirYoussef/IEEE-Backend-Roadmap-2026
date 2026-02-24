# Materials

**Goal:**

Understand asynchronous behavior in JavaScript and use callbacks, promises, and async/await to handle asynchronous operations and API calls effectively.

### Topics

- JSON - APIs - Async vs Sync - Promises - Async/Await - Error handling and more
    - [Elzero Web School](https://www.youtube.com/playlist?list=PLDoPjvoNmBAx3kiplQR_oeDqLDBUDYwVv) [169:188]
- Creational Design Patterns (Factory, Singleton, Builder)
    - [Playlist](https://www.youtube.com/playlist?list=PLNE3WjwctlOz3Gx66tO5wxXu2C5E3Oj8i) [1:5]

### Task

## Part I — Theoretical

- Explain the difference between synchronous and asynchronous code.
- Explain Event Loop concept briefly.
- Why callback hell happens?
- Explain and write the usage:
    - callbacks
    - promises
    - async/await
- Describe design patterns using an example of your own

## Part II — Practical

- using [Numbers API]([http://numbersapi.com](http://numbersapi.com/))
    - Call it using `fetch`
    - Call it using `XMLHttpRequest`
    - Compare results.
- Using [Star Wars API Documentation] ([https://swapi.info](https://swapi.info/)), write a program that gets the planet name of the character with ID **4**
- One day Seif visited the fake store to buy some fake products.
    
    Seif bought:
    
    - 3 items of product 1
    - 4 items of product 4
    - 5 items of product 3
    
    Seif is bad at math, can you help him calculate the total price of the products?
    
    Utilize the [Fake Store API Documentation] ([https://fakestoreapi.com/](https://fakestoreapi.com/))
    
- The following code suffers from callback hell. The callbacks are nested in a confusing way. Solve the callback hell problem using each of:
    - Promise Chaining
    - Async/Await Syntax
    
    ```jsx
    setTimeout(() => {
        console.log("Hey there!");
    
        setTimeout(() => {
            console.log("This code will help you understand");
    
            setTimeout(() => {
                console.log("Asynchronous Programming");
    
                setTimeout(() => {
                    console.log("What The Callback Hell!!!");
    
                    setTimeout(() => {
                        console.log("I AM STUCK");
                    }, 1000);
                }, 3000);
            }, 2000);
        }, 3000);
    }, 5000);
    ```