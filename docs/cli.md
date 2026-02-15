# Sucata CLI

This CLI of the Sucata, is a collection of helpers

## sucata run 

Runs a Sucata Lua script file

**arguments**

- <file> - It is the path of the main lua file 
- --entity <entity_file> (optional) - It is the lua file of a entity (for testing)

## sucata build

Builds Sucata into a binary game for the current OS

**arguments**

- <file> - It is the path of the main lua file 
- --icon <path> (optional) - It is the icon for your game

> For while, this is a Sucata limitation, you can only build the game for the current OS.

## sucata version

Show the Sucata game engine version and release date

## sucata shader

Util to shaders on sucata

### sucata shader build 
Builds a .glsl file to sucata shader file

#**arguments**

- <file> - It is the path of the .glsl shader you wants do build

### sucata shader create
Create a base .glsl shader file

#**arguments**

- <file> - It is the path for create a .glsl from template
- --post-procesing (optional) - Its a flag to create a template for post-processing [WIP]
- --font (optional) - Its a flag to create a template for font shader