# Mez Ops Development Homepage

Welcome to the Mez Ops GitHub page! 👋

We are a small team of 1 developer and 1 UI/UX designer.

Lead developer: [Tyler Jewell](https://github.com/tyler-jewell)

Lead UI/UX designer: Barbara Jewell

This readme is focused on the developer and contains all of our best practices when it comes to developing application for Mez Ops.

# Development 10 Commandments

1. **ALL** coding work starts with a [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues). This allows us to track all work from ideation to release
2. **ALL** GitHub issue titles shall follow standard [semantic versioning](https://www.conventionalcommits.org/en/v1.0.0/) guidelines
3. 100% unit test coverage for applications. Nothing less (or more, I guess)
4. The required IDE is [VS Code](https://code.visualstudio.com/)
5. Branches shall be named with {user}/{issueTitleCleaned} (i.e., tyler-jewell/fix-a-bug)
6. Pull request titles must be the same as the issue title it is tied to

# Development and Deployment Process

1. Create [GitHub issue](#creating-issues) (manual)
2. [Issue assigned](#assigning-an-issue-to-yourself) and branch created off main (manual)
3. Commit(s) are made to the issue branch (manual)
4. Pull request is created to merge the issue branch into main (manual)
5. Linting, unit tests, and semantic versioning checks are ran to ensure code quality and best practices (automatic)
6. Pull request is squashed into one commit (the issue title) and merged into main (manual)
7. Version files are bumped to the next semantic version (automatic)
8. Changelog is updated to document the work that was done for the latest version (automatic)
9. A tag is created and pushed to the repo (automatic)
10. Release is created from the new tag (automatic)
11. Artifacts built (apk, .ipa, etc.) (automatic)
12. App is published to appropriate repo or stores (pub.dev, Apple Store, Google Play Store, Firebase Hosting, etc.) (semi-automatic)

![image](https://user-images.githubusercontent.com/72859335/210781207-682a5418-7a12-4344-b00b-bbe8240f377f.png)


## Assigning an issue to yourself

### Using VS Code (preferred) with the [GitHub Pull Request](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) extension

 All you need to do is find the issue on the left panel and select the forward arrow. This will automatically create a branch locall and assign you to the issue. 

![image](https://user-images.githubusercontent.com/72859335/210772109-d3f846d4-f3b5-40a0-8230-b33ccd7fe5ae.png)


### Using the GitHub console

Open the issue and add your name to the assignees. You will also need to manually create a branch locally that is named {user}/{issue title}.

![image](https://user-images.githubusercontent.com/72859335/210772399-1da72059-1e45-4f1c-b660-af0b525bd487.png)


## Creating issues

A clean and well-organized project starts with a clean and standardized GitHub issue being created to tie to any work being done on an app. 

Multiple downstream automation processes use the information and links in the issue

- Automatic pull request titles
- Automatic changelog updates
- Automatic closure of issue when a PR is merged with the issue linked to it

### Using the VS Code extension

While on the GitHub extension, click the '+' icon to the right of the issues panel

![image](https://user-images.githubusercontent.com/72859335/210774064-706e41d3-6108-4062-a779-9731b255a1dc.png)

This will pop open a markdown template file for the details to be entered. Again, the issue title needs to follow convention commit standards.

**Example**

```markdown
fix: update packages

Assignees: 
Labels: 



The firebase package has been updated to 7.14.0 and we are behind a major version. This is a breaking change and we need to update our code to use the new version.
```

Assignees and Labels can be left blank. These will be filled out during triage.

When complete, hit the check button at the top right. This will create the issue. 

Finally, to quickly assign this issue to yourself AND checkout a new branch, click the arrow next to the newly created issue (you may need to refresh the issues first)

![image](https://user-images.githubusercontent.com/72859335/210774916-a848ff98-9bcf-4fc4-9f96-7b567dc48b64.png)


Note: Include any supporting documents such as Figma links, code, etc.
