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
One of the biggest things we learned while working on our project was learning how to work with tensorflow. Of course, we used tensorflow quite a bit in lecture, but actually working hands-on with using it to create our own RNNs was helpful in getting a better understanding of how it works, since we ran into a lot of errors and issues that we had to sort through ourselves. Additionally, we learned about how to save our tensorflow models instead of training them each time before use, because RNNs take a few hours to train. This proved to be a hurdle at some points, but overall was helpful since it made our end product a lot more efficient.

We also learned how to use Flask to present our project in a much more user-friendly way. This isn’t a web development course, so naturally it wasn’t required for us to do this, but it did help in furthering our experience with integrating our programming skills into a UI. Being able to work with a UI is a pretty useful skill, as it allows people who don’t feel as comfortable with programming to still use the project. Additionally, it can certainly help us demonstrate our programming skills in a much more direct way, since the UI grants the project a more streamlined user experience with the visual appeal of a webapp.

Lastly, we learned a decent amount about data storage, retrieval, and manipulation. Since our dataset was so large, we had to be clever about the way we stored it in places like GitHub and Google Drive, and it was somewhat difficult figuring out how to integrate it with our Flask site. The data itself was also in an unfamiliar format, namely compressed with a .tar.gz extension, so we needed to figure out how to unpack that. Additionally, we had to do more research on SQL queries, since our `find_recipe` function needed to retrieve matching recipes from a list of ingredients, which at first we weren’t sure how to do. We also had to be a bit creative about how we figured out which recipes were the best (i.e. which recipes had the most ingredient matches), and learning a bit about certain pandas methods that we hadn’t used before was quite helpful.


# In the Future
For me, this project was a great stepping stone both in terms of exposure to different technological practices and capabilities and group work. Throughout the quarter we encountered different roadblocks, the main one being that our desired output required knowledge and skills that we hadn't yet covered in lecutres and they seemed very difficult to learn on our own. I think we surprised ourselves in our ability to replicate some very complex python processes on our own before Professor Chodrow lectured on RNNs. 

Given that I'll be working in Analytics, this type of project ressembles the work I'll be doing full time. Outside of college, there isn't a set curriculum or specific way of doing things to achieve any given task. I will have to lead much of my learning and find ressources on my own to build out whatever it is I need. This project was a great way to jump into that "real world" work flow, as much of what we lerned was gathered on our own, but we still were able to rely on our amazing teaching staff. I'm very grateful for this experience and I'm excited to see what else is achievable with python programming.