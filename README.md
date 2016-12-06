# Install

1. Install Java if you don't have `sudo apt-get install default-jre`
* `npm install`
* `npm install -g nightwatch`
* `npm install -g selenium-standalone@latest`
* `selenium-standalone install`

# Run integration (end-to-end) test

First you must run selenium server:

`npm run selenium`

After server start you can run tests:

* On Chrome `npm run test:chrome`
* On Firefox `npm run test:firefox`

If your tests fail you can watch screens after each fail in `/test/e2e-screens/`
