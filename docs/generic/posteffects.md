
# Deleting Post Effects on Unreal Engine

Depending on the game a few things can be done.

## Unreal Engine 4

- Motion Blur
- Depth of Field
- Chromatic Abberation

### Phase 1

1. Head over to `%APPDATA%` or `%LOCALAPPDATA%`

    - Steam

        ``"GAME"\Saved\Config\WindowsNoEditor `

    - Windows Game Store

        `"GAME"\Saved\Config\WinGDK`

2. Open the `Engine.ini` file and at the bottom of the file. Add:

    ```
    [SystemSettings]
    r.DepthOfFieldQuality=0
    r.MotionBlur.Max=0
    r.MotionBlurQuality=0
    r.DefaultFeature.MotionBlur=0
    r.SceneColorFringe.Max=0
    r.SceneColorFringeQuality=0
    ```

3. Save the file and set it to `Read Only`.

There are other effects you can disable and control here. But, this guide only to get you going.

Keep in mind if you change your setting in game you may need to restart so that this INI can remove the problem Post Effects.

Also understand this may not always work in every instance.

A good source for modding this INI is <https://www.pcgamingwiki.com/>

## Unreal Engine 5

Please Note *Unreal Engine 5* Needs Different Settings.

HellBlade 2:

```
[SystemSettings]
r.SceneColorFringeQuality=0
r.Tonemapper.GrainQuantization=0
r.Tonemapper.Quality=0
r.NT.Lens.Distortion.Intensity=0
r.NT.Lens.Distortion.Stretch=0
r.NT.Lens.ChromaticAberration.Intensity=0
r.NT.DOF.RotationalBokeh=0
r.NT.DOF.NTBokehTransform=0
r.FilmGrain=0
```

For letterboxing removal:

```
r.NT.AllowAspectRatioHorizontalExtension=0
r.NT.EnableConstrainAspectRatio=0
```

## Shader Toggler

This ReShade Add-on is free and can disable certain effects that can cause issues with Depth3D.

You can read more about it [here](shadertoggler.md).

Video Guide coming soon™️
