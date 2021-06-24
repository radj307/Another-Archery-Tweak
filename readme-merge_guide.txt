//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

Another Archery Tweak - Merging AAT with zEdit


DIFFICULTY: 
		Very Easy

		
REQUIREMENTS:
		zEdit setup & configured for your mod manager.	( https://github.com/z-edit/zedit/releases )
		All AAT .esp files active in your load order.

		
PROCESS:		
		1.	Open zEdit, select "zMerge" in the dropdown.
		
		2.	Click "Create Merge" at the bottom, a pop-up will open with 4 tabs. Steps for each are below:
		
		3.	(Details)
			Name:		Name of the new mod folder, as it will appear in your mod manager.
			Filename:	Name of the new merged ESP. I recommend naming it "Another_Archer_Tweak.esp", 
						Ignore the "A plugin with this filename already exists" warning.
			Method:		"Clean - Merge down (improved)"
		
		4.	(Plugins)
			Select all of the plugins beginning with "Another_Archery_Tweak"
			
		5.	(Load Order)
			Select "Use game load order"
			
		6.	(Data)
			Open the "INI Files" dropdown, ensure "Handle INI Files" is checked if you want the ini tweaks. (Defaults to On)
			Open the "General Assets" dropdown, check "Copy General Assets" if you want the readme to be included. (Defaults to Off)

		7.	Click the "Ok" button, then you should see the merge you just created in the center panel. 
		
		8.	Click "Build" next to the name, and wait for the process to complete.
		
		9.	When its done building, close zEdit. It will make a new mod folder located at the path you set in the zEdit settings.
			Activate the merged mod, and deactivate the original mod. Make sure the plugin is active, then run LOOT.
			It should be placed below any mods that edit the same settings, like WACCF (Weapons Armor Clothing & Clutter Fixes.esp)
				
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////