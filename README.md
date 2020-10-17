[![Andalusia Bush Trip](/misc/logo_cordoba_ingame.png)](https://github.com/marccreal/AndalusiaBushTrip)
[![Latest release](https://img.shields.io/github/v/tag/marccreal/AndalusiaBushTrip?label=release&style=for-the-badge)](https://github.com/marccreal/AndalusiaBushTrip/releases/latest) [![](https://img.shields.io/github/downloads/marccreal/AndalusiaBushTrip/total?style=for-the-badge)](https://github.com/marccreal/AndalusiaBushTrip/releases/latest)

A bush trip through the Spanish region of Andalusia for Microsoft Flight Simulator.

## Note
This bush trip is an alpha version. Only the first few legs are (fully) implemented. I would be happy for any kind of feedback, so please feel free to use the [issues page](https://github.com/marccreal/AndalusiaBushTrip/issues). Aside from technical issues, I am very interested in feedback on the difficulty level, length and quality of the legs.

## Install
1. Grab the latest [release](https://github.com/marccreal/AndalusiaBushTrip/releases/latest) and unzip to a directory of your choice.
2. Move the `marccreal-bushtrip-andalusia` folder into the `Community` folder of your MSFS installation. This folder can be located in different places:
   * Steam (standard): C:\Users\\[YOUR USERNAME]\AppData\Roaming\Microsoft Flight Simulator\Packages\Community
   * Microsoft Store (standard): C:\Users\\[YOUR USERNAME]\AppData\Local\Packages\Microsoft.FlightSimulator_[RANDOMLETTERS]\LocalCache\Packages\Community
   * Boxed (standard): C:\Users\\[YOUR USERNAME]\AppData\Local\MSFSPackages\Community
   * Custom folder (for packages downloaded by the ingame installer): [YOUR CUSTOM INSTALL FOLDER]\Community

## Play
Simply start the game and go to the bush trip menu. The new trip should appear there and you can play it exactly in the same way as the bush trips initially provided with the game.

## Known issues
### General
Unfortunately, there are several bugs in the bush trip system of the main game which also effect this custom made bush trip:
- No/empty navlog and no VFR map when continuing the bush trip:
  - Workaround: Try reloading from previous leg, use the developer menu to directly jump to the destination. The "leg completed" message should pop up and you should be able to start the next leg.
- "Leg completed" message does not appear although you landed at the correct airport.
  - This bug appeard after one of the recent patches for MSFS. A bush trip that was started with the previous version could be continued but the completion of the leg was not detected correctly.
  - Workaround: Restart from the first leg (afaik just restating the previous leg does not help) and with the help of the developer menu, jump to the destinations of the legs until you reach the point where you want to continue.
  - It might be necessary to delete the saves first. Just delete the corresponding folder that can be found at `...\Users\[USERNAME]\AppData\Roaming\Microsoft Flight Simulator\MISSIONS\ACTIVITIES\[BUSHTRIPNAME]_SAVE`

### Specific
- Route and waypoints are not displayed on VFR-map.

## Change aircraft
There are currently two release versions provided that use the DA40 NG (G1000) and the DA 40 TDI (steam gauges), respectively. If you want to fly another plane, you can either change the aircraft in flight via developer mode (note that the times in the navlog will not adapt to the new plane) or you can change the FLT-file `..\Community\marccreal-bushtrip-andalusia\Missions\marccreal\BushTrips\andalusia\ANDALUSIA.FLT` with a text editor. Find the section `[Sim.0]` and change the line `Sim=DA40-NG Asobo` to the desired aircraft. To find out, what name to put in there, go to the world map, create a simple flight with the desired plane and save the flightplan. You can then find the name in the created FLT file. You have to restart the sim in order to make changes in the FLT file take effect.
