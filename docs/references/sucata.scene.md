# sucata.scene

The scene module of the Sucata.

---

## Entity

Represents a game object in the scene.

An `Entity` can contain lifecycle functions and any custom properties defined by the user.

### fields

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

## sucata.scene.load_scene(entities)

Loads a scene with the given entities.

### parameters
- entities `Entity[]` - Array of entity tables to load into the scene  

---

## sucata.scene.spawn(entity)

Spawns an entity in the scene.

### parameters
- entity `Entity` - The entity table to spawn  

### return
- entity_id `string` - The ID of the spawned entity  

---

## sucata.scene.spawns(entities)

Spawns multiple entities in the scene.

### parameters
- entities `Entity[]` - Array of entity tables to spawn  

### return
- entity_ids `string[]` - Array of IDs of the spawned entities  

---

## sucata.scene.find_by_id(entity_id)

Finds an entity by its ID.

### parameters
- entity_id `string` - The ID of the entity to find  

### return
- entity `Entity | nil` - The entity table or `nil` if not found  

---

## sucata.scene.destroy(entity_or_id)

Destroys an entity from the scene.

### parameters
- entity_or_id `Entity | string` - The entity table or entity ID to destroy  

### return
- success `boolean` - Whether the entity was successfully destroyed  

---

## sucata.scene.destroys(entities)

Destroys multiple entities from the scene.

### parameters
- entities `Entity[]` - Array of entity tables to destroy  

### return
- undestroyed_ids `string[]` - Array of IDs of entities that could not be destroyed  

---

## sucata.scene.add_tag(entity_or_id, tag)

Adds a tag to an entity.

### parameters
- entity_or_id `Entity | string` - The entity table or entity ID  
- tag `string` - The tag to add  

### return
- success `boolean` - Whether the tag was successfully added  

---

## sucata.scene.has_tag(entity_or_id, tag)

Checks if an entity has a tag.

### parameters
- entity_or_id `Entity | string` - The entity table or entity ID  
- tag `string` - The tag to check  

### return
- success `boolean` - Whether the entity has the tag  

---

## sucata.scene.remove_tag(entity_id, tag)

Removes a tag from an entity.

### parameters
- entity_id `string` - The ID of the entity  
- tag `string` - The tag to remove  

### return
- success `boolean` - Whether the tag was successfully removed  

---

## sucata.scene.get_entities()

Gets all entity IDs in the scene.

### return
- entity_ids `string[]` - Array of all entity IDs in the scene  

---

## sucata.scene.get_entities_by_tag(tag)

Gets all entity IDs with a specific tag.

### parameters
- tag `string` - The tag to filter by  

### return
- entity_ids `string[]` - Array of entity IDs with the given tag  

---

## sucata.scene.clear_entities()

Clears all entities from the scene.
