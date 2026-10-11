# FirstShaderInUnity

A Unity project for learning shader writing. It contains a small sci-fi maze scene with turrets, enemies and a flyer, used as a test bed for custom shaders, materials and post-processing.

## Versions

| Item | Version |
| --- | --- |
| Unity Editor | 6000.3.23f1 (Unity 6) |
| Render pipeline | Built-in |
| Post Processing | Post Processing Stack v1 (bundled in `Assets/PostProcessing`) |
| UI | `com.unity.ugui` 2.0.0 |

The project was upgraded from an older Unity version. Upgrade fixes applied:

- Added the `com.unity.ugui` package, which the Standard Assets need.
- Replaced the removed `GUIText` and `GUITexture` in `Standard Assets/Utility` with `UnityEngine.UI.Text` and `UnityEngine.UI.Image`.
- Aliased `MinAttribute` in `PostProcessing/Editor/PropertyDrawers/MinDrawer.cs` to resolve the clash with `UnityEngine.MinAttribute`.

## Getting started

1. Install Unity `6000.3.23f1` through Unity Hub.
2. Open this folder as a project in Unity Hub.
3. Open `Assets/Scenes/MainForShaderSession.unity` and press Play.

## Project structure

| Path | Contents |
| --- | --- |
| `Assets/Shaders` | Custom shaders. `InvisibleShader.shader` is an Amplify Shader Editor export that distorts a screen grab. |
| `Assets/Materials` | Materials for the maze, turret, enemy and flyer models. |
| `Assets/Scripts` | `PatrolAgent` (NavMesh waypoint patrol) and `HoloManGlitcher` (random shader glitch effect). |
| `Assets/Models`, `Assets/Textures`, `Assets/Animation` | Meshes, textures and animations. |
| `Assets/PostProcessing` | Post Processing Stack v1 and its profile. |
| `Assets/Standard Assets` | Unity's legacy Standard Assets. |

## Tutorial

The project follows this YouTube playlist:

https://www.youtube.com/playlist?list=PLX2vGYjWbI0RS_lkb68ApE2YPcZMC4Ohz

<!-- TODO: add the playlist's video titles here, in order. -->
