# Backend Mid

Develop a Rest API

## Task

### Use case

AlwaysNote is a tech startup that aims to replace quick notes apps such as Keep and Notes.

### Resources

#### Create Note
As an API Client, I need to make a request with the POST method to create a new annotation. The annotation must be saved in a database with my user ID, also informed in the request, the current date and time and the title, which is always the first line of the annotation.

#### Edit Note
As an API Client, I need to make a request with the PUT method to edit an existing annotation. The annotation must be updated in the database with the date and time the update was performed.

Note: the annotation can only be edited by the user who created it.

#### List Annotations
As an API Client, I want to make a request with the GET method to list my user's notes. The listing must be paginated, allowing a minimum of 1 note and a maximum of 10 notes per page and must bring only the title of the note and its date of update.

#### Get an Annotation
As an API Client, I want to make a request with the GET method to get the entire content of an annotation

#### Send a Note to the trash
As an API Client, I want to make a request with the DELETE method to make a logical deletion of an annotation.

#### Batch to empty trash
Annotations that have been logically deleted within a 30-day period must be permanently removed from the database. For this, the application must run an activity daily at midnight to carry out this process.

## How to deliver it?

The task can be marked as finished if it has a Github repository containing the source code, and a readme with the instructions to build and test it. As a database is required to finish this task, a docker-compose and instructions on how to use it would be great.

