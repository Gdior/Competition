# Configurations

* Configurations files for chibios 19.1
* MCU type STM32F429BIT6

# Author

* NineLivesCat(esdcasdcd@126.com)

# Structure

* board:    configurations files for board (unfinished)
* cfg:      configurations files for hal, ch and mcu(unfinished)
* os:       chibios
* src:      source files and header
* tools:    required environment and some tools
* Makefile: main makefile for whole project

# Todo

* finish configuration files

# Configure environment

## For Linux (tested on Ubuntu 18.04)

* run command `sudo apt-get install openocd gcc-arm-none-eabi`
* download the configurations flies and put it on any directory you want
* change to directory where you put configurations flies
* run command `make` or `make -j`
* if `build` directory and `*.elf` is created, the environment is configured well
* (optional) download VSCode and buy a Jlink for better coding and debugging 

## For MAC OSX

* install homebrew via https://brew.sh
* install XCode command line toolchain
* `xcode-select --install`
* `brew cask install xquartz java`
* `brew install open-ocd`
* `brew tap PX4/px4`
* `brew install px4-dev`
* download the configurations flies and put it on any directory you want
* change to directory where you put configurations flies
* run command `make` or `make -j`
* if `build` directory and `*.elf` is created, the environment is configured well
* (optional) download VSCode and buy a Jlink for better coding and debugging

## For Windows

* download configurations flies
* copy `./tools/fmpp`(ues`{FMPP_Directory}` to represent its directory below), `./tools/GNU Tools`(ues`{GNUTOOLS_Directory}` to represent its directory below) and `./tools/GNU Tools for ARM Embedded`(ues`{ARMTOOLS_Directory}` to represent its directory below) to another directory
* install `JDK` ,configure the system environment and restart computer 
* run cmd or powershell enter `java -version` to check if JDK is installed
* add `{FMPP_Directory}/fmpp/bin` 
* `{GNUTOOLS_Directory}/GNU Tools/bin` 
* `{ARMTOOLS_Directory}/GNU Tools ARM Embedded\7.0 2017q4\bin`
* to system environment and restart computer
* run cmd or powershell enter `fmpp -v`,`arm-none-eabi-gcc -v` and `make -v` to check the environment configuration
* change to directory where you put configurations flies
* run command `make` or `make -j`
* if `build` directory and `*.elf` is created, the environment is configured well
* (optional) download VSCode and buy a Jlink for better coding and debugging

# Update

* 2019/2/20   By:NLC      Initialization
