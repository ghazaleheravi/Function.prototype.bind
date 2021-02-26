# Function.prototype.bind

You are tasked with writing code to update the number of attendees as they arrive at a conference.
You create a simple webpage that has a button that, when clicked, increments the numOfAttendees property on 
the confrence object. You use jQuery to add a click handler to your button,
but after clicking the button the confrence object has not changed. 

why?
-This is a common problem when working with jQuery and JavaScript.
-When a function is used as an event handler, its 'this keyword' is set to the element on which the listener is placed,
-in the other words references the button and not the conference object.

solution:
You can use bind() to create a bound function(new funtion) and change the this value to the object that you need(here confrence),
and solve the problem.
