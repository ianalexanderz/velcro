## <img src="https://i.imgur.com/sX12DTc.png">

Title: Bootstrap - CSS Frameworks <br>
Type: Morning Exercise<br>
Duration: "0:45"<br>
Creator:<br>
Original creators: Kristyn Bryan & Greg Dunn, WDI-Funke<br>
Adapted by: Jerrica Bobadilla, Taylor Darneille<br>
Further Adapted by: Colin Jaffe<br>
Competencies: CSS Frameworks, Bootstrap<br>
Prerequisites: CSS, HTML <br>

---

# Velcro

Because bootstraps should be simple.

## What Is A CSS Framework?

A CSS framework can save you time when styling applications. A framework is really just a (hopefully cohesive) stylesheet that has been designed by someone else and made available to others.

To implement these styles, you simply add a class to the HTML element that you'd like to style; the class name can be pulled straight from your framework's documentation.

In addition, you can make changes to the styles using your own stylesheet. Combine and conquer!

You can use Bootstrap to jazz up your projects, but we also want you to be familiar with it because when you jump into a company that has a pre-existing codebase, you'll be using their classes.

### The framework that we will be looking at today:

[Bootstrap](http://getbootstrap.com/)<br>
_Probably the most popular framework out there right now. Originally created by some devs who were working at Twitter._

## Activity

We're going to style this page using Bootstrap:

![unstyled page](https://i.imgur.com/sdRQg2x.png)

To look something like this:

![styled page](https://i.imgur.com/9imBki4.png)

## Setup

1. Fork and clone this repository.
2. Open this directory in VS Code and run Live Server to see the results in your browser.
3. Using `index.html`, add classes to the HTML elements to code along with this exercise.

## Let's Look at Bootstrap

Bootstrap's website catalogs everything that you can use to style your application. Note that their styles are responsive.

To use Bootstrap, you can download a file and keep it in your application or use a link to their CDN.

Bootstrap is a very robust framework! It has pretty much everything that you need (plus more). After this lesson, take some time to explore the site to see more of the offerings. Consider using it in your homework or projects.

## Installation

1. Go to [Bootstrap's framework page](https://getbootstrap.com/docs/5.0/getting-started/download/#cdn-via-jsdelivr) to get their stylesheets. You'll add the CDN link (both the `link` and `script` tags) to the head of your HTML document. Preferably ABOVE your own stylesheet link, so that your own styles (should you add any) will take precedence.

2. Refresh your browser and take a look at what happened after just initially linking Bootstrap! If you blinked and missed it, try deleting he line again to see what you got--without even adding any classes in. Thanks, Bootstrap!

3. We'll be using classes from the `Layout`, `Content`, and `Components` section of [Bootstrap's documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/). You can browse through these sections in the sidebar on Bootstrap's page to see some options for what we can do.

## Nav bar

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/components/navs/

1. Add the `class="nav"` to the `ul` of your nav bar

2. We also have to specify which `li` elements are nav items by adding the class `nav-item`

3. Further, we need to specify which `a` elements are nav links by adding the class `nav-link`

4. We can add additional styling to this. Let's add the class `nav-tabs` to our`ul` to adjust the formatting and turn our links into navigation tabs.

![nav](https://i.imgur.com/AXLSUlS.png)

## Adjust the image

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/content/images/

1. If we wanted our image to be responsive, we could add the `class="img-fluid"`

2. If we always want it to stay centered, tack on `class="text-center"` onto the image's parent `div`

## Container

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/layout/overview/

Let's start by wrapping our site content in a container: `class = "container"`. What does this do?

We can use `.container` for a responsive fixed width container.

![container](https://i.imgur.com/VQT8U0F.png)

If we want the container to span the entire width of the viewport, we can use `class="container-fluid"`

![container fluid](https://i.imgur.com/nbdIF1f.png)

## Bootstrap's grid

Let's use the built-in grid system that Bootstrap supplies.

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/layout/grid/

1. On the three paragraphs below the Example header, let's put `class="row"` on a div that surrounds all three.

2. Let's give each of these paragraphs a `class="col-sm"`

![grid](https://i.imgur.com/DmpDs9U.png)

## Update a button

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/components/buttons/

Bootstrap has multiple button options:

- The primary button style:
  `class="btn btn-primary"`

![primary button](https://i.imgur.com/5UYSelU.png)

- Quickly style to denote an action (success, danger, warning, etc.)

  - `class="btn btn-success"`

    ![button success](https://i.imgur.com/hdZdrF0.png)

  - `class="btn btn-danger"`

    ![button danger](https://i.imgur.com/8tSt2l4.png)

- Change the style to an outlined button instead of filled

  - `class="btn btn-outline-primary"`

    ![button outline](https://i.imgur.com/RikDvpo.png)

- Or change the size of the button

  - `class="btn btn-primary btn-lg"`

  ![button large](https://i.imgur.com/UCkuKtI.png)

Choose one and add it in the `a` tag to turn the `Learn More` link to a button.

#### Style the table

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/content/tables/

1. Add Bootstrap's default table style: `class="table"`.

![table](https://i.imgur.com/h8zEAQU.png)

2. Add the class `table-striped` to give our table zebra stripes.

![striped table](https://i.imgur.com/DHPEEsi.png)

#### Sections that you want to showcase

> Direct link to documentation:
> https://getbootstrap.com/docs/4.0/components/jumbotron/

Bootstrap has something called `jumbotron` which has styling to showcase a section.

Let's add `class="jumbotron"` to the section marked as `callout` in our index.html.

![jumbotron](https://i.imgur.com/2bPaxXf.png)

NOTE: Bootstrap is fully responsive! Change the sizes of your screen to check it out.

# And you're done!

You've Bootstrapped a page!

# Takeaways

- With a component framework, you can style your page--and, for many frameworks, even lay it out--without writing a single line of your own CSS.
- As in the bonus section below, you CAN write your own CSS rules for the framework's classes in your own CSS files, and, of course, add your own classes and ids.
- A component system is a great way to get an app presentable right away (pull it up by its bootstraps), but you don't publish an app with a generic Bootstrap look.

# Bonus

Add your own style to `style.css`! As long as your CSS is linked _after_ Bootstrap in your HTML file's `head`, it will take precedence.

Practice each of the following:

- Add style rules for Bootstrap classes you're already using, overwriting some properties already in there. Change the color of a button, for example; they already have colors, but your rules will take precedence.
- Add style rules for Bootstrap classes, adding rules for CSS properties that aren't already in there. For example, you could add a background image to an element with a particular class.
- Add your own classes/ids and rules for them. For example, maybe not EVERY nav item should have the same hover rules. Play with it!

# Other CSS frameworks if you don't love Bootstrap:

[Skeleton](http://getskeleton.com/)<br>
_Lightweight framework that has a nice, simple grid system._

[Materialize](http://materializecss.com/)<br>
_This framework is difficult to manipulate, but I like it for the parallax and the cards._

[Pure CSS](http://purecss.io/)<br>
_Similar to skeleton, this is a light framework with a grid system and responsive design._
