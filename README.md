![SmartInvs Logo](http://minuskube.fr/img/smart-invs/smart_invs.png)

[![License](https://img.shields.io/github/license/minuskube/smartinvs.svg?style=flat-square)](https://github.com/MinusKube/SmartInvs/blob/master/LICENSE.md)
[![Javadocs](https://img.shields.io/maven-central/v/fr.minuskube.inv/smart-invs.svg?label=javadoc&style=flat-square)](https://javadoc.io/doc/fr.minuskube.inv/smart-invs)

# SmartInvs
Advanced Inventory API for your Minecraft Bukkit plugins.

**Note** This is a fork of the original [SmartInvs](https://github.com/MinusKube/SmartInvs) project, which appears to be 
abandoned. 

**Tested Minecraft versions**: 1.21  

## Features
* Inventories of any type (workbench, chest, furnace, ...)
* Customizable size when possible (chest, ...)
* Custom titles
* Allows to prevent the player from closing its inventory
* Custom listeners for the event related to the inventory
* Iterator for inventory slots
* Page system
* Util methods to fill an inventory's row/column/borders/...
* Actions when player clicks on an item
* Update methods to edit the content of the inventory every tick

## Usage
To use the SmartInvs API, either:
- Put it in the `plugins` folder of your server, add it to your dependencies in your plugin.yml (e.g. `depend: [SmartInvs]`) and add it to the dependencies in your IDE.
- Put it inside your plugin jar, initialize an `InventoryManager` in your plugin (don't forget to call the `init()` method), and add a `.manager(invManager)` to your SmartInventory Builders.

You can download the latest version on the [Releases page](https://github.com/MinusKube/SmartInvs/releases) on Github.

You can also use a build system:
### Gradle
```gradle
repositories {
    mavenCentral()
}

dependencies {
    compile 'fr.minuskube.inv:smart-invs:1.2.7'
}
```

## TODO
* JavaDoc
* Maven Central release

## Issues
If you have a problem with the API, or you want to request a feature, make an issue [here](https://github.com/MinusKube/SmartInvs/issues).
