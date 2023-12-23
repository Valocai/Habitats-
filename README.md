# Welcome to the Habitat project! 
Boxed Survival Worlds with IridiumSkyblock

Note: This tutorial is only applicable before version 4.0.0 of IridiumSkyblock as the required generatorSettings feature is not yet available.

Overview
This tutorial will guide you on how to create a boxed mini world survival using IridiumSkyblock and Multiverse. It's important to note that this is not a feature but rather a bug that we will be exploiting.

# Step 1: Create a World with Multiverse
Before installing IridiumSkyblock, create a world with Multiverse and name it IridiumSkyblock. You can use any world generator that supports Multiverse, such as TerraformGenerator. Example command:
/mv create IridiumSkyblock normal -g TerraformGenerator, it can also work without any generators. Example /mv create IridiumSkyblock normal

# Step 2: Install and Modify the Plugin.yml File
Install the IridiumSkyblock .jar file and make a few small changes to the plugin.yml file inside the jar using a tool like WinRAR. Modify the file to include the following soft dependencies:
````
  - "MVdWPlaceholderAPI"
  - "PlaceholderAPI"
  - "Essentials"
  - "EssentialsSpawn"
  - "RoseStacker"
  - "WorldEdit"
  - "Multiverse-Core"
loadbefore:
#  - "Multiverse-Core"
````

This will trigger the bug and allow us to use any world generator with Multiverse while giving Multiverse priority.

# Step 3: Configure the GeneratorSettings in Configuration.yml
In the configuration.yml file, set the generatorSettings to the following:
```
generatorSettings:
generatorType: "OCEAN"
waterHeight: 0
minOceanFloorLevel: 0
maxOceanFloorLevel: 0
oceanFloorBottomMaterial: "AIR"
oceanFloorTopMaterial: "AIR"
```
Create a schematic file with WorldEdit that only contains AIR blocks. This will be the schematic for your island.

# Step 4: Generate Your Island
Generate your island with the AIR schematic, and it will now be a boxed mini world survival. Do not regenerate your island, as this will cause issues. Instead, delete and recreate it.

# Conclusion
Although this is not a feature, we hope that this tutorial will help you create boxed mini world survival in IridiumSkyblock. We also suggest that this should be a feature in future versions. If you have any suggestions or feedback, feel free to submit them to ⁠suggestions-skyblock.
