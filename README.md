Box-Model
=========

# The Box Model

![alt tag](/imgs/box.png?raw=true "BOX MODEL")

The term box model is used to talk about the design and layout of HTML elements. Every HTML element can be considered a box, no matter the shape. The element consists of the actual content (image, text, etc.), padding, margin, and border.

# Margin

* Sets space around an element
* Falls outside the border
* Transparent background
* Useful for positioning; breathing room

* Setting margin left to auto will put your element flush to the right
* Setting margin right to auto will put your element flush to the left
* Setting both left and right margins to auto will center your element

<pre><code>
	div {
		margin: 20px;

		margin-top: 20px;
		margin-right: 20px;
		margin-bottom: 20px;
		margin-left: 20px;
	}	
</code></pre>

# Padding

* Sets space in between an element and its border
* Keeps the background color of the element

<pre><code>
	div {
		padding: 20px;

		padding-top: 20px;
		padding-right: 20px;
		padding-bottom: 20px;
		padding-left: 20px;
	}	
</code></pre>

# Inline-level vs. block/inline-block

* Inline-level only allows margin left and right to work
* All padding sides work for inline-level, but top and bottom may bleed above and below the element

# Border

* Lies on the edge of an element, in between the margin and padding
* Broken up into width, color, and style properties
* Border-radius property allows you to define the shape element
* Styles include solid, double, dotted, dashed, outset, [and more](http://www.w3schools.com/cssref/pr_border-style.asp)

A good tool to find what values you might want to use for your border-radius property: <http://www.cssmatic.com/border-radius>

<pre><code>
	div {
		border: 20px solid black;

		bottom-top: 20px;
		bottom-right-style: dotted;
		bottom-bottom-width: 1px;
		bottom-left-color: red;

		border-radius: 10px;
		border-top-right-radius: 5px;
	}	
</code></pre>

# Outline

* Must always go around all sides; all sides have same properties
* Not a part of the box model
* Does not affect positioning
* Will lie just outside the border
* Useful for styling something like clicking a link without affecting anything

# Box Sizing (CSS3)

The box model has always been an additive design, meaning that margins, padding, and borders will add to the overall width and height of your element.

However, with CSS3 allows the box-sizing property, which affects the element differently. Different values include:

* Content-box: The default, additive box model
* Padding-box: Will include padding width in the elements width
* Border-box: Will include border width in the elements width
* No value for margins

<pre><code>
	div {
  		box-sizing: padding-box;
	}

	div2 {
  		box-sizing: border-box;
	}
</code></pre>

# Resources

<http://www.cssmatic.com/border-radius>
<http://www.w3schools.com/cssref/pr_border-style.asp>
<http://learn.shayhowe.com/html-css/opening-the-box-model/>
<http://css-tricks.com/almanac/properties/o/outline/>


