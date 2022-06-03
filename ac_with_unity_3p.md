Do the setup to create a Unity third person game but no mobile...base 3D as if building for desktop or web.

[unity_third_person.md](unity_third_person.md)

Then using Adventure Creator create a new 3D game. Keyboard and mouse input were specified as the input method.

The game runs but there are error messages:

InvalidOperationException: You are trying to read Input using the UnityEngine.Input class, but you have switched active Input handling to Input System package in Player Settings.
UnityEngine.Input.get_mousePosition () (at <633a381d082145f4a4cfa49ce9be3da8>:0)
AC.PlayerInput.InputMousePosition (System.Boolean _cursorIsLocked) (at Assets/AdventureCreator/Scripts/Controls/PlayerInput.cs:1696)
AC.PlayerInput.UpdateInput () (at Assets/AdventureCreator/Scripts/Controls/PlayerInput.cs:297)
AC.StateHandler.Update () (at Assets/AdventureCreator/Scripts/Game engine/StateHandler.cs:154)

To resolve, use:

<https://adventure-creator.fandom.com/wiki/Input_System_integration>

This script demonstrates one way to add support for Unity's new Input System. It works by defining Input Actions directly within a component, but it can be adapted to work with an asset file instead.

There was a warning about the UI_EventSystem that was added to support the on-screen touch controls. The UI_EventSystem was removed and everything appeared to continue to work okay.



