
## Moving from sandbox to production;

- [ ] change app id in appengine-web.xml ;
- [ ] change app id in pom.xml ;
- [ ] change WEB_CLIENT_ID in net.cryptonomica.constants.Constants;
- [ ] make changes to header on index.html (i.e.: Cryptonomica Key Server // Pre-alpha (v. 0.01));
- [ ] make changes to alert on home.html;

(log in from GoogleApps administrator to add users form GoogleApps)
- [ ] put API keys in DS: 1) AppSettings.class, "SendGridApiKey";
- [ ] check: Cloud Storage bucket name, in sandbox:  "cryptonomica-test.appspot.com" );


- [ ] app.js : $sceDelegateProvider.resourceUrlWhitelist - change
- [ ] app.js :  var CLIENT = '602780521094-jim3gi59m9d2clhsi2kvuvad59c9m57l.apps.googleusercontent.com'; -> to production
                var BASE = 'https://cryptonomica-test.appspot.com/_ah/api'; -> to production
                $rootScope.gaeProjectDomain = "cryptonomica-test.appspot.com"; -> to production
- [ ] dashboard.html : replace test payment buttons for real payment buttons

## for first run on new GAE project:

- [ ] add custom domains
- [ ] add SSL Certificates
- [ ] add Permissions - for other developers, and webmaster account
- [ ] APIs & auth > Credentials > Add Credentials > OAuth 2.0 Client ID > Configure consent screen.
- [ ] APIs & auth > Credentials > Add Credentials > OAuth 2.0 Client ID > Web application
- [ ] add email(s) of in "Email API authorized senders" in:
                    GAE -> Settings -> Application Settings
- [ ] create first user with 'Cryptonomica officer' rights
- [ ] set up Google Cloud Storage

## additional

- [ ] set up git repo on GAE
