---
title: "Week 05c - 11.02 Thu"
lecture_date: 2023-11-02
description: "work on team02 or team03"
ready: true
layout: default
parent: lectures
slides: 
github_org: ucsb-cs156-f23
num: team03
---

# For lecture today:

* Start with standup
* Organize "in progress" issues for team03 (even if not done with team02; see below)
* Discuss whether to appoint a scrum master, or share the responsiblity, and post your decision to your team channel

I would prefer not to make this a "participation assignment"; I'd prefer to invite the teams to hold one another accountable for these three items.

# Organizing In Progress issues for team03

Even if not finished with team02, please do the following *today during class*
* Find your repo and Kanban board for team03
* Find the first issue for your database table (the tables are the same as for team02).  This could be either the creation of your dokku dev deployment, or it could be migrating your @entity, @repository, controller and controller tests from team02 to team03.
* Drag that issue into In Progress and assign it to yourself on the Kanban board.

# The Scrum Master role

There is a particular structured approach to Agile called "Scrum" (a term from the sport of Rugby).  One of the roles in Scrum is the "Scrum Master", a team member that has responsibility for making sure that the issues on the Kanban board are getting assigned, worked on, reviewed, and merged.

Some teams assign a specific individual as the "Scrum Master".   Other teams make "the whole team" be the Scrum Master, i.e. everyone on the team shares the responsibility of "auditing" the board periodically to look for anomalies and try to help the team correct those.  By anomalies I mean such things as:

* A team member that is not assigned to any issue
* An issue "In Progress/In Review/Done" not assigned to any team member
* An issue "In Review" that has no connected Pull Request
* An issue "In Review" that has been in that status for more than 24 hours with no one actually doing a code review
etc...

Today, in lecture, I'll ask each team to decide whether to
* (a) appoint a specific scrum master
* (b) share that responsibility as a whole team.

Please discuss, and then post your decision to the slack channel.

I will add that if you decide to appoint a specific scrum master, you might ask that person to serve in that rule through week 6, and then either ask them to continue, switch to someone else as scrum master for weeks 7/8, or switch to "whole team scrummaster".   Contemplating that could be part of your next retro.


# Going forward: make sure you have an In Progress issue before standup

I'd like to suggest that for future standups, that this be a part of the process, i.e.
* As part of your sharing on the slack channel, make a note of whether you have something in the in progress column for the project the team is working on,
* If you don't personally have something in the "in progress" column, fix that before standup. 
* During the out loud part of the standup, someone bring up the kanban board and verify that each person has an "in progress" issue.

The only time it would be normal to NOT have something there is if/when all of the issues for the team are "In Review" or "Done".
Even if all the issues for your database table are finished, if there are other issues to be done, you can assign yourself as a pair partner and help your teammates finish.



# Github Projects: Kanban / Table view

Each of your project boards (linked below) has two tabs labelled "Kanban" and "Table".  Please take a moment to familiarize yourself with the table view.  Note that you can sort by columns.

* The Kanban board view is better for getting a quick overview of the big picture status of the project
* The table view may be better for answering questions such as:
  * which issues in In Progress do/do not have team members assigned
  * which team members are/are not assigned to issues in the In Progress column
  * which issues under "In Review" do/do not have PRs connected to them

So whether you are the scrum master, or just a member of the team seeking to help keep the team on track, this can be a very useful tool.

Team02

| 5pm | 6pm | 7pm|
|-----|-----|----|
| [team02-{{site.qxx}}-5pm-1](https://github.com/orgs/{{page.github_org}}/projects/14) |[team02-{{site.qxx}}-6pm-1](https://github.com/orgs/{{page.github_org}}/projects/18) | [team02-{{site.qxx}}-7pm-1](https://github.com/orgs/{{page.github_org}}/projects/22) |
| [team02-{{site.qxx}}-5pm-2](https://github.com/orgs/{{page.github_org}}/projects/15)|[team02-{{site.qxx}}-6pm-2](https://github.com/orgs/{{page.github_org}}/projects/19)| [team02-{{site.qxx}}-7pm-2](https://github.com/orgs/{{page.github_org}}/projects/23)|
| [team02-{{site.qxx}}-5pm-3](https://github.com/orgs/{{page.github_org}}/projects/16)|[team02-{{site.qxx}}-6pm-3](https://github.com/orgs/{{page.github_org}}/projects/20)| [team02-{{site.qxx}}-7pm-3](https://github.com/orgs/{{page.github_org}}/projects/24)|
| [team02-{{site.qxx}}-5pm-4](https://github.com/orgs/{{page.github_org}}/projects/17) |[team02-{{site.qxx}}-6pm-4](https://github.com/orgs/{{page.github_org}}/projects/21) | [team02-{{site.qxx}}-7pm-4](https://github.com/orgs/{{page.github_org}}/projects/25) |

Team03

| 5pm | 6pm | 7pm|
|-----|-----|----|
| [team03-{{site.qxx}}-5pm-
1](https://github.com/orgs/{{page.github_org}}/projects/30) |[team03-{{site.qxx}}-6pm-1](https://github.com/orgs/{{page.github_org}}/projects/34) | [team03-{{site.qxx}}-7pm-1](https://github.com/orgs/{{page.github_org}}/projects/38) |
| [team03-{{site.qxx}}-5pm-2](https://github.com/orgs/{{page.github_org}}/projects/31)|[team03-{{site.qxx}}-6pm-2](https://github.com/orgs/{{page.github_org}}/projects/35)| [team03-{{site.qxx}}-7pm-2](https://github.com/orgs/{{page.github_org}}/projects/39)|
| [team03-{{site.qxx}}-5pm-3](https://github.com/orgs/{{page.github_org}}/projects/32)|[team03-{{site.qxx}}-6pm-3](https://github.com/orgs/{{page.github_org}}/projects/36)| [team03-{{site.qxx}}-7pm-3](https://github.com/orgs/{{page.github_org}}/projects/40)|
| [team03-{{site.qxx}}-5pm-4](https://github.com/orgs/{{page.github_org}}/projects/33) |[team03-{{site.qxx}}-6pm-4](https://github.com/orgs/{{page.github_org}}/projects/37) | [team03-{{site.qxx}}-7pm-4](https://github.com/orgs/{{page.github_org}}/projects/41) |

