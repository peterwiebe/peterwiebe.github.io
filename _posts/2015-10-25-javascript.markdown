---
layout: post
title:  "JavaScript and Ruby Comparison"
date:   2015-10-25 12:00:00 -0800
categories: ruby javascript
---
We spent the last week at DBC going through JavaScript for the first time and discovered some good things and not so good things when it comes to the programming language for the web. Below are some code snippets comparing the two languages - their similarities and their differences.

<div class="begin-ruby"></div>

### Ruby

<div class="begin-javascript"></div>

### JavaScript

<div class="begin-ruby"></div>

type conversion from integer to string:

{% highlight ruby %}
x = 10.to_s
{% endhighlight %}

<div class="begin-javascript"></div>

{% highlight javascript %}
x = 10.toString(); // or
x = "" + 10;       // apparently this is faster in most browsers : http://stackoverflow.com/questions/5765398/whats-the-best-way-to-convert-a-number-to-a-string-in-javascript
{% endhighlight %}

<div class="begin-ruby"></div>

for loops:

{% highlight ruby %}
arr = [1,2,3,4]
for i in 0..(arr.length-1)
  p arr[i]
end
{% endhighlight %}

<div class="begin-javascript"></div>

{% highlight javascript %}
var arr = [1,2,3,4];
for(var i = 0; i < arr.length; i++) {
  console.log(arr[i])
};
{% endhighlight %}

<div class="end-example"></div>


  Across all of the examples for JavaScript you will notice that I have included the semicolon. While not always necessary, I have started to get into the habit of using them since it may be difficult to discern when it is required vs. not required.

  As in the type conversion example above you will find that Ruby is much more concise and to the point than JavaScript. It isn't only in the methods though, you can see it in the lack of endline characters for Ruby and throughout many more aspects of the Ruby language. A lot of times this makes debugging Ruby much easier.

  A second example that I wanted to incorporate was the for loop. I was a bit confounded that there wasn't a similar for loop in Ruby as you see it in JavaScript. I first learned programming languages using Java and the structure for 'for' loops in JavaScript was right at home for me. I recently found myself trying to force a Ruby for loop in a situation where it wasn't ultimately needed but it was what my gut reaction wanted me to use. It was because I wanted to increment by not just one but two in the Ruby equivalent to only make changes to every second element in an array. We found another way but I felt as though the JavaScript way was better - I obviously have many things still to learn with ruby.

  In comparison, the for loop for the Ruby syntax is again much simpler but a bit cumbersome (which is why I would probably recommend a different iterator method). The JavaScript for loop gives you a bit more control than Ruby's and can sometimes be easier to process when you first see it.

  More examples yet to come!