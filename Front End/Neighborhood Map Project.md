##[Project Rubric](https://review.udacity.com/#!/projects/2711658591/rubric)

# For Reviewers
## How Grading Works

Please refer to the reviewer tips column in the [rubric](https://review.udacity.com/#!/projects/2711658591/rubric) for advice on how to evaluate specific rubrics. Email in to review-support@udacity.com if you have any questions.

# Project Overview

## How will I complete this Project?

Review the Neighborhood Map [Project Rubric](https://review.udacity.com/#!/projects/2711658591/rubric)

1. Review our course <a href="https://www.udacity.com/course/ud989-nd" target="_blank">JavaScript Design Patterns</a>.
2. Download the <a href="http://knockoutjs.com/" target="_blank">Knockout framework</a>. Knockout must be used to handle list, filter, and any other information on the page that is subject to changing state. Things that should not be handled by knockout: anything the map api is used for, tracking markers, making the map, refreshing the map.
3. Asynchrony and Error Handling. Note that All data APIs used in the project should [load asynchronously](https://discussions.udacity.com/t/handling-google-maps-in-async-and-fallback/34282) and errors should be handled gracefully.  In case of error (e.g. in a situation where a third party api does not return the expected result) we expect your webpage to do one of the following:  A message is displayed notifying the user that the data can't be loaded, **OR** There are no negative repercussions to the UI. **Note:** Please note that we expect students to handle errors if the browser has trouble initially reaching the 3rd-party site as well. For example, imagine a user is using your neighborhood map, but her firewall prevents her from accessing the Instagram servers. Here is a reference article on [how to block websites](http://www.digitaltrends.com/computing/how-to-block-a-website/) with the hosts file. It is important to handle errors to give users a consistent and good experience with the webpage. Read [this blogpost](http://ruben.verborgh.org/blog/2012/12/31/asynchronous-error-handling-in-javascript/) to learn more .Some JavaScript libraries  provide special methods to handle errors. For example: refer to .fail() method discussed [here](http://api.jquery.com/jquery.ajax/#jqXHR) if you use jQuery's ajax() method. We strongly encourage you to explore ways to handle errors in the library you are using to make API calls.
4. Write code required to add a full-screen map to your page using the <a href="https://developers.google.com/maps/" target="_blank">Google Maps API</a>. For sake of efficiency, the map API should be called only once.
5. If you are prompted to do so, you may want to get a [Google Maps API key](https://developers.google.com/maps/documentation/javascript/get-api-key), and include it as the value of the `key` parameter when loading the Google Maps API in **index.html**:
```<script  src="http://maps.googleapis.com/maps/api/js?libraries=places&key=[YOUR_API_KEY]"></script> ``` You may have some initial concerns with placing your API key directly within your JavaScript source files, but rest assured this is perfectly safe. All client-side code must be downloaded by the client; therefore, the client must download this API key - it is not intended to be secret. Google has security measures in place to ensure your key is not abused. **It is not technically possible to make anything secret on the client-side.**
6. Write code required to display map markers identifying a number of locations you are interested in within this neighborhood. This is the set of locations on which you will be searching and filtering in step 6. Your project should include at least 5 locations and display those locations when the page is loaded.
7. Implement input text area to filter your map markers displayed in step 5. The input text area should filter on markers that already show up. Simply providing a search function through a third-party API and displaying the results is not enough.
8. Implement a list view of the set of locations defined in step 5, filtering the locations via the input text area will filter the list view and map marker locations accordingly.
9. Add functionality using third-party APIs to provide information when a map marker or list view entry is clicked (ex. Yelp reviews, Wikipedia, Flickr images, etc). Note that StreetView and Places don't count as an additional 3rd party API because they are libraries included in the Google Maps API. If you need a refresher on making AJAX requests to third-party servers, check out our <a href="https://www.udacity.com/course/ud110-nd" target="_blank">Intro to AJAX</a> course.
10. Add additional functionality to animate a map marker when either the list item associated with it or the map marker itself is selected.
11. Add additional functionality to open an infoWindow with the information described in step 8 when either a location is selected from the list view or its map marker is selected directly.
12. Interface should be very intuitive to use. For example, the input text area to filter locations should be easy to locate. It should be easy to understand what set of locations is being filtered. Selecting a location via list item or map marker should cause the map marker to bounce or in some other way animate to indicate that the location has been selected and associated info window opens above map marker with additional information.
13. We expect your application to provide a filter option on the map markers displayed by default on load. The list view and the markers should update accordingly in real-time. Providing a search function through a third-party API is not enough to meet specifications.

## Example: BART Locations San Francisco

1. All locations displayed on map and in list view. Map marker selected and bounced. Info window opened.
2. List view item selected and highlighted. Associated map marker bounced and info window opened. 
3. Filtered items displayed on map and in list view. Map marker selected.
4. App displayed on mobile device with hamburger menu. (One possible mobile implementation.)

![Bart-1](http://i.imgur.com/7SJztlY.png)
![bart-2](http://i.imgur.com/74IC6X6.png)
![bart-3](http://i.imgur.com/KCYzG3L.png)
![bart-4](http://i.imgur.com/Dj2sWt7.png)

## Helpful Resources
None of these are required, but they may be helpful.

* <a href="https://developer.foursquare.com/start" target="_blank">Foursquare API</a>
* <a href="http://www.mediawiki.org/wiki/API:Main_page" target="_blank">MediaWikiAPI for Wikipedia</a>
* <a href="https://developers.google.com/maps/documentation/javascript/streetview" target="_blank">Google Maps Street View Service</a>
* <a href="https://developers.google.com/maps/documentation/" target="_blank">Google Maps</a>
* <a href="https://github.com/udacity/fend-office-hours/tree/master/Javascript%20Design%20Patterns/P5%20Project%20Overview" target="_blank">Project 5 Overview WebCast</a>
* <a href="http://learn.knockoutjs.com/" target="_blank">Knockout JS Tutorials</a>
* <a href="http://todomvc.com/examples/knockoutjs/" target="_blank">Todo MVC Knockout Example</a>

# Evaluation and Submission
## Evaluation
Your project will be evaluated by a Udacity reviewer according to the rubric below. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass. 

#[Project Rubric](https://review.udacity.com/#!/projects/2711658591/rubric)


## Submission
1. If build tools are used, submit both your source and production code in the same repository in separate directories.  These directories are usually named ```src``` and ```dist``` respectively.
2. If build tools are used the gulp or grunt.js file as well as the package.json file must be included in the submission.
3. If build tools are used, the instructions for building the project and running the tool must be included in the README.md. You may find the short [Writing READMEs course](https://www.udacity.com/course/writing-readmes--ud777) helpful.
4. The node_modules directory may contain thousands of files and should not be contained in the submission. See the forum post [how to remove node_modules directory from Github repository](https://discussions.udacity.com/t/how-to-remove-node-modules-directory-from-github-respository/40929) for instructions.
5. If you are prompted to do so, you may want to get a [Google Maps API key](https://developers.google.com/maps/documentation/javascript/get-api-key), and include it as the value of the `key` parameter when loading the Google Maps API in **index.html**:
```<script  src="http://maps.googleapis.com/maps/api/js?libraries=places&key=[YOUR_API_KEY]"></script> ``` You may have some initial concerns with placing your API key directly within your JavaScript source files, but rest assured this is perfectly safe. All client-side code must be downloaded by the client; therefore, the client must download this API key - it is not intended to be secret. Google has security measures in place to ensure your key is not abused. **It is not technically possible to make anything secret on the client-side.**
6. The master branch is the default Github repository branch. If you wish to submit another branch, you'll need to set it as the [new default branch](https://help.github.com/articles/setting-the-default-branch/) inside your Github repository.
7. When you're ready to submit your project go back to your <a href="https://www.udacity.com/me" target="_blank">Udacity Home</a>, click on Project 5, and we'll walk you through the rest of the submission process. Due to the high volume of submissions we receive, please allow up up to **7 business days** for your evaluation to be returned.
8. If you are having any problems submitting your project or wish to check on the status of your submission, please email us at **frontend-project@udacity.com** or visit us in the <a href="http://discussions.udacity.com" target="_blank">discussion forums</a>.


## What's Next?
You will get an email as soon as your reviewer has feedback for you. In the meantime, review your next project and feel free to get started on it or the courses supporting it!
