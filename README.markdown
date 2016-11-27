everywordbot-dokku
-------------

Implementation of [everywordbot](http:///aparrish/everywordbot) for Dokku.

### Using
Mount the /data volume with a folder containing your 'words.txt' (containing a list of words to be tweeted) and 'index.txt' (to track how far through the wordlist the bot is).

Set the following environment variables for your Twitter credentials:
(see [aparrish's guide](https://github.com/aparrish/everywordbot) for obtaining Twitter credentials.

    CONSUMER_KEY
    CONSUMER_SECRET
    ACCESS_TOKEN
    TOKEN_SECRET

and set at least one of:

    PREFIX
    SUFFIX

Set up a cronjob to run `dokku --rm run YOURAPP console` on desired frequency.
