---
layout: post
title:      "Hashes for the New Programmer"
date:       2019-12-06 13:28:17 +0000
permalink:  hashes_for_the_new_programmer
---


A hash is like a key ring, and each key unlocks a value of information. Hashes are an incredible tool when properly utilized and a cumbersome mess when mishandled.  If you have a collection of data wherein each item has its own specific attributes that are important to be able to access later, you need a hash.

A hash works well for storing data like resume information if you're a hiring manager. In that position you may create one like this:

```
  Potential_employees = [
				      {name: "Ebony Sharrock", manager_experience: "yes", years_in_field: 2, availability: "M-F 8:00-16:30", education: 
					  		"High School", desired_salary: 40000},
							{name: "Maria Ramirez", manager_experience: "no", years_in_field: 8, availability: "Any", education: "High School", 
					  		desired_salary: 45000},
							{name: "Ryan Hollman", manager_experience: "yes", years_in_field: 5, availability: "M-Sa 6:00-20:00", education: 
					  		"Bachelor's Business", desired_salary: 50000}
				 ]
```
	   Here we have created an array of hashes that hold information relevant to compatablity with the available job while 
		 keeping the information seperated by person. I used symbols (like :name) for keys because it makes code take up 
		 less memory. The use of JSON syntax was a matter of personal preference because it uses fewer keystrokes but 
		 `:name => "Ebony Sharrock", :manager_experiece => "yes"` is equally valid code.
	
	
Upon review, you have selected a candidate to offer the job, but you didn't save any contact information! You can just add it to your existing hash with  `Potential_employees[2][:phone_number]="302-867-5309"` .  Here it is imortant to remember that we created an array of hashes so that we know how to call each element to reference or manipulate it's data.

As you can see hashes can keep similar information seperated by instance (be that a person applying for a job, a breed of dog, a recipe, or whatever information is pertinent to your code). It is important to keep it in a clean format that you can read to ensure its utility is not lost in your confusion.  That being said, Ruby is not upset by extra space characters so if you need to write it like this--

```
  Potential_employees = [
	
				      {name: "Ebony Sharrock",        manager_experience: "yes",       years_in_field: 2,        availability: "M-F 8:00-16:30", 
							  education: "High School",                                     desired_salary: 40000},
								
							{name: "Maria Ramirez",           manager_experience: "no",          years_in_field: 8,        availability: "Any", 
							  education: "High School",   		                              desired_salary: 45000},
								
							{name: "Ryan Hollman",           manager_experience: "yes",         years_in_field: 5,       availability: "M-Sa 6:00-20:00", 
							   education: "Bachelor's Business",                    desired_salary: 50000}
				 ]
```

Or even

```
  Potential_employees = [
				      {name: "Ebony Sharrock", 
							        manager_experience: "yes", 
											years_in_field: 2, 
											availability: "M-F 8:00-16:30", 
											education: "High School", 
											desired_salary: 40000},
							{name: "Maria Ramirez", 
							        manager_experience: "no", 
											years_in_field: 8, 
											availability: "Any", 
											education: "High School",
											desired_salary: 45000},
							{name: "Ryan Hollman", 
							        manager_experience: "yes", 
											years_in_field: 5, 
											availability: "M-Sa 6:00-20:00", 
											education: "Bachelor's Business", 
											desired_salary: 50000}
				 ]
```

-- to keep your thoughts stratight, that is perfectly valid Ruby and fine to do! You need to write your code in a way that you and others can read it. Just make sure to stay consistent in formatting and walk through it one piece at a time.
