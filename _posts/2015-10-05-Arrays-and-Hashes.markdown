---
layout: post
title:  "Arrays and Hashes - The Basics"
date:   2015-10-05 12:00:00 -0800
categories: ruby array hash
---
The topic of today's blog is on Ruby colletions: Arrays and Hashes. Related programming structures, Arrays and Hashes are both tools that you would use when you want to store multiple objects in one variable.

Arrays and Hashes contain locations within them. The number of locations can grow and shrink as necessary and can contain any object in the ruby language. Because a whole bunch of values are located within one variable, going through each variable becomes very easy especially with the built in functions that ruby provides - this is called iterating. You can loop through the values performing a function on each of them in a short amount of time.

The structure of both Arrays and Hashes are similar and different. The objects that each structure contains are located in a sequential position, but only Arrays are typically used for their sequentially ordered locations. That is, in Arrays, each item is stored at a given index within the Array located by an integer value.  The only way you can access a value within the Array is by referring to the locations by index values. It should be noted that Arrays start at an index of 0 and increase by 1 for every index.

Hashes also have integer index value for each object stored in the hash but it is much more common to set and retrieve objects in a hash by a key. A key is a string or symbol that one uses to locate a specific value. For example, say you wanted to represent a car with a hash, you could create a string called 'tires' and then store the name of the tires at the location tires in the hash. Whenever you call the hash key of tires it would respond back with the name of the tires that were purchased.

When choosing between an Array and a Hash a guideline would be that an Array is most effective when the objects that are stored in it are of the same type. Iterating through an Array with all of the same objects is fast and convenient. Hashes, however, are more effective when storing different types of objects but are all associated to the same purpose. Iterating through hashes are not any more difficult than arrays with Ruby's prebuilt functions but there is less order to a hash than an array. It should be noted that both could be used almost interchangeably.

I encourage reader feedback, so if you have any comments please contact me via any of the mediums below.