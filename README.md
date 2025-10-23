# ZMK Module for AKDK 

To include this module in your ZMK project, add the following entries.

## west.yaml

```yaml
manifest:
  remotes:
    - name: zmkfirmware
      url-base: https://github.com/zmkfirmware
    - name: skubmdi
      url-base: https://github.com/skubmdi
  projects:
    - name: zmk-component-akdk-nrf52840
      remote: skubmdi
```

## build.yaml

Please adjust the shield name to match your own keyboard.

```yaml
include:
  - board: akdk_nrf52840
    shield: akdk
```
