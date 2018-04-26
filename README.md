# Fake News Demo! (CS 377I Project #1)

A Polymer 2.x application to teach people about how fake news spreads. 

## Setup
Visit https://www.polymer-project.org/2.0/start/install-2-0 and follow the installation instructions for installing polymer-cli. 

Then 
```bower install```

## Development
Run

```firebase serve --project cs-377i-fake-news```

and visit localhost:5000. You may be asked to authenticate first. 

To install new bower things, (e.g. a-bower-package):
```bower install a-bower-package --save```

## Deployment

```firebase deploy --project cs-377i-fake-news```

Deployment config is in firebase.json. Right now it just sends the whole current directory, since we don't really have a build process. Hence, I don't recommend viewing this app on your phone outside of wifi range! 

## Layout
The page you see should be demo/index.html. 

Every element referenced like `<element-name>` has a matching filename element-name.html. 

`<fake-news-app>` has two main components, a `<sign-up>` and a container with (1) a `<feed-items>` and (2) a `<brain-image>`. They are written as Polymer Elements, but it shouldn't matter too much, since most of the Polymer stuff is done. Most of the work we need to do is content creation! So that'll be drawing and writing markdown. 

The `<feed-items>` element maintains a list of `<feed-item>`, which are keyed on a property called `markdownId`. It corresponds to filenames in the markdown directory. A major task we need to work on is updating the items in `<feed-items>` according to user clicks. Right now, there's code that shows how to read the user's action in the function `_updateItems`. 

The demo/markdown folder contains the content we'd like to display on cards, formatted as markdown. You should name files in that directory like demo/markdown/<markdownId>.md. 

## Visualization -- the brain!
TODO...
  
  

