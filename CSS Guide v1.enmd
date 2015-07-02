# CSS Guide


#### Link your CSS to HTML

```html
<link rel="stylesheet" type="text/css"
href="YOUR_FILE_NAME.css">
```
used at top of HTML to "require" it. 

 >   Your file needs to be in the same folder as your HTML sheet, specifiy file location.  
    if you link multiple style sheets, the order of your style sheets matter.


#### Basic Syntax
> `selector {property: value;}` - standard syntax of CSS

> > *example:* `p { color: red; }`

> `/* This is a Comment */` - Comments can be used in our outside of the blocks.

---

### CSS Selectors

 >`p { /* p-tag style declerations here */ }` - changes all the "p" tags in your HTML.



##### Class: Multi-Selectors  

###### using class selectors 

```css
    .special { 
    color:#FF0000;
    font-family: "Comic Sans MS", cursive;
    }
```    
changes any item with class = "special" to have font of "Comic Sans MS".

 >`<p classs="special">I'm Special!</p>` - how items call the special class in HTML.
 

##### ID: Single-Selectors 
> ` #header {
  font-size: 36px;
}` - applied to one item on a page.

> `<div id="header">I'm big!</div>` - exmaple of calling the ID'd item.

---

### Long Attribute Selecors.
###### will give only Text boxes the border. Specifically targeting the 'type' field.

```css  
input[type="text"]{
border: 1px green solid;
}
```
This will give an input box that accepts text, a green solid border.

---

### Group Selectors  
###### Dry up your CSS, this can be used to change multiple headers at once.

```css
h1, h2, h3, h4, h5, h6 {
  color: #2D958F
} 
```
This will change all `h#`'s color to #2D958F.

###### More group selectors.  

```css
h1, .special, #header {
  color: red;
}
```
this will give all `h1` elements and class `"special"` a red font.
    
---    
    
### Descendant Selectors
> `h1 strong {color: red;}` - only if theres a `strong` in `h1`, give it this style.


###### In the Example, all the a elements in div will 
###### css

```css    
    div a {color: red;}
```    
###### html

```html    
    <div>
        <ul>
            <li>
                <a href="#">Link</a>
            <li> 
        </ul>
    </div>
```

`body > h1{color: red;}` - will color the first `h1` element in `body`, red.
    

##### Siblings

> `h1 + p {font-style:italic;}` -  when using a `+`, it should only give you adjacent siblings. Only works for sibling tags.  
###### In the example below, notice how only the siblings *directly* next to each other will get stylized.

```html
<div class=”parent”>
    <h1>Heading</h1>
    <p>Adjacent Sibling Paragraph</p>
    <p>Non-adjacent Sibling Paragraph</p>
</div>
```

    

### Pseudo Classes/Elements

##### Pseudo Class
> `selector:pseudo-class{...}` - used to target the state of an element. (hovering)

###### examples:
    for links: 
    a:link - before you click on link.  
    a:visited - a visited link.  
    a:hover - while hovering over the link.  
    a:active - when you click on the link.  
    
    for text:
    input:focus - when you are currently typing into a field.

##### Pseudo Element
> `selector:pseudo-element{...}` - create a style that targets th first character, lke in a fairytale novel. (text currently highlighted by mouse)

###### Examples of pseudo-elements

```css
p::before {
    content: "FYI: ";
}
```

This will add an "FYI" before every p element.

---

### Which styling wins?
> When styling elements, the most specific styler will dominate.
> The below CSS examples are written differently, but target the same element.

###### css

```css
p .alink { color: blue; }
.plink a { color: red; }
```
###### html

```html
<p class="plink">
    Visit <a class="alink" href="#">website.
</a> </p>
```
> Here, the last styling will take over as they are both targeting the same element.    

---
## STYLING

#### Texts
- font-family:
- color:
- font-size: px, em, keywords, percentages
- spacing:
-text-align:, text-indent:

---

##### Media Queries
######CSS

```css
    @media screen and (min-width: 480px)
    {
    /*CSS rules that apply IF
    **we are rendering on a screen
    **and the window is at least 480px wide
    */
    }
```

used to style different sized screens.

##### Bootstrap.

```html
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">
    
```

used to help clean up your HTML (*not recomended long term*)

