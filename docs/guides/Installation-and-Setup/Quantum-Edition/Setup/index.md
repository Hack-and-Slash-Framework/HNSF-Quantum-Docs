# Setup
Under `Tools > HnSF` in the top menu bar, choose `Configuration`.
![ConfigurationMenuBar]

A window should open with a `No Configuration File found.` message. 
Click `Create Configuration File`, placing it where ever you want.

# Creating Mod Definition
In HnSF, anything that adds content is considered a "mod". 
This assumption makes mod support simple, so you should consider even your own content as just a mod.
To make this work, we'll be making use of Addressables for any content we create.

We first need to create the mod definition for our contnet, so let's do that in the "Create Mod" section.

![CreateModInitial]

For Mod Type we'll keep it as "ADDRESSABLES_LOCAL", but to explain each option briefly:

* **ADDRESSABLES_LOCAL**: Use when working directly in the project.
* **ADDRESSABLES**: Use when making content in a separate project. Primarily for modders.
* **UMOD**: Use when making content in a separate project while using UMod. This method supports adding new scripts and state logic, so it's the preferred modding method.

Set the path, the identifier (string with no spaces), and  mod name, then create it.   
I recommend creating it in a subfolder, I'll be putting it in "Assets/2_Content".

![CreateModFilled]

![CreateModAsset]


[ConfigurationMenuBar]: ../../../../assets/images/Unity_Tl7mJuE1ZW.png
[CreateModInitial]: ../../../../assets/images/Unity_6GZf4Hba1L.png
[CreateModFilled]: ../../../../assets/images/Unity_dtFEw7aO9n.png
[CreateModAsset]: ../../../../assets/images/Unity_fiSMwRUwdN.png