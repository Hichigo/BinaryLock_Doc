# BP\_LCDLock\_16Bit\_Wall

* Lock inherited from **BP\_CoreBinaryLock**.
* The number of buttons by default (16 pieces).
* Added static mesh component (**SM\_LCDPanelLite**). There are 5 materials in this grid that show the number that is currently entered.

![](<../../.gitbook/assets/image (19).png>)

* Redefined function **CreateDynamicMaterialsForDigits** which creates and stores links to dynamic materials for changing numbers, the function is called on **BeginPlay**.

{% hint style="warning" %}
For the **CreateDynamicMaterialsForDigits** function to work, it is important to specify the material indices in which the numbers are displayed.

This is indicated in the variables:

* **FirstIndexDigitMat** (integet): in this case 2
* **LastIndexDigitMat** (integet): in this case 6


{% endhint %}

![](<../../.gitbook/assets/image (6).png>)

![](<../../.gitbook/assets/image (1).png>)

Each digit can be assigned a material with any color

![](<../../.gitbook/assets/image (4).png>)

### Maximum number for a correct password

from 0 to 65535

![](<../../.gitbook/assets/image (15).png>)
