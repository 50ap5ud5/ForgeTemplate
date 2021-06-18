# Minecraft Modding Template

A simple template based off of <a href="https://github.com/SizableShrimp/ForgeTemplate">SizableShrimp's modified Forge MDK Template</a> that I use to create new projects quicker by extracting all mod-related info to `gradle.properties`.

Included are both Forge and Fabric Templates

## Setting up
* Open up `gradle.properties` and change all the necessary properties
* Rename the main package to be the same as `${mod_base_package}.${mod_id}`, e.g. `me.soapsuds.examplemod`

### Using mixins?
* Delete `build.gradle`
* Rename `mixinbuild.gradle` to `build.gradle`
* Rename `examplemod.mixins.json` to start with your mod id
* Add mixins under the `mixin` package inside your base package, e.g. `me.soapsuds.examplemod.mixin`

### Not using mixins?
* Delete `mixinbuild.gradle`
* Delete `src/main/resources/examplemod.mixins.json`
* Remove `mixin_version` from `gradle.properties`

Finally, import into your IDE of choice.