
# Clojure Bots

![clj-bots-logo](https://raw.githubusercontent.com/scgilardi/slingshot/master/imgs/clj-bots-logo.png)

Welcome!
Clojure Bots is a group dedicated to bringing Clojure to the world of physical computing.

## Vision

Physical systems are inherently concurrent, and as we all know, Clojure was designed from the ground up with concurrency in mind.
This makes it an ideal language for physical computing.

The world of physical computing is complicated by the presence of so many available computing devices.
There's Arduino and Spark over Firmata, Raspberry Pi, and BeagleBone Black, to name just a few.
Most popular languages with APIs for these varied devices approach the problem piecemeal.
Consequently, switching from one device to another means learning a completely different API.
One of the core visions of Clojure Bots is that there has to be a better way.

## Enter `pin-ctrl`

Pin Ctrl was largely inspired by `core.matrix`, a Clojure library which has successfully served as a common API for doing matrix algebra, regardless of the underlying implementation.
In our setting, `pin-ctrl` provides a common API for device programming, independent of the underlying hardware.
This means that you can take a program written for a Raspberry Pi, and with nothing more than configuration changes port it over to a BeagleBone Black or Arduino over Firmata.

This works via a set of protocols which `pin-ctrl` implementations must satisfy.
On loading, these implementations register themselves through the `pin-ctrl` API, thereby becoming available to any programmer who wishes to use them.

To learn more about the pin-ctrl API please visit the [Clojure Bots wiki](https://github.com/clj-bots/clj-bots-home/wiki).

## Other projects on the horizon

When it comes to serious state of the art robotics programming, nothing beats the Robotic Operating System.
All of the Robotics competition contenders use it, including Google's robots.
It would be great if the Clojure community could jump on board here.

Thankfully, there are java bindings for this project, which it might be possible to piggie back on.
However, it would also be interesting to see how the project is structured, and evaluate whether a more thoroughly Clojuric solution might be advantageous.


