Node.js wrapper for the Google Contacts API.

# install

    npm install google-contacts-api

# usage

```javascript
var GoogleContacts = require('google-contacts-api');
var contacts = new GoogleContacts({ token : req.token });
contacts.getContacts(function(err, contacts) {
    // ...
});
```
# Refresh Your Token

```javascript
var GoogleContacts = require('google-contacts-api');
var contacts = new GoogleContacts();
contacts.refreshAccessToken(req.refreshToken , function(err, function(err,newToken)) {
    // ...
});
```

# test 

To test this module, `$GOOGLE_API_TOKEN` must be set.

```
$ export GOOGLE_API_TOKEN="ya29.WDVMYoReyJOKac3AFWMDg6lfMv8jyilWpjtQBqL99IKuiWTInpEqZFDi"
$ npm test
```
