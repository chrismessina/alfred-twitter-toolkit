# Twitter Toolkit for Alfred

<img src="./assets/icon-twitter.png" alt="Twitter logo" width="128" height="128">

The Twitter Toolkit for Alfred lets you quickly interact with Twitter through its website, [Mac app](https://apps.apple.com/us/app/twitter/id1482454543?mt=12&uo=4), and [Tweetbot](https://tapbots.com/tweetbot/mac/).

It makes it easy to quickly search and find your own content or the content of people you follow (shown using my <a href="https://github.com/chrismessina/alfred-theme-chirp">Chirp Theme</a>):

<img src="./assets/preview.gif" alt="Preview of Twitter Toolkit">

This workflow doesn't support programmatic access to Twitter, like tweeting directly or sending DMs. For that kind of integration, try [AlfredTweet](http://dferg.us/alfredtweet-2/) by David Ferguson.


# Installation

<a href="https://github.com/chrismessina/alfred-twitter-toolkit/releases/latest"><img src="./assets/icon-workflow.png" alt="Workflow File Icon" width="128" height="128"></a>

1. Download [latest release here](https://github.com/chrismessina/alfred-twitter-toolkit/releases/latest).
2. Double-click the `.alfredworkflow` to install it.

_You will need to be an [Alfred Powerpack](https://www.alfredapp.com/powerpack/) user to enable this workflow._


# Configuration

Once the workflow is installed, launch **Alfred Preferences**, choose **Workflows** and then select **Twitter Toolkit**.

<span style="color:red;">➊</span> Access the **Workflow Environment Variables** in the top right of the window:

<img src="./assets/workflow-config.png" alt="How to access the Alfred Workflow Environment Variables">


## Set your username and user ID

This workflow makes it easy to search your own tweets or find content from the people you follow ("followees").

<span style="color:red;">➋</span> To configure this feature, you must set the `account` variable in the configuration to *your own username*.

<span style="color:red;">➍</span> Set the `userId` variable to your own user ID. You can find this number if you navigate to a Twitter.com message thread and look at the number after `messages/` and to the left of the hyphen in the URL.

## Platform selection

This workflow supports interacting with Twitter on the web, Twitter for Mac, or Tweetbot. If a keyword is not supported by a certain platform, it will fallback to the web.

<span style="color:red;">➌</span> Set the `platform` variable to <img src="./assets/icon-twitter-16.png" alt="Twitter Icon" width="16" height="16"> `web`, <img src="./assets/icon-appstore-16.png" alt="App Store Icon" width="16" height="16"> `app` or <img src="./assets/icon-tweetbot-16.png" alt="Tweetbot Icon" width="16" height="16">`tweetbot` .


# Keywords

The following keywords are used to interact with the Twitter Toolkit.

Modifier keys change the behavior as described, and subtext will appear in Alfred to help guide your interaction.

`⌥` is typically used to scope content to your own content.

`⌘` is typically used to scope content from people you follow.

`⇧` is used to toggle the nearby scope.

|   Keyword    	|   Modifier  	|   Description                                             	|   <img src="./assets/icon-twitter-16.png" alt="Twitter Icon" width="16" height="16">  	|   <img src="./assets/icon-appstore-16.png" alt="App Store Icon" width="16" height="16">  	|   <img src="./assets/icon-tweetbot-16.png" alt="Tweetbot Icon" width="16" height="16">  	|
|--------------	|:-----------:	|-----------------------------------------------------------	|:------:	|:------:	|:-----------:	|
|  `!        `  	|             	|   View my Twitter Notifications                           	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `@        `  	|             	|   Go to Twitter user @{query}                             	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `@        `  	|       ⌥     	|   Search Twitter users for @{query}                       	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `#        `  	|             	|   Search Twitter for #{query}                             	|    ☑️   	|    ☑️   	|             	|
|  `#        `  	|             	|   Go to #{query}                                          	|    ☑️   	|        	|             	|
|  `#        `  	|       ⌘     	|   Search my tweets for #{query}                           	|    ☑️   	|        	|             	|
|  `$        `  	|             	|   Search Twitter for ${query}                             	|    ☑️   	|    ☑️   	|      ☑️      	|
|  `access`       |               |   Access accessibility, display and language settings       |    ☑️   	|       	|             	|
|  `account`      |               |   Access your Twitter account settings                      |    ☑️   	|       	|             	|
|  `analytics`  	|             	|   Go to Twitter Analytics                                 	|    ☑️   	|        	|             	|
|  `birdwatch`    |               |   Go to Birdwatch                                           |    ☑️   	|   |   |
|  `bookmarks`  	|             	|   Go to Twitter Bookmarks                                 	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `connect`      |               |   See Who to Follow on Twitter                              |    ☑️   	|   |   |
|  `data`         |               |   Download your Twitter data                                |    ☑️   	|       	|             	|
|  `dm       `  	|             	|   Compose a Twitter message                               	|    ☑️   	|    ☑️   	|             	|
|  `dms      `  	|             	|   Go to Twitter messages                                  	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `download`     |               |   Download your Twitter data                                |    ☑️   	|       	|             	|
|  `embed    `  	|             	|   Embed tweet                                             	|    ☑️   	|        	|             	|
|  `explore  `  	|             	|   See what’s happening                                    	|    ☑️   	|    ☑️   	|             	|
|  `follow   `  	|             	|   Follow @{query} on Twitter                              	|    ☑️   	|        	|       ☑️     	|
|  `help     `  	|             	|   Go to Twitter Help Center                               	|    ☑️   	|        	|             	|
|  `home     `  	|             	|   Go to Twitter Home                                      	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `images   `  	|             	|   Search Twitter images for {query}                       	|    ☑️   	|    ☑️   	|             	|
|  `images   `  	|       ⌥     	|   Search my Twitter images for {query}                    	|    ☑️   	|    ☑️   	|             	|
|  `images   `  	|       ⌘     	|   Search Twitter images from people I follow for {query}  	|    ☑️   	|    ☑️   	|             	|
|  `inbox    `  	|             	|   Go to Twitter messages                                  	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `lists    `  	|             	|   View Suggested Twitter Lists                            	|    ☑️   	|    ☑️   	|             	|
|  `likes    `  	|             	|   View my Twitter Likes                                   	|    ☑️   	|        	|       ☑️     	|
|  `lists    `  	|       ⌥     	|   View my Twitter Lists                                   	|    ☑️   	|        	|       ☑️     	|
|  `lists    `  	|       ⌘     	|   View Twitter Lists You’re On                            	|    ☑️   	|        	|             	|
|  `me       `  	|             	|   View my profile on Twitter                              	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `me       `  	|       ⌥     	|   Copy my Twitter profile link                            	|    ☑️   	|        	|             	|
|  `media    `  	|             	|   Go to Twitter Media Studio                              	|    ☑️   	|        	|             	|
|  `my       `  	|             	|   Search people I follow for {query}                      	|    ☑️   	|    ☑️   	|             	|
|  `messages `  	|             	|   Go to Twitter messages                                  	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `my       `  	|             	|   Search my top tweets for {query}                        	|    ☑️   	|    ☑️   	|             	|
|  `my       `  	|             	|   Search my recent tweets for {query}                     	|    ☑️   	|        	|             	|
|  `my       `  	|             	|   Search my tweets for #{query}                           	|    ☑️   	|    ☑️   	|             	|
|  `my       `  	|             	|   Search my Twitter videos for {query}                    	|    ☑️   	|    ☑️   	|             	|
|  `my       `  	|             	|   View my Twitter Likes                                   	|    ☑️   	|        	|       ☑️     	|
|  `my       `  	|             	|   View my Twitter Media                                   	|    ☑️   	|        	|             	|
|  `my       `  	|             	|   View my Twitter Moments                                 	|    ☑️   	|        	|             	|
|  `my       `  	|             	|   View my Twitter Lists                                   	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `my       `  	|             	|   View my Twitter Bookmarks                               	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `my       `  	|             	|   View my Twitter Notifications                           	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `nearby   `  	|             	|   Search nearby Twitter photos for {query}                	|    ☑️   	|    ☑️   	|             	|
|  `nearby   `  	|             	|   Search nearby Twitter videos for {query}                	|    ☑️   	|    ☑️   	|             	|
|  `nearby   `  	|             	|   Search nearby Twitter people for {query}                	|    ☑️   	|    ☑️   	|             	|
|  `new      `  	|             	|   New Tweet with text {query}                               |    ☑️   	|    ☑️   	|       ☑️     	|
|  `notifs   `  	|             	|   View my Twitter Notifications                           	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `notifs`       |               |   Access your Twitter notification settings                 |    ☑️   	|       	|             	|
|  `photos   `  	|             	|   Search Twitter photos for {query}                       	|    ☑️   	|        	|             	|
|  `photos   `  	|       ⌘     	|   Search Twitter photos from people I follow for {query}  	|    ☑️   	|        	|             	|
|  `photos   `  	|       ⇧     	|   Search nearby Twitter photos for {query}                	|    ☑️   	|        	|             	|
|  `privacy`      |               |   Access your Twitter privacy settings                      |    ☑️   	|       	|             	|
|  `reply    `  	|             	|   Create a link in-reply-to a Tweet                        	|    ☑️   	|        	|             	|
|  `resources`    |               |   Access additional Twitter resources                       |    ☑️   	|       	|             	|
|  `security`     |               |   Access your Twitter security settings                     |    ☑️   	|       	|             	|
|  `social   `  	|             	|   Search top tweets from my extended network for {query}    |    ☑️   	|       	|             	|
|  `settings`     |               |   Access Twitter settings                                   |    ☑️   	|       	|             	|
|  `top      `  	|             	|   Search top tweets for {query}                           	|    ☑️   	|    ☑️  	|             	|
|  `top      `  	|       ⌥     	|   Search top tweets from people I follow for {query}      	|    ☑️   	|    ☑️  	|             	|
|  `top      `  	|             	|   Search top tweets from last week from people I follow for {query}      	|    ☑️   	|    ☑️  	|             	|
|  `topics   `  	|             	|   View my Twitter Topics                                  	|    ☑️   	|    ☑️   	|             	|
|  `topics   `  	|             	|   Go to Topic Picker                                  	|    ☑️   	|        	|             	|
|  `trending `  	|             	|   See what’s happening                                    	|    ☑️   	|    ☑️   	|             	|
|  `trending `  	|       ⌥     	|   See what’s happening for you                            	|    ☑️   	|        	|             	|
|  `trusted  `  	|             	|   Search top tweets from my trusted network for {query}     |    ☑️   	|       	|             	|
|  `tweet    `  	|             	|   Compose new Tweet                                       	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `tweets   `  	|             	|   Search Twitter for {query}                              	|    ☑️   	|    ☑️   	|       ☑️     	|
|  `tweets   `  	|             	|   Search top tweets from people I follow for {query}      	|    ☑️   	|    ☑️   	|             	|
|  `tweets   `  	|             	|   Search recent tweets from people I follow for {query}   	|    ☑️   	|    ☑️   	|             	|
|  `tweets   `  	|       ⌥     	|   Search my recent tweets for {query}                     	|    ☑️   	|        	|             	|
|  `unfollow `  	|             	|   Unfollow @{query} on Twitter                            	|        	|        	|       ☑️     	|
|  `users    `  	|             	|   Search Twitter users for {query}                        	|    ☑️   	|    ☑️   	|             	|
|  `users    `  	|       ⌘     	|   Search Twitter users I follow for {query}               	|    ☑️   	|    ☑️   	|             	|
|  `users    `  	|       ⇧     	|   Search nearby Twitter people for {query}                	|    ☑️   	|    ☑️   	|             	|
|  `verified `  	|             	|   Search top tweets from verified users for {query}         |    ☑️   	|       	|             	|
|  `videos   `  	|             	|   Search Twitter videos for {query}                       	|    ☑️   	|    ☑️   	|             	|
|  `videos   `  	|             	|   Search Twitter videos from people I follow for {query}  	|    ☑️   	|    ☑️   	|             	|
|  `videos   `  	|       ⇧     	|   Search nearby Twitter videos for {query}                	|    ☑️   	|    ☑️   	|             	|
|  `videos   `  	|       ⌘     	|   Search my Twitter videos for {query}                    	|    ☑️   	|    ☑️   	|             	|


# Tips

One of the most convenient features of this workflow is the ability to quickly search for your own tweets and tweeted media. By using the `my` keyword followed by search terms, you can quickly continue previous threads or link to things you said before.

<img src="./assets/twitter-toolkit-my.png" alt="Twitter Toolkit's support for searching for my tweets">

# Changelog[¹](https://keepachangelog.com/)

## [v0.3.9] - 2022-04-13
### Added
- Added `likes` keyword as synonym for `me` to "See my Twitter Likes"
- Added `topic` keyword to "See Twitter Topic Picker" ([#9](https://github.com/chrismessina/alfred-twitter-toolkit/issues/9))


## [v0.3.8] - 2021-08-26
### Added
- Added `lists` keyword to "See which Lists I'm on" and to "View my Lists"
- Added `connect` keyword to "See Who to Follow" (h/t [@nima_owji](https://twitter.com/nima_owji))
- Added `tweet` keyword (which takes a URL to a tweet) to create a beautiful image using [@rang_ali](https://twitter.com/rang_ali)'s [Poet.so](https://poet.so).

## [v0.3.7] - 2021-06-19
### Added
- Added `validator` keyword to access [Twitter's Card validator](https://cards-dev.twitter.com/validator).
- Added several keywords for accessing Settings on the web:
  - `access`
  - `account`
  - `data`
  - `download`
  - `notifs`
  - `privacy`
  - `resources`
  - `security`
  - `settings`

### Changed
- Trimmed whitespace for `@` keyword.

## [v0.3.6] - 2021-05-04
### Added
- Added keyword `@` view user's profile photo
- Added `birdwatch` List Filter
- Added `my` Birdwatch notes access
- Added shift modifier to `@` keyword to view user's profile photo
- Added verified icon
- Added {var:actionPrefix}

### Changed
- Edited `domain` variable to include trailing slash for consistency.
- Added `{var:service}` to videos searches
- Capitalized "Tweet" and other nouns
- Set userId to not export

## [v0.3.5] - 2021-01-03
### Added
- Added search for latest hashtagged tweets using `my` keyword
- Added new searches:
  - for top post from the last week from people you follow with keyword `top` (h/t [@wongmjane](https://twitter.com/wongmjane/status/1345886070794141696))
  - for top post from my extended network with keyword `social` (h/t [@IgorBrigadir](https://twitter.com/IgorBrigadir/status/1345894508588900353))
  - for top post from my trusted network with keyword `trusted`
  - for top post from verified users with keyword `verified`
- Added search for cashtags using `$` keyword

### Changed
- Added text for `my` search to include 'Top' label
- Changed Worflow icon
- Changed OneUpdater to look for recent GitHub releases

## [v0.3.4] - 2020-11-26
### Added
- Added synonym keywords `inbox` and `messages`
- Added keyword `reply` to create a new status in-reply-to a tweet
- Added keyword `new` for composting a new tweet; added {query} to this object to preview text

### Changed
- Updated OneUpdater to new repository
- Updated Twitter and Tweetbot icons

### Fixed
- Tweak the way `me` works to take an optional argument.
- Replaced several instances of "Twitter" with `{var:service}`
- Hooked up OneUpdater so it'll do its thing!

## [v0.3.3] - 2020-09-17
### Fixed
- Quick fix for errant curly brace in `Go to hashtag` query.

## [v0.3.2] - 2020-09-07
### Fixed
- Quick fix for missing non-personalized `users` query.

## [v0.3.1] - 2020-09-06
### Fixed
- Replaced "(from:{var:account})" with "from:{var:account}" (no parens) from app searches.
- Fixed on errant search that targeted videos rather than all tweets.

## [v0.3.0] - 2020-09-04
### Added
- Support for [Tweetbot URL Schemes](https://tapbots.net/tweetbot4/support/url-schemes/) by setting `tweetbot` as `platform` variable (thanks [@bemawr](https://www.alfredforum.com/profile/16163-bemawr/ )!) (Closes [#3](https://github.com/chrismessina/alfred-app/issues/3))
- Support for `nearby` searches:
  - tweets
  - photos
  - videos
  - users
- keywords to go to:
  - hashtag page
  - topics
  - Alternative keyword `!` for notifs
- Descriptive notes in Workflow
- OneUpdater (Closes [#6](https://github.com/chrismessina/alfred-app/issues/6))

### Changed
- Added `service` and `domain` variables to make it easier to develop other Toolkits
- Drastically increased support for Twitter for Mac thanks to new routes included in 8.34 (thanks [@nolanobrien](https://twitter.com/@nolanobrien)!) (Closes [#4](https://github.com/chrismessina/alfred-app/issues/4))

### Removed
- followees keyword

## [v0.2.0] - 2020-08-17
### Added
- All new icons!
- Support for new keywords: `analytics`, `explore`, `help`, `media`, `notifs`
- New additions to the "my" collection: Bookmarks, Lists, Moments, Notifications

## [v0.1.0] - 2020-08-06
- Initial Release


# About

This workflow is unaffiliated with nor endorsed by Twitter.

You can [file bugs](https://github.com/chrismessina/alfred-twitter-toolkit/issues/new) or [submit feature requests](https://github.com/chrismessina/alfred-twitter-toolkit/issues/new) on GitHub using the label `workflow:twitter-toolkit`.

<a href="https://www.alfredforum.com/topic/15390-workflow-twitter-toolkit-for-alfred/">Alfred Forum link</a>.
