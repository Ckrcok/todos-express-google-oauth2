# express-4.x-google-oauth2-example

This example illustrates how to use [Express](https://expressjs.com) 4.x and
[Passport](https://www.passportjs.org) to sign in users with [Google](https://www.google.com).
Use this example as a starting point for your own web applications.

## Quick Start

To get started with this example, clone the repository and install the
dependencies.

```bash
$ git clone git@github.com:passport/express-4.x-google-oauth2-example.git
$ cd express-4.x-google-oauth2-example
$ npm install
```

This example requires credentials from Google, which can be obtained by [setting
up](https://developers.google.com/identity/protocols/oauth2/openid-connect#appsetup)
a project in [Google APIs console](https://console.developers.google.com/apis/).
The redirect URI for the OAuth client should be set to: `http://localhost:3000/oauth2/redirect/accounts.google.com`

Once credentials have been obtained, create a `.env` file and add the following
environment variables:

```
GOOGLE_CLIENT_ID={{INSERT_CLIENT_ID_HERE}}
GOOGLE_CLIENT_SECRET={{INSERT_CLIENT_SECRET_HERE}}
```

Start the server.

```bash
$ npm start
```

Navigate to [`http://localhost:3000`](http://localhost:3000).

## Overview

This example illustrates how to use [Passport](https://www.passportjs.org) and
the [`passport-google-oauth20`](https://github.com/jaredhanson/passport-google-oauth2)
strategy within an [Express](https://expressjs.com) application to sign users in
with [Google](https://www.google.com).

This example builds upon the scaffolding created by [Express generator](https://expressjs.com/en/starter/generator.html),
and uses [EJS](https://ejs.co) as a view engine and plain CSS for styling.  This
scaffolding was generated by executing:

```
$ express --view ejs express-4.x-google-oauth2-example
```

Added to the scaffolding are two files which add authentication to the application.

#### boot/auth.js


#### routes/auth.js




## License

[The Unlicense](https://opensource.org/licenses/unlicense)
