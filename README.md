# splas-runner

A cross-platform binary to change the desktop background from Unsplash. (uses the [splas-php][splas] composer package)

[![Build Status](https://travis-ci.org/PXgamer/splas-runner.svg?branch=master)](https://travis-ci.org/PXgamer/splas-runner)
[![Version](https://img.shields.io/packagist/v/pxgamer/splas-runner.svg)](https://packagist.org/p/pxgamer/splas-runner)
[![License](https://img.shields.io/packagist/l/pxgamer/splas-runner.svg)](https://opensource.org/licenses/mit-license)

## Supported operating systems

OS      | Supported?
------- | ----------
Windows | ✓
Mac OSX | ✗
Ubuntu  | ✓
Linux   | ✗

_Note: Running in an unsupported OS will result in an ErrorException._

## Usage

- Install through Composer globally/locally using `composer global require pxgamer/splas-runner`
- Get an API key from [Unsplash][us]
- Either set the `UNSPLASH_API_KEY` environment variable, or provide a `--key {key}` option in the command
- Run the binary using `splasr run [options]`

## Options

Name | Description
---- | -----
--keep / -k | Specify whether to keep or remove images. Defaults to remove any images before downloading.
--key | Specify your API key. Defaults to use the environment variable.
--interval / -i | Specify an integer (minutes) when running in looped mode. By default will exit after the first run.

## Credits

All credit for images and API goes to [Unsplash][us].  
The [wallpaper.exe](resources/bin) ([repo][wallpaper]) credit goes to [@sindresorhus][sindresorhus].  

[us]: https://unsplash.com
[wallpaper]: https://github.com/sindresorhus/win-wallpaper
[sindresorhus]: https://github.com/sindresorhus
[splas]: https://github.com/pxgamer/splas-php
