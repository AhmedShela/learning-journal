# Css

#### * The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element*


CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
`Selector {`
`font-family: Arial;}`

### ther are 3 ways o link css style to htlm page:
* link:
> `<link href="css/styles.css" type="text/css"    rel="stylesheet" /> `
* internal Css:
`<style>`
You can also include CSS rules within an HTML page by placing them inside a <style> element, which usually sits inside the <head> element of the page. 
The <style> element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/ css.
* Css Selector:
which is using the css elements inside the html tags

#### *the best way to use Css is using external Style Sheets*


# Foreground Color 
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
* rgb values 
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
*  hex Codes
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
* Color names 
There are 147 predefined color names that are recognized by browsers. For example: DarkCyan

## baCkground Color
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.
