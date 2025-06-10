[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs) 
[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
# Custom brand icons
Custom brand icons for Home Assistant

![logo](https://res.cloudinary.com/dcongin7u/image/upload/v1707320837/cbi-logo.jpg)

# Install

 1. Add the following to the `frontend` section of your `configuration.yaml`

  ```yaml
frontend:
  extra_module_url:
    - /local/community/custom-brand-icons/custom-brand-icons.js
```
2. (optional) Or add the following to your lovelace configuration using the Raw Config editor under Configure UI or ui-lovelace.yaml if using YAML mode.

```yaml
resources:
  - type: js
    url:  /local/community/custom-brand-icons/custom-brand-icons.js
```

# Use
you can use icons by entering the prefix `bef:`

Example of integration in the card

```yaml
entities:
  - entity: light.lampada_entrance
    icon: 'bef:go'
    name: Go
  - entity: light.monitor_2_right
    icon: 'bef:play'
    name: play 1
  - entity: light.monitor_2_left
    icon: 'bef:play'
    name: play 2
show_header_toggle: false
title: Custom brand icons
type: entities
```

A system restart is required after this step

# Icons/Brands Available
See the full list on [Github](https://github.com/elax46/custom-brand-icons#iconsbrands-available).
