---
layout: essay
type: essay
title: "Final Project Idea: Manoa Spots"
date: 2019-03-26
labels:
  - Software Engineering
  - Meteor
---

# Overview
#### Problem:
UH students need spots to hang out, wait or study, but finding the perfect location to do so may be a difficult task. Most students are unaware of the variety of spots available on campus.
#### Solution:
This website lists various spots on campus along with pictures, description. It displays information on the noise level, crowdedness, outlet availability, windows, table sizes, etc. Users may log in to their accounts to add reviews/ratings or add their own spots to be added to the site. There is a lot of freedom to users as almost anywhere on campus can be considered a spot that can be rated and reviewed.

Admins will be able to delete comments and spots as well as ban a user from leaving spots/comments. This would be done by adding a role to the user such as ‘banned’.

# Mockup Page Ideas
  * Landing Page
  * List Spots
  * Admin List Spots
  * Spot Info Page
  * Profile Edit Page
  * Add Spot
  * Edit/Delete Spot
  * Login/Logout/Sign up
  
#### Landing Page
The landing page welcomes the user to the Manoa Spots site. It contains some information on what the site does and explains how to use it. It will be accessible via the navbar and also be the base page.

#### List Spots
This will appear in the navbar but also be linked separately on the landing page. This page with contains a list of Spots around UH. It can be sorted by popular, new and highest rated. It can also be filtered by noisiness, indoor/outdoor, AC and a number of other attributes. It can also be filtered by keyword in that it will check if a word appears in the title or description.

#### Admin List Spots
Almost identical to the ‘List Spots’ page but is only accessible to admins. Admins can use this page to delete any Spot. This allows admins to maintain some level of order on the site.

#### Spots Info Page
This page would appear when a spot is clicked from the ‘List Spots’ Page. It would have images of the Spot as well as some information regarding the Spot. There would be a list of reviews from users as well as a box to allow users to leave their own reviews. A review contains a rating using a typical 5-star rating system as well as a short blurb of their review. The review can optionally also contain attributes A user can also edit/delete their comments on this page. An admin can delete any comment on this page.

#### Profile Edit Page
This page appears on the navbar and allows users to view their profile. This profile contains some volunteered information from the user as well as a list of their Spots. From here they can change their personal information as well as add/edit/delete spots.

#### Add Spot
This page appears when clicking on an ‘add spot’ button. This page allows a user to fill out a form to create a spot. This form would include information such as a brief description, noisiness, indoors, capacity etc. There will be a warning explaining that spots not meeting certain guidelines will be removed.

#### Edit/Delete Spot
This page appears when clicking on the edit button on a spot that appears on the ‘Profile Edit Page’. This allows a user to edit or delete a page that they have created. There will be a warning explaining that spots not meeting certain guidelines will be removed.

#### Log in/Log out/Sign up Page
This page allows users to log in, log out, or sign up for an account. Will appear in the navbar

# Use Case Ideas
#### Creating a New User:
User goes to the landing page, signs up, edits profile page, returns to Landing page
Landing Page → Sign Up Page → Profile Edit Page → Home Landing Page
#### Users:
User goes to the landing page, logs in, goes to list spots page, goes to a spot’s page and leaves a comment
Landing Page → Login Page → Landing Page → List Spots Page → Spot Info Page
#### Admins:
Admin goes to the landing page, logs in, goes to admin list spots page, deletes a vulgar spot.
Landing Page → Login Page → Landing Page → Admin List Spots Page

# Beyond the Basics
  * Allow users to create/edit/delete spots
  * Allow users to create/edit/delete reviews
  * Search for spots by keyword
  * Filter spots by attributes (noisiness, indoors, air-conditioned)

# Team
This essay was collaboratively written by Andrew Millard, Isaac Lee, and David Liang
