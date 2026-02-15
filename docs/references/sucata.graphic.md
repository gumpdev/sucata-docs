# sucata.graphic

The graphic module of the Sucata.

---

## RectProps

Properties used to draw a rectangle.

**fields**
- x? `number` - The x position (default: 0)  
- y? `number` - The y position (default: 0)  
- width? `number` - The width (default: 50)  
- height? `number` - The height (default: 50)  
- color? `string` - The color in hex format (default: "#ffffff")  
- z_index? `number` - The z-index for layering (default: 0)  
- texture? `string` - Path to texture file (default: "")  
- scale? `number` - Uniform scale factor (default: 1.0)  
- scale_x? `number` - Scale factor on X axis (default: 1.0)  
- scale_y? `number` - Scale factor on Y axis (default: 1.0)  
- fixed? `boolean` - Whether the rectangle is fixed to the screen (default: false)  
- origin? `number` - Uniform origin point (default: 0.0)  
- origin_x? `number` - Origin point on X axis (default: 0.0)  
- origin_y? `number` - Origin point on Y axis (default: 0.0)  
- rotation? `number` - Rotation in radians (default: 0.0)  
- opacity? `number` - Opacity value from 0.0 to 1.0 (default: 1.0)  
- atlas_size? `number` - Size of the texture atlas (default: 0.0)  
- atlas_width? `number` - Width of each frame in the texture atlas (default: 0.0)  
- atlas_height? `number` - Height of each frame in the texture atlas (default: 0.0)  
- atlas_spacing? `number` - Spacing between frames in the texture atlas (default: 0.0)  
- atlas_margin? `number` - Margin around the frames in the texture atlas (default: 0.0)  
- atlas_x? `number` - X index of the frame in the texture atlas (default: 0.0)  
- atlas_y? `number` - Y index of the frame in the texture atlas (default: 0.0)  
- shader? `string` - ID of the shader to use (default: "")  
- shader_args? `table` - Arguments for shader rendering (default: {})  

---

## TextProps

Properties used to draw text.

**fields**
- x? `number` - The x position (default: 0)  
- y? `number` - The y position (default: 0)  
- text? `string` - The text to display (default: "")  
- size? `number` - The font size (default: 16)  
- font? `string` - Path to font file (default: "")  
- color? `string` - The color in hex format (default: "#ffffff")  
- z_index? `number` - The z-index for layering (default: 0)  
- scale? `number` - Uniform scale factor (default: 1.0)  
- scale_x? `number` - Scale factor on X axis (default: 1.0)  
- scale_y? `number` - Scale factor on Y axis (default: 1.0)  
- fixed? `boolean` - Whether the text is fixed to the screen (default: false)  
- origin? `number` - Uniform origin point (default: 0.0)  
- origin_x? `number` - Origin point on X axis (default: 0.0)  
- origin_y? `number` - Origin point on Y axis (default: 0.0)  
- rotation? `number` - Rotation in radians (default: 0.0)  
- opacity? `number` - Opacity value from 0.0 to 1.0 (default: 1.0)  
- align? `string` - Text alignment: `"left"`, `"center"`, or `"right"` (default: `"left"`)  
- max_width? `number` - Maximum width of the text (default: 0.0)  
- shader? `string` - ID of the shader to use (default: "")  
- shader_args? `table` - Arguments for shader rendering (default: {})  

---

## sucata.graphic.draw_rect

Draws a rectangle.

**parameters**
- props `RectProps` - Properties for the rectangle  

---

## sucata.graphic.draw_text

Draws text.

**parameters**
- props `TextProps` - Properties for the text  

---

## sucata.graphic.set_background_color

Sets the background color of the window.

**parameters**
- color `string` - Hex color string (e.g., `"#RRGGBB"` or `"#RRGGBBAA"`)  

---

## sucata.graphic.load_shader

Loads a Sucata shader.

**parameters**
- path `string` - File path to the Sucata shader  
- name? `string` - Optional shader name  

**return**
- shader_name `string` - The name of the shader  
