# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model layer in Rails ideally does most of the the actual processing of data
and holds the logic components of the program.  The model is made up of classes
and their methods.

```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller layer receives input from the server and communicates to the
models layers what the user is looking for.  This would be any action that the
user inputed to the browser, but the controller ideally does not process any of
the requests.

```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The router sees URLs and requests the correct controller according to the
specifications of the URL.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
The GET request from the browser is sent to the web server, which uses the
routers to get the correct controller.  The controller is created by a dispatcher
with the correct routing of '/controller/action/id'.
The controller finds the model that is responsible for the correct action and
asks it to find the correct id of whatever it is.  The model will perform the
action and give a response to the controller.  The controller returns a response
body to the server, which combines the data into an HTTP response and sends that
information to the user.

```
