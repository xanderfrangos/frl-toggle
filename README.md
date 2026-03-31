# dlssfg-fps

Command line app for Windows to toggle Nvidia's DLSS-FG MFG Target FPS. Based on: https://github.com/FrogTheFrog/frl-toggle

# How to use

----

Run the app in terminal for usage instruction, but in case you're lazy:
```
  Usage example:
    dlssfg-fps status                         prints the current MFG FPS target. Value 0 means it's disabled.
    dlssfg-fps 0                              turns off the MFG FPS target.
    dlssfg-fps 120                            sets the FPS target to 120 (allowed values are [0, 1023]).
    dlssfg-fps 120 --save-previous            sets the FPS target to 120 and saves the previous value to a file.
    dlssfg-fps 120 --save-previous-or-reuse   sets the FPS target to 120 and saves the previous value to a file.
                                              If the file already exists, its value will be validated and reused instead.
                                              This is useful in case the system has crashed and we want to reuse the value from before the crash.
    dlssfg-fps load-file                      loads the value from file (e.g., saved using "--save-previous") and uses it to set the target.
                                              File is removed afterwards if no errors occur.
```
