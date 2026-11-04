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
    
