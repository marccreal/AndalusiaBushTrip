![https://github.com/marccreal/AndalusiaBushTrip](/misc/logo_alhambra.png)
![https://github.com/marccreal/AndalusiaBushTrip/releases/latest](https://img.shields.io/github/v/tag/marccreal/AndalusiaBushTrip?label=release&style=for-the-badge) ![](https://img.shields.io/github/downloads/marccreal/AndalusiaBushTrip/total?style=for-the-badge)

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

## Change aircraft
There are currently two release versions provided that use the DA40 NG (G1000) and the DA 40 TDI (steam gauges), respectively. If you want to fly another plane, you can either change the aircraft in flight via developer mode (note that the times in the navlog will not adapt to the new plane) or you can change the FLT-file `..\Community\marccreal-bushtrip-andalusia\Missions\marccreal\BushTrips\andalusia\ANDALUSIA.FLT` with a text editor. Find the section `[Sim.0]` and change the line `Sim=DA40-NG Asobo` to the desired aircraft. To find out, what name to put in there, go to the world map, create a simple flight with the desired plane and save the flightplan. You can then find the name in the created FLT file. You have to restart the sim in order to make changes in the FLT file take effect.
