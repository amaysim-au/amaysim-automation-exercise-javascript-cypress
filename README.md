# Amaysim Test Automation Exercise - Javascript/Cypress

Base Test framework for a test automation exercise. This version is built with cypress, using the javascript programming language.

## Important files/folders in this test tramework

### Tests
1. All tests are in the folder `cypress/e2e`. The test files have the name suffix `.spec.cy.js`.
1. There's currently one test `mobile_autorenewal.spec.cy.js`. This test does the below:
   1. Visit the amaysim home page, login as an existing customer and view the dashboad page. The username and password are read from the `cypress/fixtures/tesData.json` file.
   1. From the dashboard page, go to the mobile settings page.
   1. On the Mobile Settings page, verify that `AutoRenewal` for this mobile service is turned off.
1. The tests use the Page Object Model. The page classes are in `cypress/e2e/pageObjects`.
1. This Cypress framework works best in `Chrome`. You will likely run into 

### Cypress Configuration
1. These are in the file `cypress.config.js`. Among other things, it contains the base URL.

### Test Data
1. These are under the folder `cypress/fixtures`.

### Page Classes/Objects
1. These are in the folder `cypress/e2e/pageObjects`

## How to execute tests

### Install the git client
Install `git`. Please google for installation instructions. If you already have this installed, you dont need to do it again.

### Install Node and Npm
Install `node` and `npm` on your machine. Please google for installation instructions. If you already have this installed, you dont need to do it again.

### Create a fork for yourself and checkout the code
1. On your browser, login to github.com.
1. Navigate to this code repository.
1. Fork this repository. as below:
![Fork](/readme-assets/fork.png)
![New Fork](/readme-assets/new_fork.png)
If you need it, here are the [intructions] (https://docs.github.com/en/get-started/quickstart/fork-a-repo) on Github for how to crate a fork.

Note: **Please make all your changes on this fork, and NOT on the original repo.**

1. Once you've created a fork, checkout the code, by running this in your terminal/command line: `git clone git@github.com:<your github username>/amaysim-automation-exercise-javascript-cypress.git`

### Install dependancies
1. Go to your folder where you checked out the code: `cd amaysim-automation-exercise-javascript-cypress`
1. Run `npm install` on your terminal/command line.

### Run tests
In your commandline/terminal, from inside the `amaysim-automation-exercise-javascript-cypress` folder, run the command `npx cypress run --browser chrome --headed`.

(You can also run `npx cypress open` to open the Cypress runner window. This might be useful while developing the test.)

## How to submit your code

**Please make all your changes on your fork, and NOT on the original repo.**

### Push your changes into your forked repo
1. In your command line/terminal, run `git status` to see all local changes.
2. Once you are happy with the changes, run `git add .` to stage all your local changes.
3. Run `git commit -m "<a commit message of your choice>"` to commit your changes.
4. Run `git push` to push your changes to your forked repository.

*ps: Feel free to use whatever steps you're familiar with to commit/push. You do not have to follow the exact same steps above. Some candidates feel more comfortable using GUI-based tools.*

### Send us a link to this fork
After you're done with your changes, send us a link to your repo.