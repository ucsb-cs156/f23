---
title: project
desc: "Legacy Code Project instructions"
assigned: 2023-11-07 14:00
due: 2023-11-29 11:59
github_org: ucsb-cs156-f23
layout: lab
layout: default
parent: lab
num: project
nav_order: 300
proj_courses_slack_url: https://ucsb-cs156-f23.slack.com/archives/C066057BBHA
proj_happycows_slack_url: https://ucsb-cs156-f23.slack.com/archives/C065XJGBVL3
proj_gauchoride_slack_url: tbd
proj_organic_slack_url: https://ucsb-cs156-f23.slack.com/archives/C065H6A9VM5
qxx: f23
githubOrgUrl: https://github.com/ucsb-cs156-f23
githubProjectsUrl: https://github.com/orgs/ucsb-cs156-f23/projects
githubPagesUrl: https://ucsb-cs156-f23.github.io
sections:
  - 
      time: 5pm
      product: proj-happycows
      productShort: happycows
      teams:
        - 
          num: 1
          dokku: "01"
          kanban: 43
        - 
          num: 2
          dokku: "02"
          kanban: 44
        - 
          num: 3
          dokku: "03"
          kanban: 45
        - 
          num: 4
          dokku: "04"
          kanban: 46
  - 
      time: 6pm
      product: proj-organic
      productShort: organic
      teams:
        - 
          num: 1
          dokku: "05"
          kanban: 47
        - 
          num: 2
          dokku: "06"
          kanban: 48
        - 
          num: 3
          dokku: "07"
          kanban: 49
        - 
          num: 4
          dokku: "08"
          kanban: 50
  - 
      time: 7pm
      product: proj-courses
      productShort: courses
      teams:
        - 
          num: 1
          dokku: "09"
          kanban: 51
        - 
          num: 2          
          dokku: "10"
          kanban: 52
        - 
          num: 3
          dokku: "11"
          kanban: 53
        - 
          num: 4
          dokku: "12"
          kanban: 54
---

# Links


<details markdown="1">
<summary markdown="1">Open this section for links to the legacy code project resources    
</summary>


{% for section in page.sections %}
## Section: {{ section.time }} ({{section.product}})

