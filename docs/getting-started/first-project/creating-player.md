# First Entity

In this section, we will create the first entity of the game, the player, and we
will make it move around the screen.

## Creating the player entity

To create the player entity, we need to create a new file called `player.lua` in
the project folder, import the classic, and we will define the player entity in
this file.

```lua
local Object = require("classic")

local Player = Object:extend()

function Player:new(x, y)
    self.x = x
    self.y = y
		self.width = 64 -- width of the player
		self.height = 64 -- height of the player
		self.speed = 300 -- speed of the player
end

-- This is a function that will be called by the engine every frame, and we can use it to draw the player on the screen
function Player:draw()
	sucata.graphic.draw_rect({
		x = self.x, -- The x position of the player, in pixels
		y = self.y, -- The y position of the player, in pixels
		width = self.width, -- The width of the player sprite, in pixels
		height = self.height, -- The height of the player sprite, in pixels
		origin = 0.5, -- The origin of the player sprite, 0.5 means that the sprite will be drawn from the center, 0 means that the sprite will be drawn from the top left corner
	})
end

return Player
```

Then we will call the player entity in the `main.lua` file, and spawn it in the
scene.

```lua
local Player = require("player")

sucata.scene.spawn(Player(480, 500)) -- Spawn the player in the center of the screen
```

The game should show like this:

![Player Entity](./images/first-entity-draw.png)

Now we will make the player move around the screen using the arrow keys.

to get the input from the player we will use the `sucata.input`, and we need to get the delta, that is the time passed between frames.

```lua

function Player:update() -- This a callback from sucata that be called all frame
	local delta = sucata.time.get_delta() -- The time between frames
	if sucata.input.is_held("a", "left") then -- Check if the keys "a" or "left arrow" are pressed
		self.x = self.x - self.speed * delta -- Add a value to x 
	end
	if sucata.input.is_held("d", "right") then
		self.x = self.x + self.speed * delta
	end
end

```
