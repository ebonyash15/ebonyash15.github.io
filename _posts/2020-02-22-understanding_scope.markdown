---
layout: post
title:      "Understanding Scope"
date:       2020-02-23 01:04:22 +0000
permalink:  understanding_scope
---


When trying to understand scope, it may prove beneficial to picture nesting dolls. The smallest and innermost doll looks out at the larger doll encasing it,but the largest and outermost doll cannot see any of the other dolls it holds.

Like the small doll, instances have their own scope but can also access the scopes of the objects they are within. Classes cannot access information held by their instances, like a larger doll.If an instance of #cherry_pie is the innermost doll, the class Pie is a larger doll which holds it. They could both be incased in a larger doll, the class Dessert, from which the Pie class inherits.

The instance above would be able to access variables and methods (if properly called) from the Pie and even Dessert classes. Due to scope limitations, the Pie class cannot use instance information, only its own and that inherited from the Dessert class.  The desert class has a scope restricted to itself and can only use it's own variables and methods, it does not respond to those of the other scopes.


According to Tutorialspoint.com, A scope is a region of the program and broadly speaking there are three places, where variables can be declared − 
      Inside a function or a block which is called local variables,
      In the definition of function parameters which is called formal parameters.
      Outside of all functions which is called global variables.

Class scope is the area of code where a class variable or method is valid.  Class variables in Ruby are denoted as @@variable_name and class methods are mentioned as .method_name.

Instance scope is used to refer to variables and methods that are accessable to individual instances of a class. Instance variables are defined and called with @variable_name and the standard syntax for mentioning an instance method is #method_name.

If you are confused about the current scope these standard Ruby syntax rules can help distinguish.  If there are multiple classes and still lies confusion you can ask an object.method pair for it's owner:

        object_name.method_name.owner
          => Owning_object_name
