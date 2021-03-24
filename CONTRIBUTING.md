# Contributing to The Best Package

If you're reading this, you're awesome! Thank you for helping us make this project great and being a part of the community. Here are a few guidelines that will help you along the way.

## Code of Conduct

The Best Package has adopted the [Contributor Covenant](https://www.contributor-covenant.org/) as its Code of Conduct, and we expect project participants to adhere to it.
Please read [the full text](/CODE_OF_CONDUCT.md) so that you can understand what actions will and will not be tolerated.

## A large spectrum of contributions

There are many ways to contribute to the project, code contribution is one aspect of it. For instance, documentation improvements are as important as code changes.

## Your first Pull Request

Working on your first Pull Request? You can learn how from this free video series:

[How to Contribute to an Open Source Project on GitHub](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)

If you decide to fix an issue, please be sure to check the comment thread in case somebody is already working on a fix. If nobody is working on it at the moment, please leave a comment stating that you have started to work on it so other people don't accidentally duplicate your effort.

If somebody claims an issue but doesn't follow up for more than a week, it's fine to take it over but you should still leave a comment.
If there has been no activity on the issue for 7 to 14 days, it is safe to assume that nobody is working on it.

## Sending a Pull Request

This is a community project, so Pull Requests are always welcome, but, before working on a large change, it is best to open an issue first to discuss it with the maintainers.

When in doubt, keep your Pull Requests small. To give a Pull Request the best chance of getting accepted, don't bundle more than one feature or bug fix per Pull Request. It's often best to create two smaller Pull Requests than one big one.

1. Fork the repository.

2. Clone the fork to your local machine and add upstream remote:

```sh
git clone https://github.com/<your username>/the-best-package.git
cd the-best-package
git remote add upstream https://github.com/igoradamenko/the-best-package.git
```

3. Synchronize your local `next` branch with the upstream one:

```sh
git checkout next
git pull upstream next
```

4. Install the dependencies with yarn or npm:

```sh
npm install
```

5. Create a new topic branch:

```sh
git checkout -b my-topic-branch
```

6. Make changes, commit and push to your fork:

```sh
git push -u origin HEAD
```

7. Go to [the repository](https://github.com/igoradamenko/the-best-package) and make a Pull Request.

The core team is monitoring for Pull Requests. We will review your Pull Request and either merge it, request changes to it, or close it with an explanation.

### How to increase the chance of being accepted?

CI runs a series of checks automatically when a Pull Request is opened. 

Make sure the following is true:

- The branch is targeted at `master`. We do our best to keep `master` in good shape, with all tests passing. 
- If a feature is being added:
  - If the result was already achievable with the core library, explain why this feature needs to be added to the core.
  - If this is a common use case, consider adding an example to the documentation.
- When adding new features or modifying existing, please include tests to confirm the new behavior. 
- If new features were added or old ones were changed, the TypeScript declarations were updated.
- The branch is not behind its target.

If you have missed a step, don't worry, the Continuous Integration will run a thorough test on your commits and the maintainers of the project can assist.

### Coding style

Please follow the coding style of the project. Project uses ESLint, so if possible, enable linting in your editor to get real-time feedback.

`npm run lint` lints and reformats the code.

Finally, when you submit a Pull Request, they are run again by our continuous integration tools, but hopefully, your code is already clean!

## License

By contributing your code to the igoradamenko/the-best-package GitHub repository, you agree to license your contribution under the MIT license.
