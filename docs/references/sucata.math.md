# sucata.math

The math module of the Sucata.

---

## Rect

Represents a rectangle in 2D space.

### fields
- x `number` - The x position  
- y `number` - The y position  
- width `number` - The width  
- height `number` - The height  

---

## ScreenRelativeRect

Represents a rectangle using screen-relative percentages (0–1).

### fields
- top? `number` - Top position as percentage (0–1) (default: 0)  
- left? `number` - Left position as percentage (0–1) (default: 0)  
- right? `number` - Right position as percentage (0–1) (default: 0)  
- bottom? `number` - Bottom position as percentage (0–1) (default: 0)  

---

## sucata.math.clamp(value, min, max)

Clamps a value between a minimum and maximum.

**parameters**
- value `number` - The value to clamp  
- min `number` - The minimum value  
- max `number` - The maximum value  

**return**
- clamped `number` - The clamped value  

---

## sucata.math.distance(point1, point2)

Calculates the distance between two points.

**parameters**
- point1 `table` - First point with `x` and `y` fields  
- point2 `table` - Second point with `x` and `y` fields  

**return**
- distance `number` - The distance between the points  

---

## sucata.math.lerp(a, b, t)

Performs linear interpolation between two values.

**parameters**
- a `number` - The start value  
- b `number` - The end value  
- t `number` - The interpolation factor (0–1)  

**return**
- result `number` - The interpolated value  

---

## sucata.math.overlapping(rect1, rect2)

Checks if two rectangles are overlapping and returns the intersection.

**parameters**
- rect1 `Rect` - First rectangle with `x`, `y`, `width`, `height`  
- rect2 `Rect` - Second rectangle with `x`, `y`, `width`, `height`  

**return**
- overlapping `boolean` - Whether the rectangles overlap  
- intersection `Rect | nil` - The intersection rectangle if overlapping, `nil` otherwise  

---

## sucata.math.screen_relative(rect)

Converts screen-relative coordinates to pixel coordinates.

**parameters**
- rect `ScreenRelativeRect` - Rectangle with `top`, `left`, `right`, `bottom` as percentages (0–1)  

**return**
- x `number` - The x position in pixels  
- y `number` - The y position in pixels  
- width `number` - The width in pixels  
- height `number` - The height in pixels  

---

## sucata.math.smooth_index(current_time, interval, max_time?)

Converts time into integer steps based on an interval.

**parameters**
- current_time `number` - The current time (accumulated delta time)  
- interval `number` - The interval time in seconds  
- max_time? `number` - The maximum time to cap the result (optional)  

**return**
- index `number` - The calculated integer index  

---

## sucata.math.normalize(...)

Normalizes a vector (accepts a variable number of components).

**parameters**
- ... `number` - Vector components (`x`, `y`, `z`, etc.)  

**return**
- ... `number` - Normalized vector components (same count as input)  

---

## sucata.math.move_towards(current, target, step)

Moves a value towards a target by a maximum step.

**parameters**
- current `number` - The current value  
- target `number` - The target value  
- step `number` - The maximum step to move per call  

**return**
- result `number` - The new value moved towards the target  
