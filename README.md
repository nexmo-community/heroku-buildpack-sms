# Heroku Buildpack - SMS

Use this Heroku Buildpack to purchase a new phone number and set up a callback URL to handle inbound SMS

## Usage

This buildpack is designed to be used in conjunction with an `app.json` manifest.

The applicaiton will require 3 Environment Varibles to be setup (usually done in app.json)

`API_KEY` - Your Nexmo API Key
`API_SECRET` - Your Nexmo API Secret
`CC` The ISO-3361-2 Country code where you want a number to be purchased

See the example `app.json` included in this repo to use as a base

> Note that if you are including this buildpack then you need to also specify the buildpack which will run your code in the appropriate language as this will overide herokus default detection, in the example `app.json` this is set to `heroku/python`

https://devcenter.heroku.com/articles/buildpacks#officially-supported-buildpacks
