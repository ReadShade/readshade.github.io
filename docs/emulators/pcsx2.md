
# PCSX2 Basic Settings

This Guide will focus on basic adjustments for ReShade and it's use in PCSX2: Emulator.

## Display

For this guide we will be using the DX11 API.

![](images/PCSX2/PCSX2_Renderer_Zoomed.png)

This is due to compatibility with other add-ons. Now please look at the settings in this menu.

![](images/PCSX2/PCSX2_Settings00.png)

1. You will be looking for `Fullscreen Mode & Aspect Ratio ` Like in the image below.

    ![](images/PCSX2/PCSX2_Fullscreen_AR.png)

    > The reason we want to set Aspect Ratio to Fit to Window. Is because the depth buffer is set to this internally.

2. `Anti-Blur` is a good one to keep on to keep distortions to a minimal.

    ![](images/PCSX2/PCSX2_Anti-Blur.png)

## Rendering

As I said above. We are focusing on DX11, You can always try different APIs as long you get a depth buffer out you should be fine.

![](images/PCSX2/PCSX2_Settings01.png)

1. Make sure to set Rendering to `Direct3D 11` for this example.

    ![](images/PCSX2/PCSX2_Renderer.png)

    > Because, we want compatibility with most of ReShade's add-ons.

2. Now we want to set our Internal Resolution: `Native` for most cases.

    ![](images/PCSX2/PCSX2_Rendering.png)

    > It also helps with ReShade own generic depth add-on.

## ReShade

You need to install ReShade under your current `API Setting`.

![](images/PCSX2/PCSX2_Renderer_Zoomed.png)

So Now please turn off the emulator and install [ReShade](../reshade/reshadeversions.md).
Once that is done....

Please start your game and go into the ReShade menu and check the depth buffer.

![](images/PCSX2/PCSX2_ReShade_Depth_Add-on.png)

This is in the add-ons tab inside the ReShade own menu.

## Extra Info

Make sure you do all the other things like the games and bios things on your end........... I will not explain that.

## Conclusion

This may not be the case for every game. But, this should be a good starting point.
