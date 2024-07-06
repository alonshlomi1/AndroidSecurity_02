
### How to Decompile, fix and run the APK file:

- Decompile the APK file using http://www.javadecompilers.com/apktool.
- Look in manifest file and see that the app has 2 activities, Activity_game and Activity_menu.
- Open new empty android project.
- Find in the decompile files the Activity_game and Activity_menu (java and xml) and copy it into the new project.
- Read Activity_game and Activity_menu to figure how the game works.
- Find ic_down, ic_up, ic_left, ic_right in to drawable.
- Fixed fix some import issues and manifest file.
- Trying to run the app and handle some errors:
	- Copy strings from the decompile files into the new project.
	- Added internet permissions.
	- In Activity_game change to Toast.LENGTH_LONG.

### How to win the game:
To win you need to do Modulo 4 do each digit in your id and than change the result to arrows with this:
0 -> Left
1 -> Right
2 -> Up
3 -> Down

The displayed country name depends on the 7 digit in your id.

<img src="https://github.com/alonshlomi1/AndroidSecurity_02/assets/98226796/7d35601d-cd98-4b06-894e-237cdf8a6c9d" alt="game winner" width="300">
