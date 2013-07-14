### Drupal-Chromelogger

Drupal ChromeLogger makes calls to Drupal's Watchdog function visible in the browser via [Chromelogger][].

The idea behind this is that calls to `dpm()` are not the best way to represent structured data for inspection, and they are often left in themes and modules, causing issues in production.

After using Chrome for lots of front end work, the debugger seemed a much better place to dump this kind of information for exploring, and this was a good excuse to try making a new drupal module, using the php specific project for using Chromelogger, [Chromephp][]

## Usage

1) Install the `chromelogger` drupal module, from this github url.

2) Enable the `chromelogger`drupal module, with:

```shell

drush en chromelogger

```

3) Call the `watchdog()` function when you want to log details, and see it turn up in the browser.

## Installation

At present this module is only available on github, largely because I'm working out how to use the Libraries API to include Apache 2 licenced code into a drupal module and have it hosted drupal.org.

I'd welcome some help, as it wasn't immediately clear when I first read over it.


## Credits

* Original idea and code by [Craig Campbell][]


[Chromelogger]: http://craig.is/writing/chrome-logger
[Chromephp]: https://github.com/ccampbell/chromelogger
[Craig Campbell]: http://craig.is/
