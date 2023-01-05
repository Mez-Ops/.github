Welcome to the Mez Ops GitHub page! 👋

We are a small team of 1 developer and 1 UI/UX designer.

This readme is focused on the developer and contains all of our best practices when it comes to developing application for Mez Ops.


## Development 10 Commandments

1. **ALL** coding work starts with a [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues). This allows us to track all work from ideation to release
2. **ALL** GitHub issue titles shall follow standard [semantic versioning](https://www.conventionalcommits.org/en/v1.0.0/) guidelines
3. 100% unit test coverage for applications. Nothing less
4. The required IDE is [VS Code](https://code.visualstudio.com/)
5. Branches shall be named with {user}/{issueTitleCleaned} (i.e., tyler-jewell/fix-a-bug)


## Development Process

1. A [GitHub issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) is created to track work. This can be an idea, feature request, bug, etc.
2. Issue admin investigates and approves the issue to be worked on by the team
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

### Creating issues


