# OctoPrint-Gpioshutdown

GPIO Shutdown is a simple plugin that can shutdown the Raspberry Pi if a switch connected to ground and one of the GPIO pins pressed. This plugin also turns On a led when Octoprint server is up and running. Connect a led to one of the GPIO pins and other end to ground, then set the pin number (BCM Mode) in plugin settings in web interface.


## Setup

Install via the bundled [Plugin Manager](https://docs.octoprint.org/en/master/bundledplugins/pluginmanager.html)
or manually using this URL:

    https://github.com/fmalekpour/OctoPrint-Gpioshutdown/archive/master.zip


## Configuration

In web interface, install the plugin and reload if necessary, then click on GPIO Shutdown, you will have:

- Pin Shutdown: Raspberry Pi GPIO pin (BCM Mode) your shutdown switch is attached to.
- Pin Led: Raspberry Pi GPIO pin your ready-to-run led attached to. This led will turn On when OctoPrint is up and ready to run/connect.
- Debounce Time: When press the shutdown switch, wait for this amount of time to wait for the signal to stabilize.

You can find the GPIO pin number assignments at [Raspberry Pi GPIO Pinout](https://www.raspberrypi.org/documentation/usage/gpio/).

