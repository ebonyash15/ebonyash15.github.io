---
layout: post
title:      "Previous Hashes Lab"
date:       2020-01-03 04:15:34 +0000
permalink:  previous_hashes_lab
---


For one of the previous lessons through FlatIron School's Software Engineering course, I built a family tree for fictional characters utilizing hashes and nested data collection types.

The code involved a deeply nested arrangement of arrays and hashes depending on the number of data points necessary. 
                [{Lord: {
								     name: "value", 
										 age: integer, 
										 status: "value", 
										 attitude: "value", 
										 mother: {
										       name: "value", 
													 age: integer, 
													 status: "value", 
													 attitude: "value"}, 
										father: {
										      name: "value", 
													age: integer, 
													status: "value", 
													attitude: "value"}, 
								  	friends: {
									        friend_1: {
												         name: "value",
																 age: integer, 
																 status: "value", 
																 attitude: "value"}, 
												   friend_2: {
												         name: "value", 
																 age: integer, 
																 status: "value", 
																 attitude: "value"}}}},
								{Lady: {
								        name: "value", 
												age: integer, 
												status: "value", 
												attitude: "value", 
												mother: {
												        name: "value", 
																age: integer, 
																status: "value", 
																attitude: "value"}, 
											 father: {
											          name: "value",
																age: integer,
																status: "value", 
																attitude: "value"}, 
											 friends: {
											          friend_1: {
																       name: "value", 
																			 age: integer, 
																			 status: "value", 
																			 attitude: "value"}, 
																friend_2: {
																        name: "value", 
																				age: integer, 
																				status: "value", 
																				attitude: "value"}}]

Once finished a person could reference elements from the hashes and learn the progression of bloodlines but in order to properly utilize it one had to have the order of nesting memorized and this was inconvinient. 

I would have revised and improved this code by adding a "TreeMap" function to my code so that users could reference the basic structuring of the tree.

This would be a method that printed to screen the family tree catagories in the following manner:

     Base of the trees- Please select either Lord or Lady
				       Search the resulting branches for Parents or Friends
     All of the above entities, base and branches of the family tree, can respond the following requests:
			        Status
							Attitude
							Age
							Name
		
Although names and spelling would still need to be memorized being able to print the entire tree at once would be a bit overwhelming on the screen and defeat the purpose of having a data collection that can be searched and interpolated from to meet user needs.

Hashes can be incredibly useful but also very difficult to keep track of and I kept a reference table of the basic set up to help myself organize any lines calling out an element. I believe that the ability to print a "Menu" that works much like the table of contents for books can deeply help improve the user-frinedliness of your code which is vital.
              
			
