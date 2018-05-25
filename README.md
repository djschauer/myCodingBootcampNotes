# myCodingBootcampNotes
Notes from class


### This is my Readme file

# Terminal Commands:

### cd < some directory >
Change Directory. This changes the current working directory. Working directory is the file path you are currently on in your terminal.

< some directory > can be any folder on your system. If it doesn't start with / like for example Documents/Misc, it means your current directory should have documents.

If it isnt there, it will give you this error.

`-bash: cd: Documents: No such file or directory`

### pwd

stands for present working directory. It lists the directory you are currently in.

### ls (dir  is the windows cmd version)

Lists all the files and directories within the current working directory.

### ls < some directory >

List all the files and directories in < some directory >

### mkdir

Makes a new directory within the current working directory


### touch < some filename >

Creates a new file, with the name < filename > 

### rm < filename >

Removes or deletes a file. Totally deletes your file.

### rmdir < directory >

Removes or deletes a directory. Totally deletes your file.

### cp < target file > < destination file >

copies file

### mv < target file > < destination file >

moves file to destination

# Cool Terminal Commands

### Up Key

Fills in previous command

### Tab Key (While Typing file or folder name)

Autofills out file name if exists and unique

### Special directories:

~/ - user directory

../ - one directory up (one directory closer to the root, the parent directory)

./ - the current directory

/ - root directory

# Git Commands

### git clone < link >

Clones file and pulls from git hub

### git add < name of file >

adds file for inclusion in git. Tells git to watch file/directory for changes

### git commit

notes changes to local repository.

### git push

sends the changes to hosting service ie git hub.

### git pull

pulls newest version of repository.

### git status

Tells you what state your git is in.

_If Windows, and see this:_

*Warning: CRLF will be converted to LF*

Not an error message.


# HTML Notes

### Tags

Tags have opening and closing tags: eg. < h1 > </ h1 >

Attributes go within tags: eg. < a href= "LINK" > Link </ a >

## Common Tags

### Headings

h1-h5 - heading tags, 1 largest 5 smallest

### Containers

Html - wraps entire page

Head - wraps header of page

body - wraps main content

div - logical container (generic container)

p - wraps individual paragraphs

### Others

Strong: Bolds text

em: emphasis texts

img: image, puts image on page

a href: link, anchor with href

li: list item

title: title

br: break, puts break between content

table: table, creates items into table

!-- -- : comments, cannot be seen on webpage

### UI Form Elements

form - creates a form section for your html

(Finish notes later)

# CSS Notes

### Syntax

Styling in HTML:

Style tag
Selector { Property: Value; }
End Style tag

Styling classes in CSS:

.Class/element/Id
{
    property: value;

}

### Key CSS Attributes

(Finish notes later)

### Selectors

Element selctor: styles all of one element
h1 {

}
Class selector: styles all of one class
.class {

}

ID Selector: stlyes all of one class, ID is usually one individual element.
(#)iditem {

}

Hashtag means ID, period means class

ID supercedes Class in order.

### Relative File Paths

Referencing images, links, files etc. need to tell where they are in folders.

"...href=folder/file.filetype"

Do not use absolute paths.

When referenceing a file your reference will begin in the folder you are in. If you want to move backwards a directory, begin with "../". To move forward use "/".

Pay attention to Parent and subdirectories (the hieraarchy of folders), when referencing.

### Box Model

In CSS every element rests within a series of boxes with customizable space properties:

Margin - How positioned On a wall

Border - Frame on the painting

Padding - The distance from the picture to the frame

Content - The picture

Spacing values are written in order of TRBL (Top, Right, Bottom, Left.)

### Floats

Float, everything will float to a particular part of the page. Things will word wrap and position around the floated element. It works incredibly similarly as MSWord text wrap options. (Ie. behind text, inline text, etc.)

Block positioning - Each block takes up a line

Inline Block - Each separate element will display adjacently.

sidebar {
    float: left;
}

Clear fix - Sets a line that ends the floats.

.clearfix::after {
    content: "content";
    display: block;
    clear: both;
}

### Position

Static position of a div, is statically positioned as a default.

Switching position to relative, makes it position itself relatively to the container its in.

Absolute position, relative to nearest ancestor. Where it physically sits on a webpage.

Fixed position, Keeps div set where it is regardless of scrolling.

# Z Index

Z index allows for layering.

positon: absoltute; z-index: 2;

Display: none; hides elements from view.

### Chrome Developer Tools

Debugs your webpages by finding and displaying errors in your code.

Can modify any page instantly and see your results instantly.

### CSS Resets

Can deploy multiple CSS files simultaneously.

Loading order matters: Last file loaded takes precedence.

CSS reset, list out all html elements and setting the values to a baseline 0.

### CSS Typogrphy

Line Height - Distance between lines of text on a page (Golden Ratio of 1.5x font)

Font size - Actual size of lettering. Should be atleast 16px on modern pages.

Line Length - Not CSS property, but should b about 50-75 chars per line on desktop.

Letter Spacing - Spacing between the letters.

Sans Serif Fonts - Easier to read online. Fonts without their serifs.

### Google Fonts

fonts.google.com

### Psuedo Styles

Keywords can be added to selectors to highlight a special state of the selected element. (ie. hover, click, visited etc.)

Used for styling things during specific states.

(element):(psuedo class) {

}

## Psuedo elements

https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements

Adds content as opposed to style.

## Bootstrap

Sketches: Design with a grid in mind

Bootstrap is built on the idea of grid; columns and merging columns.

