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
* On Phantom JS `npm run test:phantomjs`

If your tests fail you can watch screens after each fail in `/test/e2e-screens/`

#### PhantomJS browser

Some websites serve different content for different browser or different page size (for example http://www.google.com).
For default PhantomJS use own userAgent string and same browser window is small (644x444). To solve this we change 
userAgent for PhantomJS in `nithwatch.json` to 

`Mozilla/5.0 (Windows NT 6.3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2490.80 Safari/537.36`

this simulate `Windows Chrome 46`

To read more see: https://github.com/nightwatchjs/nightwatch/issues/243#issuecomment-155199713
