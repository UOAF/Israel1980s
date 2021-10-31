Israel 1980s, Version 1.7:
This theater is a mod of the existing Israel theater for Falcon BMS 4.35.


Theater Installation:

-Download and install the official Israel Theater Of Operations for BMS 4.35 at https://forum.falcon-bms.com/topic/19428/israel-theater-of-operations-for-bms-4-35 (currently version 1.05.4 for BMS 4.35 U3). This is required to use Israel 1980s;

-Unzip "Add-On Israel1980s" into "Falcon BMS 4.35\Data\";

-Open the "Falcon BMS 4.35\Data\TerrData\TheaterDefinition\theater.lst" file and add the line "Add-On Israel1980s\Terrdata\theaterdefinition\Israel1980s.tdf";



Tacview Add-On Installation:

-To make sure Tacview references the correct BMS DB, you need to open the "C:\Programs\Tacview\Data\Xml\Data-Falcon4Theaters.xml" file and go to the <Theater ID="Israel"> entry.

Either:

 -Change the <Database> field to reference your ITO80s installation's Terrdata folder and <Terrain> field to reference the stock-ITO terrain folder, i.e:
  "<Terrain>C:\Programs\Falcon BMS 4.35\Data\Add-On Israel\Terrdata\Israel\terrain\</Terrain>" (this will properly align units with the Tacview terrain)
  "<Database>C:\Programs\Falcon BMS 4.35\Data\Add-On Israel1980s\Terrdata\objects\</Database>"

  IMPORTANT: only use backslashes "\" when setting the above paths, also make sure there is a final backslash "\" at the end of both paths, as shown above.

Or:

 -Make a copy of the existing <Theater ID="Israel"> entry and rename it to, i.e: <Theater ID="Israel1980s">, after that update the <Terrain> and <Database> fields as explained above (This method will avoid possible issues when loading stock-ITO tapes while referencing the ITO80s DB).

-Copy the "Israel1980s DB Fixes.xml" file from the "Tacview" folder within this .zip archive you downloaded and place it in "C:\ProgramData\Tacview\Data\Database\Default Properties\" (It is likely that this file will fix wonky object translations in tapes from other theaters as well, though I haven't tested that yet).