# French Language Pack for [Flarum](http://flarum.org/)

[![Code Climate](https://codeclimate.com/github/maelsoucaze/flarum-ext-french/badges/gpa.svg)](https://codeclimate.com/github/maelsoucaze/flarum-ext-french) [![StyleCI](https://styleci.io/repos/41550823/shield)](https://styleci.io/repos/41550823)

French language pack to localize the Flarum forum software, its bundled extensions and libraries.

## Informations

Includes the following French locales compatible with:

- [Flarum](https://github.com/flarum/core)'s Core [0.1.0 Beta 5](https://github.com/flarum/core/releases/tag/v0.1.0-beta.5)
  - Bundled extensions:
    - [Akismet](https://github.com/flarum/flarum-ext-akismet) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-akismet/releases/tag/v0.1.0-beta.5)
    - [Approval](https://github.com/flarum/flarum-ext-approval) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-approval/releases/tag/v0.1.0-beta.5)
    - [Facebook Login](https://github.com/flarum/flarum-ext-auth-facebook) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-auth-facebook/releases/tag/v0.1.0-beta.5)
    - [Flags](https://github.com/flarum/flarum-ext-flags) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-flags/releases/tag/v0.1.0-beta.5)
    - [GitHub Login](https://github.com/flarum/flarum-ext-auth-github) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-auth-github/releases/tag/v0.1.0-beta.5)
    - [Likes](https://github.com/flarum/flarum-ext-likes) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-likes/releases/tag/v0.1.0-beta.5)
    - [Lock](https://github.com/flarum/flarum-ext-lock) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-lock/releases/tag/v0.1.0-beta.5)
    - [Mentions](https://github.com/flarum/flarum-ext-mentions) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-mentions/releases/tag/v0.1.0-beta.5)
    - [Pusher](https://github.com/flarum/flarum-ext-pusher) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-pusher/releases/tag/v0.1.0-beta.5)
    - [Sticky](https://github.com/flarum/flarum-ext-sticky) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-sticky/releases/tag/v0.1.0-beta.5)
    - [Subscriptions](https://github.com/flarum/flarum-ext-subscriptions) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-subscriptions/releases/tag/v0.1.0-beta.5)
    - [Suspend](https://github.com/flarum/flarum-ext-suspend) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-suspend/releases/tag/v0.1.0-beta.5)
    - [Tags](https://github.com/flarum/flarum-ext-tags) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-tags/releases/tag/v0.1.0-beta.5)
    - [Twitter Login](https://github.com/flarum/flarum-ext-auth-twitter) [0.1.0 Beta 5](https://github.com/flarum/flarum-ext-auth-twitter/releases/tag/v0.1.0-beta.5)
  - Bundled libraries:
    - [Laravel](https://github.com/laravel/laravel)'s Validation Rules [5.2.27](https://github.com/laravel/laravel/releases/tag/v5.2.27)
    - [Moment.js](https://github.com/moment/moment) [2.12.0](https://github.com/moment/moment/releases/tag/2.12.0)

Released under the MIT license. Please see the [license terms](https://github.com/maelsoucaze/flarum-ext-french/blob/master/LICENSE).

## Installation

### Using Composer (Recommended)

Flarum use Composer to manage its dependencies and extensions. The French language pack is available [on Packagist](https://packagist.org/packages/maelsoucaze/flarum-ext-french) and can be managed that way. Make sure that [Composer](https://getcomposer.org/) is installed on your machine, then run the following command in the location where Flarum is installed:

```
composer require maelsoucaze/flarum-ext-french
```

The same command can be used to update independently the French language pack, without updating anything else. Note that because the French language pack will be added as a Flarum's dependency, it will also be automatically updated when updating Flarum and its dependencies via Composer.

### Manual Installation

1. Download [the latest stable release](https://github.com/maelsoucaze/flarum-ext-french/releases) (or [the latest development build](https://github.com/maelsoucaze/flarum-ext-french/archive/master.zip)).
2. Unpack the downloaded archive with [a file archiver](https://en.wikipedia.org/wiki/Comparison_of_file_archivers).
3. Log in to your server via [FTP](https://en.wikipedia.org/wiki/File_Transfer_Protocol), [SSH](https://en.wikipedia.org/wiki/Secure_Shell) or your provider's control panel.
4. Navigate to the *vendor/* directory of your Flarum installation.
5. Create a *maelsoucaze/* subdirectory into it.
6. Create a *flarum-ext-french/* subdirectory into that new subdirectory.
6. Upload all the content in the unpacked folder to the *flarum-ext-french/* subdirectory.
7. Edit the *vendor/composer/installed.json* file:

  - Find:
```
        ]
    }
]
```

  - Replace with:
```
        ]
    },
    {
        "name": "maelsoucaze/flarum-ext-french",
        "version": "v1.0.3",
        "version_normalized": "1.0.3.0",
        "source": {
            "type": "git",
            "url": "https://github.com/maelsoucaze/flarum-ext-french.git",
            "reference": "dbc4ee3008b101f710b50915a8b9a2f775f4810f"
        },
        "dist": {
            "type": "zip",
            "url": "https://api.github.com/repos/maelsoucaze/flarum-ext-french/zipball/dbc4ee3008b101f710b50915a8b9a2f775f4810f",
            "reference": "dbc4ee3008b101f710b50915a8b9a2f775f4810f",
            "shasum": ""
        },
        "require": {
            "flarum/core": "^0.1.0-beta.5"
        },
        "time": "2016-03-29 21:18:53",
        "type": "flarum-extension",
        "extra": {
            "branch-alias": {
                "dev-master": "1.0.x-dev"
            },
            "flarum-extension": {
                "title": "French",
                "icon": {
                    "image": "icon.svg",
                    "backgroundColor": "#fff",
                    "backgroundSize": "cover",
                    "backgroundPosition": "center"
                }
            },
            "flarum-locale": {
                "code": "fr",
                "title": "Français"
            }
        },
        "installation-source": "dist",
        "notification-url": "https://packagist.org/downloads/",
        "license": [
            "MIT"
        ],
        "authors": [
            {
                "name": "Maël Soucaze",
                "email": "maelsoucaze@gmail.com",
                "homepage": "http://www.maelsoucaze.com"
            }
        ],
        "description": "French language pack for Flarum.",
        "homepage": "https://github.com/maelsoucaze/flarum-ext-french",
        "keywords": [
            "locale"
        ]
    }
]
```

## Contributing

Thank you a lot to wish to contribute. I sincerely appreciate your commitment. Using the language pack is already a huge support, but best other ways to contribute are:

- Star on GitHub. Because if you use it and like it, you can at least be a stargazer!
- Follow on GitHub. You will be notified in real time of all changes. No more misses!
- Report [issues](https://github.com/maelsoucaze/flarum-ext-french/issues) on GitHub. Any feedback is welcome.
- Open pull requests on GitHub to submit fixes and improvements. Be listed as a [contributor](https://github.com/maelsoucaze/flarum-ext-french/graphs/contributors)!
- Join [the language pack's discussion](https://discuss.flarum.org/d/615-french-language-pack) on the Flarum community.
- Follow me [on Twitter](https://twitter.com/maelsoucaze). Promise, I don't spam pictures of kittens and puppies (too much).
- Let's have a drink if you are near Paris!
