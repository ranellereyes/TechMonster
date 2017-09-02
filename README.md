# README

Welcome to the TechMonster (name pending) project!

## What is this project?

This is planned to be a single-paged application that will allow users to view videos on Youtube from the most prominent Fighting Game Community content creators that include online replays, tournament replays, and other noteworthy videos. Also include the ability to sort videos by certain categorial standards.

Future versions of the product will be able to webcrawl YouTube for tutorials and guides (start small with MVPs and then work our way up to here).

### How?

Planning on incorporating the following main components:

* __Backend storage of currently found links, users, and statistics on videos__
* __Youtube crawler that searches for new content__
* __Single-page web app frontend using React__

#### Backend

Will need to incorporate the following:

* Storage of video links (somehow, by URL? Depends on how Youtube API does it)
* User storage and needed Auth
* Likes and validation criteria to each video make sure the found video is relevant
* Email capability for users to signup

#### Youtube crawler

Will need to incorporate the following:

* Successfully find relevant YouTube links, most likely by title
* Be able to be triggered by Heroku every week and search specificall through the "Last Week" criteria on YouTube
* Update the database when new video is found

#### Frontend

Will need to incorporate the following:

* Index views depending on game and character
* Show views for specific videos, comments possibly?
* Submission for user submitted content

## Current Action Tasks

* YouTube crawling research
  * Research YouTube APIs
  * Figure out the best way to store videos in the Backend
  * Figure out the best webcrawling method to scour YouTube's videos that were posted within a Week

* Database
  * Choose a database (SQL vs No-SQL?)
  * Create model schema
  * Create desired API Routes
  * Incorporate Auth
  * Incorporate Upvotes/Downvotes system and comments
  * Incorporate sorting of videos by above criteria (popular/most commented)
  * Incorporate a validation criteria to make sure the video in the database is legitimate
  * Make sure the YouTube crawler has access and ability to add new videos it finds on it's weekly crawl

* Frontend
  * Create Wireframes
  * Create component hierarchy
  * Choose design
  * Get necessary images
