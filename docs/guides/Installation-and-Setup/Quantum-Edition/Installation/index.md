# Installation
## Requirements
- Unity 6000.5.3f1 or newer
- Photon Quantum 3.1 or newer
- Photon Quantum Bot SDK

## Prerequisite Packages
### Required
- Addressables
- Timeline
- Cinemachine
- Localization
- [Serialized Dictionaries](https://github.com/ayellowpaper/SerializedDictionary)
- [UniTask](https://github.com/cysharp/unitask)
- [Serialize Reference Extensions](https://github.com/mackysoft/Unity-SerializeReferenceExtensions.git)

### Optional
These are optional, but are used in sample content.

- Input System
- Netcode for GameObjects
- [Local Multiplayer Input Management](https://github.com/christides11/LocalMultiplayerInputManagement.git)

## Required Quantum Changes
A few changes to Quantum files & code are required.

First, add these references to the Quantum.Simulation.asmdef at `Assets\Photon\Quantum\Simulation`.
![Quantum Simulation assembly references]

And then at the bottom modify the version defines.
![asmdefVersionDefines]

We also need a change in 'QuantumEntityViewUpdater.cs'. Change LateUpdate from private to public.

## Installation
Install the core in the Package Manager via git URL
```
https://github.com/Hack-and-Slash-Framework/HNSF-Quantum-Core.git#upm
```

You will have a few errors in the console, as we need to define some global variables.   
Create a .qtn file with these variables. These are used to define the array size for input buffers.
```
#define INPUT_BUFFER_SIZE 30
#define MOVEMENT_BUFFER_SIZE 2
#define CAMERA_BUFFER_SIZE 1
```

## Up Next
Next you'll want to install either the [3D Extension](2-install-3d.md) or [2D Extension](2-install-2d.md) depending on your project.   
They provide various systems and state actions tailored to their respective views.   
You can also ignore the extensions and handle these things yourself if you want.   

[Quantum Simulation assembly references]: ../../../../assets/images/Unity_TS0m6t7fO2.png
[asmdefVersionDefines]: ../../../../assets/images/Unity_JSwN18Oo6Z.png
