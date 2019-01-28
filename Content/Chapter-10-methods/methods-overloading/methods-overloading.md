# Method Overloading

In many programming languages like C# and Java the same method can be declared in **few variants** with the same name and different parameters. This goes by the term “**method overloading**”. Now let's see how to write these overloaded methods.

## Method Signature

In programming **the way** you can **identify** a method is through **the couple of elements** of its declaring – **name** of the method and **a list** containing its parameters. These two elements determine its **specification**, the so invoked **signature** of the method. 

![](/assets/chapter-10-images/16.Method-signature-01.png)

In this example the methods signature is its name (**`Print`**), and also its parameter (**`string text`**).

If our program has **methods with the same names**, but with **different signatures**, we can say that we have **method overloading**.

## Overloading Methods in C\#

As we mentioned, if you use **the same name for several methods with different signatures**, this means that you are **overloading a method**. The code below shows how three different methods can use the same name, but have different signatures and execute different actions.

![](/assets/chapter-10-images/17.Method-overloading-01.png)

## Signature and Return Value Type

It is important to say that **the returned type as a result** of the method **is not a part of its signature**. If the returned type was a part of the signature, then the compiler doesn't know which method exactly to call.

Let's look at the following example – we have two methods with different return types. Despite that, Visual Studio shows that there is a mistake, because both of their signatures are the same. Therefore when trying to call a method named **`Print(…)`**, the compiler can't know which of the two methods to run.

![](/assets/chapter-10-images/17.Method-overloading-02.png)

## Example: Greater of Two Values

The input is two values of the same type. The values can be of **`int`**, **`char`** or **`string`** type. Create a method **`GetMax()`** that returns as a result the greater of the two values.

### Sample Input and Output

| Input | Output | Input | Output | Input | Output |
| --- | --- | --- | --- | --- | --- |
|int<br>2<br>16|16|char<br>a<br>z|z|string<br>Ivan<br>Todor|Todor|

### Creating the Methods

We need to create three methods with the same name and different signatures. First we create a method, which will compare integers.

![](/assets/chapter-10-images/18.Greater-of-two-values-01.png)

Following the logic of the previous method we create another one with the same name, but this one will compare characters.

![](/assets/chapter-10-images/18.Greater-of-two-values-02.png)

The next method we need to create will compare strings. The logic here is a bit different from the previous two methods because variables of **`string`** type can not be compared with the operators **`<`** and **`>`**. We will use the method **`CompareTo(…)`**, which returns a numerical value: larger than 0 (the compared object is larger), smaller than 0 (the compared object is smaller) and 0 (the two objects are the same).

![](/assets/chapter-10-images/18.Greater-of-two-values-03.png)

### Reading the Input Data and Using the Methods

The last step is to read the input data, to use the appropriate variables and to invoke the method **`GetMax()`** from the body of the **`Main()`** method.

![](/assets/chapter-10-images/18.Greater-of-two-values-04.png)

### Testing in the Judge System

Test your solution here: [https://judge.softuni.bg/Contests/Practice/Index/594#6](https://judge.softuni.bg/Contests/Practice/Index/594#6).
