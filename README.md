# Angular Unit Tests and e2e Tests

This is the default Angular Project. It is used here to test setup for continuous integration (CI) using Travis CI so that test cases can be automated without the need for anyone to manually run them. See: https://travis-ci.com/
  
Tests to automate are: Unit Tests included in the default package(.spec.ts) and e2e (end to end) tests (.e2e-spec.ts). 

How to run Unit tests:

- npm test or ng test

How to run E2E tests :

- npm run e2e (no webdriver)
- protractor (path to protractor.conf.ts) after launching application with npm start 

How to Trigger Travis builds:

- Commit something, anything to this repository and Travis will run the unit tests and the e2e tests automatically
- Go to: https://travis-ci.org/dashboard to monitor the progress of the tests 


