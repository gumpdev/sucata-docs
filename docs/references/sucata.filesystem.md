# sucata.filesystem

The filesystem module of the Sucata.

---

## sucata.filesystem.exists

Checks if a file or directory exists.

**parameters**

- path `string` - Path of the file or directory to check  

**return**

- exists `boolean` - `true` if the file/directory exists, `false` otherwise  

---

## sucata.filesystem.remove

Removes a file or directory.

**parameters**

- path `string` - Path of the file or directory to remove  

---

## sucata.filesystem.mkdir

Creates a new directory.

**parameters**

- path `string` - Path of the directory to create  

---

## sucata.filesystem.read_file

Reads the contents of a file as a string.

**parameters**

- path `string` - Path of the file to read  

**return**

- content `string | nil` - The file contents as a string, or `nil` on error  

---

## sucata.filesystem.read_dir

Lists the contents of a directory.

**parameters**

- path `string` - Path of the directory to read  

**return**

- files `table | nil` - Table with file/directory names, or `nil` on error  

---

## sucata.filesystem.write

Writes content to a file.

**parameters**

- path `string` - Path of the file to write  
- content `string` - Content to write to the file  

**return**

- success `boolean` - `true` if the write was successful, `false` otherwise  

---

## sucata.filesystem.rename

Renames a file or directory.

**parameters**

- old_path `string` - Current path of the file or directory  
- new_path `string` - New path of the file or directory  
