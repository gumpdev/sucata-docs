# Starting the project

## Starting

First of all, make sure to have the sucata engine installed, you can follow the
installation guide in the [installation page](../installation.md).

To make sure that sucata is installed correctly, you can run the following
command in your terminal:

```bash
sucata version
```

Then you can create a new folder for the project, and inside that folder, create
a new file called `main.lua`, this will be the main entry point of the game.

## Using Classic

Is highly recommended to use [classic](https://github.com/rxi/classic) library
to create classes for your entities, but it's not mandatory, you can create your
entities using plain tables if you prefer.

To use the classic library, you need to download the `classic.lua` file from the
repository and place it in your project folder

## Configuration

To configure the project, you need to call functions from `sucata.window` to
configure the window of the game.

```lua
sucata.window.set_window_size(960, 540) -- The game window size, in pixels
sucata.window.set_keep_aspect(1) -- Keep the aspect ratio of the game, if the window is resized, it will keep the aspect ratio of the game, and add black bars on the sides if necessary. (0 = off, 1 = keep aspect with bars, 2 = keep aspect with crop)
sucata.window.set_window_title("My First Game") -- The game window title
sucata.window.set_vsync(1) -- Active Vsync in your game, Vsync will cap the max frame rate (0 = off, 1 = on, higher values for specific intervals)
sucata.window.show_debug_info(true) -- Show debug info in the game, this will show the fps, and some other information about the game, this is useful for debugging and optimizing your game.
sucata.window.set_window_icon("src://icon.png") -- The game window icon
sucata.window.set_fullscreen(false) -- Set the game to fullscreen mode
```

> For the [sokol](https://github.com/floooh/sokol) limitations, vsync will be
> always active.

> Remember to disable the sucata.window.show_debug_info when you release your
> game
