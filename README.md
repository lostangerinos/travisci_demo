# Angular Unit Tests and e2e Tests

This is the default Angular Project. It is used here to test setup for continuous integration (CI) using Travis CI so that test cases can be automated without the need for anyone to manually run them. See: https://travis-ci.com/
  
Tests automated are: Unit Tests included in the default package(.spec.ts) and e2e (end to end) tests (.e2e-spec.ts). 

Manually run the unit tests and e2e tests: 

To setup: 

- First, clone or download this repository onto your computer
- Go on your favorite editor (like Visual Studio Code) and open the root folder of the project
- run the command: npm install
- run command: webdriver-manager update

How to run Unit tests:

- run the command: npm test or ng test

![unit tests]https://github.com/lostangerinos/travisci_demo/blob/master/documentation/unit_tests.png

How to run E2E tests :

With webdriver(visual support): 
- run: npm start
- run: protractor (path to (project root)/src/e2e/files/protractor.conf.js). Note: You may have to open a new window of your editor to do this as you need to leave the application running through the previous command. For example, if you open the folder e2e under (project root)/src/e2e, you run the command: protractor files/protractor.conf.js
- You will see a window open, and this window will navigate to localhost:4200, where the application is hosted and will run the tests directly against the compiled application. 
- the e2e tests written so far are in the file: (project root)/src/e2e/files/src/ang-spec.e2e-spec.ts

![e2e manual]https://github.com/lostangerinos/travisci_demo/blob/master/documentation/e2e_manual.png

No webdriver: 
- run the command: npm run e2e 

![e2e auto](https://github.com/lostangerinos/travisci_demo/blob/master/documentation/e2e_auto.png)

How to Trigger Travis test builds (Automatic builds):

(Note: you need Git or GitHub Desktop installed on your computer commit)
- Commit something (this is the equivalent of a check-in in TFS), anything to this repository and Travis will run the unit tests and the e2e tests automatically
- Go to: https://travis-ci.org/dashboard to monitor the progress of the tests (Log in using this GitHub account) 


