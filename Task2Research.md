# Lamda expresions C#
Lambda expressions are used like anonymous functions it means that doesn`t contain any name.The **=>** is the lambda operator used in all containers
<br>For example;
in this case we represent the lambda expression with **Func**, 
can receive input parameters and will return a value 
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
___
<br>
https://www.geeksforgeeks.org/lambda-expressions-in-c-sharp/#:~:text=Lambda%20expressions%20in%20C%23%20are,used%20in%20all%20lambda%20expressions.