# sucata.time

The time module of the Sucata game engine.

---

## Timer

Configuration table used to create timers.

**fields**

- time `number`  
  The duration of the timer in seconds.

- auto_start? `boolean`  
  Whether the timer should start automatically (default: `true`).

- one_shot? `boolean`  
  Whether the timer should only run once (default: `true`).

- loop? `boolean`  
  Whether the timer should loop (default: `false`).

---

## sucata.time.get_delta

Gets the delta time (time elapsed since last frame) in seconds, multiplied by the current time scale.

**return**

- delta `number` - The delta time in seconds  

---

## sucata.time.get_fps

Gets the current frames per second.

**return**

- fps `number` - The current FPS  

---

## sucata.time.create_timer

Creates a timer with a callback function.

**parameters**

- callback `function` - The function to call when the timer expires  
- config `number | Timer` - Timer duration in seconds, or a timer configuration table  

**return**

- timer_id `string` - The ID of the created timer  

---

## sucata.time.pause_timer

Pauses a timer.

**parameters**

- timer_id `string` - The ID of the timer to pause  

---

## sucata.time.stop_timer

Stops a timer.

**parameters**

- timer_id `string` - The ID of the timer to stop  

---

## sucata.time.get_time_scale

Gets the current time scale value.

**return**

- time_scale `number` - The current time scale value  

---

## sucata.time.set_time_scale

Sets the time scale.

**parameters**

- time_scale `number` - The new time scale value  
