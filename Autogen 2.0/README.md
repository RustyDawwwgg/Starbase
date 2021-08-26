# Autogen 2.0


### Functionality:

- Gives full power to generators if batteries are < 90% charged

- Charges from 90% to 99.5% at user-definable rate (described below)

- PWR button to be used as a killswitch

- Override button for constant 100% power when needed (good for laser mining as a use case)

- Automatically detects when the ship is idle and completely shuts off power when batteries are charged to conserve fuel

- Automatically turns generators back on when engaging throttle

- The +30 value on line 5 can be adjusted to suit your needs. I needed an extra 30% to balance out the drain rate of my thrusters. Watch your batteries/gen rate at full thrust until you see them start to charge then take note of the gen rate and adjust accordingly. If your batteries start to drain after hitting 90% charge with gens fully warmed up, adjust this up. If they quickly go up to 100% adjust this down until you see them slowly going up at 90%+ charge and holding.

### Setup:

- Button named "PWR"

- Button named "Override" (I used a flip-top for this)

- Rename GeneratorUnitRateLimit to "RL" on every generator.
 
* Note: can use FuelChamberUnitRateLimit instead to make the process faster if you have 3 gens or less per chamber.

- Rename FcuForward to "Throttle" on lever and FCU

- Rename StoredBatteryPower to "B1" on one of your batteries
