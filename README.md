# AppleScripts
AppleScripts for use with OS X / macOS (tested in 10.9 Mavericks)

## AppleScript droplet for pandoc file conversion
This script provides a graphical front end for [Pandoc](https://pandoc.org). Just [save it as an AppleScript droplet](https://developer.apple.com/library/content/documentation/LanguagesUtilities/Conceptual/MacAutomationScriptingGuide/SaveaScript.html), and then drop files onto it that you want to convert. Read the comments in the script before running it.

## AppleScript droplet to create symbolic link
This script asks for a destination folder and creates symbolic links in that folder to whatever you drop onto it. Just [save it as an AppleScript droplet](https://developer.apple.com/library/content/documentation/LanguagesUtilities/Conceptual/MacAutomationScriptingGuide/SaveaScript.html), and then drop files or folders onto it that you want to link. The script ignores .webloc files since AppleScript treats those as URLs instead of as files.

## AppleScript service to create file with specified creation date
This script asks for a date and time and then creates an HTML file with that creation date and opens it for editing in TextEdit. Just [save it as a systemwide service](https://developer.apple.com/library/content/documentation/LanguagesUtilities/Conceptual/MacAutomationScriptingGuide/MakeaSystem-WideService.html) (a [Services menu](https://en.wikipedia.org/wiki/Services_menu) item) and [assign a keyboard shortcut to it](https://support.apple.com/kb/PH25372), and then press the keyboard shortcut to create and open a TextEdit HTML file with specified creation date. I use this in conjunction with WordService's "Insert Short Date & Time" command ([free from DEVONtechnologies](http://www.devontechnologies.com/products/freeware.html)) to create journal entries. The reason why the script prompts for a date is that some of my journal entries were written at an earlier date and time, so I want to be able to specify a creation date other than the current date and time when necessary. It is also possible to use this script with Apple's built-in [dictation commands](https://developer.apple.com/library/content/documentation/LanguagesUtilities/Conceptual/MacAutomationScriptingGuide/UseDictationtoRunScripts.html) and [text dictation](https://support.apple.com/en-us/HT202584) for journaling or notetaking entirely by voice. The value of the property *save_path* and the property *resource_fork_path* in the script will need to be edited before the script is run; the latter value should be the POSIX path to the file *TextEdit.r* (included in the same directory as the file you are reading). Read the comments in the script before running it.
