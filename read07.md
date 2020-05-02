# JavaScript make web pages more interactive

* ACCESS CONTENT
You can use JavaScript to select any
element, attribute, or text from an
HTML page. For example:
• Select the text inside all of the <hl>
elements on a page
• Select any elements that have a
c 1 ass attribute with a value of note
• Find out what was entered into a
text input whose id attribute has a
value of ema i 1

* MODIFY CONTENT
You can use JavaScript to add
elements, attributes, and text to the
page, or remove them. For example:
• Add a paragraph of text after the
first <hl> element
• Change the value of c 1 ass
attributes to trigger new CSS rules
for those elements
• Change the size or position of an
<i mg> element

* PROGRAM RULES
You can specify a set of steps for
the browser to follow (like a recipe),
which allows it to access or change the
content of a page. For example:
• A gallery script could check which
image a user clicked on and display
a larger version of that image.
• A mortgage calculator could collect
values from a fo rm, perform a
ca lculation, and display repayments.
• An animation could check the
dimensions of the browser window
and move an image to the bottom
of the viewable area (also known as
the viewport).

* REACT TO EVENTS
You can specify that a script should run
when a specific event has occurred. For
example, it could be run when:
• A button is pressed
• A link is clicked (or tapped) on
• A cursor hovers over an element
• Information is added to a form
• An interval of time has passed
• A web page has finished loading

## writing a script:

To write a script, you need to first
state your goal and then list the
tasks that need to be completed in
order to achieve it.

Start with the big picture of what
you want to achieve, and break
that down into smaller steps.

* DEFINE THE GOAL
First, you need to define the task you want to
achieve. You can think of this as a puzzle for the
computer to solve.

* DESIGN THE SCRIPT
To design a script you split the goal out into a series
of tasks that are going to be involved in solving this
puzzle. This can be represented using a flowchart.

* CODE EACH STEP
Each of the steps needs to be written in a
programming language that the compu ter
understands. In our case, this is JavaScript.

### EXPRESSIONS:
An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions.

* EXPRESSIONS THAT JUST ASSIGN A
VALUE TO A VARIABLE
`var color = 'beige';`
* EXPRESSIONS THAT USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE
`var area = 3 * 2;`

### OPERATORS:

Expressions rely on things called **operators;** they allow programmers to
create a single value from one or more values.

`buy= (5 > 3) && (2 < 4);`

`buy = 3 > 5;`


# Functions:

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).

> `function function_name(par1,par2){`
> `code;`
> `}`

so if we want to use the function we can just call the function using it is name
like this 
> `//some code`
> `SayHello()`
> `// some code`

those fuction can return a result value
> function getSize (width, height, depth) {
> var area = width * height;
> }
> var volume = width * height * depth;
> var sizes= [area , volume];
> return sizes;
`var areaOne = getSize (3, 2, 3)[0];`
`var volumeOne = getSize (3, 2, 3)[1];`

### FUNCTION DECLARATION:
A function declaration creates a function that you
can ca ll later in your code. It is the type of function
you have seen so far in this book.

> function area (width, height)
> return width * height;
> };
> var size= area(3, 4) ;

### FUNCTION EXPRESSION

If you put a function where the interpreter would
expect to see an expression, then it is treated as an
expression, and it is known as a function expression.
In function expressions, the name is usually omitted.

> `var ar ea = f unction(width, height) {`
> `r eturn width * height;`
> `} ;`
> `var size = area(3, 4) ;`

