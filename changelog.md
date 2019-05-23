## 3.8.0
- Added forEach and storeJson commands
- Made it so explicit wait commands (e.g., `wait for element visible`, etc.) override the built-in implicit wait mechanism
- Fixed a bug in how the runner fetches dependencies, so it only happens when features that need external dependencies are used
- Added the ability for plugins to create variables
- Changed the code export UI to prompt the user for a download location

## 3.7.4
- Fix for the runner to resolve a bug with fetching dependencies
- Fix for getting text from the page not getting white-space trimmed
- Updated the "What's New" link in the project header to open the latest IDE release page in GitHub

## 3.7.3
- Fix for the runner to resolve a dependency issue with the junit report formatter

## 3.7.2
- Fix for a bug that prevented plugins that exported code from registering with the IDE

## 3.7.1
- `selenium-side-runner` won't load multiple versions of selenium-webdriver into memory
- Fixed `store` context menu items 
- Removed `--configuration-file` flag, please use `--config` or `--config-file` instead
- Merged PR introducing the junit report formatter to the runner

## 3.7.0
- Improved plugin support for code export
- Support for recursive reused test methods in code export

## 3.6.0
- Code export for Java JUnit

## 3.5.8
- Improved recording indicator UI
- Improved recording of mouse over locators
- Enable saving projects with invalid file system characters
- Enable plugins to delete commands
- Fix for plugins to work with a suite of tests running in parallel in the runner

## 3.5.7
- Fixed performance issue during recording that would cause the browser window to become unresponsive.

## 3.5.6
- Added indication when selecting an element.  
- Added a new xpath locator strategy.  
- Base URL will resolve relatively if the target URL doesn't start with a `/`.  
- Fixed an issue where send keys ${KEY_ENTER} may not always work.  

## 3.2.0
### SIDE Runner
Can now run project files [headlessly in command line](https://www.npmjs.com/package/selenium-side-runner)
### `run` command
Use the `run` command to call tests from within tests.
### `link` locator
`link` is deprecated in favor of `linkText` and `partialLinkText`, more info [here](https://github.com/SeleniumHQ/selenium-ide/releases/tag/v3.2.0).
### Control Flow commands
You can now use conditional logic in your tests with commands `if`, `else if`, `else`, `end`, `while`, `times`, `do`, and `repeat if`.
### `assert` and `verify` commands
Use the `assert` and `verify` commands to check the value of a variable against an expected value.
### Fixes
Fixed a bug in `executeScript` and `executeAsyncScript` that caused the command to hang when a variable name wasn't provided.

## 3.1.0
### Extensions
Selenium IDE supports extensions now, more info [here](https://github.com/SeleniumHQ/selenium-ide/wiki/Getting-Started-with-Plugins)
### Reference
A new reference tab added, gives helpful information about commands, check it out (next to the logs).