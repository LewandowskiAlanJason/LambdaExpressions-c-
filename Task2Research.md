# Lamda expresions C#
Lambda expressions are used like anonymous functions. It means that it doesn`t have a name.The **=>** is the lambda operator.
<br>For example, in this case we represent the lambda expression with **Func**. It can accept input parameters and will return a value:
>Func<parameter1,output>
___
```c#
class program{

static void Main (string[] args){
    Func<int,int>b=(a)=> a*2
    int result =b(4);

}

}

```
>result=16

Also you can receive more parameters, you just have to put them at the beginning, and the return value always goes at the end
>Func<parameter1, parameter2, parameter3, output>

## Uses:
### Example 1
- Its most used when you want to pass a small piece of code to another method, i.e. as a filtering method.
___
```

Func<Book, bool> filter = (book) => book.Price > 22;

var expensivesBooks = books.Where(filter);

```
### Example 2
Let's consider the following piece of code:
```
		Func<int,int, int> addThem = (NumA,NumB) => NumA + NumB;
		Console.Write(addThem(3,3));
```
Here, we used a lambda expression to define a function and do some operation quickly.

### Example 2
___
# Reference
<br>
<ol>
[1] https://www.geeksforgeeks.org/lambda-expressions-in-c-sharp/#:~:text=Lambda%20expressions%20in%20C%23%20are,used%20in%20all%20lambda%20expressions.</li>
[2] https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/lambda-expressions</li>
</ol>