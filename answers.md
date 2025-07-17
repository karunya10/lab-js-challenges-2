1. Challenge 1:

- Answer: b)`"xyz"` and `"xyz"`
- Explanation:JavaScript is synchronous, meaning it executes code line by line. In this question, the function is invoked first. Inside the function, the globally scoped variable foo is reassigned. Therefore, the first console output will be "xyz", and the console output on the last line will also be "xyz", since the value was reassigned within the function.

2. Challenge 2:

- Answer:c) `10` and `1`
- Explanation: When the function is invoked with a as its argument, the scope of a here becomes a function, so when you reassign this a, it doesn't interfere with the a that is declared outside the function and hence the result.

3. Challenge 3:

- Answer:c) `"Hi there!"`
- Explanation: All functions in JavaScript are hoisted during the memory allocation phase, which means it is possible to invoke a function even before it is declared.But hoisting works differently for different typesof functions, hoisting works without throwing an error for named function but doesn't for anonymous and arrow function.

4. Challenge 4:

- Answer:`{ num: 90 }`
- Explanation: Here just the reference of 'a' will be copied to 'b' i.e 'b' will be pointing to the same memory reference that 'a' holds ,so 'b' will be directly manipulating the original object.

5. Bonus - Challenge 5:

- Answer:`{ name: "Bob", age: 10 }` and `{ name: "Ada", age: 20 }`
- Explanation: When I am invoking magicRabbit with rabbit1 , a new "let obj" will be passed as a parameter to the function, but this obj will still be a reference to rabbit1, therefore when we do obj.age=10 , it mutates the original object. But then after that we reassign the obj to an entirely new obj that holds a different reference in memory, so this obj will be different when returned.
