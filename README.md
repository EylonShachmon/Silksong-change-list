# Silksong-change-list
Almost every code change (AssemblyCsharp.dll) in silksong from release untill Patch 5 (1.0.3), manually annotated by me. Not being actively maintained for future updates


Notes: 

Created by Eylonsh. If needed, please contact me on Discord (Username "eylonsh", active on the wiki server and on the modding server). This version is updated as of the 22nd of September 2026.

These are not *all* the changes, it is only the changes in Assembly-CSharp.dll

Also, while every file that had changes is listed here, and I tried to write down all the changes, I sometimes skipped a few, and only mentioned the more important ones. 

The explanations are what I understood, and although I am confident in most of them, they could be wrong!

the "Number:" at the start is just what place inside Assembly-CSharp.dll that file is, sorted alphabetically. It is not fully consistent between patches because some files were created/deleted, but the stay roughly the same.

The numbers (position, line, place) before the "//" are according to the previous version, "position" is the place of the first character that is difference, "line" is the first line that is different, "place" is the character in that line.

After the "//", the numbers are according to the later version, "Line" means the change is in that specific line, "Lines" means from that line and a bit onwards (I tried to keep it roughly meaning 'Withing this scope' but I'm not promising anything). if the changes are inside a method/function, I added "in FunctionName()", if I haven't that probably means those changes were to a field/property.
"Line" that falls on a method's definition usually means the arguments were updated, "Lines" on a method's name usually means the method is new to this update.

If a change's lines point to an empty space/something that is obviously not related, that usually means the change was a deleted line, and that is where the line would be, were it not deleted.

The versions have been downloaded from steam and the code from Assembly-CSharp.dll was extracted using ILSpy. using a difference method might result in slightly different Line numbers.

If you followed the same process as me, you'd get a few files with changes, always the same 11 in each update. That change is the update number, Team Cherry had somewhere a public string they reused, that got inlined on compilation. I have removed the files were this was the only change, as it just makes the list harder to read.
These files are: Constants.cs, GameManager.cs, OnScreenDebugInfo.cs, PlayerData.cs, RestorePointData.cs, RestorePointFileWrapper.cs, SaveDataUpgradeHandler.cs, SaveRestoreHandler.cs, SetVersionNumber.cs, UnityEngine.UI\RestoreSaveButton.cs, UnityEngine.UI\SaveSlotButton.cs
Weirdly in some versions the string didn't get inlined (maybe because it's not a const), and if that happens in the same file twice in a row, a change doesn't show. Except for that, these same 11 files will always have this same change on each update.
(If you do want to do it yourself for some reason, the code to get the list of changes, as well as an explanation on how to use it, is supposed to be in a file sent together with this one, at least if you found this in the discord modding server. If you can't find it, you can ping me on discord and I'll send it)

Copyright stuff: I of course do not own the actual information, so I can't (and I don't want to) stop you from using this as a resource, if you need to find a change or want to know how your mod would hold to back-patching, I hope I helped. 
You are however **not allowed** to use the list itself (i.e. my explanations) for commercial stuff, this mainly means you are not allowed to make a video of you basically reading this out, or to fancify it and then put it behind a paywal.

