# Writing Reflection

### What resources did you use and why?
My two primary resources for this exercise were the [Mapbox Studio
Manual](https://www.mapbox.com/studio-manual/overview/) and the [Documentation Principles presented by Write the
Docs](https://www.writethedocs.org/guide/writing/docs-principles/) (WtD). (Happy to report that I found a _very minor_
typo on WtD and made a [pull request to fix it](https://github.com/writethedocs/www/pull/713) on the Documentation
Principles page.)

### What tone did you use and why?
Given the description of the user as somebody _new to Mapbox Studio and not a developer_ I settled on the current tone,
which I hope comes off as a mix of respectful towards the reader, human-yet-informative, while also mixing with the tone of
other Mapbox documentation. What I mean by "respectful of the reader" is, frankly, not treating them like a child while
acknowledging that they are not necessarily GIS developers (who understand the fundamentals of things like datasets and
tilesets). One of the choices I made, to this end, was intentionally not using analogies in explanitory phrases, though I had thought about it:

> Imagine a map as being made up of puzzle pieces, and those puzzle pieces are made up of even more puzzle pieces:
> that's just like what a tileset is.

I also did not include phrases that might indicate something is simple so as to imply that reader is deficient should
they not understand the concept or instruction:

> Determining whether to use a dataset or tileset is easy

To make my tone sound more personable and human, and keeping in line with other sections of the Mapbox Studio
documentation, I did end up settling on referring to the user as "you." In a previous iteration I used overly neutral
language to address readers: "the user will...", "they can upload to..." I was afraid to use "you" and "your" at the risk
of being too familiar. However, other Mapbox Studio documentation uses "you," so that gave me the confidence to proceed thusly.

### How did you tailor the content to your audience?
Starting right at the top, I went back and forth several times about whether or not to include the page subtitle ("Choose the
right tool for creating your custom map in Mapbox Studio") and the bulletted list that almost reads as a tl;dr. However,
given the WtD principle of [docs being skimmable](https://www.writethedocs.org/guide/writing/docs-principles/#skimmable)
and thinking the user might be coming for a quick answer I kept them in. I want to communicate quickly that, yes, this
is the right place to find the answer to their question of which is appropriate, tileset or dataset.

In that same spirit of being skimmable, I tried to keep each concept short, including links to more in-depth
documentation where appropriate, and
[cumulative](https://www.writethedocs.org/guide/writing/docs-principles/#cumulative) by putting the tilesets description
before datasets. Mainly I was keeping in mind that this documentation is, after all, here to answer a specific question and is not a
walkthrough about the mechanism of uploading or converting tilesets and datasets, respectively.

That being said, to sufficiently answer the reader's question, I felt it was appropriate to offer a brief overview of
tilesets and datasets instead of just linking to their docs. Ancillary to this I thought that, armed with information about what
these data types are, the reader gains confidence to delve deeper or, if they are not even a customer yet and on the fence
about using the product, now feel more ready to sign up. Almost documentation as a sales sheet.

Finally, I ended with three [use case examples](https://www.writethedocs.org/guide/writing/docs-principles/#exemplary), aiming these at readers who either have never used the product
or are such casual users that they forget the key concepts of custom maps. The goal here was to reinforce the basic
concepts of both data types, especially what was written in the bulletted summary: tilesets can be uploaded, datasets
can be created in the dataset editor and exported as tilesets, and datasets can be edited there, too.