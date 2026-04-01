# LUDMAP-Map-and-Grand-Strategy-Tool-
In Browser html application. 
REQUIREMENTS: A BLACK AND WHITE IMAGE OF YOUR INTENDED MAP. (HARD REQUIREMENT!) /// A PURE BLACK BLOCK USING THE SAME RESOLUTION AS YOUR INTENDED MAP (HARD REQUIREMENT IF YOU WANT WATER!)
OPTIONAL: PUT RED BORDERS ON YOUR INTENDED MAP IF YOU WANT TO SPECIFIC BORDERS THAT ALWAYS OCCUR AT EXACT SPOTS /// OPTIONAL: A RGB PATTERN ON A BLACK BACKGROUND (WILL SAVE YOU TIME!)  
--- NOTE: the images i use personally are 6k, but i see no reason why smaller images should not suffice. just make sure they have the PNG file format. ---

NOTE: HIGHER RESOLUTION SHOULD RESOLVE TO BETTER DETAIL AROUND COASTLINES! 

--- HOW TO USE: CLICK ON REGION_GEN.html A WINDOW SHOULD OPEN IN YOUR BROWSER. ---
IN THE INPUT PANEL, PICK YOUR BLACK AND WHITE MAP AS THE PRIMARY PNG. PICK THE BLACK BLOCK AS THE WATER PNG.
IN THE GENERATION PANEL, DECIDE ON HOW MANY REGIONS YOU WANT ( if you want more regions, increase the land seed count) NUMBER AND SIZE OF OCEAN TILES ARE DETERMINED BY THE WATER GRID SIZE PARAMETER. 

click "generate regions" and the black viewport should show you your map, divided into regions of various colors, along with an ocean grid if you supplied a Water PNG. Every single region and ocean grid can be clicked on. Navigate the Viewport by zooming in and out with the scroolwheel. (Scroll always targets mouse position!)
/// NOTE: I RECOMMEND " BOX" OR "COMPLEX" AS THE GENERATION MODE! ///

the left hand panel is where most of your work will be done, it contains the name, color ID and parameters for the region. ( I WOULD NOT RECOMMEND CHANGING THE COLOR )

SOME OF THE PARAMETERS ARE HARDCODED INTO THE APPLICATION, BUT YOU CAN ADD YOUR OWN BY CLICKING ON "ADD DEFAULT PARAMETER"

SPLITTING AND MERGING: Click on a region, click on " MERGE MODE" in the left hand panel, click on the region you want merged into it. /// Click on "split selected region" to split any region. It's that simple. 

WATER MODE: at the top you have a toggle for "WATER FOCUS". Click on it if you want to edit Ocean Grids under the land continents. THIS MODE LIMITS INTERACTION TO OCEAN GRIDS ONLY! 
FACTION VIEW: Using this toggle, The map changes to visualize which factions control which part of the map. 

SUBDIVIDE OCEAN GRIDS: Rather than splitting an ocean Grid randomly, you can choose to subdivide it. This will turn one Grid into four, taking up exactly the same space but giving you more flexibility.

YOU CAN ADD/REMOVE WHATEVER FACTION OR NATION YOU WANT IN THE "Control Factions" PANEL. WRITE WHATEVER YOU WANT AND CLICK " ADD FROM TEXT"

When you are happy with the Name and parameters of a region, it's important to click "Save Region". 

SAVE/ EXPORTS: Yes, there's a ton of buttons. Yes, they are all useful, and you will probably need most of them at some point. 

--- SAVE JSON: saves Metadata. You can probably ignore this one. ---

--- EXPORT JSON: Best Button in mortal existence. Writes out a long JSON file which contains all the stats, the color ID etc... of ALL your regions and Ocean Grids. Days of manual work done with one click. You love this button. ALWAYS CLICK THIS BEFORE YOU EXIT THE APPLICATION IF YOU WANT YOUR WORK TO BE SAVED! ---

--- EXPORT PNG: Takes a Snapshot of your entire viewport. ---

--- REBUILD LAND PNG: Takes a snapshot of your land regions with even more subtle color range. ALWAYS CLICK THIS BEFORE YOU EXIT THE APPLICATION IF YOU WANT LAND TO BE SAVED! ---

--- REBUILD WATER PNG: Isolated export of all your Ocean Grids in PNG form. ALWAYS CLICK THIS BEFORE YOU EXIT THE APPLICATION IF YOU WANT WATER TO BE SAVED! ---

--- BORDER PNG: Exports a Png of all the borders in your viewport. ---

WHY IS THAT USEFUL? Glad you asked. 90% of what you need for a Strategy map is colored regions, and the Parameters connected to those regions. You should in theory be able to set up an interactable map within minutes in any Game engine, depending on the code needed for parsing the colors in the JSON. 

/// (NOTE!) I recommend using the REBUILD PNGs as opposed to the unified PNG Export, for maximum color range and flexibility. ///

--- HOW TO LOAD A SAVED PROJECT! ---
Load Primary PNG and WATER PNG as normal. Head Down to the Load Panel in the Bottom Left. Choose a rebuild land PNG, A rebuild water PNG, and the EXPORT JSON. Click on "Rebuild from Save" and you should be able to continue wherever you left off. This also makes it simple to work on multiple PCs. Just e-mail yourself the Export JSON, and the 4 required PNGs. 

WHY ARE 5 DIFFERENT FILES REQUIRED FOR ONE SINGLE SAVE? Because the application will crash otherwise. 


HOW TO USE OPTIONAL PARAMETER MAP: PAINT A BLACK BACKGROUND IN WHATEVER COLOR YOU WANT ( you should be able to edit what color translates to which stats in the Parameter Map Panel!)
THE APPLICATION WILL READ THE RED, GREEN BLUE AND ALPHA VALUES AND DISTRIBUTE THOSE STATS ACROSS THE REGIONS. COLORS COMBINE SO PURE WHITE = ALL STATS MAXIMIZED.

Why does this save so much time? well, rather than editing 100 adjacent regions to have high values of wealth, sickness, Elite soldiers etc... you can simply splat a ton of bright red across where those regions are (GIMP WORKS PERFECTLY FOR PAINTING) and the application will auto-fill in high values. 

/// NOTE: MAKE SURE THAT YOUR PARAMETER MAP IS THE SAME DIMENSIONS AS YOUR PRIMARY PNG, OTHERWISE THEY MAY NOT LINE UP CORRECTLY.///

------------------------------------------------------------------------------------------------------------------------------------------
CONTACT: If you have questions, feel free to message: www.reddit.com/user/stormfoil/
LICENSE: COMPLETELY FREE TO USE FOR ANY PURPOSE. HAVE FUN AND GOOD LUCK :)

i will NOT be adding any features or customizing this any further. Feel free to do so yourself. (okay, I might, but I give no guarantees.)
