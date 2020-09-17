Created By:  
[Chandler Hulstrom](https://github.com/Chulstro)<br>
[Nick Edwin](https://github.com/NickEdwin)<br>
[Michael Alex Lynch](https://github.com/mlynch5187)<br>
[Ryan Laleh](https://github.com/RyN21)<br>

# Grow Ops

Grow Ops is a Rails Application for gardeners, new and experienced alike.
What will you grow today?

The idea behind this application is to give users a guide to set up and plan their own garden.
The user will simply need to add the size of their garden, their zip code, and the estimated lighting, and our app will give a list of all the possible vegetables and how much they can plant within their garden.

Our code is open source because we would like to show off what we have, and also invite others to contribute too if they feel inclined to do so.

# Languages/Frameworks

  - Ruby
  - Rail
  - Sinatra
  - HTML
  - CSS
  - Bootstrap

# Visual Representation of Schema   
This diagram shows all of our database tables and how they're linked to one another.  
![Visual Schema](https://i.imgur.com/BKgtBf6_d.webp?maxwidth=728&fidelity=grand)

# API's

Building out this application, we consume a few different API's.

- Trefle API
  This is the main squeeze of our application. The trefle API has an exstensive collection of plants from vegetables to flowers, and even a variety of grass types to a variety of trees.
  With each plant, we have access to a wide array of data. For the functions of this app, the data we collect is as follows:
    - plant name
    - row spacing
    - spread
    - edible
    - images
    - light
    - max and min ph
    - max and min temperatures
    - number of days to harvest

  - Soil Grids API
    In order to for our application to give the users a list of plants they can choose for their garden, we need to feed ph levels of the soil and/or the lighting levels of the garden to Trefle's API.
    To get the PH levels, we use Soil Grids.
    Soil Grids is an API where we can find the PH levels based on Longitude and Latitude

  - Open Data Soft API
    In order to get Longitude and Latitude, we need our users to give us their zip code.
    Open Data Soft is a API that allows us to convert a zip code into longitude and latitude, which we then use to collect the PH levels through Soil Grids, which we can then finally create a list of plants that our users can use for their garden.
