---
layout:     post
title:      "Innntroduction to Approachable for Developers and Makers"
subtitle:   "Start Here"
date:       2016-10-14 12:00:00
author:     "Approachable"
---

> This is Markdown Cheatsheet Demo for **Sustain**, this Jekyll theme. Please check the raw content of this file for the markdown usage.

## Typography Elements in One

Let's start with a informative paragraph. **This text is bolded.** But not this one! _How about italic text?_ Cool right? Ok, let's **_combine_** them together. Yeah, that's right! I have code to highlight, so `ThisIsMyCode()`. What a nice! Good people will hyperlink away, so [here we go](#) or [http://www.example.com](http://www.example.com).

<div class="divider"></div>

## Headings H1 to H6

# H1 Heading

## H2 Heading

### H3 Heading

#### H4 Heading

##### H5 Heading

###### H6 Heading

<div class="divider"></div>

## Footnote

Let's say you have text that you want to refer with a footnote, you can do that too! This is an example for the footnote number one [^1]. You can even add more footnotes, with link! [^2]

<div class="divider"></div>

## Blockquote

> Start by doing what's necessary; then do what's possible; and suddenly you are doing the impossible. --Francis of Assisi

**NOTE:** This theme does NOT support nested blockquotes.

<div class="divider"></div>

## List Items

1. First order list item
2. Second item

* Unordered list can use asterisks
- Or minuses
+ Or pluses

<div class="divider"></div>

## Code Blocks

{% highlight javascript %}
var s = "JavaScript syntax highlighting";
alert(s);
{% endhighlight %}

{% highlight python %}
import sys  
s = "Python syntax highlighting"
print(s)  
def run_some_function():
    "Docs..."
    return
{% endhighlight %}

{% highlight css %}
/* css synthax highlighting */ 
#container {
    float: left;
    margin: 0 -240px 0 0;
    width: 100%;
}
{% endhighlight %}

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```

<div class="divider"></div>

## Table

### Table 1: With Alignment

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

### Table 2: With Typography Elements

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

<div class="divider"></div>

## Horizontal Line

The HTML `<hr>` element is for creating a "thematic break" between paragraph-level elements. In markdown, you can create a `<hr>` with any of the following:

* `___`: three consecutive underscores
* `---`: three consecutive dashes
* `***`: three consecutive asterisks

renders to:

___

---

***

<div class="divider"></div>

## Media

### YouTube Embedded Iframe

<iframe width="420" height="315" src="https://www.youtube.com/embed/nN6QuNqmAwk" frameborder="0" allowfullscreen></iframe>

### Image

![Nature](https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcSn8cwf82ee9tfml4Wx-tsM5AUavJ_DRHIiXXE4RejRp0RF2L7f6g)

[^1]: Footnote number one yeah baby!

[^2]: A footnote you can link to - [click here!](#)
