---
layout: doc-page
doc_source: 01-welcome  # The name of this Markdown file (without the .md folder)
permalink: /docs/welcome/

title: "Welcome"
excerpt: "Welcome"
---


_Gitomator_ is a set of command-line tools for batch operations on hosted Git repositories.      

It was built to help software educators use tools like [GitHub](https://github.com) or [Travis CI](http://travis-ci.com) in their classroom, and here are some of the tasks it can help you with:

 * Create, clone and update repos
 * Create teams and update team memberships
 * Set access permissions
 * Enable/disable CI


Think of Gitomator as a _Swiss army knife for your GitHub organization_.


If you are using GitHub in academia (e.g. running a software engineering course), you might want to start by preparing your organization.


### Prepare Your GitHub Organization

 1. Create a [GitHub organization](https://help.github.com/articles/creating-a-new-organization-account/)
 2. [Request a discounted/free plan for educational use](https://education.github.com/discount_requests/new).       
   _Note:_ You can start using Gitomator before getting your discount, you just won't be able to create private repos.
 3. **Important:** In your organization's settings page, go to the **member privileges**
    section and set the **default repository permission** to None.     
    (Otherwise, every students will be able to see every repo in the organization).
 4. _Suggestion:_ Make one of your colleagues an organization owner.         
    (Extremely useful for cases where one of you cannot access their account or
     accidentally loses their owner privileges)

Note, you do not have to invite all your students to your new organization manually at this point. The gitomator tools will this to happen whenever it is necessary. (could even propose Student team trick here)
