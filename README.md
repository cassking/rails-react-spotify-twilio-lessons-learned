# rails-react-spotify-twilio-lessons-learned
* an overview of lessons learned creating a Rails-React app using the RSpotify API ruby wrapper and the twilio ruby gem

Recently I was given an interview coding challenge where I was asked to create a simple Rails App that combined both music and SMS. 
In an effort to respect the challenge owners' authors, and their hiring process,  as well as
avoid any risk of exposing sensitive API keys and secrets, the code is in a private repo with my own API keys and secrets swapped in. 
I'm keeping  my code as reference for implementation in other apps I want to build in the future.

I feel compelled to share all the lessons learned for others to be brave and take the dive into both of thes fun APIs

While buidling this out, I stumbled quite a bit, but I learn lot! ..and... it was so much fun to build! 

I will be implementing some of what I learned in some of my other existing Rails-React applications. For example, I have a Rails-React app for cycling routes and I want to have users be able to simply text themselves a cycling route from any device.

## Where to find the APIs
Experimenting and exploring the [twilio-ruby] https://github.com/twilio/twilio-ruby library, module for using the Twilio REST API.

Experimenting and exploring the [RSpotify]https://github.com/guilhermesad/rspotify ruby wrapper for the Spotify Web API.

## Lessons learned
* how to interact with an API Wrapper which makes it much easier to pull desired responses than if you had to interact directly with the Spotify API.
[RSpotify docs] http://www.rubydoc.info/github/guilhermesad/rspotify/master
* how to interact with the Twilio Rest Client
* sending SMS
* using /lib modules to handle methods used in the controllers
* how to include a module in application_controller.rb to allow inheritance
* how to call methods from a controller that have been setup in a module
* how to use the hub interface to create new repos on your machine ( you will need to `brew install hub` and head over to the [hub docs]https://hub.github.com/hub.1.html). this [gist]https://gist.github.com/alexpchin/102854243cd066f8b88e details how
* ... and much more ...


## Technologies
* Backend: Rails 5.1.5
* Webpacker
* Frontend: React.js
