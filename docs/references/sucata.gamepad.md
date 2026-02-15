# sucata.gamepad

The gamepad module of the Sucata.

---

## Axis

Gamepad axis and trigger names.

### values
- `"left_x"`
- `"left_y"`
- `"right_x"`
- `"right_y"`
- `"trigger_left"`
- `"trigger_right"`

---

## Button

Gamepad button names.

### values
- `"a"`
- `"b"`
- `"x"`
- `"y"`
- `"back"`
- `"guide"`
- `"start"`
- `"left_stick"`
- `"right_stick"`
- `"left_shoulder"`
- `"right_shoulder"`
- `"dpad_up"`
- `"dpad_down"`
- `"dpad_left"`
- `"dpad_right"`

---

## sucata.gamepad.get_count()

Gets the number of currently connected gamepads.

### return
- count `number` - The number of gamepads connected  

---

## sucata.gamepad.get_axis(axis, device?)

Gets the axis value of a gamepad.

### parameters
- axis `Axis` - The gamepad axis  
- device? `number` - The number of the device (optional)  

### return
- value `number` - The value of the axis  
- device_used `number` - The device used  

---

## sucata.gamepad.is_held(button, device?)

Checks if a button is currently held on the gamepad.

### parameters
- button `Button` - The gamepad button  
- device? `number` - The number of the device (optional)  

### return
- value `boolean` - `true` if the button is currently held  
- device_used `number` - The device used  

---

## sucata.gamepad.is_pressed(button, device?)

Checks if a button was pressed on the gamepad (only on the frame it was pressed).

### parameters
- button `Button` - The gamepad button  
- device? `number` - The number of the device (optional)  

### return
- value `boolean` - `true` if the button is pressed  
- device_used `number` - The device used  

---

## sucata.gamepad.is_released(button, device?)

Checks if a button was released on the gamepad.

### parameters
- button `Button` - The gamepad button  
- device? `number` - The number of the device (optional)  

### return
- value `boolean` - `true` if the button is released  
- device_used `number` - The device used  
