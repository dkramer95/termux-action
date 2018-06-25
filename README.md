# termux-action
Launch and execute scripts faster through a shortcut selection interface using the new input methods in the
[Termux:API](https://github.com/termux/termux-api) addon

## Prerequisites
`termux-api`

## Installation
`git clone https://github.com/dkramer95/termux-action`

Run `termux-action-install` which will install the package and needed dependencies

## Usage
For [Termux:Boot](https://github.com/termux/termux-boot) users, a persistent notification will be created automatically and show on boot (*recommended*). To manually show notification, type `termux-action-notification`. This notification provides an entry point to the `termux-action-chooser` interface. The notification will remain in place unless you click the explicit 'close' button.

`termux-action-chooser` displays a scrollable list of all executable scripts that exist in `~/.termux-actions` and can be launched with a single click. The complete filename of the scripts in this directory are what will be displayed in the list.

Termux needs a script file to execute. Add your desired command(s) inside a script file and place them in `~/.termux-actions`. For scripts that require a foreground Termux session (i.e. vim), you need to use `termux-action-launch [script]` and add an additional corresponding script in `~/.termux-actions/launch` that contains just the command.

## Screenshots
<img src="https://user-images.githubusercontent.com/6166095/41825257-7da37032-77da-11e8-97b2-fa7ab9aa4839.png" align="top"/>    <img src="https://user-images.githubusercontent.com/6166095/41825216-d0ea74ee-77d9-11e8-9fde-42c471a371c3.png" align="middle" height="600"/>
