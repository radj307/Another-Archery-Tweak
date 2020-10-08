Another Archery Tweak

I recommend merging the main file (Another_Archery_Tweak.esp) with any addon files you may have downloaded.
All .esp files are flagged as ESL, but there's no reason to have all 3 active.

Short guide to merging:
	xEdit Method (Safer)
		1.	Open xEdit and activate only the plugins from this mod, and their masters.
		2.	Open the addon entries on the left pane, and R-Click on "Projectiles"
		3.	Select "Deep copy as override into..."
		4.	Select Another_Archery_Tweak.esp and click "Yes" when it asks if you want to add masters
		5.	Repeat steps 2-4 for any other addons.
		6.	Once done, de-activate the main mod & its addons.
		Done!
	zEdit Method (Automated)
	Since none of this mod's esp files directly conflict with each other, you may prefer to use zMerge's automated system.
		1.	Activate the main file & addon files.
		2.	Open zMerge
		3.	Click "Create Merge" at the bottom
		4.	Under "Details" select "Clean - Merge down (improved)" for merge method, and you can name the plugin & mod folder.
		(IMPORTANT) If you have already installed and made new saves with any of this mod's ESPs active,
					you should name the .esp "Another_Archery_Tweak.esp". It will warn you about a plugin of the same
					name already existing, which is fine.
		5.	Under "Plugins" select all of this mod's ESPs
		6.	Under "Load Order" check the "Use game load order" box
		7.	You can safely ignore the Data tab, click "OK"
		8.	Click "Build Merge" next to the merge's name, or "Build Merges" to build all merges.
		9.	Once done, de-activate the main mod & its addons.
		Done!