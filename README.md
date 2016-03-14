# Ubuntu Setup

My ubuntu setup guide, configuration snippets and scripts.

## Update everything macro

Update package list, upgrades them and removes all unnecessary pacakges

``` bash
sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get -y dist-upgrade && sudo apt-get -y autoremove && sudo apt-get autoclean
```

## Fonts

``` bash
sudo apt-get install msttcorefonts ttf-mscorefonts-installer
sudo apt-get install fonts-cantarell fonts-droid fonts-roboto fonts-noto
```
- [Hack Font](http://sourcefoundry.org/hack/)
- [Source Code Pro](http://askubuntu.com/questions/193072/how-to-use-the-new-adobe-source-code-pro-font)

## Editors

### Atom

``` bash
sudo add-apt-repository -y ppa:webupd8team/atom
sudo apt-get update
sudo apt-get install atom
```
