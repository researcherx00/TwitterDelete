# TwitterDelete

TwitterDelete is a small application to delete your old, unpopular tweets and likes.

## Features

- Delete, unlike and unretweet tweets
- Keep tweets based on age and tweaks based on retweet or favourite count
- Delete tweets no longer exposed by Twitter API from a downloaded Twitter archive file

## Usage 

To setup locally run:

```bash
git clone https://github.com/mikemcquaid/TwitterDelete
cd TwitterDelete
bundle install
```

Get the Twitter API variables from https://apps.twitter.com and add the following variables to a `.env` file in the `TwitterDelete` folder:

```bash
TWITTER_CONSUMER_KEY=...
TWITTER_CONSUMER_SECRET=...
TWITTER_ACCESS_TOKEN=...
TWITTER_ACCESS_TOKEN_SECRET=...
```

Now run TwitterDelete:

```bash
./twitter_delete.rb --user TwitterUsername
```

If you fork this PR you can also used the [GitHub Actions scheduled workflow](https://github.com/MikeMcQuaid/TwitterDelete/blob/master/.github/workflows/scheduled.yml) combined with secrets on your fork to run this automatically.

## Status

Works for deleting relevant tweet and likes. I delete my old tweets and am not actively working on improving this but I will accept pull requests.

## Contact

[Mike McQuaid](mailto:mike@mikemcquaid.com)

## License

TwitterDelete is licensed under the [AGPLv3 License](https://en.wikipedia.org/wiki/Affero_General_Public_License).
The full license text is available in [LICENSE.txt](https://github.com/mikemcquaid/TwitterDelete/blob/master/LICENSE.txt).
