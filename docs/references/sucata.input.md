# sucata.input

The input module of the Sucata.

---

## Key

Input key and button names.

**values**
- `"mouse_left"`
- `"mouse_right"`
- `"mouse_middle"`
- `"a"` to `"z"`
- `"space"`
- `" "` (space character)
- `"escape"`
- `"esc"`
- `"enter"`
- `"return"`
- `"shift"`
- `"ctrl"`
- `"control"`
- `"alt"`
- `"up"`
- `"down"`
- `"left"`
- `"right"`

---

## sucata.input.get_mouse_position

Gets the current mouse position.

**return**
- x `number` - The x coordinate of the mouse  
- y `number` - The y coordinate of the mouse  

---

## sucata.input.get_mouse_scroll

Gets the current mouse scroll values.

**return**
- x `number` - The horizontal scroll value  
- y `number` - The vertical scroll value  

---

## sucata.input.get_key

Gets the last pressed key character code.

**return**
- key_code `number` - The character code of the last pressed key  

---

## sucata.input.is_pressed

Checks if any of the given keys or buttons were pressed this frame.

**parameters**
- ... `Key` - Key or button names to check  

**return**
- pressed `boolean` - Whether any of the keys/buttons were pressed  

---

## sucata.input.is_held

Checks if any of the given keys or buttons are currently held down.

**parameters**
- ... `Key` - Key or button names to check  

**return**
- held `boolean` - Whether any of the keys/buttons are held  

---

## sucata.input.is_released

Checks if any of the given keys or buttons were released this frame.

**parameters**
- ... `Key` - Key or button names to check  

**return**
- released `boolean` - Whether any of the keys/buttons were released  

---

## sucata.input.is_hover

Checks if the mouse is hovering over a specific area for an entity.

**parameters**
- entity `string | table` - The entity ID or entity table  
- area `table`
  - x `number` - X position of the area  
  - y `number` - Y position of the area  
  - width `number` - Width of the area  
  - height `number` - Height of the area  
  - z_index? `number` - Z-index for layering (optional)  
  - fixed? `boolean` - Whether the area is fixed to the screen (optional)  

**return**
- hovering `boolean` - Whether the mouse is hovering over the specified area  
