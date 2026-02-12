# BP\_LCDLock\_30Bit\_Wall

* Lock inherited from **BP\_CoreBinaryLock**.
* The number of buttons has been changed (30 pieces).

{% hint style="danger" %}
For locks with LCD display, you should not use the number of buttons (bits) more than 31, see [here ](../../info.md)why.
{% endhint %}

* Added static mesh component (**SM\_LCDPanelLarge**). There are 10 materials in this grid that show the number that is currently entered.

![](<../../.gitbook/assets/image (7).png>)

* Redefined function **CreateDynamicMaterialsForDigits** which creates and stores links to dynamic materials for changing numbers, the function is called on **BeginPlay**.

{% hint style="warning" %}
For the **CreateDynamicMaterialsForDigits** function to work, it is important to specify the material indices in which the numbers are displayed.

This is indicated in the variables:

* **FirstIndexDigitMat** (integet): in this case 2
* **LastIndexDigitMat** (integet): in this case 11
{% endhint %}

![](<../../.gitbook/assets/image (12).png>)

![](<../../.gitbook/assets/image (23).png>)

Each digit can be assigned a material with any color

![](<../../.gitbook/assets/image (4).png>)

### Maximum number for a correct password

from 0 to 1073741823

![](<../../.gitbook/assets/image (18).png>)

