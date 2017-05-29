Create your first GitHub page
=============================

GitHub Enterprise Pages are public webpages freely hosted and easily published on your instance. 
The quickest way to get up and running is by using the Automatic Page Generator. If you prefer to work localy you can use the command line interface.

##### Table of Contents
[User & Organization Pages](#user)  
[Project Pages](#project)  

<a name="user"/>

## User & Organization Pages

User & Organization Pages live in a special repository dedicated to GitHub Enterprise Pages files. You will need to name this repository with the account name, e.g.

- You must use the username.[hostname] naming scheme.
- Content from the master branch will be used to build and publish your GitHub Enterprise Pages site.

<a name="project"/>

## Project Pages

- User Pages are available at https://[hostname]/pages/<username>.

Both personal accounts and organizations can create Project Pages.

- Organization's URL will be http(s)://[hostname]/pages/<orgname>/<projectname>.
- URL for a personal account's Project Page will be http(s)://[hostname]/pages/<username>/<projectname>/

Project Pages are kept in the same repository as their project. 
You must use the gh-pages branch to build and publish Project Pages.
