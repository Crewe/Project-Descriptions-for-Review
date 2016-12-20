# Mashups

## Project Overview

Time to take the tools you’ve learned to build a “mashup” app. The app will pair a random image with a random quote. If your users like what they see, they can save their mashup for everyone to view later. They can also delete existing mashups from the database.

You’ll connect to two different APIs for this, and will use the MVC pattern to keep your code organized. To save your mashups, you’ll use ActiveRecord to connect to an sqlite3 database.

The APIs you choose to use are up to you! We have included a list of options to get you started, but if there’s an API you’d like to use that’s not listed, go for it!

## Completing this Project

Running `ruby app.rb` should start up the app and bring you to a page displaying a random image and quote to the user. Refreshing the page should get a new random image and quote.

When the user clicks the submit button, the mashup should be saved to the database.

There should be a `/mashups` route that gets all the current mashups in the database and displays them to the user. There should also be a way for users to remove a mashup from the list if they choose to.

Finally, each mashup should have its own Mashup page.

We have collected a list of APIs below that you may want to use. None of the APIs below require authorization to use. You may decide to choose two from this list, or use different APIs of your choice.

APIs for Random Images:
* https://github.com/Giphy/GiphyAPI#random-endpoint  (API docs)
* http://www.splashbase.co/api#images_random  (API docs)
* http://thecatapi.com/docs.html  (API docs - note: no JSON option)

APIs for Random Quotes:
* https://wisdomapi.herokuapp.com/v1/random  (API endpoint)
* http://q.uote.me/api.php?p=json  (FRANÇAIS - API endpoint)
* http://www.quotzzy.co/api/quote  (API endpoint)

## Submitting Your Project

Compress your project directory with all of its contents as a single zip file. The application should be fully implemented and functional. Your project reviewer will be asked to run and test your app.

Before submitting your project for evaluation, we recommend that you check that each of the following is true:

* Your program runs without any errors
* You are proud of your project and its output
* You completed your project according to the instructions
* You checked your project against the [rubric](https://review.udacity.com/#!/rubrics/183/view)
* When you feel ready to submit, use the blue 'Submit Project' button below!