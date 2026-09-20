================================================================================
  MAKE YOUR OWN SHUTTLE
  A template for Odyssey Shuttle Skin-Job
================================================================================

This folder is a small, complete mod that adds one more shuttle to the game.
It already works. You only change what you want to be different.

You do not need to know anything about modding. Everything here is plain text,
and Notepad is all you need.


--------------------------------------------------------------------------------
  ONE THING TO GET RIGHT FIRST
--------------------------------------------------------------------------------

Pick your defName BEFORE you build the shuttle in a save.

defName is the line <defName>MYSHUTTLE</defName> in Defs\MyShuttle.xml. It is
not the name you see in game - that one is <label> - it is how your save finds
the shuttle again when you load it.

Changing that defName later - or turning this mod off, or deleting it - makes
every shuttle you have already built disappear from that save, together with
everyone and everything inside.

Changing anything else is safe at any time: label, description, cost, cargo,
fuel, range, pictures. Only the defName is set in stone once you have built one.


--------------------------------------------------------------------------------
  THE THREE STEPS
--------------------------------------------------------------------------------

1. COPY this whole folder into RimWorld's own Mods folder:

        ...\RimWorld\Mods\

   Do not leave it inside the Odyssey Shuttle Skin-Job folder, and do not edit
   files in there. Steam can overwrite or delete anything inside a Workshop
   folder whenever that mod updates - your work would be gone without warning.

2. NAME IT. Open Defs\MyShuttle.xml in any text editor.

   Use "Replace all" to turn every MYSHUTTLE into a name of your own.
   Letters only, no spaces - for example "RedRocket".
   (only exception: <label>MYSHUTTLE</label> can be <label>Red Rocket</label>)


3. ENABLE it in RimWorld's mod list, below Odyssey Shuttle Skin-Job.

   In the mod list it is still called "OSSJ - Custom Shuttle Mod". If you would
   rather see your own title there, change <name> in About\About.xml.

That is all. After the Shuttles research your shuttle shows up in the Odyssey
tab of the build menu. It still looks like the vanilla shuttle - see below.


--------------------------------------------------------------------------------
  YOUR OWN LOOK
--------------------------------------------------------------------------------

1. Rename the folder Textures\MYSHUTTLE to the name you picked.

2. Put three pictures in it, named after your shuttle:

        RedRocket_north.png     seen from above, nose pointing up
        RedRocket_east.png      seen from above, nose pointing right
        RedRocket_south.png     seen from above, nose pointing down

   West is mirrored from east automatically, so you do not need it.
   Use PNG with a transparent background. Around 500x500 pixels is plenty.

3. In Defs\MyShuttle.xml, follow the note in the LOOK section.

If the picture looks stretched or too small in game, change drawSize.


--------------------------------------------------------------------------------
  YOUR OWN NUMBERS
--------------------------------------------------------------------------------

Every line marked CHANGE in Defs\MyShuttle.xml is yours: name, description,
build cost, hit points, cargo, fuel tank, range and picture size.

The values in the file are the ones of the vanilla passenger shuttle. Anything
smaller gives you a lighter shuttle, anything bigger a heavier one.


--------------------------------------------------------------------------------
  IF SOMETHING GOES WRONG
--------------------------------------------------------------------------------

Red errors when the game starts, or your shuttle never shows up in the build
menu: something in the .xml got broken. A single missing < or > is enough.

The quickest fix is to start over: delete your copy and copy the template folder
again. Nothing else in your game is affected - but mind the defName warning at
the top of this file if you have already built one in a save.


--------------------------------------------------------------------------------
  A SECOND SHUTTLE
--------------------------------------------------------------------------------

Copy the template folder again and pick a different name. Also change the
packageId line in About\About.xml - no two mods can share the same one.
You must also then change in your second copy in Defs\MyShuttle.xml
at least the <defName> again.
No two same defNames are allowed to exist at the same time.


--------------------------------------------------------------------------------
  WHAT YOU GET FROM ODYSSEY SHUTTLE SKIN-JOB
--------------------------------------------------------------------------------

Your shuttle carries one part from that mod (the last entry under <comps>).
It gives you the Rotate and Reposition buttons, and it keeps your own picture
while the shuttle is flying. Leave it in.

Hope you will have fun with your own shuttles!
