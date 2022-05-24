# Heroku dynos restarter

An app for booting the dinos of a heavy roaming app on Al Harco, in case it crashes. Created for https://madrichim.ovh .

# Config example

In `config.env` file in root directory.
```
TOKEN_API_HEROKU=fc0d678d-6b63-4b93-b7bc-19e5fbe8e3r9 # token heroku
 APP_NAME = madrichim # The app name in Heroku 
 SITE_URL = https: //madrichim.ovh # The address where the monitored app is available (if there is only a free heroku domain you can leave blank)```

# Deploy in heroku
The button must be pressed👇👇And fill the config..
<div  align='right'>

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

</div>

## Automatic "sleep" prevention
In heroku's free program, the server shuts down after 30 minutes without any external request to the server. This can be circumvented by verifying credit in the Harco account , thus getting a total of 1000 free hours per month, which is enough for continuous application of the app. Then a "dummy request" should be sent to the app every less than 30 minutes. This can be easily done through one of the following sites :

https://kaffeine.herokuapp.com
https://www.downnotifier.com

## Create a fixed token:
First of all, install the heroku cli ([ for Windows 64-bit](https://cli-assets.heroku.com/heroku-x64.exe))

Then login to heroku account:

heroku login
And token creation:

heroku authorizations:create

## Places of sight
* https://devcenter.heroku.com/articles/platform-api-reference#dyno-restart-all

* https://devcenter.heroku.com/articles/platform-api-quickstart#authentication
