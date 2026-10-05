D2R : TINY MOD by Gimli#4667 (e-soni@d2jsp)


# Install instructions #
------------------------
Step 1: Go to your D2R install folder - like "C:\Program Files (x86)\Diablo II Resurrected\" and create in there a new folder called "mods"

Step 2: Extract/copy/move the files/folders from the zip/7z file into this folder.
		It should look like: C:\Program Files (x86)\Diablo II Resurrected\mods\tiny\tiny.mpq

Step 3: Go to your folder "C:\Users\YOURUSERNAMEHERE\Saved Games\Diablo II Resurrected" and create a folder called "mods".

Step 4: Go into that mods folder and create a folder called "tiny". In this folder you copy the file "Settings.json" from the zip/7z
		It should look like: C:\Users\YOURUSERNAMEHERE\Saved Games\Diablo II Resurrected\mods\tiny\Settings.json
		You may have to set up your ingame spell hotkeys back again (but only once)

Step 5: Open the Battle.net Launcher, click the "settings" icon (gearwheel), got to "game settings"
		Activate "additional command line arguments"
		Type in or attach to already used arguments "-mod tiny -txt"
		You can also use even more arguments like -ns for no sound for example.
		
Step 6: Start D2R and enjoy a faster game :D

Step 7: Optional: If you use a shortcut for loading with tiny mod, you can use the icon (tiny2.ico) i've made to divide the different shortcuts :)






# Option starting process #
---------------------------
Chobotz made some nice PowerShell scripts to start D2R with preset Informations without the battle.net launcher.
It is not a compilled exe file or something, you can 100% see the code in what it is doing (no hidden spyware etc.)
https://github.com/Chobotz/D2R-multiclient-tools

Give it a try if you want to :D





# Changelog History #
---------------------

# v1.2 (05.10.2026)
	- compatibility fix for patch 3.2 "Reign of the Warlock" (game version 1.34)
	- fixes the Warlock showing as "Missing String" in character select
	  and the error prompt on game start
	- removed the mod's stale copies of these files so the game's own
	  up-to-date versions are used again (they were unmodified vanilla
	  copies from patch 2.6, so nothing the mod actually does is lost):
	      data/local/lng/strings/ui.json
	      data/local/lng/strings-legacy/ui.json
	      data/local/lng/strings/levels.json
	      data/global/excel/missiles.txt
	      data/global/excel/sounds.txt
	      data/hd/character/monsters.json
	      data/global/ui/layouts/charactercreatepanelhd.json
	- side effect: the character creation screen is now the game's stock
	  layout (it has to be - it needs 8 class slots instead of 7)
	- added the missing data/global/dataversionbuild.txt (build 93847).
	  This mod never shipped it, so newer patches showed
	  "Data version mismatch detected ... Detected data version: Unknown"
	  on startup. Required to clear that dialog.
	  This number must be bumped on EVERY game patch - the correct value
	  is the "Current data version" shown in that error message.
	- NOTE on patch 3.2: legacy / classic graphics mode is GONE in Reign
	  of the Warlock. This is not a Warlock-only limitation - no class can
	  use it in RotW. It survives only in the separate Classic/LoD game
	  versions, so the old "press G to play" workflow no longer applies.
	  The filler/black-screen use case is UNAFFECTED - entering the game
	  to a black screen still works, because that comes from the blanked
	  HD assets and has nothing to do with the legacy toggle.
	  Confirmed working on 3.2.


# v1.1 (24.02.2023)
	- updated to patch 2.6


# v1.0 (24.11.2022)
	- reworked the menu
	- updated to patch 2.5 | game version: 1.4.71776
	- removed videos, music and all that sh*t
	- added info (press G to play)
	- renamed from blockhd to TINY (due different mods called blockhd)
	- Contact me for further improvements/ideas!