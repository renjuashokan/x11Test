
# X11Test Programs 

This is a simple program to do the following operation on windows on x11 machine(ubuntu)

1. Raise Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.RaiseWindow(hdl)
    ```
2. Lower Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.LowerWindow(hdl)
    ```
3. Show Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.ShowWindow(hdl)
    ```
4. Hide Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.HideWindow(hdl)
    ```
5. Maximize Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.MaximizeWindow(hdl)
    ```
6. Remove Window Decorations
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.RemoveWindowDecoration(hdl)
    ```
7. Move Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.MoveWindow(hdl, 400, 300);
    ```
8. Resize Window
    ```cpp
    WindowManager::WindowMgrLib wmgr;
    // make sure one window with this name exists
    Window hdl = wmgr.GetWindowHandle("TestWindow", 0, 0);
    wmgr.ResizeWindow(hdl, 400, 300);
    ```

## Install X11 libraries
---
Be sure to install X11 libraries before proceeding.

```shell
sudo apt install libx11-dev
sudo apt install libxrandr-dev
```


## Build and run



```shell
cd x11test
mkdir build
cd build
cmake ..
make -j4
```
