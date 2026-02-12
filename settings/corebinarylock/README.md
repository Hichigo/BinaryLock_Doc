# BP\_CoreBinaryLock

This blueprint implements the main logic of the lock, configures the control and functions for starting and ending control of the lock.

An event (**OnCorrectPasswordEntered\_Disp**) has also been created, which is called after entering the correct password, to which you can subscribe from the outside (for example, to open a door or any other action).

## Settings

### Buttons

* **AmountButtonsByX** (integer): amount of buttons horizontally
* **AmountButtonsByY** (integer): amount of buttons vertically
* **StartHorizontalOffsetButtons** (float): initial horizontal offset of buttons
* **StartVerticalOffsetButtons** (float): initial vertical offset of buttons
* **HorizontalOffsetButton** (float): horizontal distance between buttons
* **VerticalOffsetButton** (float): vertical distance between buttons
* **PushButtonDistance** (float): button offset when pressed

### Camera

* **LengthSpringArm** (float): distance from camera to lock
* **SpringArmRotation** (Rotator): rotation of the camera around the lock

### UI

* **UIClass** (User Widget Class): hint interface

### Password

* **CorrectPassword** (integer): the password that must be entered to open the door

### Led

* **CorrectLedLight** (Linear Color): LED color after correct password entry

### LCD

* **FirstIndexDigitMat** (integer): index of the first material with numbers (materials with numbers must go in order)
* **LastIndexDigitMat** (integer): index of the last material with numbers (materials with numbers must go in order)

### Sound

* **SelectButtonSound** (Base Sound): button selection sound
* **PushButtonSound** (Base Sound): button push sound
* **CorrectPasswordSound** (Base Sound): sound of correct password
* **WrongPasswordSound** (Base Sound): wrong password sound

