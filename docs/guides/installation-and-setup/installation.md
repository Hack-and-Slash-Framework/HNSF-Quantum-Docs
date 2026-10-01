# Installation (Quantum Editon)
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

## Installation
Install the core in the Package Manager via git URL
```
https://github.com/Hack-and-Slash-Framework/HNSF-Quantum-Core.git#upm
```

[Quantum Simulation assembly references]: ../../assets/images/Unity_TS0m6t7fO2.png
[asmdefVersionDefines]: ../../assets/images/Unity_JSwN18Oo6Z.png
