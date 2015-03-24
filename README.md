Testing is essential when upgrading the wiki software or installing a new wiki.
These are Selenium Tests for Biowikifarm Wikis. 
Selenium is a testing framework which can simulate a user interacting with the wiki through a browser.
Selenium test cases are gouped in test suites. Test suites can be executed in Firefox, using the Selenium-IDE Plugin. 
Selenium stores it's test files as html. 

## What is covered
As all wikis on Biowikifarm share common settings, this tests attempt to cover as much as possible of the shared settings.
Special settings for individual wikis should be covered in their own test suites.

## Running the tests
To run the tests, please do:

### Make a test user
To test the wiki, you will need a test user. 
1. Create a test user with regular permissions (not an administrator).
2. Open the user's settings and switch off e-mail notifications
3. Switch the test user's language to English
4. In the user's settings "Editing" section, make sure the source editor is used, not the wysiwyg editor

### Install Selenium
1. Install the Selenium-IDE Plugin for Firefox (http://docs.seleniumhq.org/).
4. Verify that "Selenium IDE" is in the Firefox "Tools" menu (or "Extras" depending on your locale)

### Running the test
1. Login to the wiki you want to test, using the test account you created before.
2. Set the Base URL in Selenium to the base URL of your wiki, e.g. http://biowikifarm.net/v-mfn/wiki/ (trailing slash in needed)
3. In Selenium, open the "Integrationtests" Test Suite (File->Open Test Suite) and klick on "Play".
