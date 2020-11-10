READ ME STUFF ONLY for 11/9

<<<<<<< Updated upstream
# gruhb-doc.github.io

## Table of contents

* [Overview](#overview)
* [User Guide](#user-guide)
* [Developer Guide](#developer-guide)
=======
## Table of contents

- [Overview](#overview)
- [User Guide](#user-guide)
>>>>>>> Stashed changes

## Overview

Gruhb doc is a web application that provides available food vendors and menu items for UH Manoa.

<<<<<<< Updated upstream
* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code.
* [React](https://reactjs.org/) for component-based UI implementation and routing.
* [Semantic UI React](https://react.semantic-ui.com/) CSS Framework for UI design.
* [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

It also provides code that implements a variety of useful design concepts, including:

* Three primary collections (Profiles, Projects, Interests) as well as three "join" Collections (ProfilesInterests, ProfilesProjects, and ProjectsInterests) that implement many-to-many relationships between them.
* Top-level index pages (Profiles, Interests, and Projects) that show how to manipulate these six collections in various ways.
* Initialization code to define default Profiles, Interests, and Projects and relations between them.
* A simple Filter page to illustrate how to perform simple queries on the database and display the results.
* Use of Meteor Methods to illustrate how to simplify implementation of multiple collection updates.
* Use of indexes to enforce uniqueness of certain fields in the collections, enabling them to serve as primary keys.
* Authentication using the built-in Meteor accounts package along with Sign Up and Sign In pages.
* Authorization examples: certain pages are public (Profiles, Projects, Interests), while other pages require login (AddProject, Filter).


### Add Project page

Once you are logged in, you can define new projects with the Add Project page:

![](images/add-project-page.png)

### Filter page

The Filter page provides the ability to query the database and display the results in the page. In this case, the query displays all of the Profiles that match one or more of the specified Interest(s).

![](images/filter-page.png)


## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the [Gruhb Doc application github page](https://github.com/gruhb-doc/gruhb-doc), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.

Third, cd into the bowfolios/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000).


### Quality Assurance

#### ESLint

Gruhb-doc includes a [.eslintrc](https://github.com/gruhb-doc/gruhb-doc/blob/master/app/.eslintrc) file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
meteor npm run lint
```

Here is sample output indicating that no ESLint errors were detected:

```
$ meteor npm run lint

> gruhb-doc@ lint /Users/YOURNAME/github/gruhb-doc/gruhb-doc/app
> eslint --quiet --ext .jsx --ext .js ./imports ./tests

$
```

ESLint should run without generating any errors.

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).



## Development History

The development process for gruhb-doc conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:

* Development consists of a sequence of Milestones.
* Each Milestone is specified as a set of tasks.
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete.
* Tasks should typically consist of work that can be completed in 2-4 days.
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number.
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master.
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of BowFolios.

### Milestone 1: Mockup development

### Milestone 2: Data model development

## Milestone 3: Final touches
=======
- [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code.
- [React](https://reactjs.org/) for component-based UI implementation and routing.
- [Semantic UI React](https://react.semantic-ui.com/) CSS Framework for UI design.
- [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

The goals of the project are:

- Create a simple user interface and experience for anyone on the UH Manoa campus who want an easy-to-use tool for looking for food vendors.
- Learn and practice web development by using techniques we learned in this course and by also doing our own research.
- Learn how to work on a project with a group of people.
- Gain experience with project management (i.e. Git, issues, branches, etc.).

As stated as the first goal of the project, the system should eventually provide an easy-to-use tool for anyone who finds themselves on the UH Manoa campus and need to find a place to eat.

## User Guide

This section provides a walkthrough of the Gruhb Doc user interface and its capabilities.

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site. We plan to use [Yelp's](https://www.yelp.com) home page as a basis for the overall layout and design.

### Sign in and sign up

The user will be able to “Login” or “Sign Up” on the top right corner of the page. We will once again be using [Yelp's](https://www.yelp.com) homepage as a basis for designing the layout of the user account functionality.

![](images/landing.png)

### Home page (Vendors, Profile, Favorites)

The user home page of Gruhb Doc will allow the user to navigate through three different pages, the vendors, profile, and favorites. We will be basing this design off of [Pioneer Saloon’s](http://www.pioneer-saloon.net) website. On the home page, the user will also see the top pick of the day.

![](images/homepage.png)

### Vendors

The Vendors page will be presented in a feed type of format. Users will be able to filter the page and favorite a vendor from the list of vendors. We will be basing this design off of [Yelp's](https://www.yelp.com) feed design.

![](images/feed.png)

### Profile page

Once the user is logged in, they will be able to access a profile page where they can edit their personal information. We will be basing this design off of [Instagram’s](https://www.instagram.com) edit profile design.

![](images/profile.png)

### Favorites

The Favorites page will be once again presented in a feed type of format. Users will be able to see a feed of their favorite vendors for easy access. We will be basing this design off of [Instagram's](https://www.instagram.com) feed design.

![](images/ig_feed.png)

### Vendor

After a user clicks on a vendor from the Vendors page, the Vendor page will be displayed and the details of the vendors like the hours, menu, cuisine etc. will be shown to the user. We will be basing this design off of [Yelp's](https://www.yelp.com) vendor page design.

![](images/vendor.png)
>>>>>>> Stashed changes
