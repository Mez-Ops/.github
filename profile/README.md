Welcome to the Mez Ops GitHub page! 👋

We are a small team of 1 developer and 1 UI/UX designer.

Lead developer: [Tyler Jewell](https://github.com/tyler-jewell)

This readme is focused on the developer and contains all of our best practices when it comes to developing application for Mez Ops.

## Development 10 Commandments

1. **ALL** coding work starts with a [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues). This allows us to track all work from ideation to release
2. **ALL** GitHub issue titles shall follow standard [semantic versioning](https://www.conventionalcommits.org/en/v1.0.0/) guidelines
3. 100% unit test coverage for applications. Nothing less
4. The required IDE is [VS Code](https://code.visualstudio.com/)
5. Branches shall be named with {user}/{issueTitleCleaned} (i.e., tyler-jewell/fix-a-bug)
6. Pull request titles must be the same as the issue title it is tied to


## Development Process

1. A [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) is created to track work. This can be an idea, feature request, bug, etc.
2. Admin investigates and approves the issue to be worked on by the team
3. Issue is assigned to a developer to work on and a branch is created
4. Commit(s) are made to the development branch
5. Pull request is created to merge the development branch into main
6. Linting, unit tests, and semantic versioning checks are ran to ensure code quality and best practices
7. Pull request is squashed into one commit (the issue title) and merged into main
8. Version files are bumped to the next semantic version
9. Changelog is updated to document the work that was done for the latest version
10. A tag is created and pushed to the repo
11. Release is created from the new tag
12. Artifacts built (apk, .ipa, etc.)
13. App is published to appropriate repo or stores (pub.dev, Apple Store, Google Play Store, Firebase Hosting, etc.)




### Assigning an issue to yourself

There are two ways to assign the issue to yourself:

1. (Preferred) Using the [GitHub Pull Request](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) extension in VS Code. All you need to do is find the issue on the left panel and select the forward arrow. This will automatically create a branch locall and assign you to the issue. 

![image](https://user-images.githubusercontent.com/72859335/210772109-d3f846d4-f3b5-40a0-8230-b33ccd7fe5ae.png)

2. GitHub console - open the issue and add your name to the assignees. You will also need to manually create a branch locally that is named {user}/{issue title}.

![image](https://user-images.githubusercontent.com/72859335/210772399-1da72059-1e45-4f1c-b660-af0b525bd487.png)


### Creating issues

A clean and well-organized project starts with a clean and standardized GitHub issue being created to tie to any work being done on an app. 

Multiple downstream automation processes use the information and links in the issue

- Automatic pull request titles
- Automatic changelog updates
- Automatic closure of issue when a PR is merged with the issue linked to it

Similar to [assigning issues to yourself](#assigning-issues-to-yourself), you can either create an issue on GitHub or use the extension in VS Code. 

- **Using the VS Code extension**

1. While on the GitHub extension, click the '+' icon to the right of the issues panel

![image](https://user-images.githubusercontent.com/72859335/210774064-706e41d3-6108-4062-a779-9731b255a1dc.png)



![image](https://user-images.githubusercontent.com/72859335/210771284-e51e9485-daf9-4dc6-8db8-71aa5a88b6f0.png)



- figma link

### New repo settings


