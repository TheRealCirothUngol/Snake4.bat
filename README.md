# Snake4.bat

I searched around online and couldn't find this referenced anywhere so I decided to
upload it here for posterity until someone tells me different. It's a marvelous little
batch file and hats off to it's author Dave Benham. It's loaded with novel WinNT
batch techniques and is actually a highly playable game. 

The world would be a sadder place if this were not available online somewhere.

on WaybackMachine
https://web.archive.org/web/20170606204830if_/http://www.dostips.com/forum/viewtopic.php?f=3&t=4741&sid=4c41f50fdc0ef6d185333ff7ab2a4fd6

    SNAKE.BAT - A pure native Windows batch implementation of the classic game
    ------------------------------------------------------------------------------
    Written by Dave Benham with some debugging help and technique pointers from
    DosTips users - See http://www.dostips.com/forum/viewtopic.php?f=3&t=4741
    
    The game should work on any Windows machine from XP onward using only batch
    and native external commands. However, the default configuration will most
    likely have some screen flicker due to the CLS command issued upon every 
    screen refresh. There are two ways to eliminate screen flicker:
    
    1 - "Pure batch" via VT100 escape sequences:
    You can eliminate flicker by enabling the VT100 mode within the game's
    Graphic options menu. However, this mode requires a console that supports
    VT100 escape sequences. This comes standard with Windows 10 (and beyond).
    The Windows 10 console must be configured properly for this to work - the
    "Legacy Console" option must be OFF. Prior to Windows 10, there was no
    standard Windows console that supported VT100 escape sequences, though you
    may find a utility that provides that support.
    
    2 - CursorPos.exe cheat from Aacini:
    You can eliminate screen flicker on any Windows version by placing Aacini's
    CursorPos.exe in the same folder that contains SNAKE.BAT. This method of
    eliminating flicker is "cheating" in that it is not pure native batch since
    it relies on a 3rd party tool. A script to create CursorPos.exe is available
    at http://goo.gl/hr6Kkn.
    
    Note that user preferences and high scores are stored in %USERPROFILE%\Snake
    User saved games have an implicit .snake.txt "extension", and are saved and
    loaded from the current directory.
    
