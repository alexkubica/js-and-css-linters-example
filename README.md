# Javascript And CSS Linters Example

## Motivation
Automation and standards are key when working in a team. We want to automate syntax checks and autofix small issues as soon as possible to avoid wasting time on it while coding or doing code reviews.  

## How To Play Around
* Clone the project
* `npm install` dependencies.
* See `lint:*` scripts in `package.json`.
* Fiddle with the code and try commiting.

## Tools Used
* [create-react-app](https://github.com/facebook/create-react-app) for creating react app
* [StandardJS](https://standardjs.com/) for preconfigured eslinting
* [stylelint](https://stylelint.io/) and stylelint-config-standard for css linting
* [husky](https://github.com/typicode/husky) for linting in the pre-commit git hook
* [lint-staged](https://github.com/okonet/lint-staged) for linting only staged files and automatically adding fixes to the commit
* [VSCode StandardJS extension](https://marketplace.visualstudio.com/items?itemName=chenxsan.vscode-standardjs) for displaying linting errors in the editor

## Useful Resources

These are some links I used which helped me setup this project:

* [Gist showing how to add standardjs to your create-react-app app](https://gist.github.com/dreamorosi/6fd4048beb16a00a553fb8a7b9362caf)
* [Medium post on adding linting to git hooks](https://medium.com/gits-apps-insight/utilizing-git-hook-by-using-eslint-husky-and-lint-staged-18b6f6f60f1e)
* [Another linting setup for CI, includes stylelint too](https://codeburst.io/continuous-integration-lint-staged-husky-pre-commit-hook-test-setup-47f8172924fc)
* [Git hooks docs](https://git-scm.com/docs/githooks)
* [StandardJS docs](https://standardjs.com/)
* [ESLint docs](https://eslint.org/)

## Alternatives

Before I settled with the tools listed above I looked for some alternatives I think are worth mentioning:
* [JSLint](https://jslint.com/).
* [JSHint](https://jshint.com/).

While these tools are still used today and by big companies I preffered to stick to the more modern alternative that has a bigger community.  
The reason I chose StandardJS over ESLint is because it has preconfigured rules and I always can eject it to ESLint config. Also, it's worth to mention that StandardJS surprisingly has more github stars (24.2k compared to ESLint's 17k).