# Bambu-HomeAssistant-Flows
A (WIP) collection of HomeAssistant Dashboards and NodeRed Flows with a configurator to connect a BambuLabs printer to HomeAssistant through MQTT - based off of my Gists

The main guides that are option #1 for configuring the flows, with more helpful descriptions: https://www.wolfwithsword.com/tag/bambu-lab-guides/ 

The gist links for historical context: [Most flows](https://gist.github.com/WolfwithSword/e3e4dc4f00629cc047b7cefd70d7b350), [Dashboards & Media](https://gist.github.com/WolfwithSword/4175a46c872f69542376206bab4ccfc3), [My hardware accessory controller](https://gist.github.com/WolfwithSword/a9f2421cf90b2d67b0abfd3a94039156), [The advanced version of the bedmesh flow](https://gist.github.com/WolfwithSword/45dd17ba5250cee94136759e9923e2bb)

## What is this?
Since late 2022 I had been (with thanks to several communities) creating a set of NodeRed flows to integrate the Bambulabs printers into HomeAssistant. This includes my basic flows, my advanced FTPS and DB flows, Grafana dashboards, HomeAssistant dashboard yamls, Bed mesh level tracking/visualization and more.

Since they were previously all in gists and then configured on my website, for others to better create issues for it I have moved it all to this repository. Additionally, I will be creating a very basic githubs pages for it here which will duplicate my configurator functionality from my website, should a solar flare or rogue gamma particle ever permanently take down my website.

### Organization
This repository will be organized accordingly and treated almost entirely as just a "file storage" for the most up to date version of the files. The configurator on my website and in the soon-to-be-made github pages here will pull from the latest versions committed to *main* repository.

Going forward, I will likely look into tagging major version changes (not as github releases) and have the github pages configurator let you choose which to pull from, with latest main being default. I offer no guarantee of this, just that it's an idea I'm considering, as many of the updates *require* to always be the latest should firmware updates change details or other fixes.

Organization will be as follows:

- files/
  - nodered/
    - each nodered flow json file
  - grafana/
    - each grafana dashboard json file 
  - media/
    - all images, svg's and such that require being copied for use in my integrations 
  - homeassistant/
    - each yaml file for dashboards in homeassistant
    - a folder for blueprint automations/scripts
  - misc/ (misc files that don't really do well being separated)
    - hardware/
      - e.g., my bentobox and light controller

All files in nodered and homeassistant folders will be templated and require configuring. Each folder will have a brief readme and link to the guide and configurator(s).
