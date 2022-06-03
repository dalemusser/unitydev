# unity3rdperson1

Setup to for mobile app with touch joystick controls.

1. New Mobile Project

2. Import Third Person Starter Assets

3. Create plane with Rigidbody (constrain x, y, z) and Box Collider as ground

4. Menu: Tools > Starter Assets > Reset Third Person Controller Armature

5. Remove model (fbx) under PlayerArmature > Geometry and replace with fbx that has Animation Type of Humanoid. Select fbx to be used and set to Animation Type of Humanoid then add to Geometry. Select PlayerArmature and set Animator Avatar to match model

6. From Starter Assets drag UI_EventSystem and UI_Canvas_StarterAssetsInputs_Joysticks

7. For UI_Canvas_StarterAssetsInputs_Joysticks, set Output to PlayerArmature

Common mistakes:

* not setting to Animation Type of Humanoid
* not setting the output of the joysticks to the PlayerArmature
