# sucata.audio

The audio module of the Sucata.

---

## sucata.audio.play(props)

Plays a sound and returns its ID.

### parameters
- props `table` - Properties for the audio
  - sound `string` - Path to the sound file
  - volume? `number` - Volume of the sound (default: 1.0)
  - pitch? `number` - Pitch of the sound (default: 1.0)
  - group? `string` - Audio group (default: "default")
  - loop? `boolean` - Whether the sound should loop (default: false)

### return
- sound_id `number` - The ID of the playing sound

---

## sucata.audio.stop(sound_id)

Stops a playing sound.

### parameters
- sound_id `number` - The ID of the sound to stop

---

## sucata.audio.pause(sound_id)

Pauses a playing sound.

### parameters
- sound_id `number` - The ID of the sound to pause

---

## sucata.audio.unpause(sound_id)

Unpauses a paused sound.

### parameters
- sound_id `number` - The ID of the sound to unpause

---

## sucata.audio.get_volume(sound_id)

Gets the volume of a specific sound.

### parameters
- sound_id `number` - The ID of the sound

### return
- volume `number` - The current volume of the sound

---

## sucata.audio.set_volume(sound_id, volume)

Sets the volume of a specific sound.

### parameters
- sound_id `number` - The ID of the sound
- volume `number` - The new volume level

---

## sucata.audio.get_pitch(sound_id)

Gets the pitch of a specific sound.

### parameters
- sound_id `number` - The ID of the sound

### return
- pitch `number` - The current pitch of the sound

---

## sucata.audio.set_pitch(sound_id, pitch)

Sets the pitch of a specific sound.

### parameters
- sound_id `number` - The ID of the sound
- pitch `number` - The new pitch level

---

## sucata.audio.get_group_volume(group_id)

Gets the volume of an audio group.

### parameters
- group_id `string` - The ID of the audio group

### return
- volume `number` - The current volume of the group

---

## sucata.audio.set_group_volume(group_id, volume)

Sets the volume of an audio group.

### parameters
- group_id `string` - The ID of the audio group
- volume `number` - The new volume level

---

## sucata.audio.get_group_pitch(group_id)

Gets the pitch of an audio group.

### parameters
- group_id `string` - The ID of the audio group

### return
- pitch `number` - The current pitch of the group

---

## sucata.audio.set_group_pitch(group_id, pitch)

Sets the pitch of an audio group.

### parameters
- group_id `string` - The ID of the audio group
- pitch `number` - The new pitch level
