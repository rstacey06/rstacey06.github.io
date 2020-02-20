---
layout: post
title:      "RAILS Project"
date:       2020-02-20 17:28:22 +0000
permalink:  rails_project
---


Talk about putting in the hours, this was by far my most indepth and abstract project. I chose to go with a unfinished project I started with Sinatra( After a few hours programming I relized I'd need a couple weeks to write the code for and appointment log). So I picked up where I left off and implimented my AppointmentLog in Rails. 

 For this project i needed multiple Modles and Associations, I ended up making these pretty bland so this program could be used or formatted for many diffrent busniess models. My 4 models are a User, Client, Appointments and Locations. My User model has many Clients, Locations and appointments so they are able to interact with these models individualy and privatly. With that said Most of the work is done in my appointment model, its where my associtations between the users clients and locations are being kept track of. 
 
 Validations are another aspect of the program that were required.
 One of my biggest isseus was making sure my appointment times didnt overlap. I ended up needing a validation to compare begining an end times makeing sure they didnt conflict with each other. Here I ran into issues with the date and time, but by configuring a method in my appointment model to adjust timezones I was able to fix this right up! 
 
 Finally came Building forms with nested resources, whew! Here is where we can see what all the User can do, like create an appointment!  This is where you can fully see CRUD in action, we can create, read, update and delete! While creating an appointment we can choose a date and time obviously, but we can all select a durration, and we have optional input options such as a price and location. Here I also implimented helpers and partials for for my appointments just to keep everything clean and DRY.
 
 Once I finally was able to save an instance of an appointment I was able to install a simple calender gem to display it all cleanly. It was fairly simple just a quick bundle install, a few minor modifications and some partials I was able to display my Client, Location and a time block showing how log the appointment is for. 
 
 Overall this was a very challenging and time extencive process but i coulndnt be prouder seeing it all come together and the last month of rails in full use! 
