[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 03 - HTML Lists, JS Control Flow, CSS Box Model

*****

## Lists

Three types of lists

- Ordered lists
  - `<ul> and <li>`
- Unordered lists
  - `<ul> and <li>`
- Definition lists
  - `<dl> <dt> <dd>`

## Box Model

Box dimensions - width, height, min/max width/height  
px, %, em, rem, vh, vw  
overflow - hidden, scroll  

Border, Margin and Padding - margin is outside border, padding is inside border.  

Border can have a width, style (pg 310), color  

Box-shadow - hor. offset, ver. offset, blur dist., spread  
`inset` moves changes to inner-shadow  

border-radius- rounded corners. top,right,bottom,left  

## JS Control Flow

Arrays  

> let colors = ['white', 'yellow', 'pink'];  

index numbering (0,1,2)  ex. colors[1] is yellow  

If else - if the `if` statement evaluates true then code executes otherwise it moves to the `else` catch all code.  

switch statements  

~~~~~
 switch(variable){

   case 'one':
      title='selection one';
      break;
    case 'two':
      title='selection two';
      break;
    default:
      title='default';
      break;
}
~~~~~  

Variables are weak typed because data type for a value can change.  

Truthy and Falsy. means that a value is treated as true or false despite not strictly true or false.  (JS pg 167)  

short circuit values  
> let artist='picasso';  
> var artistName= (artist||'unknown');  

if artist holds a value (non empty string is truthy) then artistName = artist. otherwise it chooses second option 'unknown'  

## Loops

For, While, Do while

initialization (var i =0;)  
condition (i<10;)  
update (i++;)  

break - causes termination of loop and to move to code next after the loop statement.  
continue - stop current iteration and check the condition again.  

*****
