# Adhoc Website Instructions
---
These are the step-by-step instructions for putting together the Adhoc site.  
I recommend that you try each section independently before using this to check your results instead of copy off however this is perfect if you don't know where to start.  
I have rewritten the instructions a bit more and they are now a lot more dependent on `Ctrl + F` for finding what I am refering to.  
Some things have been reworded so [see the original instructions here](https://docs.google.com/document/d/1Ed2jBCxiD5MWOk4DMdlR1RulvduodNqcdALRBDBpRuM/edit).


## Editing the Navbar
Before starting the navbar, you'll notice that there's already some starter code (between the `<nav>` to `</nav>` lines)  
This code was copied straight from Bootstrap's navbar example [here](https://getbootstrap.com/docs/4.2/components/navbar/)

It’s a good template to start from but it still needs to be edited to fit our needs.  
For our purposes, remove the HTML responsible for the following:
* The Navbar item with a dropdown
* The link that says "Disabled"
* The search bar

Add the Adhoc logo to where the design specific

Locate the element with class "navbar-brand". Delete the text Navbar and replace it with an <img> element with the correct src value. You should make sure to upload the logo into the assets folder in your project first!

Remember to assign an appropriate value to the alt attribute.

According to the design spec, we should have 4 links (not including the brand) in the navbar.

Use the second link as a template and make 2 additional links. Change the text of the links to follow the design spec.

Adding the Jumbotron

Under the navbar, there’s a <div> that we’re going to turn into our jumbotron!

It currently has some inline CSS that renders a background image.

Provide it with a class of "jumbotron" and "jumbotron-fluid" to get a jumbotron that spans the entire screen/viewport.

Inside the jumbotron, add another <div>. This new <div> is going to act as a background and container for the text we want to insert. Therefore, inside the <div> add an <h1> element followed by a <p>.

Use the design spec and add the appropriate text inside both the <h1> and the <p> elements.

Time to style the elements we just added. We want the new <div> to have:

a grey background.
white and centered text.
larger top and bottom margins by assigning a class of "my-5". This utility class targets and increases the vertical margins of an element.

Also, give the <h1> element a display heading by assigning a class of "display-4".

Styling the Quote

Let’s style the quote under the jumbotron using utility classes.

Follow the design spec. Provide the <h2> element with

italic font.
a light font-weight.

Notice the styling of the name, it:

is aligned to the right
has a bold and italic font
the text inside the <span> has a normal weight.

Finish up the quote styling by increasing the top and bottom margins of the column containing the quote. You can do so by assigning a class of my-5.

Why Adhoc? - Cards

Locate the <h2> element with text Why Adhoc?.

Center the text and give it a display heading that follows the design spec.

In the next row, we’re going to continue following the design spec and add one card in each column.

In each column, add a card that:

Does not have a border.
Has an image icon on the top.
Has centered text on the bottom.

Here are the linked icons for convenience:

experienced icon.
fun icon.
smart icon.

While the columns look good on a large screen, the contents look squished on a smaller screen. Change the width of the column so that it has a width of 4 on medium, and larger, sized screens.

For extra small and small-sized screens, it should have a width of 8.

Let’s also have the row center the columns containing the cards.

Increase the vertical margins of the row with the text Why Adhoc and the row containing the cards to space out the rows.

Meet the team - Carousel

Locate the row with the text Meet the Team. According to the design spec, provide that row with utility classes that render a dark background with rounded top border.

Now let’s style <h2> element that has the text Meet the Team.

Apply the following styling for the <h2> element:

Make the text white.
Center the text.
Make it a Bootstrap display header.

16. Time to style the row below the text Meet the Team.

Give the bottom row a dark background and a rounded bottom border.

17. Take a look at the code that renders a carousel. It was copied directly from Bootstrap’s carousel with controls example.

Like with the navbar, we’re going to modify the code to fit our needs. For each <div> with a class of "carousel-item", assign the nested <img>‘s src a URL to the provided pictures in the intro’s image assets. Also, provide an appropriate value for the alt attribute 18. With the slides set up, we can add some captions to each slide.

Style the captions so that it has a black background, no vertical padding, and a rounded-pill border.

Inside the captions, add the appropriate text and style it according to the design spec.

19. Change the sizing of the carousel to only take up 50% of the width and set the margin to automatically center its contents.

Then go back and adjust the spacing of the rows to follow the design spec.

Finishing Up

20. The last element we have to style is the <footer>, center the text.

21. Congratulate yourself on a website well Bootstrapped!

There are different ways to re-create the layout of the website, so figure out what works best for you!

If you want to challenge yourself:

Add the HTML pages in the navbar and link to them.
Add more Bootstrap components.
Apply extra styling to the components.
Make the columns even more responsive by including more breakpoints.
Redesign the website to follow a different layout. This is the most involved task since it requires that you think about what you want on your site, how to arrange the layout, and how to implement this idea. While it may be challenging, it’s also extremely rewarding!
