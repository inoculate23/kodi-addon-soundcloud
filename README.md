# SoundCloud Add-on for [Kodi](https://github.com/xbmc/xbmc)

<img align="right" src="https://github.com/xbmc/xbmc/raw/master/addons/webinterface.default/icon-128.png" alt="Kodi logo">

<a href="https://github.com/jaylinski/kodi-addon-soundcloud/releases"><img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/jaylinski/kodi-addon-soundcloud.svg"></a>
<a href="http://forum.kodi.tv/showthread.php?tid=206635"><img alt="Link to Kodi forum" src="https://img.shields.io/badge/Kodi-Forum-informational.svg"></a>

This [Kodi](https://github.com/xbmc/xbmc) Add-on provides a minimal interface for SoundCloud.

## Features

* Search
* Discover new music
* Play tracks, albums and playlists

## Installation

* [Download the newest release](https://github.com/jaylinski/kodi-addon-soundcloud/releases) (`plugin.audio.soundcloud.zip`)
* Copy the ZIP-file to your Kodi system
* Open Kodi, go to Add-ons and select "Install from ZIP"
* Select the file `plugin.audio.soundcloud.zip`

## API

Documentation of the **public** interface.

### plugin://plugin.audio.soundcloud/play/?[track_id|playlist_id|url]

Examples:

* `plugin://plugin.audio.soundcloud/play/?track_id=1`
* `plugin://plugin.audio.soundcloud/play/?playlist_id=1`
* `plugin://plugin.audio.soundcloud/play/?url=https%3A//soundcloud.com/kingtheta/sets/getting-over-it`

Legacy (will be removed in v4.0):

* `plugin://plugin.audio.soundcloud/play/?audio_id=1` Use `track_id=1` instead.

## Development

This add-on uses [Pipenv](https://pypi.org/project/pipenv/) to manage its dependencies.

### Setup

[Install Pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv) and run `pipenv install --dev`.

### Build

Run `pipenv run build`.

### Lint

Run `pipenv run lint`.

### Test

Run `pipenv run test`.

> Requires at least Python 3.6!

## Roadmap

* Check for correct charsets (UTF-8)
* Resolve TODOs
* Re-implement all features from original add-on

## Attributions

This add-on is strongly inspired by the [original add-on](https://github.com/SLiX69/plugin.audio.soundcloud)
developed by [bromix](https://kodi.tv/addon-author/bromix) and [SLiX](https://github.com/SLiX69).

## Copyright and license

This add-on is licensed under the MIT License - see `LICENSE.txt` for details.