# Buffalo

Customizations I've added to my Buffalo ship from the Kbot shop.

Below is a personal maintenance log specific to my ship in chronological order as I made them. Feel free to follow along if you wish. However, please do keep in mind that your ship is your responsibility and although I am happy to help those in need of assistance whenever I have the free time to do so, I will not be liable if you break things on your ship!

As a precaution, I've saved all of the [YOLOL Defaults](https://github.com/RustyDawwwgg/Starbase/tree/main/Buffalo/Defaults) for the Buffalo in this repository should you ever need to roll back for whatever reason.

## Changelog
- Renamed all 12 generator cooling racks + button from "Backup_Coolent" to "Coolant"

- Added small, green transponder button and removed original transponder/safezone buttons/lights/displays

- Removed Kbot logo and light assembly above passenger seats in preparation for remodeling

- Changed all "FuelChamberUnitRateLimit" fields on Generator Fuel Chambers to "FCRL", "FcuForward" fields on FCU and related control lever to "Throttle", and "StoredBatteryPower" field on battery behind driver-side door to "B1" then replaced original gen management script with [Autogen 2.0](https://github.com/RustyDawwwgg/Starbase/tree/main/Autogen%202.0)

- Made several lever adjustments in an effort to fine-tune flight controls (I use PS4 controller + [DS4Windows](https://github.com/Ryochan7/DS4Windows))

<p align="center"><img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_005.png" width=20%> <img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_006.png" width=20%> <img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_007.png" width=20%> <img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_009.png" width=20%></p>

- ~~Applied fix to mining lasers found in pinned messages in Kenetor's discord~~ (replaced with new laser pulsing/automation scripts)

- Moved passenger seats, added workbench to floor and squeezed in a medium tank refueling device in the space above

<p align="center"><img src="https://github.com/RustyDawwwgg/Starbase/blob/main/Buffalo/Images/20210826_004.png" width=80%></p>

- Removed memory chip and replaced ISAN code with [updated version](https://github.com/RustyDawwwgg/Starbase/blob/main/ISAN/ISAN-2.5.yolol). Also enabled the speed estimation with the following change on line 1: `sp=1`

- Changed Propellant displays inside and in front of ship to 40 million to represent the actual amount available
>*Note: current version of Buffalo has some disconnected fuel tanks, possibly a bug*

## Works In Progress
YOLOL code & more info coming soon...
- Moved ore scanner to bottom-center mounting point and installed Scanner Auto-pitch script
>*Note: could benefit from some adjustments to close range scanning (planned for future update)*

- Added 3rd mining laser to top-center hardpoint where ore scanner was originally + laser pulsing/automation script & fine-tuned for accuracy
>*Note: experienced issues with turret bases not passing along data to the mounts/devices when attaching. Managed to fix through a combination of moving pieces in/out of my inventory, trying to attach from different angles, and crafting new pieces that were giving me trouble*
