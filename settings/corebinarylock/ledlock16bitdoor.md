# BP\_LedLock\_16Bit\_Door

* Lock inherited from **BP\_CoreBinaryLock**.
* The number of buttons by default (16 pieces).
* Added static grid component (**SM\_LedLockPanelLite**). In this grid, there is a LED material for which indicates whether the lock is open or closed (red - closed, green - open). The **SetLedGreenLight** function has also been redefined, in which the logic for changing the LED color to green has been added.
* Added static mesh component (**SM\_DoorHand**).

![](<../../.gitbook/assets/image (13).png>)

### Maximum number for a correct password

from 0 to 65535

![](<../../.gitbook/assets/image (15).png>)
