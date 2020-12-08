# sinatra
A small project testing the Sinatra web framework: http://sinatrarb.com/intro.html

## Motivation
To test Sinatra in action, to help understand how client-server request response cycles.

## Build status
Complete.

## Screenshots
![Eric the Cat](https://https://github.com/chriswhitehouse/sinatra/Screenshot 2020-12-08 at 20.04.17.png)


## Tech/framework used
Ruby

## Features
Form to personalise the cat name

## Code Example
```html
post '/named-cat' do
  p params
  @name = params[:name]
  erb(:index)
end

get '/form' do
 erb(:'cat-form')
end
```

## How to use?
In IRB `shotgun app.rb -p 4567` then use 'localhost:4567/cat-form' in your browser.
