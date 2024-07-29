2024-07-29 05:49


# Standard style
-  Class Name convention:
	BEM (Block, Element, Modifier) is a popular methodology for writing and organizing CSS code, making it more readable, scalable, and maintainable. It provides a structured approach to naming CSS classes, which helps developers understand the relationships between different parts of the user interface. Here's a breakdown of how BEM works:
	- Block: 
		A Block is a standalone entity that is meaningful on its own. It represents a high-level component.
		**Example**: A header, a menu, a button, a form.
		```jsx
		 <div className="block"> <!-- Block content --> </div>
		```
	- Element: 
		An Element is a part of a Block that has no standalone meaning and is semantically tied to its Block.
		**Example**: A menu item in a menu, a list item in a list.
		```jsx
		<div className="block"> 
			<div className="block__element"> 
				<!-- Element content --> 
			</div>
		</div>
		```
	- **Modifier**:
		A Modifier is a flag on a Block or Element. It changes the appearance or behavior of the Block or Element.
		**Example**: A button can have a modifier for its size or color, such as a large button or a green button.
		```jsx
		<div className="block block--modifier"> 
			<!-- Block with modifier -->
		</div>
		<div className="block"> 
			<div className=" block__element--modifier"> 
				<!-- Element with modifier --> 
			</div> 
		</div>
		```
- SCSS Base styles:
	in this folder, we have some of reusable style that we can use in order to build our style with less code:
	- globals:
		in this folder we have all the variables that we need to build our application like colors and font, also we have a boilerplate where we can reset the style that the browser gives by default and provide some of our default style for some tags.
	- util
		in this folder, we have all the functions and mixens that we need to build our application, in the breakpoints file we have all the sizes of the screen that we target and some mixins to create the media query.
		and in the functions file we have some useful functions that help us to facilitate the work for exemple we have rem function that takes as an argument a value in pixel and change it to a value of rem.
