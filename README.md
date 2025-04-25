# JOSM/Vespucci Presets

This is a repository to house my collection of presets for use with JOSM and Vespucci.  
A list of presets for use in JOSM or Vespucci. The links to the current downloads are listed below.

<!-- preset-start -->

# 🔽 Preset Downloads

## street_lamps
- [Vespucci](https://github.com/steglitz/josm_presets/raw/gh-pages/gen/street_lamps-1.0.0.zip)
- [JOSM](https://github.com/steglitz/josm_presets/raw/gh-pages/gen/street_lamps-josm-1.0.0.zip)

## single_trees
- [Vespucci](https://github.com/steglitz/josm_presets/raw/gh-pages/gen/single_trees-0.1.0.zip)
- [JOSM](https://github.com/steglitz/josm_presets/raw/gh-pages/gen/single_trees-josm-0.1.0.zip)


<!-- preset-end -->
# Using this repository
To use this repository, you need to install and add the following to your PATH:
 - Gradle
 - Xmlstarlet
 - rsvg-convert

Once you've done that, you can clone the repository and add your information to the gradle.properties-template file 
and rename it to gradle.properties. From there you can build the project by running `./gradlew build`.

## Configuring Presets
To add a new preset, create a folder for your new preset inside the presets folder. Include any images or icons in 
folders. 
```
/project_root
  |-presets
      |-preset_name
          |-icons
          |-images
          |-preset.xml
```
Register your preset name in your gradle.properties file or gradle will not build your preset. Removing a preset 
from gradle.properties will cause gradle to ignore changes and not try to recompile your files.

**NOTE**: Do not put a space between presets and commas (i.e., presets=preset_1,preset_2,preset_3,etc.) 

# Adding Presets

## JOSM
Add presets in JOSM by selecting `Images > Preset Preferences` and then adding the raw link for each preset under 
"active presets."

## Vespucci
You can add presets in Vespucci by selecting `Settings > Presets > Add preset`. Give the preset a name
and add the RAW link. Activate the preset with the checkbox and start using it.
