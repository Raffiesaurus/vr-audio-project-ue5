# VR Reverb Scene - UE5

A **UE5.3 VR research project** exploring spatial audio in immersive environments. Built for Meta Quest (via OculusXR/OpenXR), the scene integrates the [ReverbShift](https://github.com/Raffiesaurus/conv-reverb-plugin-ue5) convolution reverb plugin to deliver physically accurate room acoustics in VR - where audio realism matters as much as visual fidelity.

> Research project - not a shipped product.

---

## What It Explores

- Convolution reverb in a VR environment using real Impulse Response (IR) files
- Acoustic variation across different virtual spaces - how room geometry and materials change the perceived sound
- Integration of a custom UE5 MetaSounds plugin (**ReverbShift**) into a live VR session
- OpenXR and Meta Quest hand tracking / eye tracking in UE5.3

---

## Tech Stack

- **Engine:** Unreal Engine 5.3
- **Language:** C++ (`VRReverbScene` module)
- **VR Runtime:** OpenXR + OculusXR (Meta Quest / Quest 2 / Quest 3)
- **Audio:** ReverbShift plugin (FFT convolution reverb via MetaSounds)
- **Platforms:** Win64, Android (Quest)

---

## Plugins

| Plugin | Purpose |
|--------|---------|
| `OpenXR` | Cross-platform VR runtime |
| `OpenXREyeTracker` | Eye tracking input |
| `OpenXRHandTracking` | Hand tracking input |
| `OculusXR` / `MetaXR` | Meta Quest SDK integration |
| `OculusPlatform` / `MetaXRPlatform` | Meta platform services |
| `ReverbShift` *(custom)* | Real-time convolution reverb via MetaSounds |

---

## Opening the Project

1. Install **Unreal Engine 5.3** via the Epic Games Launcher
2. Install the **OculusXR** plugin from the [Marketplace](com.epicgames.launcher://ue/marketplace/product/8313d8d7e7cf4e03a33e79eb757bccba)
3. Clone the repo
4. Right-click `VRReverbScene.uproject` → **Generate Visual Studio project files**
5. Open in UE5.3 - the bundled ReverbShift plugin compiles automatically

For Quest deployment, set your Android SDK paths in **Project Settings → Platforms → Android**.

---

## Related

- **ReverbShift Plugin:** [conv-reverb-plugin-ue5](https://github.com/Raffiesaurus/conv-reverb-plugin-ue5)

---

## License

MIT