12 is the magic number for grids.

Wireframing tools:
Balsamiq
Framebox
Pen and Paper: sketch it out

### Columns

#col-(size)-(number)  VERY IMPORTANT

Container (<)div class="container"(>)

Row (<)div class="row"(>)

Column (<)div class="col-md-12"(>)

In order to separate different classes, add additional class into the bootstrap class.

ie. (<)div class="col-md-12 newclass"(>)

### (Other Grid Frameworks)

Materialize
Modernizer

## Mobile Responsive

### Media Queries

Define how CSS styles are applied in realtion to the characteristics of the device viewport. (Maximum of 5 breakpoints: Desktop, Tablet landscape, Tab portrait, Mobile Landscape, mobile portrait.)

Can change the way a web page is displayed based on width, height, orientation and even media type (screen, paper, braille, etc.)

Bootstrap uses extensive media queries under the hood.

Declare Media Queries last.

@media screen and (max-width: 768px) {

For Breakpoints, google best practices breakpoints or best practice media queries.

Viewport refers to the display being used to view the website.

# Java Script

HTML and CSS are the structure, content and aesthetics of the page, JavaScript is the logic.

## Variables

Nouns of the programming language: They have names and values. (Integers (decimals are called floats or doubles), String, Booleans.)

String, needs quotes around. var string = "String"

Integer needs no quotes. var integer = 1

Boolean can only be true or false, lowercase and needs no quotes. var boolean = true

Order of variables within  file is important (js reads it top to bottom.)

Order of files also then matters, if there are multiple files.

Keyword  Variable Name Assignment    Value     Termination
var            name        =      "snow white"      ;

## Logging

console.log(nameofvariable);

Will log it in the console, viewable on Chrome Dev tools.

## Confirms and Prompts (functions)

Confirm, yes or no question (ok and cancel) and stores the response.

Prompt, asks you to input a value and stores the value.

    var nameOfFunction = confirm(question?);

    var nameOfFunction = prompt(question?);

Data is stored just like a variable, and is called by the "nameOfFunction"

### Document Write

Dislplays text on the webpage itself.

document.write("Text");

# If/Else

    if (function === conditionyouwantmet) {
    alert("thingthatyouwanttohappen")
    }
    else {
    alert("otherthingthatcouldhappen")
    }

values:
<         Less than

">"         Greater than

==        Equal to, does not force type

"==="     Equal to, does force type

<=        Less than or equal to

">="        Greater than or equal to

&&        "And"; Add multiple conditions using and, 
    
    ie. if (functiona == condition && functionb ==condition) {
    alert("thhinghapen")
    }

Concatination: When you add two strings. "1" + "1" will equal 11. When you add an integer with a string. 1 + "1" = 11. If one of your variables is a string it will turn them all into strings.

If you ever add a Boolean to an integer it will convert the Boolean into its number value (true 1 and false 0)

# Arrays

Lists out items into an array that are positioned based on their index value starting at 0

    ie. var array = ["index0", "index1", "index2", "index3"];

    var zooAnimals = ["Zebra", "Rhino", "Giraffe", "Owl"];

Arrays can have multiple dimensions, and be nested into each other. The values in the array do not have to be all the same type, but practically this will not happen.

To look things up in an array:

    (zooAnimals[1])

    console.log(zooAnimals[1])

    (zooAnimals.indexOf("bear")) (Searches array for that values)

Side Note: control + / will auto comment things out.

To reset a value in an array simply say that it is equal to something else. This can be done with any variable type.

    zooAnimals[1] = "Kangaroo";

# For Loops

Buildig a for loop, you define a variable, then a stopping point and then set it to iterate.

    for (var i = 0; i < array.length; i++) {
        console.log(array[i]);
    }

    for (var i = 5; a > 0; i--) {
        console.log(array[i]);
    }

Declare Variable

Loop Condition

Increment

Increment can be set in multiple ways.

i++: add one

i--: subtract one

i+="integer": Add by chosen value

i-="integer": subtract by chosen value

# Functions

Call a function, give it a name, then give it a parameter.

    function logArray(list) {
        for var i = 0; i < list.length; i++) {
            console.log(list[i]);
        }
    }

    logArray(nameofaarray)

Can be used multiple times on different variables. Functions essentially create repeatable code that can be used throughout to do the same thing without having to rewrite the same code.

You can pass multiple variables.

    function logArray(list, words) {
        for var i = 0; i < list.length; i++) {
            console.log(words + " " + list[i]);
        }
    }

    logArray(nameofarray, "phrase ")

|| = or

&& = and

## Objects

(Finish later)

## Manipulating the DOM

The DOM: Abstract concept that is essentially a manipulatable object.

document.createElement("nameofelement"): Creates elements

(nameofdivtobeappended).appendChild(nameofdivtobeadded): adds divs to an element.

("").setAttribute("newattribute","nameofnewattribute"): Sets an attribute to an element

("").textContent = "content": adds content to an element.

# JQuery

$: the same as typing the word "jQuery"

$("#id): pull element

$("#id").append(element): equivalent of appendchild

forEach: takes a list, and for each of those things do x

    ie. array.forEach(function(parameter)) {
        thing you want happen
    }

## Events

$(document).ready(function() {
    thing you want happen
}

This is telling the browser to wait until the website is ready before executing function.

# Scope

In Javascript, if you define something globally it can be used anywhere in the code.

Think boxes. A box inside of another box knows everything in both boxes, but the encompassing box does not know any of the things happening inside the boxes within it.

