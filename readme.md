
# Flask Tutorial

  

I created this repo in order to follow step by step the Flask tutorial by Freecodecamp Youtube channel.

  

## In this course, i will learn:

  

- Setup and workflow

- Get a basic app running

-  *Templates* and *Static Content*

- Setting up and using Database (***SQLite***)

- Create a basic ***CRUD*** application

- Deploy to ***Heroku***

  
  

## Setup and workflow:

  

- Init repo

- Create a virtual environment

- Install all the dependencies.

- Create 'static' and 'templates' folders

  

- base.html works as a base structure. In this file we define the general purpose html, like the nav menu.

  

### Jinja 2:

  

***Jinja*** is a templating engine. This engine allows us to extends html code with a similar python syntax.

  

*Until now, i have used:*

- Curly brackets with percentage inside: '{% %}'

- Double curly brackets: '{{}}'


**- In order to extend html code, we need to use this syntax in our base file:**


~~~
{% block body %}

{% endblock %}
~~~


  Then, in the secondary file (the file that needs to inherit the main html code):


~~~
{% extends 'base.html' %}



{% block body %}

HTML CODE HERE

{% endblock %}
~~~


- Instead of the traditional way to link an style sheet, we use this syntax inside href="":
~~~
{{ url_for('static', filename='css/main.css') }}
~~~
