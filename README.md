# isshd_notifier
An alternative parser/notifier tool to send notifications when specific strings show up in user input or output streams.

Designed as an alternative to using [bro](https://www.bro.org/), and the [isshd_policy](https://github.com/set-element/isshd_policy) policies.  Not that they're bad.  I just had some stability issues with bro, and since my use case was a much smaller scope, I decided a rewrite wouldn't be that bad.

This solution still uses the [instrumented SSHd](https://github.com/set-element/openssh-hpn-isshd), and ssllogmux, to transport the events to the parsing nodes.