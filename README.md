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