# VATGlasses-Data
This repository contains official parsers from popular Sector File formats to the format used by VATGlasses.

Instructions for use:

1. Remove any Runways from the [RUNWAYS] section which belong to airports not directly under the control of this sector file. _Runways from other vACCs/vARTCCs or all runways if file is designed for controllers to open large bandboxes (such as Eurocontrol, etc) only._

2. Remove any ATC positions from the [POSITIONS] section which are not directly under the control of this sector file. _Positions from other vACCs/vARTCCs, upper level sectors which are managed by other vACCs/vARTCCs (e.g. Maastricht Jever in the EHAA file), large bandboxes such as Eurocontrol (these have their own file), etc._

3. Run the parser.

4. If errors occur, correct them then rerun.

5. Readd large bandboxes (Eurocontrol, etc.) to the _airspace.txt_ using references to their own VATGlasses data packages. _See the Wiki for more details on how to do this._

In Euroscope:

* The [RUNWAYS] section is located in the .sct file.
* The [POSITIONS] section is located in the .ese file.

In VRC:

* The [RUNWAYS] section is located in the .sct2 file.
* The [POSITIONS] section is located in the .pof file.
