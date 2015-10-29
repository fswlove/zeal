# Zeal

[![IRC](https://img.shields.io/badge/irc-%23zealdocs-blue.svg?style=flat-square)](https://kiwiirc.com/client/irc.freenode.net/#zealdocs)

> **zeal** *noun*
>
> 1. a feeling of strong eagerness (usually in favor of a person or cause)
> 2. excessive fervor to do something or accomplish some end
> 3. prompt willingness
>
> (from WordNet 3.0)

Zeal is a simple offline documentation browser inspired by [Dash](https://kapeli.com/dash).

![Screenshot](https://i.imgur.com/SiLvpz8.png)

[More screenshots](https://imgur.com/a/eVi97)

## Build Status

[![Coverity Scan](https://img.shields.io/coverity/scan/4271.svg?style=flat-square)](https://scan.coverity.com/projects/4271)

OS \ Branch | master | stable
------------|--------|-------
Linux | [![Shippable](https://img.shields.io/shippable/54ac2ce4d46935d5fbc19b84/master.svg?style=flat-square)](https://app.shippable.com/builds/54ac2ce4d46935d5fbc19b84) | [![Shippable](https://img.shields.io/shippable/54ac2ce4d46935d5fbc19b84/stable.svg?style=flat-square)](https://app.shippable.com/builds/54ac2ce4d46935d5fbc19b84)
Windows | [![AppVeyor](https://img.shields.io/appveyor/ci/trollixx/zeal/master.svg?style=flat-square)](https://ci.appveyor.com/project/trollixx/zeal) | [![AppVeyor](https://img.shields.io/appveyor/ci/trollixx/zeal/stable.svg?style=flat-square)](https://ci.appveyor.com/project/trollixx/zeal)

## Download

Get binary builds for Windows and Linux from the [download page](https://zealdocs.org/download.html).

## How to use

After installing Zeal, you need to download docsets. Go to *File->Options->Docsets*, select the ones you want, and click the *Download* button.

## How to compile

### Requirements
* [Qt](https://www.qt.io/) version 5.2.0 or above. Required modules: Qt WebKit Widgets, Qt SQL plugin for SQLite, Qt X11 Extras (X11 only).
* [libarchive](http://libarchive.org/).
* X11 only: `xcb-util-keysyms`.
* Ubuntu Unity only: [libappindicator](https://launchpad.net/libappindicator).

To compile Zeal run `qmake` and then `make`. Linux users can install Zeal with `make install` command.

## Query & Filter docsets

You can limit the search scope by using ':' to indicate the desired docsets:

`java:BaseDAO`

You can also search multiple docsets separating them with a comma:

`python,django:string`

## Command line

If you prefer, you can start Zeal with a query from command line:

`zeal python:bomb`

## Creating your own docsets

You can use [Dash's instructions for generating docsets](https://kapeli.com/docsets).
