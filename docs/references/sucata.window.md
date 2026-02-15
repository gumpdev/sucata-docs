# sucata.window

The window module of the Sucata game engine.

---

## sucata.window.set_mouse_lock(locked)

Sets whether the mouse cursor is locked to the window.

**parameters**
- locked `boolean` - Whether to lock the mouse cursor  

---

## sucata.window.get_mouse_lock()

Gets whether the mouse cursor is locked to the window.

**return**
- locked `boolean` - Whether the mouse cursor is locked  

---

## sucata.window.set_mouse_visible(visible)

Sets whether the mouse cursor is visible.

**parameters**
- visible `boolean` - Whether the mouse cursor should be visible  

---

## sucata.window.get_mouse_visible()

Gets whether the mouse cursor is visible.

**return**
- visible `boolean` - Whether the mouse cursor is visible  

---

## sucata.window.set_window_title(title)

Sets the window title.

**parameters**
- title `string` - The new window title  

---

## sucata.window.get_window_title()

Gets the current window title.

**return**
- title `string` - The current window title  

---

## sucata.window.set_window_size(width, height)

Sets the window size.

**parameters**
- width `number` - The new window width in pixels  
- height `number` - The new window height in pixels  

---

## sucata.window.get_window_size()

Gets the current window size.

**return**
- width `number` - The current window width in pixels  
- height `number` - The current window height in pixels  

---

## sucata.window.set_fullscreen(fullscreen)

Sets whether the window is in fullscreen mode.

**parameters**
- fullscreen `boolean` - Whether the window should be fullscreen  

---

## sucata.window.get_fullscreen()

Gets whether the window is in fullscreen mode.

**return**
- fullscreen `boolean` - Whether the window is fullscreen  

---

## sucata.window.set_vsync(vsync)

Sets the vsync mode.

**parameters**
- vsync `number` - The vsync mode (`0` = off, `1` = on, higher values for specific intervals)  

---

## sucata.window.get_vsync()

Gets the current vsync mode.

**return**
- vsync `number` - The current vsync mode  

---

## sucata.window.quit()

Quits the application.

---

## sucata.window.show_debug_info(show)

Sets whether to show debug information.

**parameters**
- show `boolean` - Whether to show debug information  

---

## sucata.window.set_keep_aspect(keep)

Sets whether to keep the aspect ratio with black bars.

**parameters**
- keep `number` - Whether to maintain the aspect ratio  
  - `0` = off  
  - `1` = keep aspect with bars  
  - `2` = keep aspect with crop  

---

## sucata.window.get_keep_aspect()

Gets whether the window keeps aspect ratio with black bars.

**return**
- keep `number` - Whether aspect ratio is maintained  
  - `0` = off  
  - `1` = keep aspect with bars  
  - `2` = keep aspect with crop  

---

## sucata.window.set_window_icon(path)

Sets the window icon from a file path.

**parameters**
- path `string` - The file path to the icon image  

---

## sucata.window.get_window_icon()

Gets the current window icon path.

**return**
- path `string` - The file path of the current window icon  
