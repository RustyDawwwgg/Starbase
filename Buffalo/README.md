# Buffalo

Customizations I've added to my Buffalo ship. 

Below is a presonal maintnenance log specific to my ship in chronological order as I made them. Feel free to follow along if you wish!

## Changelog
- Made several lever adjustments in an effort to fine-tune flight controls (ongoing)

<img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_005.png" width="200">

- Renamed all 12 generator cooling racks + button from "Backup_Coolent" to "Coolant"

- Added small, green transponder button and removed original transponder/safezone buttons/lights/displays

- Removed Kbot logo and light above passenger seats in preparation for remodeling

- Changed all "FuelChamberUnitRateLimit" fields on Generator Fuel Chambers to "FCRL", "FcuForward" fields on FCU and related control lever to "Throttle", and "StoredBatteryPower" field on battery behind driver-side door to "B1" then replaced original gen management script with Autogen 2.0

- ~~Applied fix to mining lasers found in pinned messages in Kenetor's discord~~ (replaced with new laser pulsing/automation scripts)https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_004.png

- Moved passenger seats, added workbench to floor and squeezed in a medium tank refueling device in the space above.

<img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_004.png" width="800">

- Removed memory chip and replaced ISAN 2.5 code with updated version. Also enabled the speed estimation with the following change on line 1 sp=1

- Changed Propellant displays inside and in front of ship to 40 mil to represent the actual amount available

- Moved ore scanner to bottom-center mounting point and installed scanner auto-pitch script from video: https://youtu.be/FgYT2hmM4zE

- Added 3rd mining laser to top-cnter hardpoint where ore scanner was origionally

- Added mining laser pulsing/automation script & fine-tuned for accuracy
