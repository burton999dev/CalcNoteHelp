# How to use
The `CalcNote` is a calculator but it has appearance similar to the notepad.So you might be confused but it's simple and easy to use.  
This section describes the basic usage of CalcNote.  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/screen_description.png">

|Area|Description|
|:-----------|:------------|
LineNo|Show the line number. You can input the [Line references](#lineno) to tap the line number.<br>This area can be hidden by [Editor Settings](settings.md).
Editor Area|Write the expression to calculate your problems. You can copy, cut or paste a expression like a notepad.
Results Area|Calculation results are displayed. The results are calculated in real-time when you write a expression on the editor.<br>You can show the result as hexadecimal, binary, tax included and tax excluded to tap the result. You need to configure tax rate if you want to calculate the tax included and tax excluded.
Toatal Area|A running total of all your lines is displayed.<br>You can show the result as hexadecimal, binary, tax included and tax excluded to tap the result. You need to configure tax rate if you want to calculate the tax included and tax excluded.
Keypad|You can switch the keypad to swipe to left or right.There are three keypads.<br>[Numeric keypad] <-> [Function keypad] <-> [Hexadecimal keypad]
Keypad Switches|You can show/hide the software keyboard. And also you can show/hide the keypad.

## Menu
You can access various functions via side menu.  You can show the side menu to tap the action bar menu or to swipe from the left side to the right side or tap the hardware menu key.

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/open_menu.png">
<br>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/menu_description.png">

|Menu Item|Description|
|:-----------|:------------|
New File|Save an editing note as draft and open new file.
Save|Save an editing note under a new file name.
Export|Export an editing note to other applications or copy to editing note to clipboard.
Undo|Erase the last change done to the note. You can erase up to 10 operations.
Format expression|Format an editing note to beautify a expression.
Settings|Move to [Setting](settings.md) screen.
Online Help|Jump to this page using default browser
Drafts|List of drafts will be displayed. You can open a draft to tap. And also you can delete a draft to tap the trash.
Saved Files|List of saved files will be displayed. You can open a file to tap. And also you can delete a file to tap the trash.

## <a name ="lineno">Line no and Line references</a>
When you want to use a previous line's answer in your expression, just tap the line number.Currently, CalcNote can refer to previous answer only.  
If a line being referred to moves up or down, `CalcNote` will ensure any references to it are updated automatically.  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/line_no.png">

## Editor Area
Write the expression to calculate your problems. The CalcNote works like notepad so you can play around with and edit your numbers like never before.  
You can line break to tap the <img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png" width="20px" align="top">.  
Do calculations over multiple lines, and even connect the lines together using line references. When one line changes, the other lines update.  If expression has syntax error, the result won't shown.  
Also you can write a memo with your problems.

## Results Area and Total Area
The results are calculated in real-time when you write a expression on the editor. If expression has error, results won't be shown.  
Tap the results of numerical, then the popup window is displayed on the screen.The popup window has the result as hexadecimal, binary, tax included and tax excluded. You can copy these results to clipboard to tap the result. And also you can tap the line number in order to input the line references.  

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/result_popup1.png">
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/result_popup2.png">

## Keypad
**The height of keypad is adjusted to the same as the height of software keyboad. You can adjust height of keypad by the [Keypad Settings](settings.md).**  
`CalcNote` has three keypads that makes it easier to do calculations. You can switch the keypad to swipe to left or right.  
<br>
[Numeric keypad] <-> [Function keypad] <-> [Hexadecimal keypad]  
<br>

To get to the standard alphabetical keyborad, tap `ABC`.  
The button can have the sub button. If ellipsis mark `...` is drawn on the button, it has the sub button. You can show the sub button to long-press the button. Also you can do the assigned operation to the sub button by swipe to the up or down. (Need to configure [Keypad Settings](settings.md))


<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/keypad.png">
<br>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/popup_pad.png">
<br>
<br>
You can show the operations on the button instead of ellipsis mark to configure [Keypad Settings](settings.md).
<br><br>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/swipe.png">
<br>

### Popup buttons that appears by the long tap

|Button|Popup Button1|Popup Button2|
|:-----------|:------------|:------------|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_backspace_black_18dp.png">|Clear all|Clear line
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_return_black_18dp.png">|`${LineNo}`|
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_left_bold_black_18dp.png">|Move to the beginning of the line|Select to the beginning of the line
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_arrow_right_bold_black_18dp.png">|Mode to the end of the line|Select to the end of the line
**×**|**()**|
**÷**|**mod**|
**.**|**,**|
**sin**|**asin**|**sinh**
**cos**|**acos**|**cosh**
**tan**|**atan**|**tanh**
**log**|**log2**|**ln**
**round**|**round half up**|
**ceil**|**round up**|
**floor**|**round down**|
**√**|**cbrt**|
**!**|**nPr**|**nCr**
**^**|**^2**|**^3**

### Tablet support
If you are using a tablet, number of buttons will be increased. So you can input some functions without long-tap.

#### For 7inch tablet
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/keypad7.png">

#### For 9inch tablet
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/keypad9.png">

### Keypad for parameters
When you input such as `√`, `^` or functions, popup keypad will be shown. You can input argument easily. You can input an argument easily.

<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/function_pad.png">

## Keypad Switches
|Button|Description|
|:-----------|:------------|
123|Hide the software keyboard.
ABC|Show the software keyboard.
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/all/ic_keyboard_close_black_18dp.png">|Hide the keypad.

<br><br>
[HOME](index.md)　[Grammar](http://burton999dev.github.io/CalcNoteHelp/grammar_en.html)　[Operators and Functions](operator_and_function.md)　[Floating Widget](floating_widget.md)　[Settings](settings.md)　[Customizing Keypad](customizing_keypad.md)　[FAQ](faq.md)　[Customization Example](example4theme.md)  
