---
layout: post
title:  "Ruby - Enumerable Method: each_slice"
date:   2015-10-12 12:00:00 -0800
categories: ruby enumerable each_slice
---
What is the <code>each_slice</code>?

each_slice is an enumerable method that takes an enumerable and yields a number of elements in the enumerable to be operated in the following block of code.

An example given from the ruby docs:
{% highlight ruby %}
  (1..10).each_slice(3) { |a| p a }
  # outputs below
  [1, 2, 3]
  [4, 5, 6]
  [7, 8, 9]
  [10]
{% endhighlight %}

Why should you use <code>each_slice</code>?

The Enumerable class is inherited by arrays, hashes, ranges, sets - all of which contain a collection of objects in them, sometimes all of those objects are all the same, sometimes they are different but have a certain pattern to them. You would want to use the slice to work on a group of the items in the collection at one time.

When should you use <code>each_slice</code>?

Imagine for a second that you have an array of people's names. You want to create a new array with arrays of groups of those names. The initial single dimension array could be parsed through with the <code>each_slice</code> method with the number of people you want to have in your groups and then in the code block that follows you could push that group into a new array called groups.

Another situation could be that you know that the data returned in a collection object has a certain structure in a certain order. The order could be a name, a phone number, and an email. Knowing that, you could use `each_slice(3)` to look through your enumerable data, 3 elements at a time and add them to your page or into your database.

`each_slice` saved my bacon challenge 5.6 this week and it could save yours in the future. Have fun testing it out! --> You can see the offical docs here: <a href="http://ruby-doc.org/core-2.2.3/Enumerable.html#method-i-each_slice">http://ruby-doc.org/core-2.2.3/Enumerable.html#method-i-each_slice</a>