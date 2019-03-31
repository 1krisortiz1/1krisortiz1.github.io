---
layout: post
title:      "My First Solo Sinatra Project"
date:       2019-03-30 21:45:29 -0400
permalink:  my_first_solo_sinatra_project
---

![Sinatra](data:image/jpeg;base64,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)
[](http://)
## Intro to me
My Learn.co journey has been an interesting one, interesting to me at least :).  There have been many ups and downs for me throughout this journey but I pushed through and reached the Sinatra project section of the curriculum and while it was nerve wrecking to start from scratch and a little challenging throughout, I had so much fun!  

 ![cactus](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdu_OJafF8tOFPmoMe7nyvBSh_CdCpSQnlHOCIfR7G2-kMbLxy)  
 
 ![Flower](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTngZkCHCV-t-pmt4U_Lx0_N-sXOQIZNDwlmULtwA2eN8Pi1kvY)

So, I moved to Arizona about 10 years ago and whenever I was asked about living here I always talked about wanting to leave…but I never did.  An maybe it's just me getting older, or maybe AZ has started to grow on me but recently I've really appreciated the beauty of the desert.  Cactus are beautiful in their own way and the desert mountains have this really beautiful look about them during sunrise and sunset.  As a result of my new found love of desert plants I found myself taking random pictures of desert plants and sunrises so I decided to build a Sinatra application similar to pinterest or Instagram where users are able to create an account to share the things that they love, specifically desert plants and cactus. 

## The wonderful `corneal gem`

Luckily we were introduced to the `corneal gem` created by Brian Emory.  As a newbie to coding,  I was really grateful! So, the corneal gem is a Sinatra app generator that uses a file structure similar to what you see with Rails.  

To install, run 
```
gem install corneal
```

Create app
```
corneal new APP-NAME
```


Then run:
```
bundle install
```

 Below is a screen shot of the directory structure: 
```
├── config.ru
├── Gemfile
├── Gemfile.lock
├── Rakefile
├── README
├── app
│   ├── controllers
│   │   └── application_controller.rb
│   ├── models
│   └── views
│       ├── layout.erb
│       └── welcome.erb
├── config
│   ├── initializers
│   └── environment.rb
├── db
│   └── migrate
├── lib
│   └── .gitkeep
└── public
|   ├── images
|   ├── javascripts
|   └── stylesheets
|       └── main.css
└── spec
    ├── application_controller_spec.rb
    └── spec_helper.rb
```


And here are the commands:
```
corneal -v              # Show Corneal version number
corneal help [COMMAND]  # Describe available commands or one specific command
corneal new APP-NAME    # Creates a new Sinatra application
corneal model NAME      # Generate a model
corneal controller NAME # Generate a controller
corneal scaffold NAME   # Generate a model with its associated views and controllers
```


This gave me a good starting point.  The `environment.rb` file is prepopulated and so is the `config.ru` file however I did need to make sure to mount my controller as well as make sure to use  `use Rack::MethodOverride`. Corneal has this great scaffold command that generates a model with its aassociated views and controllers but I built mine on my own. 

## Models, Controllers, Views, and Database
Then it was up to me to take what was taught and practiced in previous lessons to build out my the models, controlers, views, and of course the database. 

Like I mentioned above, my application is really basic and was built to just meet the project requirements but I am really excited to circle back around down the road to really turn this into something to show off.  

