# CSE204Final
A readme for CSE 204

## Welcome to my final project

* The goal of this project was to create a GitHub base social media site that allows users to post thier projects and view other's projects via README writeups.

## Features

* Login using your GitHub account (scopes are set to read profile info only.) This was accomplished using [FirebaseAuth](https://firebase.google.com/docs/auth)
* Upon login your public repos (not inluding those created through another organization like this class) will be displayed on the right of the screen along with a post button.
//IMG

* When the post button is clicked, the contents of your readme file are requested from Github. Once the reponse is received a second request is sent to convert the .md file to html. Finally, profile information, repo information and the html version of the readme are sent to a [firebase cloud firestore databse](https://firebase.google.com/docs/firestore).
//IMG

* On logging in a listener is set to listen for changes to the database stroing all posts so when any user adds a new post, it will immediately be displayed for all users on the left side of the screen.
//IMG

* Each post contains the repo name, owner's username, a link to the repo, and the owner's profile picture in the post header. Below the post header is the readme for the repo.  
//IMG

## Notes
* Readme images must be specified using a url (not just the file location in the repo) to be displayed correctly.


