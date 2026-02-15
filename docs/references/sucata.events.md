# sucata.events

The events module of the Sucata.

---

## Entity

Represents a game object in the Sucata engine.

An `Entity` can contain lifecycle functions and any custom properties defined by the user.

**fields**

- id? `string`  
  The unique identifier of the entity.  
  It will have a value when the entity is spawned.

- update? `function(self)`  
  The update function called every frame.  
  Receives `self` as parameter.

- draw? `function(self)`  
  The draw function called every frame.  
  Receives `self` as parameter.

- free? `function(self)`  
  The function called when the entity is destroyed.  
  Receives `self` as parameter.

- init? `function(self)`  
  The function called when the entity is spawned.  
  Receives `self` as parameter.

- [string] `any`  
  Custom properties.  
  You can add any additional fields you want to the entity.

---

## sucata.events.emit

Emits an event with the given name and optional data.

**parameters**

- name `string` - The name of the event  
- data `table` - Additional data to pass with the event  

---

## sucata.events.on

Registers a handler for an event.

**parameters**

- owner `string | Entity` - The entity owner of the handler (can be an entity table or entity ID)  
- name `string` - The name of the event  
- callback `function` - The function to call when the event is emitted  
