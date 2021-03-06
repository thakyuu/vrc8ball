# VRChat / Harry_T 8 Ball source mirror

![](https://i.imgur.com/3cHrbf1.jpg)

### Bugs / Feature requests
Please feel free to submit anything to the issues page here

## For World Creators
This project can be downloaded from [The releases page](https://github.com/Terri00/vrc8ball/releases)

### Dependencies / Setup
- Install VRCSDK 3
- Install [Udon Sharp](https://github.com/MerlinVR/UdonSharp)
- Import the package

#### Collision layers
There are some objects that need to be set to only collide on a seperate layer.

Check the scene `ht8b` for a full setup example

Recommended steps:
- Edit > Project Settings > Tags and Layers
- Add a new layer to the list
- Edit > Project Settings > Physics
- In the collision matrix deselect all apart from itself for the new layer as so:

![](https://i.imgur.com/eZpXQ65.png)

- Finally, in the prefab, you should set all `ball00-ball15` to this layer, as well as `table_col` object

### Quest / PC Toggles
The project includes some small scripts to change / toggle stuff between quest/pc versions

It has to be manually changed


On the top of the prefab there is one:

![](https://i.imgur.com/HPtMBiH.png)

And in the scene `__MAIN__` also has one of these scripts

### Caveats
- HT8B once again has a position requirement, this time its that the Y position in the scene of this prefab should equal 0.0 
- This project is currently not designed / tested with more than one instance of a table in a world and is currently unsupported
