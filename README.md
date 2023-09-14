# Project: Pineapple
## Initial functionality requirements include:

- File Display: I'm considering a tree dll—widely adopted—for GUI construction. While the explorer shell is an option, it's quite antiquated. A modernized interface is preferable.
{Research windows GUI libraries compatible with tree dll or its alternatives}

- File Access: Autohotkey simplifies this, but the design needs to be efficient, coherent, maintainable, and omnipresent.

- Open Files: The objective is to change autohotkey configurations based on varying contexts. While the run command is one option, it's crucial to document every ahk_exe, class combo, and the application's window title protocol. A nimble database would be apt for tracking open windows and their contexts. The project might integrate both ahk and C, or perhaps Rust for added flair. Utilizing non-standard apps like VLC instead of Windows Media Player, which offer greater command line utility, is likely.

- Core Architecture: Both the engine and GUI must be versatile and adaptive to the context system and script library alterations.

- Context System: This will be somewhat of a database, keeping track of file windows and their contexts.

- Configuration System: A system state and event definition that activates scripts.

- Script Library: A compilation of scripts triggered by the configuration system with access to the context system.

- Command Line Interface: The GUI will offer basic text input for command and script execution and modifying context system variables.

- GUI: A display unit for the filesystem, context, configuration system, and script library. However, primary interaction is expected via input line commands rather than mouse actions.

- File Types:
 .ahk
 .txt
 .csv
 (audio/video)
 .mp4
 .mkv
 .gif
 .png
 .jpg
 .pdf

- File Information:
 - File name
 - File path
 - File type
 - Thumbnail

Big Picture:
 [] Open file window with default application
 [] Open with a specific app based on configuration
 [] Batch open files in specified apps
 [] Track open file windows (might be resource-consuming)
 [] Resize and place file window by context, file name (or ID), type, and other open windows
 [] Modify hotkey configurations for an opened, closed, or focused file window
 [] Launch multiple GUI windows with the same global and local context

### Todo:

 [] Display the file system in the GUI
 [] Traverse the file system
 [] Open files
 [] Keep track of open file windows
 [] Develop the command line interface
 [] Settle on the design of the core codebase and script library
 [] Execute scripts from the command line interface and a context system that exposes file windows to scripts


## Script Library:

 [] Define the design of the configuration system, including where and how the context system will be accessed
 [] Script to open files in a non-default specific app
 [] Script to position a file window in a predetermined screen location

