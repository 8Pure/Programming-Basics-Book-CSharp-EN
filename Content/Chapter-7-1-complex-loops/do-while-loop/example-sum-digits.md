### Example: Sum Digits

Sum up the digits of a **positive** integer **n**. For example, if **n = 5634**, the result will be: 5 + 6 + 3 + 4 = **18**.

We can use the following idea to solve the problem:

   * We create the variable **`n`**, to which we assign a value equal to the number entered by the user.
   * We create a second variable - **`sum`**, which initial value is 0. We will use it for the calculation and storage of the result.
   * For a loop condition, we will use **`n > 0`** because after each calculation of the result in the body of the loop, we will remove the last digit of **`n`**.
   * In the body of the loop:
       * We assign a new value of **`sum`** that is the result of the sum of the current value of **`sum`** with the last digit of **`n`**.
       * We assign a new value to **`n`**, which is the result of removing the last digit of **`n`**.
   * Outside the body of the loop, we print the final value of the sum.

![](/assets/chapter-7-images/09.Sum-digits-01.png)

<table><tr><td><img src="/assets/alert-icon.png" style="max-width:50px;" /></td>
<td><code><strong>n % 10</strong></code>: <b>returns</b> the last digit of the number <code><strong>n</strong></code>.<br>
<code><strong>n / 10</strong></code>: <b>deletes</b> the last digit of <code><strong>n</strong></code>.</td>
</tr></table>

#### Testing in the Judge System

Test your solution here: [https://judge.softuni.bg/Contests/Practice/Index/514#8](https://judge.softuni.bg/Contests/Practice/Index/514#8).
