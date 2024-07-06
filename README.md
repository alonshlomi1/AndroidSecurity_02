

- decompile the APK file.
- look in manifest file and see that the app  has 2 activities, Activity_game and Activity_menu.
- open new empty android project.
- find in the decompile files the Activity_game and Activity_menu (java and xml) and copy it into the new project.
- find ic_down, ic_up, ic_left, ic_right in to drawable
- fixed some import issues
- tring to run the app and handle some errors:
	- copy strings from the decompile files into the new project.
	- added internet permisions
	- in Activity_game change to Toast.LENGTH_LONG
- read Activity_game and Activity_menu to figure how to win

To win you need to do Modulo 4 do each digit in your id
and than change the result to arrows with this:
0 -> Left
1 -> Right
2 -> Up
3 -> Down

The displayed country name depends on the 7 digit in your id.
