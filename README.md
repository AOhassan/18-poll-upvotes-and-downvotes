# ![CF](http://i.imgur.com/7v5ASc8.png) Poll Upvotes and Dowvotes 

Create a webpage that allows users to enter questions and upvote and downvote
them. This assignment is all about practicing creating routes on controllers to 
receive information from a webpage and interacting with a database. There is no
auth in this assignment, there's no user accounts, anyone is allowed to submit
questions, and anyone can upvote or downvote as much as they want.

## Feature Tasks
* Create a Spring Application that serves a default homepage
  * The homepage should have a form where users can enter questions
  * The homepage should display a list of questions everyone has entered
  * The homepage should sort the questions so top-rated questions appear
    at the top of the list.
  * "Top-rated" questions is defined as questions with the largest total value
    after subtracting downvotes from upvotes. Here's an example ordering:
      * 12 upvotes 0 downvote
      * 23 upvotes 13 downvotes
      * 0 upvotes 17 downvotes
* Add a `POST` route at `/polls` to create a new poll
* Add a route for upvotes at `/polls/{poll_id}/upvote`
* Add a route for downbotes at `/polls/{poll_id}/downvote`
* Add CSS styling to make your page look like something more than a bare-bones
  HTML page.

## Stretch Goals
Build `/api/polls` routes and wire the entire application to interact with AJAX
instead of server-side templates.

## Submission Instructions
* Work in a fork of this repository
* Work in a branch on your fork
* Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-susan`
* Open a pull request to this repository
* Submit on canvas a question and observation, how long you spent, and a link to
  your pull request
