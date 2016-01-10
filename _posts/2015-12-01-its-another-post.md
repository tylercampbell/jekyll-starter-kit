---
layout: post
title:  "A Sample Post"
summary:    This post contains several examples of markdown.
categories: updates
---

> Howdy! This is an example blog post that shows several types of content supported in this theme.

## Header 2

### Header 3

#### Header 4

Links : [Title](URL)  
Bold : **Bold**  
Italicize : *Italics*  
Paragraphs : Line space between paragraphs  

Line break : Add two spaces to the end of the line  
Lists : * an asterisk for every new list item.  
Quotes : > Quote  
Inline Code : `alert('Hello World');`  
Horizontal Rule (HR) : ---  

## Footnotes

Footnotes are supported as part of the Markdown syntax. Here's one in action. Clicking this number[^fn-sample_footnote] will lead you to a footnote. The syntax looks like:

{% highlight text %}
Clicking this number[^fn-sample_footnote]
{% endhighlight %}

Each footnote needs the `^fn-` prefix and a unique ID to be referenced for the footnoted content. The syntax for that list looks something like this:

{% highlight text %}
[^fn-sample_footnote]: Handy! Now click the return link to go back.
{% endhighlight %}

You can place the footnoted content wherever you like. Markdown parsers should properly place it at the bottom of the post.

### Code

Inline code is available with the `<code>` element. Snippets of multiple lines of code are supported through Pygments. Longer lines will automatically scroll horizontally when needed.

{% highlight js %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}

You may also optionally show code snippets with line numbers. Add `linenos` to the Pygments tags.

{% highlight js linenos %}
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
{% endhighlight %}

### Gists via GitHub Pages

{% gist 13f94b734a4ddb132735 gist.md %}

### Lists

Muris condimentum nibh, ut fermentum massa justo sit amet risus.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

Donec ullamcorper nulla non metus auctor fringilla.

1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

### Images

![placeholder](http://placehold.it/740x400 "Large example image")

### Tables

| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | $1600 |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |

Nullam id dolor id nibh ultricies vehicula ut id elit.

-----

[^fn-sample_footnote]: Handy! Now click the return link to go back.
