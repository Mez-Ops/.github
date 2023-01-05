# Mez Ops Development Homepage

Welcome to the Mez Ops GitHub page! 👋 We are a small team of 1 developer and 1 UI/UX designer striving to develop the best looking and performing apps using Flutter and Firebase for backend and modern UI/UX design practices.

Lead developer: [Tyler Jewell](https://github.com/tyler-jewell)

Lead UI/UX designer: Barbara Jewell

This readme covers our best practices for developing applications for Mez Ops.

# Development Commandments

1. All coding work begins with a GitHub issue to track progress from idea to release. 🚀
2. GitHub issue titles follow [semantic versioning](https://www.conventionalcommits.org/en/v1.0.0/) guidelines 📜
3. All applications must have 100% unit test coverage. 💯
4. The required IDE is VS Code. 💻
5. Branches are named with {user}/{issueTitleCleaned} (e.g., tyler-jewell/fix-a-bug). 🌱
6. Pull request titles must match the issue title they are linked to. 💬

# Development and Deployment Process

1. [Create a GitHub issue](#creating-issues) 📝
2. [Assign the issue to yourself](#assigning-an-issue-to-yourself) and create a branch off main 📅
3. Make commit(s) to the issue branch 💻
4. Create a pull request to merge the issue branch into main 📥
5. Run linting, unit tests, and semantic versioning checks to ensure code quality  🧪
6. Squash the pull request into a single commit (the issue title) and merge it into main  🛠️
7. Bump version files to the next semantic version 📈
8. Update the changelog to document the work done in the latest version  📝
9. Create and push a tag to the repository 🏷️
10. Create a release from the new tag 🚀
11. Build artifacts (apk, .ipa, etc.) 📦
12. Publish the app to the appropriate repository or store (pub.dev, Apple Store, Google Play Store, Firebase Hosting, etc.)🌍

![image](https://user-images.githubusercontent.com/72859335/210781207-682a5418-7a12-4344-b00b-bbe8240f377f.png)


## Assigning an issue to yourself

### Using VS Code with the [GitHub Pull Request](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) extension (preferred)

Find the issue in the left panel and select the forward arrow. This will automatically create a local branch and assign you to the issue.

![image](https://user-images.githubusercontent.com/72859335/210772109-d3f846d4-f3b5-40a0-8230-b33ccd7fe5ae.png)


### Using the GitHub console

1. Open the issue and add your name to the assignees. 
2. Manually create a local branch named {user}/{issue title}.

![image](https://user-images.githubusercontent.com/72859335/210772399-1da72059-1e45-4f1c-b660-af0b525bd487.png)


## Creating issues

To create a new issue on GitHub, follow these steps:

1. Navigate to the GitHub extension in VS Code.
2. Click the '+' icon to the right of the issues panel.
3. Fill out the markdown template with the details of the issue. The issue title should follow semantic versioning standards.
4. Assignees and Labels can be left blank. These will be filled out during triage.
5. Hit the check button at the top right to create the issue.
6. To assign the issue to yourself and create a new branch, click the arrow next to the newly created issue (refresh the issues list if necessary).

Include any supporting documents such as Figma links, code, etc. with the issue.

**Example**

```markdown
fix: update packages

Assignees: 
Labels: 



The firebase package has been updated to 7.14.0 and we are behind a major version. This is a breaking change and we need to update our code to use the new version.
```

Note: Automatic pull request titles, automatic changelog updates, and automatic closure of the issue when the PR is merged with the linked issue will be handled by downstream automation processes.

![image](https://user-images.githubusercontent.com/72859335/210774916-a848ff98-9bcf-4fc4-9f96-7b567dc48b64.png)
