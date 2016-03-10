# Ubuntu Setup

My ubuntu setup guide, configuration snippets and scripts.

## Update everything macro

Update package list, upgrades them and removes all unnecessary pacakges

``` bash
sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get -y dist-upgrade && sudo apt-get -y autoremove && sudo apt-get autoclean
```

