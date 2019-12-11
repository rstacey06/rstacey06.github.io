---
layout: post
title:      "ITERATORS "
date:       2019-12-11 15:46:39 -0500
permalink:  iterators
---


We have collections of data in Ruby that we call Arrays and Hashes. With these collections we can use Iterators, iterators are simply methods that are supported by these collections. They will return all elements of an array or hash, one after another. This blog will talk about the different types of iterators and when we use them. 

First we’ll start with `.each`
The each iterator will return all of the elements in your array or hash. This is particularly handy when you need to return your whole collection, it looks something like this:

ex:
`collection = ['a', 'b', 'c']
collection.each do |i|
   puts i
end`

output: 
`a
 b
 c`
 You should use .each when you want iteration but don’t care about what it returns.
 
 Next we have `.select` 
 The select iterator will filter through an array and return any element that is TRUE of the expression. Using select requires a block, inside the block you have to return something that evaluates to true or false, and .select will use that to filter your array. For example: 
 
 ex;
 `collection = [1,2,3,4,5]
  collection.select { |number|  number.odd? }
	end`
	
  output:
 `[1, 3, 5]`
 Basically it goes through an array and grabs all elements that are returnred true. Select is great when you want to filter a list & get an array with the results. The select method works in a similar way as .each, but constructs a new array containing all of the elements that match the condition, instead of just returning a single value and stopping.

`.find`
This iterator is used to take an expression and find the first element that is returned TRUE. Essentially this method will return the first element in an array that meets the criteria.

ex:
`collection = [ 1, 2, 3, 4, 5] 
  collection.find {|number| number.odd?}
	end`
	
	output:
	`1` 
	The .find iterator is good to use when you're looking for a specific element in an array.
	
	
	Finally we have `.map` or `.collect`
	These operator names are just synonyms, so they do the exact same thing. These iterators will return an array constructed as the result of calling the block for each item in the array. Basically the .map or .collect iterator performs an action on each array element, the original array is not modified and it will return a new modified array.
	
	ex:
	`collection = [ 1, 2, 3, 4, 5] 
  collection.map {|number| number + 1}
	end`
	
	output:
	`[2, 3, 4, 5, 6]`
	This  will always return an array with the same number of elements as the array on which you called it, this method is great to use for transforming the contents of array!
	
	In summary, there are multipule ways we can iterate in our program but being able to understand how each of these iterators work and selecting the correct one will is extreamly helpful when programing. 
	









