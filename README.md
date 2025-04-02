# Html Tags 

## h1 to h6
<h1>We have heading tag from h1 to h6 
Don't have more than one h1's if we need another level of heading go to h2,h3 ,till h6 
Don't skip level after h1 go to h2 - Don't jump from h1 to h3 
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements

## P
<P> This is not a void element </P> should always contain content
use paragraph tag for paragraph don't replace it with br tag 

## void elements
Void elements contain only closing tag 
<hr/> or <hr> - horizontal rule 
<br/> or <br>- break

To comapare html we use this online tool -->https://www.diffchecker.com/
## list 
Unordered list  they can be nested too 
<ul>
<li></li>
</ul>

Ordered list  th
<ol start=5>
<li></li>
</ol>

## anchor
<a href='https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a' draggable=true> Anchor Tag Information</a>
<li><a href="https://www.producthunt.com/">Product Hunt</a></li>
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a

## img 
<img src='https:/picsum.photos/200' alt='sunrise'/>  --> 
200 is pixel size 
alt describes what img is about 
Void element 

## path
Relative path is ideal 
./ --> same directory 
../ --> move up 

## BoilerPlate code

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>My website</title>
    </head>
    <body>
        <h1>Hello world</h1>
    </body>
</html>



# CSS

We can add css in 3 ways inline, internal , external

inline--> inside html element --> useful when we want to traget a single element
<html style="background:blue">
</html>
style--> attribute , backrground:blue--> value
background-->property , blue---> value 

internal --> It is limnited to one page document --> useful when we want to target a single web page
we add style in head section
<html>
<head>
<style>
    html{
        background:red;
    }
    </style>
</head>    
</html>

External --> 
----------------------------
<html>
<head>
<link rel="stylesheet" href="./styles.css"/>
</head>
</html>
-----------------------------

style.css
html{
    background:green 
}
rem --> from root (html)
em--> from parent 
 <p style="color:coral">Color</p>
  <p style="font-size:2rem">Font Size</p>
  <p style="font: weight 900px;">Font Weight</p>
  <p style="font-family:'Caveat',cursive;"> <a ref='https://fonts.google.com/specimen/Caveat'>Font Family</a></p>
  <p style="text-align:right">Text Align</p>

  # border: 30px solid black
   border-top:0px

  border-width: 20px 10px;
      border-top: 20px solid black;
      border-bottom: 20px solid black; 
      border-left: 10px solid black;
      border-right: 10px solid black;

   border-width:0 px 10 px 20 px 30 px

   padding - 20 px 

   ## Rules on CSS

 ### position 
  Lower down rule will be applied so color would be green 

   li{
    color:red
    color:green
   }

 ### Specificity 

   4. li {color :red} -[element]
   3. .first-class{color:red;} -[class-name]
   2. li[draggable] {color:purple;}-[attribute]
   1. #first-id{color:organge}-[id]
 
 ### Type 

  3. <link rel="stylesheet" href="./style.css"> -[external- can be applied to many]
  2. <html><head><style></style></head></html> -[internal-only exists inside one webpage]
  1. <h1 style="">Hello</h1>-[inline- targets only one element]


### Importance
 
 color:red;
 color :green !important; -[this !important- key word is most important we have to apply on element]
