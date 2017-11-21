# PulsewayPush

Send "push" from ProcessWire to Pulseway.

## Description

PulsewayPush simply send a push to a Pulseway instance. If you are using this
module, you probably installed Pulseway on your mobile device: you will receive
notification on your mobile.

To get more information about Pulseway, please visit their website.

#### Note
They have a **free** plan which include **10 notifications (push)** each day.

## Usage

[Install](http://modules.processwire.com/install-uninstall/) the PulsewayPush module.

Then call the module where you like in your module/template code :
```
<?php $modules->get("PulsewayPush")->push("The title", "The notification message.", "elevated"); ?>
```

#### Hookable function
```___push()```
```___notify()```
(the two function do the same thing)

## Examples of use case

- I needed for our work a system which send notification to mobile device in case
of a client request immediate support. Pulseway was choosen because it is already
used to monitor our infrastructure.

- An idea, you could use the free plan to monitor your blog or website regarding the number
of failed logins attempts (hooking Login/Register?), the automated tool then block the attacker's ip with a firewall rules.
