# Klaxon (for the Star Tribune)

Klaxon watches webpages and sends notifications when they change.  See the README.md for much more detail.

This README is maintained separately for Star Tribune specific use documentation.

## Customizations

Overall, we don't want to customize the code on this without a matching pull request, otherwise updating can be a problem.

(currently no customizations)

## Setup

The following will install the tools necessary to work on and deploy this Klaxon instance:

1. Install [Heroku command line tools](https://devcenter.heroku.com/articles/heroku-cli)
    * On a Mac: 'brew install heroku'
1. Make sure you are logged into the command line tools: `heroku login`
1. Get this code: `git clone https://github.com/striblab/klaxon-strib.git && cd klaxon-strib`
1. Add link to original Klaxon in order to do updates: `git remote add upstream https://github.com/themarshallproject/klaxon.git`
1. Add connection to Heroku: `heroku git:remote -a klaxon-strib`

## Updates

Updates from the original Klaxon repo can be done with the following.

1. `git pull upstream master`

## Deploy

To deploy with new updates, just push to Heroku:

1. `git push heroku master`
