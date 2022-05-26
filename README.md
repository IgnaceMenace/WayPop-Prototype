# WayPop

**Warning, I'm not even sure to have the time necessary to build this,
don't expect it to be ready soon, this is one of my first programming project,
I'm not even a software engineer and the project hasn't even started yet !**

WayPop is a popup menu for wayland, its goal is to provide a GNOME like quick setting
window to manage all the different stuffs in a compact way with expandable area.
It should also be able to let the user add some features via a configuration file.
This project is inspired from a [mockup](https://gitlab.gnome.org/Teams/Design/os-mockups/-/commit/f07e260f25afb96dcfa7fcf4401a47c73bdc8f72) submitted by a graphic designer to the GNOME
shell gtilab repository. Another inspiration comes from [nwg-panel](https://github.com/nwg-piotr/nwg-panel), as he is already building everything in python, I'd like to afterward try to rebuild my project using rust or C to actualy have a lightweight integration.

I'll use [this tutorial](https://github.com/Taiko2k/GTK4PythonTutorial) to start learning python and GTK4. 
## List of functionalities to provides
- [ ] GTK4
    - Use the standard GTK4 theme
- [ ] Python => Rust / C  
    - It's going to be prototyped in python but should be ported to Rust or C afterward
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
        - Example of a such module : Lokinet client connection interface
## Difficulties
- Expanding all the settings to new output or input
## Strategy
I'll use this project to perfect myself in Python and try to learn new stuff and ways doing things professionaly. I like standardization because it simplify overall complexity even if it can make some simple things harder to do and in a way I think it is a minimalist way of doing stuff. Also GNOME will always be around and GTK too and always be free and backed up by RedHat etc. I like to learn skills that I will be able to use later even in a few years. 
- GTK instead of Qt
    - Gtk is developped only under free and open source licences, which is philosophicaly better in my opinion than the Qt licences. We never know at some point open source version of Qt might end up not being as well supported as the paid one.
- .ui file
    - I will create the GUI using xml in .ui file because it will be easier to change the code afterward, especially if I switch to rust
    - Those .ui file will be build using Cambalache or GNOME Builder's designer
- GTK application
    - Since the application isn't originaly designed for GNOME it will be based on the GTK Application template
- I'll try to generate the documentation the same way GNOME propose to do it because I'd like to experiment with their way of building apps
- Since this is an experimentation and I have no clue how it will go, I might go back to programming in a more generic way using python Qt from a text editor and without fitting into a framework.
# Installation
it will be packaged into a pip package and using the GTK Application template if both are compatible and if I ever port it to rust I will package it in a cargo package but need to create another repo anyway
