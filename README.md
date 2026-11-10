# Instructions and Notes

## In this session
1.   Install playwright
- `npm init playwright@latest`
2. check if installed properly
- `npx playwright --help`

## In this session

1. Run the test -> `npx playwright test --headed`
2. Show the Report -> `npx playwright show--report`

**windows**
- For running webkit in windows, add these in `use` object
```ts
use: {
    ignoreHTTPSErrors: true,
},
```
** Recommended VS Code Extensions**
- vscode-icons
- prettier - code formatter
- path Intellisense
- npm Intellisense
- DotENV
- JavaScript (ES6) code snippets
- .gitignore generator

**Git Installation for windows/macOS**
1. Check version -> `git --version`
2. Check once installed using the same command

**Setup Git Repo**
1. Git commands
    - `git init`
    - `git status`
    - `git add`
    - `git commit -m  "<commit-message>"`

2. git ignore the following files
    - /debug
    - logs/
    - .env
    - allure-results
    - tests-examples/
    - examples.*
    - *.log

**Push changes to Remote**
1. Git commands
    -`git branch -M main`
    -`git remote add origin<remote url>`
    -`git remote -v`
    -`git push -u origin main`

2. Issues
    -`git config --list
    -`git push -f origin main -> force push
3.Remember this - `ACP` - `Add commit push`

**Writing First Test**
1. Target web app: `https://katalon-demo-cura.herokuapp.com/`
2. Stpes
    1. Go to the home page
    2. Assert if the title is correct
    3. Assert header text
3. Done!

**Common Errors**
1. Spec/test file not having `.spec or .test` .init
2. Navigation timeout error


```ts
use: {
    navigationTimeout: 30_000,  //Set timeout to 30 seconds
},
```
3. Missing `await` keyword before action methods
4. Done!

**Option 1 - Install VS Code Extension**
1. VS Code Extension -> `Playwright Test for VSCode`

**Option 2 -CLI**
-Help -> `npx playwright codegen --help`
-CLI basic command - `npx playwright codegen`
-with URL `npx playwright codegen https://Katalon-demo-cura.herokuapp.com/`

**Codegen Demo**
- URL -> `https://Katalon-demo-cura.herokuapp.com/`


**Deep Dive into playwright Locators**
- [] `page.getBy*()` and `page.locator()` methods returns the `locator` object
- [] The above methods not to be `awaited`
- [] The type of locator is an `object`
- [] Locators are LAZY until an action is fired on them

**Interacting with Web Elements**
- codegen CLI: `npx playwright codegen https://Katalon-demo-cura.herokuapp.com/`



