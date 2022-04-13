# Flex-Grow-Flex-Shrink-Flex-Shorthand-
Some Practice with Flex


'flex-basis' is recommended to use because it is along the main axis.  so for instance when setting 'flex-direction' to either row or column, 'flex-basis' will accomodate whichever the direction is.  If just the height or just the width is set then that will be the only property affected.  'flex-basis' will also increase the size of the container.

                        Flex Grow
'flex-grow' will occupy the remaining blank space with the selected element that the property is assigned to.  if there's 200px of empty space and you set 

div:nth-of-type(3){
    flex-grow: 1;
}

then the third element will occupy that remaining 200px of blank space and push its fellow elements aside to do so.  
If multiple elements are selected in this manner then they will split up the remaining blank space.  
If all elements are selected then the same principle is applied, but all the space will be divided amongst all the elements.
The number that is entered as the properties argument represents how many divedends are given to that element.  

div:nth-of-type(1){
    flex-grow: 1;
}

div:nth-of-type(5){
    flex-grow: 3;
}

This states that the fifth element (good movie by the way) gets three times as much of the empty space while the first element only gets 1 quarter of it.

                        Flex-Shrink

'flex-shrink' is the exact opposite of 'flex-grow'.  It takes an element and shrinks it to fit in with the other elements the way the entire 'flex-box' is meant to fit

                        Shorthand

Cause ain't none of us got time to type out all those properties and their values.
     The shorthand is 

.BobLawBlah{
    flex: 1 2 3em;
}

The first number represents 'flex-grow', the second number 'flex-shrink' and the third number 'flex-basis'

if there happens to be only one value for the property

.BobLawBlah{
    flex: 3px;
}

it will represent 'flex-grow' only.

if there are only two

.BobLawBlah{
    flex: 2 8px;
}

the first will represent 'flex-grow' and the second will represent 'flex-basis'
