# MRTK2 Template

Unity/MRTK2 basic template.

Using

	- Unity 2020.3.42f1
	- Mixed Reality Feature Tool v1.0.2209.0
	- [MRTK 2](https://learn.microsoft.com/en-us/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)

## MRTK2 Installed Features

- Mixed Reality OpenXR Plugin v1.8.0
	
	- com.microsoft.mixedreality.openxr
	- **DEPENDENCY** com.unity.xr.arfoundation v4.1.7
	- **DEPENDENCY** com.unity.xr.management v4.2.0
	- **DEPENDENCY** com.unity.xr.openxr v1.5.3
	- **DEPENDENCY** com.unity.xr.core-utils v2.1.0

- Mixed Reality Toolkit Standard Assets v2.8.3
	
	- Shaders, common materials and fonts
	- com.microsoft.mixedreality.toolkit.standardassets
	- **DEPENDENCY** com.unity.textmeshpro v2.1.4

- Mixed Reality Toolkit Foundation v2.8.3
	
	- com.microsoft.mixedreality.toolkit.foundation
	- **DEPENDENCY** com.microsoft.mixedreality.toolkit.standardassets v2.8.3

- Mixed Reality Toolkit Extensions v2.8.3
	
	- Hand Physics Service, Lost TRacking Service, Scene Transition Service
	- com.microsoft.mixedreality.toolkit.extensions
	- **DEPENDENCY** com.microsoft.mixedreality.toolkit.foundation v2.8.3

- Mixed Reality Toolkit Tools v2.8.3
	
	- com.microsoft.mixedreality.toolkit.tools
	- **DEPENDENCY** com.microsoft.mixedreality.toolkit.foundation v2.8.3

## Unity MRTK2 Manifest (from installation process)

```json
{
  "dependencies": {
    "com.unity.collab-proxy": "1.17.6",
    "com.unity.ide.rider": "3.0.16",
    "com.unity.ide.visualstudio": "2.0.16",
    "com.unity.ide.vscode": "1.2.5",
    "com.unity.test-framework": "1.1.33",
    "com.unity.textmeshpro": "3.0.6",
    "com.unity.timeline": "1.4.8",
    "com.unity.ugui": "1.0.0",
    "com.unity.modules.ai": "1.0.0",
    "com.unity.modules.androidjni": "1.0.0",
    "com.unity.modules.animation": "1.0.0",
    "com.unity.modules.assetbundle": "1.0.0",
    "com.unity.modules.audio": "1.0.0",
    "com.unity.modules.cloth": "1.0.0",
    "com.unity.modules.director": "1.0.0",
    "com.unity.modules.imageconversion": "1.0.0",
    "com.unity.modules.imgui": "1.0.0",
    "com.unity.modules.jsonserialize": "1.0.0",
    "com.unity.modules.particlesystem": "1.0.0",
    "com.unity.modules.physics": "1.0.0",
    "com.unity.modules.physics2d": "1.0.0",
    "com.unity.modules.screencapture": "1.0.0",
    "com.unity.modules.terrain": "1.0.0",
    "com.unity.modules.terrainphysics": "1.0.0",
    "com.unity.modules.tilemap": "1.0.0",
    "com.unity.modules.ui": "1.0.0",
    "com.unity.modules.uielements": "1.0.0",
    "com.unity.modules.umbra": "1.0.0",
    "com.unity.modules.unityanalytics": "1.0.0",
    "com.unity.modules.unitywebrequest": "1.0.0",
    "com.unity.modules.unitywebrequestassetbundle": "1.0.0",
    "com.unity.modules.unitywebrequestaudio": "1.0.0",
    "com.unity.modules.unitywebrequesttexture": "1.0.0",
    "com.unity.modules.unitywebrequestwww": "1.0.0",
    "com.unity.modules.vehicles": "1.0.0",
    "com.unity.modules.video": "1.0.0",
    "com.unity.modules.vr": "1.0.0",
    "com.unity.modules.wind": "1.0.0",
    "com.unity.modules.xr": "1.0.0",
    "com.microsoft.mixedreality.toolkit.extensions": "file:MixedReality/com.microsoft.mixedreality.toolkit.extensions-2.8.3.tgz",
    "com.microsoft.mixedreality.toolkit.foundation": "file:MixedReality/com.microsoft.mixedreality.toolkit.foundation-2.8.3.tgz",
    "com.microsoft.mixedreality.toolkit.standardassets": "file:MixedReality/com.microsoft.mixedreality.toolkit.standardassets-2.8.3.tgz",
    "com.microsoft.mixedreality.toolkit.tools": "file:MixedReality/com.microsoft.mixedreality.toolkit.tools-2.8.3.tgz",
    "com.microsoft.mixedreality.openxr": "file:MixedReality/com.microsoft.mixedreality.openxr-1.8.0.tgz"
  }
}
```

## MRTK 2 First Configuration Settings

- using Unity OpenXR Plugin (recommended)
- using API compatibility level : .NET standard v4.x (check player settings)
- OpenXR Plugin Management
	- Plug-In provider : OpenXR with Microsoft HoloLens fature group
	- Interaction profile : Eye Gaze Interaction Profile (it requires Gaze Input Capability)
	- Render Mode : Single Pass Instance
	- Depth Submission Mode : 16bit
- Audio Spatializer : default config
- Import textMeshPro Essentials

## Build settings

- Target Platform : Universal Windows Platforms
- Target device : HoloLens
- Arch : ARM64

Default for all the other build settings

## Repo Settings

- [Suggested GitIgnore for the project](https://learn.microsoft.com/en-us/windows/mixed-reality/mrtk-unity/mrtk2/performance/large-projects?view=mrtkunity-2022-05#gitignore)