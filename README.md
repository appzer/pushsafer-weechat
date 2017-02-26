![Pushsafer](https://www.pushsafer.com/de/assets/logos/logo.png)

Pushsafer for Weechat
====================

Send private messages and highlights to your Android, iOS or Windows 10 devices via
the Pushsafer service (https://www.pushsafer.com)

##How to send push-notification out of weechat with Pushsafer

[Pushsafer.com](https://www.pushsafer.com) make it easy and safe to send &amp; receive push-notifications to your
- Android devices
- iOS devices (iPhone, iPad, iPod Touch, Watch)
- Windows 10 Phone & Desktop
- Browser (Chrome & Firefox)

Install
-------

Load the pushsafer-weechat.rb plugin into Weechat. Place it in the
~/.weechat/ruby directory:

    /ruby load pushsafer-weechat.rb

It also requires a Pushsafer account and Ruby, the Ruby OpenSSL libraries, and RubyGems installed on your host.

Setup
-----

Set your Pushsafer private key.

    /set plugins.var.ruby.pushsafer-weechat.privatekey XXXXXXXXXXXXXXXXXXX

Options
-------

* plugins.var.ruby.pushsafer-weechat.privatekey

  The private or alias key for your Pushsafer service. Defaults to an empty string and must be set for pushsafer-weechat to work.

* plugins.var.ruby.pushsafer-weechat.interval
   The interval between notifications. Doesn't notify if the last
   notification was within x seconds.
   Default: 60 seconds

* plugins.var.ruby.pushsafer-weechat.sound
  Set your notification sound options (Current listing located at https://www.pushsafer.com/en/pushapi)
  a number 0-28 0 = silent, blank = device default
  Default: blank (Sound will be device default)

* plugins.var.ruby.pushsafer-weechat.icon
  Set your notification icon (Current listing located at https://www.pushsafer.com/en/pushapi)
  a number 1-98
  Default: blank



