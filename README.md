[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg) ](https://github.com/custom-components/hacs)![Validate with hassfest](https://github.com/jinglyjangles/home-assistant-robart/workflows/Validate%20with%20hassfest/badge.svg?branch=master) ![Validate with HACS](https://github.com/jinglyjangles/home-assistant-robart/workflows/Validate%20with%20HACS/badge.svg)

# home-assistant-robart
Home Assistant integration of RobartAI run robot vacuums. 
Thanks to @eworme for the original code

Tested on:
- Hoover Rogue 970
- Robart MyVacBot

# Install
- Add custom repository to HACS, install Robart

- Add **vacuum** section to **configuration.yaml**

```
  vacuum:                                                                                                                                      
    - platform: robart                                                                                                                         
      host: <ip address>
```
  
# To Do:
- See https://github.com/jinglyjangles/hoover_970_integration for additonal api calls available
- Add importing the custom robot name; current on the 970's it defualts to Josephine unless you call the name endpoint
- Add support for only cleaning certain rooms; see maps endpoint 
- Add support for live/static room map; maps endpoint provides x,y coords and rooms
- Add support for no-go zones and cleaning intensity; see cleaning power in misc_notes
