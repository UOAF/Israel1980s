Israel 1980s, Version 1.0:
This theater is a mod of the existing Israel theater for Falcon BMS 4.35.


Theater Installation:

-Download and install the official Israel Theater Of Operations for BMS 4.35 at https://www.benchmarksims.org/forum/showthread.php?40653-Israel-Theater-Of-Operations-for-BMS-4-35 (currently version 1.05 for BMS 4.35 U1). This is required to use Israel 1980s;

-Unzip "Add-On Israel1980s" into "Falcon BMS 4.35\Data\";

-Open the "Falcon BMS 4.35\Data\TerrData\TheaterDefinition\theater.lst" file and add the line "Add-On Israel1980s\Terrdata\theaterdefinition\Israel1980s.tdf";



Tacview Add-On Installation:

-To make sure Tacview references the correct BMS DB, you need to open the "C:\Programs\Tacview\Data\Xml\Data-Falcon4Theaters.xml" file and go to the <Theater ID="Israel"> entry.

Either:
 -Change the <Terrain> and <Database> fields to reference your ITO80s installation's Terrdata folder, i.e:
  "<Terrain>C:\Programs\Falcon BMS 4.35\Data\Add-On Israel1980s\Terrdata\terrain\</Terrain>" (the "Terrain" path does not exist, but add it anyway)
  "<Database>C:\Programs\Falcon BMS 4.35\Data\Add-On Israel1980s\Terrdata\objects\</Database>"
Or:
 -Make a copy of the existing <Theater ID="Israel"> entry and rename it to, i.e: <Theater ID="Israel1980s">, after that update the <Terrain> and <Database> fields as explained above (This method will avoid possible issues when loading stock-ITO tapes while referencing the ITO80s DB).

-Copy the "Israel1980s DB Fixes.xml" file from the "Tacview" folder within this .zip archive you downloaded and place it in "C:\ProgramData\Tacview\Data\Database\Default Properties\" (It is likely that this file will fix wonky object translations in tapes from other theaters as well, though I haven't tested that yet).