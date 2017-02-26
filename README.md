Pushsafer for Weechat
====================

Send private messages and highlights to your Android, iOS or Windows 10 devices via
the Pushsafer service (https://www.pushsafer.com)

Install
-------

Load the pushsafer-weechat.rb plugin into Weechat. Place it in the
~/.weechat/ruby directory:

    /ruby load pushsafer-weechat.rb

It also requires a Pushsafer account and Ruby, the Ruby OpenSSL libraries, and RubyGems installed on your host.

Setup
-----

Set your Pushsafer user key.

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
   
  Default: blank (Sound will be device default)



