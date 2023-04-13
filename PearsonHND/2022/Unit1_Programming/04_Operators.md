# Unit 1 - Programming 

[Home](README.md) | [Prev](03_ConstVar.md) | [Next](05_ConStructs.md)

## 4.1 Operators

- C# supports a wide-variety of operators
- These operators can be mainly classified into the following
	- Arithmetic
	- Assignment
	- Unary (Increment/Decrement)
	- Relational (Comparison)
	- Bit-wise operators (out of scope for this)
	- Bit shift operators (out of scope for this)
	- Ternary Operator (out of scope for this)

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Type</th>
    <th class="tg-0pky">Operator</th>
    <th class="tg-0pky">Description</th>
    <th class="tg-0pky">Example</th>
    <th class="tg-0lax">Output</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="5">Arithmetic</td>
    <td class="tg-0lax">+</td>
    <td class="tg-0lax">Addition: Sum of two number types<br>Concatenation: String with any other type</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(5 + 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">11</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">-</td>
    <td class="tg-0lax">Subtraction: Difference of two number types</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(5 - 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">-1</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">*</td>
    <td class="tg-0lax">Multiplication: Multiple of two numbers</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(5 * 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">30</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">/</td>
    <td class="tg-0lax">Division: Quotient of the dividend divided by divisor</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(6.0 / 5.0);</pre></td>
    <td class="tg-0lax"><pre lang="c#">1.2</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">%</td>
    <td class="tg-0lax">Modulo: Remainder of the dividend divided by divisor</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(6 % 5);</pre></td>
    <td class="tg-0lax"><pre lang="c#">1</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="2">Assignment</td>
    <td class="tg-0lax">=</td>
    <td class="tg-0lax">Value on the right is assigned to the variable on the left </td>
    <td class="tg-0lax"><pre lang="c#">
int a = 10;
Console.WriteLine(a);
int b = a;
Console.WriteLine(b);
int c = a * b;
Console.WriteLine(c);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
&nbsp;
10
&nbsp;
10
&nbsp;
100</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">+=<br>-=<br>*=<br>/=<br>%=</td>
    <td class="tg-0lax">Combined assignment: Assigns the result of the operation over the two values, to the variable on the left</td>
    <td class="tg-0lax"><pre lang="c#">
int a = 10;
Console.WriteLine(a += 5);
int b = 10;
b = b + 5;
Console.WriteLine(b);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
&nbsp;
15
&nbsp;
&nbsp;
15</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="3">Unary</td>
    <td class="tg-0lax">++</td>
    <td class="tg-0lax">Unary Increment (prefix): Increase the value of the variable by one</td>
    <td class="tg-0lax"><pre lang="c#">
int a = 10;
Console.WriteLine(++a);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
<br>
11</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">--</td>
    <td class="tg-0lax">Unary Decrement (prefix): Decrease the value of the variable by one</td>
    <td class="tg-0lax"><pre lang="c#">
int a = 10;
Console.WriteLine(--a);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
<br>
9</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">Unary Increment (postfix): Same as prefix, but has lesser precedence</td>
    <td class="tg-0lax"><pre lang="c#">
int a = 10;
Console.WriteLine(a++);
Console.WriteLine(a);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
&nbsp;
10
11</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax" rowspan="6">Relational</td>
    <td class="tg-0lax">==</td>
    <td class="tg-0lax">Equality: Checks if two values are equal; True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(5 == 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">False</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">!=</td>
    <td class="tg-0lax">Inequality: Checks if two values are not equal: True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">Console.WriteLine(5 != 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">True</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">&gt;</td>
    <td class="tg-0lax">Greater than: Checks if the value on the left is greater: True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">
Console.WriteLine(5 > 6);
Console.WriteLine(6 > 5);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
False
True</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">&gt;=</td>
    <td class="tg-0lax">Greater than or equal: Checks if the value on the left is greater than or equal: True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">
Console.WriteLine(5 >= 6);
Console.WriteLine(6 >= 5);
Console.WriteLine(6 >= 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
False
True
True</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">&lt;</td>
    <td class="tg-0lax">Less than: Checks if the value on the left is smaller: True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">
Console.WriteLine(5 < 6);
Console.WriteLine(6 < 5);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
True
False</pre></td>
  </tr>
  <tr>
    <td class="tg-0lax">&lt;=</td>
    <td class="tg-0lax">Less than or equal: Checks if the value on the left is less than or equal: True if they in fact are, False otherwise</td>
    <td class="tg-0lax"><pre lang="c#">
Console.WriteLine(5 <= 6);
Console.WriteLine(6 <= 5);
Console.WriteLine(6 <= 6);</pre></td>
    <td class="tg-0lax"><pre lang="c#">
True
False
True</pre></td>
  </tr>
</tbody>
</table>

## 4.2 Operator Precedence

- In an expression with multiple operators, the operators with higher precedence are evaluated before the operators with lower precedence.
- In the following example, the multiplication is performed first because it has higher precedence than addition:

```csharp
var a = 2 + 2 * 2;
Console.WriteLine(a); //  output: 6
```

- Use parentheses to change the order of evaluation imposed by operator precedence:

```csharp
var a = (2 + 2) * 2;
Console.WriteLine(a); //  output: 8
```

Read more about [C# operators and expressions - List all C# operators and expression | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/)
***
[Home](README.md) | [Prev](03_ConstVar.md) | [Next](05_ConStructs.md)