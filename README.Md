# EASY LAB lib

A library for facilitating communication through XMPP and Ubiquiti mfi Smart Plugs. 

## mfi

Provides functions to create a custom configuration.  This includes:

 - reading the original configuration and updating it
 - disabling unsecure services like telnet

At the moment `sshpass` is used to push configuration updates.

## xmpp

It's a wrapper around `github.com/mattn/go-xmpp`. It provides:

 - automatic reconnects after failures with a secure back-off
 - keep-alive functionality through ping, cf. XEP-0199
 - data serialization

## TODO

- properly disable sshd
