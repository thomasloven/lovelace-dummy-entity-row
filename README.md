dummy-entity-row
================

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

An entity row that displays only an icon and the name of an entity. No controls.

# Installation instructions

For installation instructions [see this guide](https://github.com/thomasloven/hass-config/wiki/Lovelace-Plugins).

The recommended type of this plugin is: `module`.

```yaml
resources:
  url: /local/dummy-entity-row.js
  type: module
```

# Usage instructions

This is probably most useful as a header for [fold-entity-row](https://github.com/thomasloven/lovelace-fold-entity-row).

```
type: entities
entities:
  - type: custom:dummy-entity-row
    entity: light.bed_light
  - type: custom:dummy-entity-row
    entity: sun.sun
    icon: mdi:home-assistant
    name: Home Assistant
  - type: custom:dummy-entity-row
    entity: sun.sun
    icon: mdi:this-icon-does-not-exist
    name: No icon
  - type: custom:dummy-entity-row
    entity: sun.sun
    icon: mdi:home-assistant
    name: " "
```

![dummy-entity-row](https://user-images.githubusercontent.com/1299821/55743659-29a4aa00-5a33-11e9-81d7-4e094a372350.png)


---
<a href="https://www.buymeacoffee.com/uqD6KHCdJ" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
