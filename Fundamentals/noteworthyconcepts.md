## Note-Worthy Concepts

<details>
  <summary>🎁 Storage vs Memory</summary>

  Storage is a computer’s long-term space for keeping data, like your hard drive or SSD.

  Memory (RAM) is temporary space used while the computer is running programs. It stores and processes data actively to avoid delays that would occur if everything had to be read directly from storage.

  When you install an app, it’s saved in storage. When you open it, the app’s data and operations are loaded into memory. The amount and speed of memory largely determine how fast the app can run.

  That's why most memory intensive programs like Davinci Resolve or Adobe After Effects often recommend users to allocate more memory space to the program.
</details>

<!-- Problem Solving -->
<details>
  <summary>🎁 Problem Solving</summary>

  When working on DSA problems, it’s helpful to first break down the problem in plain language, sketch visuals, or outline the formula needed to solve it before writing any code. This step represents the “Algorithm” part of DSA.

  Take recurssion for instance, at its core, recurssion is simply `Factorials (!)`, where:

  ```
  n! = n * (n - 1) * (n - 2) ... * 1;

  OR 

  n! = n * (n - 1)!
  ```

  This same concept applies to recurssion, it simply breaks down a problem into smaller chunks.
</details>

<!-- Recurssion -->
<details>
  <summary>🎁 Recurssion & Memoisation</summary>

  Recurssion is a method of solving complex problems by creating a function that calls itself, breaking down the problem into smaller units until it gets to the smallest unit. The result from each operation is returned up the call stack, layer by layer, untill it bubbles all the way back to the top.

  Example: Factorials with Recurssion.

  We know that the formular for factorials is n! = n * (n-1)!

  Also that 1! is 1 and 0! is 1 as well, so we can create a recurssive function using this formular.

  ```
  function fact(n) {
    if (n <= 1) return 1;
    return n * fact(n - 1);
  }
  ```
  
  Now this works, but the memory space and time required can grow quickly for large numbers - that's where Memoization comes in.

  ### Memoization 
  Memoization means storing computed values so that future calls can reuse them instead of recalculating the same results.

  In recursion, we do this by saving each computed value in an array (or object) and checking if it already exists before computing again:`.

  Here's the initial code, but with memoizaiton implemented.

  ```
  function fact(n, memo = []) {
    if (n <= 1) return 1;

    if (memo[n]) return memo[n];

    memo[n] = n * fact(n - 1, memo);
    return memo[n];
  }

  ```

  Now, each result is stored and reused, making it far more efficient for larger inputs.
</details>