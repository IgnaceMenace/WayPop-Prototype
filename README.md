# WayPop

**Warning, I'm not even sure to have the time necessary to build this,
don't expect it to be ready soon, this is one of my first programming project,
I'm not even a software engineer and the project havn't even started yet !**

WayPop is a popup menu for wayland, its goal is to provide a GNOME like quick setting
window to manage all the different stuffs in a compact way with expandable area.
It should also be able to let the user add some features via a configuration file.
This project is inspired from a [mockup](https://gitlab.gnome.org/Teams/Design/os-mockups/-/commit/f07e260f25afb96dcfa7fcf4401a47c73bdc8f72) submitted by a graphic designer to the GNOME
shell gtilab repository.

I'll use [this tutorial](https://github.com/Taiko2k/GTK4PythonTutorial) to start learning python and GTK4. 
## List of functionalities to provides
- [ ] GTK4
    - Use the standard GTK4 theme
- [ ] Python => Rust  
    - It's going to be prototyped in python but should be ported to Rust afterward
- [ ] Power menu
    - Power Off
    - Log Out
    - Suspend
- [ ] Power management
    - Battery saver
    - Balanced
    - Performance
- [ ] Sway settings
    Inspired by GNOME's PopOS_Shell quick settings
    - Changing tiling mode
    - Changing gap size
- [ ] Output Menu
    - Enable monitor
    - Disable monitor
- [ ] Input Menu
    - Change keyboard layout
- [ ] Brightness
    - Change brightness of a monitor
    - Enable night mode
    - Change red shift settings
- [ ] Audio menu
    - Change volume of each output devices
    - Change volume of each input devices
    - Change volume of system or applications
    - Quick mute toggle
- [ ] Network manager
    - Select your wifi
    - Open your NetworkManager GUI or a small Pop UP
    - Problem is that enterprise Wifi are much more complicated to configure and this will be time consumming
    - VPN selecter
    - Bluetooth selecter
    - Airplane mode
- [ ] Container manager
    - Launch, or stop Podman container or toolbox
- [ ] Scratchpad
    - View what's in the Sway scratchpad
- [ ] Extensibility
    - Add new module via easy interface (python scripting, shell scripting)
## Difficulties
- Expanding all the settings to new output or input
# Installation
it will be packaged into a pip package and if I ever port it to rust I will package it in a cargo package but need to create another repo anyway
