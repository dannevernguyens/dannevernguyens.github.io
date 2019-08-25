[Home](/)|[About Me](aboutme)|[Learning Blog](learningblog)|[ProTips](tips.a)

### Reading & Lab 05 - Design web pages with CSS
##### August 24, 2019 - Saturday

###### READING 05 Notes - CSS

CSS is the prettification of the HTML skeleton. THE SKIN ON OUR BONESSSS.

It is helpful to imagine that there is an invisible box around every HTML element. CSS allows you to create rules and control the way that each individual box and that box’s contents is presented. 

**Block VS Inline Elements**
Block level elements look like they start on a new line. 
Ex: h1, h6, p, div
Inline elements flow within the text and do not start on a new line. 
Ex: b, I, img, em, span

Boxes:
- Width, height
- Borders (colors, width, style)
- Background color
- images
- Position in window

Text: 
- typeface
- size
- color
- Italics, bold, casing, small-caps

Specific:
- Lists
- Tables
- Forms

**Internal VS External CSS**
Internal CSS is coded on the page.
External CSS is coded elsewhere. Typically a reference for that external file will be placed in the HEAD of the HTML file. 

Best practice is to have CSS done externally. This is especially important when building a site with more than one page, that way you don’t have to duplicate styling on each page to get a consistent look. This will also keep the content separate from the style. And it means you can change styling for all pages by changing only a single file. 

CSS syntax:
- selector (h1)
- Property (font-family:)
- value (Arial;)
	
There is also a CSS selector hierarchy to be aware of. 

Specificity
If one selector is more specific than the others (h1 vs b for example) then the more specific selector will take precedence. 

Last Rule
If two selectors are identical, the latter of the two will take precedence. Order is determined top to bottom.

Important
You can add \!important\ after any property value to indicate that it should be considered more important than other rules that apply to that same element. 

Inheritance
If you apply properties to the body element, they will apply to most child elements. You can force lots of properties to inherit values from parent elements by using **inherit** for the value of the properties. 

###### READING 05 Notes - Color

Foreground color properties allow you to specify the color of text inside an element. You can specify color in 3 ways: 
1. RBG values, rgb(100,100,90)
2. hex codes, #ee3e80
3. color names, DarkCyan

Background color properties set the color of the background of the box around an HTML element. The background is transparent if you do not specify a color. Most browsers have a white background by default. 

**Contrast**
* Low contrast
    * Bad bad. Text is harder to read when there is low contrast between background and foreground colors
* High contrast
    * Text is easier to read when there is higher contrast. But this can become exhausting if you are reading a large amount of text. 
* Medium contrast
    * For long spans of text, medium contrast is ideal for reading comfort. 

**Opacity** 
Opacity value is a number between 0 and 1.0. So a value of 0.5 is 50% opacity and 0.15 is 15% opacity. 

**HSL & HSLA colors**
Hue, saturation, lightness, alpha (transparency)
Kinda complicated. Some advanced level color science for fine tuning your page. 