| Team | Repo | Github Pages | Kanban | Dokku Prod | Dokku qa |
|------|------|--------------|--------|------------|----------|{% for team in section.teams %}{% capture teamName %}{{page.qxx}}-{{section.time}}-{{ team.num }}{% endcapture %}{% capture repoName %}{{section.product}}-{{teamName}}{% endcapture %}
|  {{teamName}} |  [ repo ]({{page.githubOrgUrl}}/{{repoName}}) |   [ github pages ]({{page.githubPagesUrl}}/{{repoName}}) | [ kanban ]({{page.githubProjectsUrl}}/{{team.kanban}}) | [ dokku prod ](https://{{section.productShort}}.dokku-{{team.dokku}}.cs.ucsb.edu) | [ dokku qa ](https://{{section.productShort}}-qa.dokku-{{team.dokku}}.cs.ucsb.edu) | {% endfor %}

{% endfor %}
  
</details>

# The Assignment, Briefly.

In this project:

* You will be assigned a legacy code base, and a set of issues 
  (new features, refactorings, bug fixes)
* The list of issues contains more work than we expect you will need to complete
  in order to get a perfect score on the project, so don't worry that you have
  to finish them all; *you do not have to finish them all*.
* Each issue you complete earns points for your team after it is:
  * code reviewed and approved by a member of your team that didn't work on it
  * code reviewed and approved by a member of the course staff (instructor, TA, LA)
  * merged into the main branch of your repo.
* Issues earn different numbers of points: typically, 5, 10 or 20 depending on 
  the complexity of the issue (more on this below).
* There may be a few issues that are marked as "must do".  You *must
  complete these* or their point values will be subtracted from the points you
  earn. These are assigned point values in advance.  
* For other issues,
  points are assigned after completion. If you want to ask for a point
  estimate, you may do so, but keep in mind that actual points can differ
  from estimated points.
* Unlike in previous team projects, where your Issues list and 
  Kanban board may have been
  pre-populated with issues by the staff,
  in the legacy code phase, populating the Kanban board
  is the responsibility of the team.  More on that below.
* The aim of the team is to earn 100 points before the deadline.  This forms the 
  most important part of you project grade, which is 25% of your course grade.
* Another part of your project grade is your "CATME multiplier", which is a number
  based on your peer evaluations.  This number is typically 100 unless your team
  has rated you significantly below the team average
* Points beyond 100 can count as extra credit as explained below.

# Points beyond 100


If you accumulate more than 100 project points, the additional points may count as extra credit, at a rate of 1 extra credit point for each 10 points over 100 earned, up to a maximum project grade of 110.  For example:

| Points Earned | Project Grade |
|---------------|---------------|
|    80         |    80         |
|    90         |    90         |
|   100         |  100          |
|   105         |  100.5        |
|   110         |  101          |
|   115         |  101.5        |
|   150         |  105          |
|   180         |  108          |
|   ≥200        |  110          |

Your final project grade is maxed out at 110 total project points--any points in excess of 110 will not count towards your grade (though you'll probably learn a lot from having under taken the work to earn them.)


# Sprint Planning for Legacy Code project

Each team already has a Kanban board setup for the legacy code project (see links below).   However unlike in your team01, team02, and team03 projects, it's up to you to populate this yourself.

| 9am | 10am | 
|-----|-----|
| [f23-9am-1]({{page.f23_9am_1}}) | [f23-10am-1]({{page.f23_10am_1}}) | 
| [f23-9am-2]({{page.f23_9am_2}}) | [f23-10am-2]({{page.f23_10am_2}}) | 
| [f23-9am-3]({{page.f23_9am_3}}) | [f23-10am-3]({{page.f23_10am_3}}) | 
|                         | [f23-10am-4]({{page.f23_10am_4}}) | 


You should add the `In Review` column if it is not already present.

Then, you should populate your todo column with issues, start assigning them to your team, and start working.   I'll cover where these issues come from in a moment.

You may not get through all of the Sprint planning today, but by the end of discussion section on Wednesday:
* Each of the six team members should be assigned to an issue in the todo column
* The previous bullet point shoudl *remain true* until your team reaches 100 points

Teams accumulate points when PRs are merged into main
* That is only done by the course staff for these projects.
* Each PR requires at least one code review from a team member, and at least one code review from a staff member
* The staff estimate points. Most issues are 5 to 10 points.
  - 5 points for very straightforward issues addressing a single concern
  - 10 points for issues that require a bit more work, but are nevertheless reasonably straightforward application of skills from team01, team02, team03.
  - 20 points is rare, and is reserved for issues that may be more complex, and/or require students to go significantly beyond the skills from previous course assignments.
* Note that breaking down issues into smaller chunks works to your benefit in multiple ways:
  - Easy to code review and merge (fewer merge conflicts), so faster point accumulation
  - Three 10 points issues and three 5 points issues adds up to 45 points; combining all of those together might only get you 20.
  - But the aim here should not be to "game the points". It should be to "get the issues implemented", in incremental "right sized" pieces.
  - If you do that, the points will take care of themselves.  
  
Points belong to the whole team, not to individuals
* Work as a team, and help each other.
* We do want to see every team member contribute
* Ultimately, it's a team project and a team grade.
* Having said that, really low CATME scores might result in a grade reduction.
 
  
## Where do issues come from?

For issues, you'll need to do a bit more work that in the previous team projects.

Here is where you'll get issues from:
* The three starter code repos have issues lists (as shown in the table below).
* These have been copied to your repo
* These issues come in different sizes 
  - A handful of these may be small easy issues. 
  - However, many (most?) of these issue *may not translate one-to-one into issues for your Kanban board*.
  - Instead, you are encouraged to try to *break the larger ones down into smaller issues*, each of which could be a single PR; more on this below.
  - This Sprint Planning meeting is where you can do some of that.
  - You may even need to add "issues about issues", e.g. an issue that says: "break issue #34 from proj-happycows into multiple issues on our team's repo".  Such an issue doesn't result in a PR, but it can still be moved across the Kanban board from `To Do`, to `In Progress`, to `In Review`, to `Done`.
* Your team's own ideas for features, based on the notes your team took last Wednesday during meetings with
  - Mike Fogelsanger for proj-gauchoride
  - Prof. Mattanjah deVries for proj-happycows
  <!-- - Prof. Phill Conrad for proj-courses -->

## Existing issues

Staff may add to these issues over the course of the project; when we do, we'll post an announcement in the project slack channels.

| Project |  Starter Code Repo | Issues Link | Project Slack Channel |
|---------|--------------------|-------------|-----------------------|
| proj-gauchoride | [Starter Code Repo](https://github.com/ucsb-cs156/proj-gauchoride) | [Issues](https://github.com/ucsb-cs156/proj-gauchoride/issues) | [`#proj-gauchoride`]({{page.proj_gauchoride_slack_url}}) |
| proj-happycows | [Starter Code Repo](https://github.com/ucsb-cs156/proj-happycows) | [Issues](https://github.com/ucsb-cs156/proj-happycows/issues) | [`#proj-happycows`](https://ucsb-cs156-s23.slack.com/archives/C058QUC16QP) |
<!-- | proj-courses | [Starter Code Repo](https://github.com/ucsb-cs156/proj-courses) | [Issues](https://github.com/ucsb-cs156/proj-courses/issues) |  [`#proj-courses`](https://ucsb-cs156-s23.slack.com/archives/C058BPFQZ42) | -->

## You are encouraged to keep each PR small.

For example, implementing a new feature may require
* A new React Component (with tests and storybook entries, and perhaps fixtures to support those)
* A new React Page
  - This page might start out with a simple PR that establishes a placeholder with text "New feature coming soon", and a trivial set of tests and a storybook entry
  - It might later get data from the backend and display it using a component, and be linked to from the navigation bar.
* A new database table (or a new column in an existing database table, requiring modifications to an `@Entity` and/or `@Repository` class
* New API backend endpoints, which require controller methods and tests.

Each of these could (and arguably should be) a separate PR!  This helps to keep PRs small, which makes code review easier, and also helps the team to divide up work among the team members.

Still, you may need to document in the issues what the dependencies are (e.g. "do issue 12 and 13 before starting 14").

# Legacy Code Background information

For each of the teams, there is already:
* A repo, seeded with the starter code from previous quarters
* A prod and qa dokku instance
* A Kanban board

For each, I've set up Google OAuth client id and client secret.
<!-- I've also set up the `UCSB_API_KEY` and `MONGODB_URI` for the `courses` project.   -->
You are welcome to use `dokku config:show app-name` to get these values and use them for your localhost setup.


# Staff Information

Information in the dropdown below is intended for course staff.  Students are welcome to look at it, but it's really targetted at a different audience.

<details markdown="1">
<summary>
Staff information for legacy code phase  
</summary>

# Creating the repos for the teams

To set up repos for the legacy code project phase, use the <https://ucsb-cs-github-linker.herokuapp.com> tool.

The menu option you want is "Teams // Create Team Repos":

<img width="444" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/a354dd8d-6a1c-4c2c-a870-f8b15ab2d528">

As an example, to create the repos for the `f23-5pm-.*` teams that are working on `proj-happycows`, fill in the form this way:

<img width="632" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/29f11a9c-4272-43ac-88d6-ce3a3aa37cb8">

Repeat for each group of teams and each project.

We assign `Write` permission rather than `Admin` permission so that the staff can control the `main` branch with branch protection rules.

# Why we don't do this with a fork

We don't use the `fork` approach for this reason: If we created the team repos as forks, then every time students create a PR, the default would be a PR back to the main repo.  This would be
fine if each of the teams was working on an independent set of tasks, but if the design is to have each of the teams work on the *same* set of tasks, then their PRs would clash and be redundant.

So, instead, we create independent repos in the course organization for the class offering (e.g. <https://github.com/ucsb-cs156-f23>, or <https://github.com/ucsb-cs156-w24>, etc.) that are initially populated with the `main` branch of the repo from the <https://github.com/ucsb-cs156/> organization. 

# Set up project channels

In the Slack workspace, set up channels for each project:

<img width="704" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/9a856d20-24e6-4f8e-b872-a84c2f47655b">

<img width="562" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/fcb80862-6fce-45f9-9fc2-105598137e5b">

<img width="559" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/f05d35ae-1ee0-49c0-8863-1024425b8168">

You can click "Skip for Now" and add folks to the channels later, or invite the students and staff to add themselves to the channels.

Then, update the links at the top of this page to the project slack channels (in the front matter):

Copy the link to the channel:

<img width="708" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/aa9a8129-336b-4932-a995-cefb34f093bf">

And then configure in the front matter of this page:

```
proj_courses_slack_url: https://ucsb-cs156-f23.slack.com/archives/C066057BBHA
```

Repeat for every project.

# Setting up Kanban boards

To set up Kanban boards for the legacy code project:

1. Make sure your github organization has a suitable template, i.e. a Kanban board set up with the
   views you want.  For example, this one: <https://github.com/orgs/ucsb-cs156-f23/projects/28/views/2>
2. Navigate to the template board so that your screen looks like this:

   <img width="1110" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/876a93c8-3561-4db3-990b-d12b9e37aee4">

3. For each team, click the `Use Template` button, and in the box that comes up, paste in the
   name of the repo for which you are creating a Kanban board; for example, pasting in `proj-happycows-f23-5pm-2` as shown here.  Also be sure that the owner is the github org for the course, e.g. `ucsb-cs156-f23`:

   <img width="608" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/7f49f240-f3c2-45b2-bb7d-8e9b0e6683e5">

   A kanban board will be created:

   <img width="663" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/579e7152-e75a-44d9-a7b8-6ea02cf41943">

   Repeat for each team.  To make this efficient, you may find that hitting the back button gets you back to the page where you can click `Use Template`; have the previous project name in your copy/paste buffer so that all you have to do is change the team number.

5. If you do these operations consecutively, in order from first to last team, you'll get a range of
   project numbers, e.g. twelve projects ranging in number from `43` to `54`.   

## Add project numbers (kanban board numbers) to Front matter

Next, put these numbers in the front matter of this page.  For example (only a portion of the yml shown here):

   ```yml
      time: 7pm
      product: proj-courses
      productShort: courses
      teams:
        - 
          num: 1
          dokku: "09"
          kanban: 51
        - 
          num: 2          
          dokku: "10"
          kanban: 52
        - 
          num: 3
          dokku: "11"
          kanban: 53
        - 
          num: 4
          dokku: "12"
          kanban: 54
   ```

## Link the kanban board to the repos

For each repo, visit the repo page and link the repo to the kanban board.

For example, on the repo page, click the `Projects` link:

<img width="1115" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/bdce9655-1d26-4ff4-8c3d-ad3668b8fbd6">

Find and click the `Link a Project` button:

<img width="276" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/2b65960d-0306-47cb-86ee-3b89bbe0de37">

Use the search box to find the project that matches the repo:

<img width="586" alt="image" src="https://github.com/ucsb-cs156/f23/assets/1119017/dfc5a7d8-80c0-4b96-b026-8ca0585ba951">

Click to link the repo to the project.





</details>
