# Web 3 Hackathon

Welcome to the Web 3 hackathon!

Today's challenge is to deploy a website for a new Creative Coding club in Kortrijk, Belgium.
As the founders of the CCK, you will make this a team effort. Off course, you will manage this using Git and GitHub Flow.

[Let's git ready to rumble!](https://www.youtube.com/watch?v=nendMLrpI-s&t=20s)

## CHALLENGE 0: Team Up

Divide yourselves into teams of **three**.

## CHALLENGE 1: Set Up the project (1 per team)

One team member should complete the following steps:

- open the starter project in your code editor
- initialize a new git repository
- create a new repository on GitHub and push the local repository to GitHub
- [add the other team members as collaborators to the GitHub repository](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository)
- make your repository public.

Provide the URL of your GitHub repository via [this form](https://forms.gle/VHo5o13paYTLBANU8).

The leaderboard will be updated every 10 minutes.

[leaderboard](https://repo-leaderboard.pages.dev/)

## CHALLENGE 2: Readme file

- on a new feature branch named `feature/readme`:
- 1 team member should create a readme.md file in the root of the repository.
- The readme file should contain the names of all team members.
- After committing and pushing the changes, create a pull request to merge the feature branch into the main branch.

## CHALLENGE 3: Build the CCK website (all team members)

There are 3 different content collections set up for this website: Workshops, Foundations and Team members. Additionally, there is a News collection to share news items. (But that's for a later chanllenge)

Have a look at the `src/content.config.js` file. This file contains the configuration for the content collections. When fields are missing in the markdown file, the build will fail.

Every team member will take care of one of the content collections. Each one will work on a separate feature branch. When one is done, create a pull request to merge the feature branch into the main branch. Make sure to resolve any merge conflicts that may arise and to pull the latest changes from the main branch in the end.

### ##PLACEHOLDERS##

We've added some placeholders in the code in a form of ##WHAT-SHOULD-BE-HERE##. These are meant to be replaced by the actual content.
You don't have to edit CSS or write any plain HTML. But you will have to write some logic in the provided files.

### Workshops (Student 1)

- Create a feature branch named 'feature/workshops' from the `main` branch and work on this branch.
- Add the `Workshops` component to the /index page
- List all the workshops in the `Workshops` component (See `Content collections` chapter above)
  - Make use of the `WorkshopCard` component to display the workshop data
- Show all the necessary data in the `WorkshopCard` component
- Provide the detail page, you can use the id as an dynamic route parameter.
  - You can find a starterfile in resources/workshops/detailpage

### Foundations (Student 2)

- Create a feature branch named 'feature/foundations' from the `main` branch and work on this branch.
- Add the `Foundations` component to the /index page
- List all the foundations in the `Foundations` component (See `Content collections` chapter above)
  - Make use of the `FoundationsCard` component to display the foundations data
- Show all the necessary data in the `FoundationsCard` component
- Provide the detail page, you can use the id as an dynamic route parameter.
  - You can find a starterfile in resources/foundations/detailpage

### Team (Student 3)

- Create a feature branch named 'feature/team' from the `main` branch and work on this branch.
- Feel free to change the contents of the markdown files to match the team members of your group
- Add the `Team` component to the /index page
- List all the team members in the `Team` component (See `Content collections` chapter above)
  - Make use of the `TeamCard` component to display the team member data
- Show all the necessary data in the `TeamCard` component
- Provide the detail page, you can use the id as an dynamic route parameter.
  - You can find a starterfile in resources/team/detailpage

## CHALLENGE 4: News (All students, each one news item)

- Every student should create a feature branch for their news item from the `main` branch and work on this branch.
- Everyone should add one news item to the news collection. (see resources/news)
- Decide on who will implement what:
  - Define the news collection in the `src/content/config.js` file (hint: look at the other collections and don't forget to export it)
  - The whole content of all the items are listed on the /news page
    - Find out how you can get the 'Content' (hint) of a markdown file on that page (this is something else than frontmatter data...)
  - Sort them descending by date
  - You can make use of .toDateString() or .toISOString() to format the date of the news item

## CHALLENGE 5: Deployment

- One team member should set up the deployment of the website to GitHub Pages.
- Make sure that the website is automatically deployed when changes are made on the main branch.
- Follow all the steps described in the [Astro documentation](https://docs.astro.build/en/guides/deploy/github/).

## CHALLENGE 6: Hide the code! (all team members)

Since this is a rather boring website for a Creative Coding club, let's add at least some wordplay om 'code' to make it more fun. The idea is that the users should find hidden digits for a 4-digit code somewhere on the website. Each of you will hide at least one digit on your part of the website. The digits should be hidden in a way that they are not immediately visible, but can be found by users who do a little effort. (console logs, hover effects, clickHandlers etc...) Make sure to document where you have hidden your digit in the README.md file of the project. Naturally, each one of you should create a new feature branch for this challenge.

Create a `/code` page that implements the `Code` component so that the users can enter the digits found. You will figure out how to set this up.

## Award ceremony

Info will follow.

![Award](./readme-assets/award.jpg)
