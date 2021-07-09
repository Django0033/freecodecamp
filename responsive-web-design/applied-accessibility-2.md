# Applied Accessibility

## Table of Content

* [Add a Text Alternative to Images for Visually Impaired Accessibility](#add-a-text-alternative-to-images-for-visually-impaired-accessibility)
  * [Example](#example)
* [Know When Alt Text Should be Left Blank](#know-when-alt-text-should-be-left-blank)
  * [Example](#example)
* [Use Heandings to Show Hierarchical Relationships of Content](#use-heandings-to-show-hierarchical-relationships-of-content)
  * [Example](#example)
* [Jump Straight to the Content Using the main Element](#jump-straight-to-the-content-using-the-main-element)
  * [Example](#example)
* [Wrap Content in the article Element](#wrap-content-in-the-article-element)
  * [Example](#example)
* [Make Screen Reader Navigation Easier with the header Landmark](#make-screen-reader-navigation-easier-with-the-header-landmark)
  * [Example](#example)
* [Make Screen Reader Navigation Easier with the nav Landmark](#make-screen-reader-navigation-easier-with-the-nav-landmark)
  * [Example](#example)
* [Make Screen Reader Navigation Easier with the footer Landmark](#make-screen-reader-navigation-easier-with-the-footer-landmark)
  * [Example](#example)
* [Improve Accessibility of Audio Content with the audio Element](#improve-accessibility-of-audio-content-with-the-audio-element)
  * [Example](#example)
* [Improve Chart Accessibility with the figure Element](#improve-chart-accessibility-with-the-figure-element)
  * [Example](#example)
* [Improve Form Field Accessibility with the label Element](#improve-form-field-accessibility-with-the-label-element)
  * [Example](#example)

## Add a Text Alternative to Images for Visually Impaired Accessibility

You've likely seen an `alt` attribute on an `img` tag in other challenges. `alt` text describes the image's content and provides a text-alternative for it. An `alt` attribute helps in cases where the image fails to load or can't be seen by a user. Search engines also use it to understand what an image contains to include it in search results. Here's an example:

```HTML
<img src="importantLogo.jpeg" alt="Company logo">
```

People with visual impairments rely on screen readers to convert web content to an audio interface. They won't get information if it's only presented visually. For images, screen readers can access the `alt` attribute and read its contents to deliver key information.

Good `alt` text provides the reader a brief description of the image. You should always include an `alt` attribute on your images. Per HTML5 specification, this is now considered mandatory.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Add a Text Alternative to Images for Visually Impaired Accessibility
        </title>
    </head>
    <body>
        <img src="doingKarateWow.jpeg" alt="Camper Cat doing karate" />
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Know When Alt Text Should be Left Blank

In the last challenge, you learned that including an `alt` attribute when using `img` tags is mandatory. However, sometimes images are grouped with a caption already describing them, or are used for decoration only. In these cases, `alt` text may seem redundant or unnecessary.

When an image is already explained with text content or does not add meaning to a page, the `img` still needs an `alt` attribute, but it can be set to an empty string. Here's an example:

```HTML
<img src="visualDecoration.jpeg" alt="">
```

Background images usually fall under the `decorative` label as well. However, they are typically applied with CSS rules, and therefore not part of the markup screen readers process.

_Note_: For images with a caption, you may still want to include `alt` text since it helps search engines catalog the image's content.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Know When Alt Text Should be Left Blank</title>
    </head>
    <body>
        <h1>Deep Thoughts with Master Camper Cat</h1>
        <article>
            <h2>Defeating your Foe: the Red Dot is Ours!</h2>
            <p>To Comme...</p>
        </article>
        <img src="samuraiSwords.jpeg" alt="" />
        <article>
            <h2>Is Chuck Norris a Cat Person?</h2>
            <p>To Come...</p>
        </article>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Use Heandings to Show Hierarchical Relationships of Content

Headings (`h1` through `h6` elements) are workhorse tags that help provide structure and labeling to your content. Screen readers can be set to read only the headings on a page so the user gets a summary. This means it is important for the heading tags in your markup to have semantic meaning and relate to each other, not be picked merely for their size values.

*Semantic meaning* meansthat the tag you use around content indicates the type of information it contains.

If you were writing a paper with an introdiction, a body, and a conclusion, it
wouldn't make much sense to put the conclusion as a subsection of the body in
your outline. It should be its own section. Similarly, the heading tags in
a webpage need to go in order and indicate the hierarchical relationships of
your content.

Headings with equal (or higher) rank start new implied sections, headings with
lower rank start subsections of the previous one.

As an example, a page with an `h2` element followed by several subsections
labeled with `h4` tags would confuse a screen reader user. With six choices,
it's tempting to use a tag because it looks better in a browser, but you can use
CSS to edit the relative sizing.

One final point, each page should always hove one (and only one) `h1` element,
which is the main subject of your content. This and the other headings are used
in part by search engines to understand the topic of the page.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Use Headings to Show Hierarchical Relationships of Content
        </title>
    </head>
    <body>
        <h1>How to Become a Ninja</h1>
        <main>
            <h2>Learn the Art of Moving Stealthily</h2>
            <h3>How to Hide in Plain Sight</h3>
            <h3>How to Climb a Wall</h3>
            <h2>Learn the Art of Battle</h2>
            <h3>How to Strengthen your Body</h3>
            <h3>How to Fight like a Ninja</h3>
            <h2>Learn the Art of Living with Honor</h2>
            <h3>How to Breathe Properly</h3>
            <h3>How to Simplify your Life</h3>
        </main>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Jump Straight to the Content Using the main Element

HTML5 introduced severas new elements that give developers more options while also incorporating accessibility features. These tags include `main`, `header`, `footer`, `nav`, `article`, and `section`, among others.

By default, a browser renders these elements similar to the humble `div`. However, using them where appropriate gives additional meaning to your markup. The tap name alone can indicate the type of information it contains, which adds semantic meaning to that content. Assistive technologies can access this information to provide better page summary or navigation options to their users.

The `main` element is used to wrap (you guessed it) the main content, and there should be only one per page. It's meant to surround the information related to your page's central topic. It's not meant to include items that repeat across pages, like navigation links or banners.

The `main` tag also has an embedded landmark feature that assistive thechnology can use to navigate to the main content quickly. If you've ever seen a "Jump to Main Content" link at the top of a page, using the `main` tag automatically gives assistive devices that functionality.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Jump Straight to the Content Using the main Element</title>
    </head>
    <body>
        <header>
            <h1>Weapons of the Ninja</h1>
        </header>
        <main></main>
        <footer></footer>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Wrap Content in the article Element

`article` is another one of the new HTML5 elements thet add semantic meaning to your markup. `article` is a sectioning element and is used to wrap independent, self-contained content. The tap works well with blog entries, forum posts, or news articles.

Determining wether content can stand alone is usually a judgment call, but you can use a couple of simple tests. Ask yourself if you removed all surrounding context, would that content still make sense? Similarly, for text would the content hold ug if it were  in an RSS feed?

Remember that folks using assistive technologies rely on organized semantically meaningful markup to better understand your work.

**Note**: The `section` element is also new with HTML5, and has a slightly different semantic meaning than `article`. An `article` is for standalone content, and as `section` is for grouping thematically related content. They can be used within each other, as needed. For example, if a book is the `article`, then each chapter is a `section`. When there's no relationship between groups of content, then use a `div`.

`<div>` - groups content <section> - groups related content `<article>` - groups independent, self-contained content.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Wrap Content in the article Element</title>
    </head>
    <body>
        <h1>Deep Thoughts with Master Camper Cat</h1>
        <main>
            <article>
                <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
                <p>
                    The internet is littered with varying opinions on
                    nutritional paradigms, from catnip paleo to hairball
                    cleanses. But let's turn our attention to an often
                    overlooked fitness fuel, and examine the protein-carb-NOM
                    trifecta that is lasagna...
                </p>
            </article>
            <img src="samuraiSwords.jpeg" alt="" />
            <article>
                <h2>Defeating your Foe: the Red Dot is Ours!</h2>
                <p>
                    Felines the world over have been waging war on the most
                    persistent of foes. This red nemesis combines both cunning
                    stealth and lightning speed. But chin up, fellow fighters,
                    our time for victory may soon be near...
                </p>
            </article>
            <img src="samuraiSwords.jpeg" alt="" />
            <article>
                <h2>Is Chuck Norris a Cat Person?</h2>
                <p>
                    Chuck Norris is widely regarded as the premier martial
                    artist on the planet, and it's a complete coincidence anyone
                    who disagrees with this fact mysteriously disappears soon
                    after. But the real question is, is he a cat person?...
                </p>
            </article>
        </main>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Make Screen Reader Navigation Easier with the header Landmark

The next HTML5 element that adds semantic meaning and improves accessibility is the `header` tag. It's used to wrap introductory information or navigation links for its parent tag and works well around content that's repeated at the top on multiple pages.

`header` shares the embedded landmark feature you saw with `main`, allowing assistive technologies to quickly navigate to that content.

**Note**: The `header` is meant for use in the `body` tag of your HTML document. It is different than the `head` element, which contains the page's title, meta information, etc.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Make Screen Reader Navigation Easier with the header Landmark
        </title>
    </head>
    <body>
        <header>
            <h1>Training with Camper Cat</h1>
        </header>
        <main>
            <section id="stealth">
                <h2>Stealth &amp; Agility Training</h2>
                <article>
                    <h3>
                        Climb foliage quickly using a minimum spanning tree
                        approach
                    </h3>
                </article>
            </section>
            <section id="combat">
                <h2>Combat Training</h2>
                <article>
                    <h3>
                        Dispatch multiple enemies with multithreaded tactics
                    </h3>
                </article>
                <article>
                    <h3>
                        Goodbye world: 5 proven ways to knock out an opponent
                    </h3>
                </article>
            </section>
            <section id="weapons">
                <h2>Weapons Training</h2>
                <article>
                    <h3>
                        Swords: the best tool to literally divide and conquer
                    </h3>
                </article>
                <article>
                    <h3>
                        Breadth-first or depth-first in multi-weapon training?
                    </h3>
                </article>
            </section>
        </main>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Make Screen Reader Navigation Easier with the nav Landmark

The `nav` element is another HTML5 item with the embedded landmark feature for easy screen reader navigation. This tag is meant to wrap around the main navigation links in your page.

If there are repeated site links at the bottom of the page, it isn't necessary to markup those with a `nav` tag as well. Using a `footer` (covered in the next challenge) is sufficient.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Make Screen Reader Navigation Easier with the nav Landmark</title>
</head>
<body>
    <header>
        <h1>Training with Camper Cat</h1>
        <nav>
            <ul>
                <li><a href="#stealth">Stealth &amp; Agility</a></li>
                <li><a href="#combat">Combat</a></li>
                <li><a href="#weapons">Weapons</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="stealth">
            <h2>Stealth &amp; Agility Training</h2>
            <article>
                <h3>Climb foliage quickly using a minimum spanning tree approach</h3>
            </article>
            <article>
                <h3>No training is NP-complete without parkour</h3>
            </article>
        </section>
        <section id="combat">
            <h2>Combat Training</h2>
            <article>
                <h3>Dispatch multiple enemies with multithreaded tactics</h3>
            </article>
            <article>
                <h3>Goodbye world: 5 proven ways to knock out an opponent</h3>
            </article>
        </section>
        <section id="weapons">
            <h2>Weapons Training</h2>
            <article>
                <h3>Swords: the best tool to literally divide and conquer</h3>
            </article>
            <article>
                <h3>Breadth-first or depth-first in multi-weapon training</h3>
            </article>
        </section>
    </main>
</body>
</html>
```

* [Table of Content](#table-of-content)

## Make Screen Reader Navigation Easier with the footer Landmark

Similar to `header` and `nav`, the `footer` element has a built-in landmark feature that allows assistive devices to quickly navigate to it. It's primarily used to contain copyright information or links to related documents that usually sit at the bottom of a page.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Make Screen Reader Navigation Easier with the footer Landmark
        </title>
    </head>
    <body>
        <header>
            <h1>Training</h1>
            <nav>
                <ul>
                    <li><a href="#stealth">Stealth &amp; Agility</a></li>
                    <li><a href="#combat">Combat</a></li>
                    <li><a href="#weapons">Weapons</a></li>
                </ul>
            </nav>
        </header>
        <main>
            <section id="stealth">
                <h2>Stealth &amp; Agility</h2>
                <article>
                    <h3>
                        Climb foliage quickly using a minimum spanning tree
                        approach
                    </h3>
                </article>
                <article>
                    <h3>No training is NP-complete without parkour</h3>
                </article>
            </section>
            <section id="combat">
                <h2>Combat Training</h2>
                <article>
                    <h3>
                        Dispatch multiple enemies with multithreaded tactics
                    </h3>
                </article>
                <article>
                    <h3>
                        Goodbye world: 5 proven ways to knock out an opponent
                    </h3>
                </article>
            </section>
            <section id="weapons">
                <h2>Weapons Training</h2>
                <article>
                    <h3>
                        Swords: the best tool to literally divide and conquer
                    </h3>
                </article>
                <article>
                    <h3>
                        Breadth-first or depth-first in multi-weapon training?
                    </h3>
                </article>
            </section>
        </main>
        <footer>&copy; 2018 Camper Cat</footer>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Improve Accessibility of Audio Content with the audio Element

HTML5's `audio` element gives semantic meaning when it wraps sound or audio stream content in your markup. Audio content also needs a text alternative to be accessible to peaple who are deaf or hard of hearing. This can be done with nearby text on the page or a link to a transcript.

The `audio` tag supports the `controls` attribute. This shows the browser default play, pause, and other controls, and supports keyboard functionality. This is a boolean attribute, meaning it doesn't need a value, its presence on the tag turns the setting on.

Here's an example:

```HTML
<audio id="meowClip" controls>
  <source src="audio/meow.mp3" type="audio/mpeg">
  <source src="audio/meow.ogg" type="audio/ogg">
</audio>
```
**Note**: Multimedia content usually has both visual and auditory components. It needs synchronized captions ond a transcript so users with visual and/or auditory impairments can access it. Generally, a web developer is not responsible for creating the captions ro transcript, but needs to know to include them.

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Improve Accessibility of Audio Content with the audio Element
        </title>
    </head>
    <body>
        <header>
            <h1>Real Coding Ninjas</h1>
        </header>
        <main>
            <p>A sound clip of Zersiax's screen reader in action.</p>
            <audio controls>
                <source src="https://s3.amazonaws.com/freecodecamp/screen-reader.mp3" type="audio/mpeg"></source>
            </audio>
        </main>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Improve Chart Accessibility with the figure Element

HTML5 introduced the `figure` element and the related `figcaption`. Used together, thene items wrap a visual representation (like an image, diagram, or chart) along with its caption. Wrapping these elements together gives a two-fold accessibility boost by semantically grouping related content and providing a text alternative explaining the `figure`.

For data visualizations like charts, the caption can be used to briefly note the trends or conclusions for users with visual impairments. Another challenge covers how to move a table version of the chart's data off-screen (using CSS) for screen reader users.

Here's an example - note that the `figcaption` goes inside the `figure` tags and can be combined with other elements:

```HTML
<figure>
    <img src="roundhouseDestruction." alt="Photo of Camper Cat executing a roundhouse kick">
    <br>
    <figcaption>Master Camper Cat demonstrates proper form of a roundhouse kick</figcaption>
</figure>
```

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>Improve Chart Accessibility with the figure Element</title>
    </head>
    <body>
        <header>
            <h1>Training</h1>
            <nav>
                <ul>
                    <li><a href="#stealth">Stealth &amp; Agility</a></li>
                    <li><a href="#combat">Combat</a></li>
                    <li><a href="#weapons">Weapons</a></li>
                </ul>
            </nav>
        </header>
        <main>
            <section>
                <figure>
                    <br />
                    <figcaption>
                        Breakdown per week of time to spend training in stealth,
                        combat, and weapons.
                    </figcaption>
                </figure>
            </section>
            <section id="stealth">
                <h2>Stealth &amp; Agility Training</h2>
                <article>
                    <h3>
                        Climb foliage quickly using a minimum spanning tree
                        approach
                    </h3>
                </article>
                <article>
                    <h3>No training is NP-complete without parkour</h3>
                </article>
            </section>
            <section id="combat">
                <h2>Combat Training</h2>
                <article>
                    <h3>
                        Dispatch multiple enemies with multithreaded tactics
                    </h3>
                </article>
                <article>
                    <h3>
                        Goodbye world: 5 proven ways to knock out an opponent
                    </h3>
                </article>
            </section>
            <section id="weapons">
                <h2>Weapons Training</h2>
                <article>
                    <h3>
                        Swords: the best tool to literally divide and conquer
                    </h3>
                </article>
                <article>
                    <h3>
                        Breadth-first or depth-first in multi-weapon training?
                    </h3>
                </article>
            </section>
            <footer>&copy; 2018 Camper Cat</footer>
        </main>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Improve Form Field Accessibility with the label Element

Improving accessibility with semantic HTML markup applies to using both appropriate tag names and attibutes. The next several challenges cover some imgortant scenarios using attributes in forms.

The `label` tag wraps the text for a specific form control item, usually the name or label for a choice. This ties meaning to the item and makes the form more readable. The `for` attribute on a `label` tag explicitly associates that `label` with the form control and is used by screen readers.

You learned about radio buttons and their labels in a lesson in the Basic HTML section. In that lesson, we wrapped the radio button input element inside a `label` element along with the label text in order to make the text clickable. Another way to achieve this is by using the `for` attribute, as explained in this lesson.

The value of the `for` attribute must be the same as the value of the `id` attribute of the form control. Here's an example:

```HTML
<form>
    <label for="name">Name:</label>
    <input id="name" type="text" name="name">
</form>
```

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title></title>
    </head>
    <body>
        <header>
            <h1>Deep Thoughts with Master Camper Cat</h1>
        </header>
        <section>
            <form>
                <p>Sign up to receive Camper Cat's blog posts by email here!</p>
                <label for="email">Email:</label>
                <input id="email" type="text" name="email" />
                <input type="submit" name="submit" value="Submit" />
            </form>
        </section>
        <article>
            <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
            <p>
                The internet is littered with varying opinions on nutritional
                paradgms, from catnip paleo to hairball cleanses. But let's turn
                our attention to an often overlooked fitness fuel, and examine
                the protein-carb-NOM trifecta that is lasagna...
            </p>
        </article>
        <img src="samuraiSwords.jpeg" alt="" />
        <article>
            <h2>Defeating your Foe: the Red Dot is Ours!</h2>
            <p>
                Felines the world over have been waging war on the most
                persistent of foes. This red nemesis combines both cunning
                stealth and lightning speed. But chin up, fellow fighters, our
                time for victory may soon be near...
            </p>
        </article>
        <img src="samuraiSwords.jpeg" alt="" />
        <article>
            <h2>Is Chuck Norris a Cat Person?</h2>
            <p>
                Chuck Norris is widely regarded as the premier martial artiost
                on the planet, and it's a complete coincidence anyone who
                disagrees with this fact mysteriously disappears soon after. But
                the real question is, is he a cat person?...
            </p>
        </article>
        <footer>&copy; 2018 Camper Cat</footer>
    </body>
</html>
```

* [Table of Content](#table-of-content)

## Wrap Radio Buttons in a fieldset Element for Better Accessibility

The next form topic covers the accessibility of radio buttons. Each choice is given a `label` with a `for` attribute tying to the `id` of the corresponding item as covered in the last challenge. Since radio buttons often come in a group where the user must choose one, there's a way to semantically show the choices are part of a set.

The `fiesdset` tag surrounds the entire grouping of radio buttons to achieve this. It often uses a `legend` tag to provide a description for the grouping, which screen readers read for each choice in the `fiesdset` element.

The `fieldset` wrapper and `legend` tag are not necessary when the choices are sely-explanatory, like a gender selection. Using a `label` with the `for` attribute for each radio button is sufficient.

Here's an example:

```HTML
<form>
    <fieldset>
        <legend>Choose one of these three items:</legend>
        <input id="one" type="radio" name="items" value="one">
        <label for="one">Choice One</label>
        <br>
        <input id="two" type="radio" name="items" value="two">
        <label for="two">Choice Two</label>
        <br>
        <input id="three" type="radio" name="items" value="three">
        <label for="three">Choice Three</label>
        <br>
    </fieldset>
</form>
```

### Example

```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <title>
            Wrap Radio Buttons in a fieldset Element for Better Accessibility
        </title>
    </head>
    <body>
        <header>
            <h1>Deep Thoughts with Master Camper Cat</h1>
        </header>
        <section>
            <form>
                <p>Sign up to receive Camper Cat's blog posts by email here!</p>
                <label for="email">Email:</label>
                <input id="email" type="text" name="email" />
                <fieldset>
                    <legend>What level ninja are you?</legend>
                    <input
                            id="newbie"
                            type="radio"
                            name="levels"
                            value="newbie"
                            />
                    <label for="newbie">Newbie Kitten</label>
                    <br />
                    <input
                            id="intermediate"
                            type="radio"
                            name="levels"
                            value="intermediate"
                            />
                    <label for="intermediate">Developing Student</label>
                    <br />
                    <input
                            id="master"
                            type="radio"
                            name="levels"
                            value="master"
                            />
                    <label for="master">Master</label>
                </fieldset>
                <input type="submit" name="submit" value="Submit" />
            </form>
        </section>
        <article>
            <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
            <p>
                The internet is littered with varying opinions on nutritional
                paradigms, from catnip paleo to hairball cleanses. But let's
                turn our attention to an of ten overlooked fitness fuel, and
                examine the protein-carb-NOM trifecta that is lasagna...
            </p>
        </article>
        <img src="samuraiSwords.jpeg" alt="" />
        <article>
            <h2>Defeating your Foe: the Red Dot is Ours!</h2>
            <p>
                Felines the world over have been waging war on the most
                persistent of foes. This red nemesis combines both cunning
                stealth and lightning speed. But chin up, fellow fighters, our
                time for victory may soon be near...
            </p>
        </article>
        <img src="samuraiSwords.jpeg" alt="" />
        <article>
            <h2>Is Chuck Norris a Cat Person?</h2>
            <p>
                Chuck Norris is widely regarded as the premier martial artist on
                the planet, and it's a complete coincidence anyone who disagrees
                with this fact mysteriously disappears soon after. But the real
                question is, is he a cat person?...
            </p>
        </article>
    </body>
</html>
```

* [Table of Content](#table-of-content)
