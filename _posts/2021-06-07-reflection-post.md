---
layout: post
title: Reflection Post
---

In this blog post, we reflect on the work we've done this quarter in the course project. We will discuss what went well (and not so well) and our eventual takeaways. The three of us wrote this document together, with the exception of the section on applications to future work, which is very individual.

# Overall Achievement
We created a local web application centered on recipes. Our aim was to help people who needed inspiration in the kitchen or had ingredients they wanted to use up. Our web app does two things: it finds recipes for the user that best match a list of ingredients, and it also can generate a brand new recipe based off of a seed string of user input.

To create the recipe finder, we used a pre-existing dataset called Recipes1M. Using the database and data manipulation skills we learned in class, we converted the data from its original format (a compressed tarfile) into a sqlite3 database. Then we designed a function to accept a list of user-inputted ingredients and then find a recipe in the database that was the closest match.

For the recipe generator, we built and trained a variety of machine learning models using the Recurrent Neural Network (RNN) framework. Then, using the weights of the trained models, we implemented a function to generate original text, seeded with a user-inputted string.

# Successes
We were really excited when we were able to get the web app up and running. This was, in our opinion, a great way to wrap the whole project together with a clean user interface. A consumer of our project wouldn't want to have to run a bunch of code in different notebooks to get started, so being able to simplify the process for them in this way was really big for us.

Another good achievement was being able to successfully train the recipe generation model. Several times, we thought that we had correctly designed a model, only to find out at the last step that things weren't working, for various reasons. While those moments were certainly very frustrating, it made it much sweeter when we were finally able to compile and train our first model.

# Improvements
Though we are very proud of the outputs we were able to achieve this quarter, our generated recipes are far from actual recipes one could follow. To further improve our project we would have wanted to train our model for a much longer period of time and hopefully have access to stronger computers to generate more successful recipes. 

We also would have liked for our website to be accessible on the world wide web for anyone to use. Much of the time we spent on the web app was dedicated to integrating our models and database to be accessible to flask, in the future we could work to integrate our website on a server. That would also require us to take more serious security measures to protect our own data as well as that of our users when they log onto our website. 

Finally, we had some other ideas for features to include in our website. One of them was to have a game in which we have users identify whether a recipe was a real one from our database or one that our model generated. This would of course require that our RNN model generate more reasilitc recipes as the game would be far too easy as the model is now.
# Comparison to Proposal
With respect to our proposal, we’ve achieved the majority of what we set out to do. Our idea of full success was to create a machine learning model that can create new recipes based on the ingredient data that it is given. We wanted  someone with no coding experience to be able to seamlessly use our product.

We did generate a working recipe generation model, which is somewhat coherent. As we outlined in the above section, we recognize that our model could be improved upon to generate more coherent text. Though the flask app is very usable once it is loaded, it’s usage does depend on a somewhat working knowledge of using the command line and having installed the proper packages, like tensorflow. 

# What We Learned

# In the Future
For me, this project was a great stepping stone both in terms of exposure to different technological practices and capabilities and group work. Throughout the quarter we encountered different roadblocks, the main one being that our desired output required knowledge and skills that we hadn't yet covered in lecutres and they seemed bery difficult to learn on our own. I think we surprised ourselves in our ability to replicate some very complex ython processes on our own before Professor Chodrow lectured on RNNs. 

Given that I'll be working in Analytics, this type of project ressembles the work I'll be oing full time. Outside of college, there isn't a set curriculum or specific way of doing things to achieve any given task. I will have to lead much of my learning and find ressources on my own to build out whatever it is I need. This project was a great way to jump into that "real world" work flow, as much of what we lerned was gathered on our own, but we still were able to rely on our amazing teaching staff. I'm vvery grateful for this experience and I'm excited to see what else is achievable with python programming.