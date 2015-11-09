---
layout: post
title:  "CSS Classes and IDs"
date:   2015-09-28 12:00:00 -0800
categories: css class id
---
Classes and IDs are both great ways to style specific parts of your page, allowing you to select individual or separate parts of your page by tagging them with the class or id attribute.

A best practice for using classes is to only use it when you are trying to style a number of items that you intend to style similarly. For instance, if you want an unordered list to have all of its list items to maintain a certain style then assigning a single class to all of the list items will usually be the best route. They all should have the same style and if you need to make a change, all of the list items get updated at the same time when that change is made. Imagine if that list had dozens of items included in it and each item had its own class, it would take quite a while to make all those changes and make sure that they are all exactly the same.

Here is an example of a set of widget divs that have the same class as they will need to be styled similarly:

![CSS Class Screenshot](/assets/class.png)


A best practice of using ids is that you only use it once for anything on your page. Should you use an id on more than one element then your code will not pass validation. Situations where you may want to use an id over a class is would be where the web page has single elements that need to have its own styling like a content wrapper for instance. Some web pages will have a container where all of the content is placed. Because that container only appears once in the page it is defintitely worthwhile to having an id for the element to style it.

Here is an example of a container element that holds a bunch of items. Because the styling is specific to that individual element it has its own id tag:

![CSS ID Screenshot](/assets/id.png)

That being said, there may be instances where you may need to use both an id and a class on the same element. You can do that. You can have multiple selectors when styling your HTML including both the id and class.

And lastly, here are two div elements that share the same class tag but also have separate id tags for separate styling:

![CSS Class and ID Screenshot](/assets/both.png)