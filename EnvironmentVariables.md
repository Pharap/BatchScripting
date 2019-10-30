# Environment Variables

## Special Functions

### `%PATH%`

Stores a semicolon separated list of paths to directories that will be searched when the command line is trying to identify a command.

Specifically when a command is given to `cmd`, if the first 'word' of the command is not a built-in and no such file is present in the current directory then `cmd` will iterate through the entries in `%PATH%` and look for the command in each of the specified directories. If it finds a suitable match then it will use the first match it finds, otherwise if it finds no match it will report an error.

### `%PATHEXT%`

Stores a semicolon separated list of file extensions that `cmd` will try to substitute onto the first 'word' of a command in order to resolve the command to a particular program.

## System Data

### `%OS%`

Typically `Windows_NT`.

### `%COMPUTERNAME%`

The 'name' given to the computer.

### `%NUMBER_OF_PROCESSORS%`

### `%PROCESSOR_ARCHITECTURE%`

E.g. `AMD64`

### `%PROCESSOR_IDENTIFIER%`

### `%PROCESSOR_LEVEL%`

### `%PROCESSOR_REVISION%`

## User Data

### `%USERNAME%`

The active user profile's username.

### `%USERDOMAIN%`

Typically the 'name' of the computer (i.e. `%COMPUTERNAME%`).

### `%USERDOMAIN_ROAMINGPROFILE%`

Typically the same as `%USERDOMAIN%`.

### `%USERPROFILE%`

Typically `\Users\<username>` where `<username>` is the name of the active user (i.e. `%USERNAME%`).

## Drives

### `%HOMEDRIVE%`

Typically `C:`.

### `%SystemDrive%`

Typically `C:`.

## Special Folders

### `%windir`

Typically `C:\Windows`.

### `%SystemRoot%`

Typically `C:\Windows`.

### `%ProgramData%`

Typically `C:\ProgramData`.

### `%ProgramFiles%`

Typically `C:\Program Files`.

### `%ProgramFiles(x86)%`

Typically `C:\Program Files (x86)`

### `%APPDATA%`

Where 'roaming' (shared between users) application data is kept.

### `%LOCALAPPDATA%`

Where 'local' (user-specific) application data is kept.

### `%HOMEPATH%`

Typically `\Users\<username>` where `<username>` is the name of the active user (i.e. `%USERNAME%`).

### `%PUBLIC%`

Typically `C:\Users\Public`

### `%TEMP%`

Temporary folder.

### `%TMP%`

Temporary folder. _Should_ be the same as `%TEMP%`, but might not be.

## Misc

### `%ComSpec%`

Typically `C:\Windows\system32\cmd.exe`.

## Unknown

### `%PROMPT%`

### `%ALLUSERSPROFILE%`

### `%SESSIONNAME%`

### `%FP_NO_HOST_CHECK%`

### `%configsetroot%`

### `%LOGONSERVER%`

## Assorted Third Party

### `%PSModulePath%`

A semicolon-separated list of paths to Windows Power Shell module directories.

### `%DXSDK_DIR%`

A path to the directory of the Direct X Software Development Kit, if installed.

### `%VS120COMNTOOLS%`

A path to the Microsoft Visual Studio 12.0 Tools directory, if installed.

### `%VS140COMNTOOLS%`

A path to the Microsoft Visual Studio 14.0 Tools directory, if installed.

### `%VSSDK140Install%`

Something to do with the Microsoft Visual Studio 14.0 Visual Studio Software Development Kit?

### `%PLATFORMIO_HOME_DIR%`

A path to PlatformIO's 'home' directory, if installed.

### `%BESIEGE_GAME_ASSEMBLIES%`

Created by the game Besieged, if installed. Points to `steamapps/common/Besiege/Besiege_Data\Managed/`.

### `%BESIEGE_UNITY_ASSEMBLIES%`

Created by the game Besieged, if installed. Points to `steamapps/common/Besiege/Besiege_Data\Managed/`.