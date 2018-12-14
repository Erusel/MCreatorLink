# Minecraft Link

**Minecraft Link enables you to connect hardware devices such as Arduino and Raspberry Pi with Minecraft game via MCreator procedures, commands and general API for Minecraft mod developers.**

## Setup and getting started

Setup instructions can be found on the Minecraft Link official website: https://mcreator.net/link

## Issue tracker

Issues can be reported on the official MCreator development team issue tracker
found on https://mcreator.net/tracker

## Development

To contribute to Minecraft Link, clone this repository and setup this workspace as you would do
with any Minecraft mod. We recommend to use Intelij IDEA for the development.

To setup workspace, set Gradle version to Gradle 3.0

`gradlew --wrapper 3.0`

Then setup the Minecraft Mod workspace:

`gradlew setupDecompWorkspace`

## Implementations

Here are links to the current implementation of device support for the Minecraft Link:
* Arduino (included as submodule in this repository)
* Raspberry Pi (included as submodule in this repository)

## Link protocol specification

All commands sent from the controller (Minecraft client) to the device have this format:

`command?data;\n`

All commands sent from the device to the controller have this format:

`command:data\n`