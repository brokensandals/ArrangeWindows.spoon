# ArrangeWindows.spoon

A spoons (plugin) for [hammerspoon](https://www.hammerspoon.org) that lets you quickly rearrange all your windows to match various layouts.

## Setup

Clone this repository inside of `~/.hammerspoon/Spoons`, then add `hs.loadSpoon("ArrangeWindows")` to your `init.lua`.

## Usage

Some default layouts are provided, such as two-column 50/50, two-column 60/40, or three panels with two stacked vertically on the right half of the screen.
You can also hardcode additional layouts by modifying `spoon.ArrangeWindows.layouts`.

It also supports saving the current arrangement of windows, with a given name, so that you can load it again later.
Saved layouts are currently persisted using the `hs.settings` module.

|Function name|Description|
|---|---|
|chooseLayout|Shows a fuzzy finder for selecting a layout.|
|chooseWindow|Shows a fuzzy finder full of window titles so you can choose one to switch focus to.|
|clearSavedLayouts|Forget all saved layouts.|
|maximize|maximizes the current window|
|saveLayout|Saves the current arrangement of windows to a name of your choosing.|

## License

This is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
