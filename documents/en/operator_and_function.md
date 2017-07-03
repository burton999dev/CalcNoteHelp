# Operators and Functions
`CalcNote` supports many operators and mathematical functions which is great for trigonometry, for instance.

## Operators
|Operator|Description|Example|
|:-----------|:------------|:------------|
`+`|Addition|1 `+` 1 = 2
`-`|Subtraction|1 `-` 1 = 0
`*`|Multiplication|2 `*` 3 = 6
`/`|Division|10 `/` 2 = 5
`mod`|Gets the remainder of a division.|5 `mod` 2 = 1
`%`|Percentage calculations.|1000 + 10`%` = 1100
`$`|Line references ${LineNo}|`$1` + `$2`
`0x`|Prefix for the hexadecimal|`0xFA8B`
`0o`|Prefix for the octal|`0o7712`
`0b`|Prefix for the binary|`0b0101`
`&`|Logical AND|0b0101 `&` 0b0011 = 0b0001
`&#124;`|Logical OR|0b0101 `&#124;` 0b0011 = 0b0111
`~`|Logical NOT|`~`0b10 = 0b01
`XOR`|Logical XOR|0b0101 `XOR` 0b0011 = 0b0110
`<<`|Left arithmetic shift|0b0110 `<<` 2 = 0b11000
`>>`|Right arithmetic shift|0b0110 `>>` 2 = 0b0001
`nPr`|Permutation|`5P2` = 20
`nCr`|Combination|`5C2` = 10
`!`|Factorial|5`!` = 120
`√`|Square root|`√`9 = 3
`^`|Power|3 `^` 2 = 9
`=`|Variable assignment|MB `=` 1024 * 1024

**All operators can be used for decimal, hexadecimal and binary.**

## Functions
|Function|Parameter|Description|Example|
|:-----------|:------------|:------------|:------------|
`sin(x)`|`x`:An angle, in radians|Returns the trigonometric sine of an angle.|
`asin(x)`|`x`:The value whose arc sine is to be returned|Returns the arc sine of a value; the returned angle is in the range -pi/2 through pi/2.|
`sinh(x)`|`x`:The number whose hyperbolic sine is to be returned|Returns the hyperbolic sine of a value. The hyperbolic sine of x is defined to be (ex - e-x)/2 where e is Euler\'s number.|
`cos(x)`|`x`:An angle, in radians|Returns the trigonometric cosine of an angle.|
`acos(x)`|`x`:The value whose arc cosine is to be returned|Returns the arc cosine of a value; the returned angle is in the range 0.0 through pi.|
`cosh(x)`|`x`:The number whose hyperbolic cosine is to be returned|Returns the hyperbolic cosine of a value. The hyperbolic cosine of x is defined to be (ex + e-x)/2 where e is Euler's number.|
`tan(x)`|`x`:An angle, in radians|Returns the trigonometric tangent of an angle.|
`atan(x)`|`x`:The value whose arc tangent is to be returned|Returns the arc tangent of a value; the returned angle is in the range -pi/2 through pi/2.|
`tanh(x)`|`x`:The number whose hyperbolic tangent is to be returned|Returns the hyperbolic tangent of a value. The hyperbolic tangent of x is defined to be (ex - e-x)/(ex + e-x), in other words, sinh(x)/cosh(x). Note that the absolute value of the exact tanh is always less than 1.|
`log(x)`|`x`:A value|Returns the base 10 logarithm of a value.|
`log2(x)`|`x`:A value|Returns the base 2 logarithm of a value.|
`ln(x)`|`x`:A value|Returns the natural logarithm (base e) of a value.|
`exp(x)`|`x`:The exponent to raise e to|Returns Euler's number e raised to the power of a value.|
`round(x)`|`x`:A floating-point value to be rounded to an integer|Returns the closest int to the x, with ties rounding up.|round(100.4) = 100<br>round(100.5) = 101
`rhup(x, places)`|`x`:The value to round to places number of places<br>`places`:The number of decimal places to which to round.places may be negative, in which case value is rounded at the specified number of digits to the left of the decimal point.|Rounds a number to a certain number of decimal places according to standard rules.|rhup(153.47, 0) = 153<br>rhup(153.47, 1) = 153.5<br>rhup(153.47,-1) = 150
`ceil(x)`|`x`:A value|Returns the smallest (closest to negative infinity) value that is greater than or equal to the argument and is equal to a mathematical integer.|ceil(100.3) = 101<br>ceil(-100.3)= -100
`rup(x, places)`|`x`:The value to round to places number of places, always rounding up<br>`places`:The number of decimal places to which to round.places may be negative, in which case value is rounded at the specified number of digits to the left of the decimal point.|Rounds a number to a certain number of decimal places, always rounding up to the next valid increment.|rup(153.47, 0) = 154<br>rup(153.47, 1) = 153.5<br>rup(153.47,-1) = 160
`floor(x)`|`x`:A value|Returns the largest (closest to positive infinity) value that is less than or equal to the argument and is equal to a mathematical integer.|floor(100.3) = 100<br>floor(-100.3) = -101
`rdown(x, places)`|`x`:The value to round to places number of places, always rounding down.<br>`places`:The number of decimal places to which to round.places may be negative, in which case value is rounded at the specified number of digits to the left of the decimal point|Rounds a number to a certain number of decimal places, always rounding down to the next valid increment.|rdown(153.47, 0) = 153<br>rdown(153.47, 1) = 153.4<br>rdown(153.47,-1) = 150
`cbrt(x)`|`x`:A value|Returns the cube root value. For positive finite x, cbrt(-x) == -cbrt(x); that is, the cube root of a negative value is the negative of the cube root of that value\'s magnitude.|
`abs(x)`|`x`:The argument whose absolute value is to be determined|Returns the absolute value. If the argument is not negative, the argument is returned. If the argument is negative, the negation of the argument is returned.|abs(100) = 100<br>abs(-100)= 100
`sum(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the sum of a series of numbers and/or line references.|sum($1, $6)
`avg(val1, val2)`|`val1`:The first line reference<br>`val3`:The second line reference|Returns the average of a series of numbers and/or line references.|avg($1, $6)
`max(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the maximum of a series of numbers and/or line references.|max($1, $6)
`min(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the minimum of a series of numbers and/or line references.|min($1, $6)
`var(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the variance of a series of numbers and/or line references.|var($1, $6)
`stdev(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the standard deviation of a series of numbers and/or line references.|stdev($1, $6)
`median(val1, val2)`|`val1`:The first line reference<br>`val2`:The second line reference|Returns the median of a series of numbers and/or line references.|median($1, $6)

## Subtotals
You can calculate subtotals using `Subtotal` keyword.
`Subtotal` only calculates up to the last `Subtotal`.Subtotal results are not included in the total.


```java
Drink
120 * 6    /*=720*/
250 * 6    /*=1500*/
Subtotal   /*=2220*/

Food
480 * 2    /*=960*/
235 * 1    /*=235*/
890 * 2    /*=1780*/
Subtotal   /*=2975*/
Total      /*=5195*/
```

<br><br>
[HOME](index.md)　[How to use](how2use.md)　[Grammar](http://burton999dev.github.io/CalcNoteHelp/grammar_en.html)　[Unit Converter](unit_converter.md)　[Currency Converter](currency_converter.md)　[Floating Widget](floating_widget.md)　[Settings](settings.md)　[Customizing Keypad](customizing_keypad.md)　[CalcNotePlugin for GoogleDrive](google_drive_plugin.md)　[FAQ](faq.md)　[Customization Example](example4theme.md)  
