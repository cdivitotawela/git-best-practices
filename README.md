# Git Best Practice Guide

## One Conceptual Group per Repository
Consider setting-up single repository for single cenceptual unit. Each repository will have single build file which gnerate single unit of logical artefact. If considering CI such as Jenkins Pipelines each repository has single Jenkins file which build and test single unit.

## Selecting Collaborating Workflow
There are few popular collaborating workflows and select one that will best suite to project team and the team culture. Ref: https://www.atlassian.com/git/tutorials/comparing-workflows

### Centralised Workflow
Great for teams transitioning from SVN. This is better if one developer work on the changes at a given time. If the team is large and many developers work on the code same time, this would not be recommended. Only maintain the master branch and all the changes committed to the master branch. However it is advised to keep the master branch clean by squashing the commits if you are a person who create commits for every small change.


### Feature Branching
This workflow is best suite for a team where multiple team members making changes to code base at the same time. Each team mebmber working on its changes create a branch and work on the branch. Branch is typically created from the master. Work well if team work on small frequent changes and commit to master daily. Team probably need to rebase with master daily not fall far behind the master.
