# Adhoc Website Instructions

---

These are the step-by-step instructions for putting together the Adhoc site.  
I recommend that you try each section independently before using this to check your results instead of copy off however this is perfect if you don't know where to start.  

I have rewritten the instructions a bit more and they are now a lot more dependent on `Ctrl + F` for finding what I am refering to.  
Some things have been reworded so if some parts seem confusing, [also see the original instructions here](https://docs.google.com/document/d/1Ed2jBCxiD5MWOk4DMdlR1RulvduodNqcdALRBDBpRuM/edit).

## Editing the Navbar

Before starting the navbar, you'll notice that there's already some starter code (between the `<nav>` to `</nav>` lines. It is very long)  
This code was copied straight from Bootstrap's navbar example [here](https://getbootstrap.com/docs/4.2/components/navbar/)

It’s a good template to start from but it still needs to be edited to fit our needs.  
For our purposes, remove the HTML responsible for the following:

- The navbar item with a dropdown
- The link that says "Disabled"
- The search bar

#### The Logo

Add the Adhoc logo to the navbar where the design spec indicates it should be.

1. Locate the element with class `navbar-brand`
2. Delete the text Navbar and replace it with an `<img>` element with the correct src value
   - Make sure to upload the logo from the `zip` file into the `assets` folder first!
3. Remember to assign an appropriate value to the alt attribute.

#### The Navigation Links

According to the design spec, we should have 4 links (not including the brand) in the navbar.
Using the second link as a template, make 2 additional links and update the link texts to match the design spec.

## Adding the Jumbotron

Under the navbar, there’s a `<div>` that we’re going to turn into our Jumbotron! (`id="this-is-the-jumbotron-div"`)  
It currently has some inline CSS that renders a placeholder background image.

1. Provide it with a class of "jumbotron" and "jumbotron-fluid" to get a jumbotron that spans the entire viewport/screen.
2. Inside the jumbotron, add another ``<div>`
   - This new `<div>` will act as a background and container for the text we want to insert. Therefore, insert an `<h1>` element followed by a `<p>` element inside it
3. Follow the design spec and add the appropriate text inside both the `<h1>` and the `<p>` elements.
4. Time to style the elements we just added. We want the new `<div>` to have:
    - A grey background
    - White and centered text.
    - Larger top and bottom margins by assigning a class of `my-5`
     - This utility class increases the vertical margins of an element
    - Also, give the `<h1>` element a [display heading](https://getbootstrap.com/docs/4.2/content/typography/#display-headings) by assigning a class of `display-4`

#### Styling the Quote

Let’s style the quote under the jumbotron using utility classes.  
Following the design spec, provide the `<h2>` element with:

- An italicized font
- A light font-weight

Notice the styling of the name, it:

- Is aligned to the right
- Has a bold and italic font
- Has normal weight text inside the `<span>` element

Finish up the quote styling by increasing the top and bottom margins of the column containing the quote. You can do so by assigning a class of `my-5`.

## Cards - Why Adhoc?

1. Locate the `<h2>` element with the text `Why Adhoc?`.
2. Center the text and give it a display heading that follows the design spec.
3. In the next row, we’re going to continue following the design spec and add one card in each column.
4. In each column, add a card that:
    - Does not have a border
    - Has an image icon on the top
    - Has centered text on the bottom  
      The icons can be found in the `zip` file as:
      - `experienced.png`
      - `fun.png`
      - `smart.png`

5. While the columns look good on a large screen, the contents will look squished on smaller screens. Change the width of the column so that it has a width of 4 on medium screens and larger.
6. For extra small and small-sized screens, it should have a width of 8.
7. Also have the row horizontally center the columns containing the cards.
8. Increase the vertical margins of the row with the text Why Adhoc and the row containing the cards to space out the rows.

## Carousel - Meet the Team

Locate the row with the text `Meet the Team`.  
Using utility classes, make the row render a dark background with rounded top border as indicated by the design spec.
Now style `<h2>` element that has the text `Meet the Team`:

1. Apply the following styling for the <h2> element:

    - Make the text white.
    - Center the text.
    - Make it a Bootstrap display header.

2. Next, style the row below the text `Meet the Team`

    - Give the bottom row a dark background and a rounded bottom border.

3. Take a look at the code that renders a carousel copied [directly from Bootstrap’s carousel with controls example](https://getbootstrap.com/docs/4.2/components/carousel/#with-controls).

    - Like with the navbar, we’re going to modify the code to fit our needs. For each `<div>` with a class of `carousel-item`, assign the nested `<img>`‘s src a URL to the provided pictures in the intro’s image assets. Also, provide an appropriate value for the alt attribute

4. With the slides set up, we can now add some captions to each slide.
5. Style the captions with a black background, no vertical padding, and a rounded-pill border.
6. Inside the captions, add the appropriate text and style it according to the design spec.
7. Change the width of the carousel to only take up 50% of the screen and set the margin to automatically center its contents.
8. Then go back and adjust the spacing of the rows to follow the design spec.

## Footer - Finishing Up

The last element we have to style is the `<footer>`, simply center the text.  
And you're done! Congratulate yourself on a completely Bootstrapped website!  
There are different ways to re-create the layout of the website, so figure out what works best for you!

### Challenges

If you want to challenge yourself:

- Add the HTML pages in the navbar and link to them.
- Add more Bootstrap components.
- Apply extra styling to the components.
- Make the columns even more responsive by including more breakpoints.
- Redesign the website to follow a different layout. This is the most involved task since it requires that you think about what you want on your site, how to arrange the layout, and how to implement this idea
  - While it may be challenging, it’s also extremely rewarding!
