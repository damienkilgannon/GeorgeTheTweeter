# GeorgeTheTweeter

> A Simple, Controllable, Configurable Twitter Bot


[![Build Status](http://img.shields.io/travis/badges/badgerbadgerbadger.svg?style=flat-square)](https://travis-ci.org/badges/badgerbadgerbadger) [![Coverage Status](http://img.shields.io/coveralls/badges/badgerbadgerbadger.svg?style=flat-square)](https://coveralls.io/r/badges/badgerbadgerbadger) [![Github Issues](http://githubbadges.herokuapp.com/badges/badgerbadgerbadger/issues.svg?style=flat-square)](https://github.com/badges/badgerbadgerbadger/issues) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

---

## Table of Contents (Optional)

> If your `README` has a lot of info, section headers might be nice.

- [Clone](#clone)
- [Run Locally](#run locally)
- [Deploying to Heroku](#deploying to heroku)
- [License](#license)

---

### Clone

- Clone this repo to your local machine using `git@github.com:damienkilgannon/GeorgeTheTweeter.git`

### Run Locally


> update and install this package first

```
$ pip install -r requirements.txt
$ export KEY="my API key"
$ export SECRET="my API secret"
$ export TOKEN="my API token"
$ export TOKEN_SECRET="my API token secret"
$ python app.py
```

> change target keywords and actions by setting the following env

```
$ export HASHTAG="your target keyword/hashtag"
$ export LIKE="set to true if you want to like tweets found"
$ export RETWEET="set to true if you want to retweet tweets found"
$ export COMMENT="set to true if you want to comment tweets found"
$ export MSG="set this to the text that you wish to use when replying to a tweet (only used if COMMENT=true)"
```

> change throttle and duration of the stream listener by setting the following env

```
$ export THROTTLE="set this to the time in secs between each run of the stream listener"
$ export THROTTLE="set this to the time in secs of lenght of each run"
```

---

## Deploying to Heroku

```
$ heroku login
$ heroku create
$ git push heroku master
$ heroku ps:scale web=1
```

> to set the config vars on Heroku

e.g.
```
$ heroku config:set KEY="my API key
```

---

## License

- **[GNU GPL license](https://www.gnu.org/licenses/gpl-3.0.en.html)**
