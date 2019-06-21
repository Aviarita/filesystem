# Filesystem library

Table of Content

[**open_file**](https://github.com/Aviarita/filesystem/blob/master/README.md#open_filefilename-pathid-mode)<br>
[**read_file**](https://github.com/Aviarita/filesystem/blob/master/README.md#read_filefilename-pathid)<br>
[**write_file**](https://github.com/Aviarita/filesystem/blob/master/README.md#write_filefilename-pathid-text)<br>
[**append_file**](https://github.com/Aviarita/filesystem/blob/master/README.md#append_filefilename-pathid-text)<br>
[**file:read**](https://github.com/Aviarita/filesystem/blob/master/README.md#fileread)<br>
[**file:write**](https://github.com/Aviarita/filesystem/blob/master/README.md#filewritetext)<br>
[**file:clear**](https://github.com/Aviarita/filesystem/blob/master/README.md#fileclear)<br>
[**file:close**](https://github.com/Aviarita/filesystem/blob/master/README.md#fileclose)<br>

### open_file(filename, [pathid](https://github.com/Aviarita/filesystem/blob/master/README.md#paths-ids), [mode](https://github.com/Aviarita/filesystem/blob/master/README.md#modes))
    filename - name of the file you want to open
    path id - pathid of the path where the file will be created/opened in/from
    Returns a table with the following functions.
    
### read_file(filename, [pathid](https://github.com/Aviarita/filesystem/blob/master/README.md#paths-ids))
    filename - name of the file you want to open
    path id - pathid of the path where the file will be created/opened in/from
    Returns the content of the file.
    
### write_file(filename, [pathid](https://github.com/Aviarita/filesystem/blob/master/README.md#paths-ids), text)
    filename - name of the file you want to open
    path id - pathid of the path where the file will be created/opened in/from
    text - text you want to write to the text
    Returns the size of the file.
    
### append_file(filename, [pathid](https://github.com/Aviarita/filesystem/blob/master/README.md#paths-ids), text)
    filename - name of the file you want to open
    path id - pathid of the path where the file will be created/opened in/from
    text - text you want to write to the text
    Returns the size of the file.

### file:read()
    Returns the content of the file.
    
### file:write(text)
    text - text you want to write to the text
    Writes the given text ot the file.
    
### file:clear()
    Clears the file.
    
### file:close()
    Closes the file.

### Paths IDs
    MOD
        The first SearchPath only.
    GAME
        All SearchPaths, including those inside GCFs.
    GAMEBIN
        The game binaries folder (client, server).
    EXECUTABLE_PATH
        The engine binaries folder.
    DEFAULT_WRITE_PATH
        Wherever the game is currently configured to write out to. Defaults to the first SearchPath.

### Modes
    [r]  Open for reading
    [w]  Create for writing (will overwrite existing)
    [a]  Append to
    [r+] Open for read/write
    [w+] Create for read/write
    [a+] Append to or create for read/write
    [b]  When used with any of the above, flags file as binary
