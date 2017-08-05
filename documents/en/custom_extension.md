# Custom Extension

## User Defined Constant
User defined constant allows you to define your own constants. CalcNote has constant `π` that value is `3.14159265358979323846` by the default. As well as this, you can define your constant that is a commonly used value.

### List of user defined constants
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_const_list.png">

List of user defined constants is displayed. You can create new constant to tap the `+` button. Also you can edit and delete an existing constant to tap the `...` button.

### Editing a user defined constant
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_const_edit.png">

#### Constant Name
Enter the constant name. Constant name is displayed on keypad. You cannot use the same name as a function name or constant name already defined. The accepted characters are alphanumeric and "_" (underscore) and name must start with other than numeric.
#### Constant Value
Enter the constant value. The value must be numeric.
#### Save button
Save a user defined constant and back to the list of user defined constants. Saved constant can be assigned to the keypad.

## User Defined Action
User defined action allows you to define your own button. For instance, you can define the `TAX` button with a expression `+ 10%`. If you define commonly-used calculations as action, you can save the trouble of inputting.

### List of user defined actions
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_action_list.png">

List of user defined actions is displayed. You can create new action to tap the `+` button. Also you can edit and delete an existing action to tap the `...` button.

### Editing a user defined action
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_action_edit.png">

#### Action Name
Enter the action name. Action name is displayed on keypad.
#### Action Value
Enter the action value. You can set any expressions and comments as the action value.
#### Save button
Save a user defined action and back to the list of user defined actions. Saved action can be assigned to the keypad.

## User Defined Function
User defined function is like an excel macro. User defined function enables you to create a function using `JavaScript`.

### List of user defined functions
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_list.png">

List of user defined functions is displayed. You can create new function to tap the `+` button. Also you can edit and delete an existing function to tap the `...` button.

### Editing a user defined function(Definition)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit1.png">

#### Function Name
Enter the function name. You cannot use the same name as a function name or constant name already defined. Function name must be 1 to 8 characters. The accepted characters are alphanumeric and "_" (underscore) and name must start with other than numeric.
#### Description of Function
Enter the description of function. This description is used in the help. This field is optional.
#### Number of Parameters
Select the number of parameters.
#### Description of Return Value
Enter the description of return value. This description is used in the help. This field is optional.
#### NEXT button
Move to the next step.

### Editing a user defined function(Parameters)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit2.png">

#### Parameter Name
Enter the parameter name. The accepted characters are alphanumeric and "_" (underscore) and name must start with other than numeric.
#### Description of Parameter
Enter the description of parameter. This description is used in the help. This field is optional.
#### NEXT button
Move to the next step.
#### BACK button
Back to the previous step.

### Editing a user defined function(Code)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit3.png">

#### Source Code
Write the code of function in `JavaScript`.
#### NEXT button
Move to the next step.
#### BACK button
Back to the previous step.

### Editing a user defined function(Test)
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/user_fuction_edit4.png">

#### Value of Argument
Enter a value of argument to test.
#### ▲ Execution button
Tests a user defined function using specified arguments. The return value will be shown on the bottom of screen.
#### COMPLETE button
Save a user defined function and back to the list of user defined functions. Saved function can be assigned to the keypad.
#### BACK button
Back to the previous step.

### Builtin functions for user defined functions
You can use following functions in your code.

|Function|Description|
|:-----------|:------------|
val(x)|Gets the value of parameter. You must use this function if you want to support the line reference `$n` as parameter.
vals(x, y)|Gets an array object that contains results of specified range. For instance, `vals($1, $4)` returns the results from the first line to the fourth line as an array. Returned results is array of string. so you need to call `parseInt` function.
isRef(x)|Returns a Boolean value indicating whether `x` is a line reference.
get(url)|Downloads a specified URL and returns contents of response as a string. This function is executed synchronously. The response is cached for one hour.
sin(x)|This is a built-in function of the CalcNote.
asin(x)|This is a built-in function of the CalcNote.
sinh(x)|This is a built-in function of the CalcNote.
cos(x)|This is a built-in function of the CalcNote.
acos(x)|This is a built-in function of the CalcNote.
cosh(x)|This is a built-in function of the CalcNote.
tan(x)|This is a built-in function of the CalcNote.
atan(x)|This is a built-in function of the CalcNote.
tanh(x)|This is a built-in function of the CalcNote.
ln(x)|This is a built-in function of the CalcNote.
log2(x)|This is a built-in function of the CalcNote.
log(x)|This is a built-in function of the CalcNote.
sqrt(x)|This is a built-in function of the CalcNote.
cbrt(x)|This is a built-in function of the CalcNote.
floor(x)|This is a built-in function of the CalcNote.
ceil(x)|This is a built-in function of the CalcNote.
round(x)|This is a built-in function of the CalcNote.
pow(x, y)|This is a built-in function of the CalcNote.
exp(x)|This is a built-in function of the CalcNote.
rup(x, y)|This is a built-in function of the CalcNote.
rdown(x, y)|This is a built-in function of the CalcNote.
rhup(x, y)|This is a built-in function of the CalcNote.
abs(x)|This is a built-in function of the CalcNote.

### Limitations
1. CalcNote uses [Rhino v1.7.7.1](https://github.com/mozilla/rhino) to execute JavaScript. So supported feature depends on the Rhino.
2. User defined functions are compiled each time and then executed. So multiple calls to user-defined functions and complicated function can be affect performance.
3. `get` function sends a http request synchronously.

### Sample code
##### 1. Calculate the body mass index
```javascript
function bmi(height, weight) {
    var height_meter = val(height) / 100;
    return val(weight) / (height_meter * height_meter);
}
```

##### 2. Calculate the product
```javascript
function product(p1, p2) {
    var values;
    if (isRef(p1) && isRef(p2)) {
        values = vals(p1, p2);
    } else {
        values = [val(p1), val(p2)];
    }
    var total = 1;
    values.forEach(function(value) {
        total *= parseInt(value);
    });
    return total;
}
```

##### 3. Convert bitcoin to JPY
```javascript
function btc_jpy(btc) {
    var response = get('http://api.coindesk.com/v1/bpi/currentprice/JPY.json');
    var rate = JSON.parse(response);
    return rate.bpi.JPY.rate_float * val(btc);
}
```

<br><br>
[HOME](index.md)　[How to use](how2use.md)　[Grammar](http://burton999dev.github.io/CalcNoteHelp/grammar_en.html)　[Operators and Functions](operator_and_function.md)　[Unit Converter](unit_converter.md)　[Currency Converter](currency_converter.md)　[Floating Widget](floating_widget.md)　[Settings](settings.md)　[Customizing Keypad](customizing_keypad.md)　[CalcNotePlugin for GoogleDrive](google_drive_plugin.md)　[FAQ](faq.md)　[Customization Example](example4theme.md)  
