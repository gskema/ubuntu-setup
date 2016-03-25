![Ubuntu](http://i.imgur.com/YcPevAu.jpg)
![Linux](http://i.imgur.com/y7tCjqG.jpg)

# Ubuntu Web Developer Setup

My ubuntu setup guide, configuration snippets and scripts.

## Commands

### Update everything macro

Update package list, upgrades them and removes all unnecessary pacakges

``` bash
sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get -y dist-upgrade && sudo apt-get -y autoremove && sudo apt-get autoclean
```

### Import MySQL database dump using command line

``` bash
mysql -u username -p database_name < file.sql
```

### Ignore file permission changes in git root

``` bash
git config core.fileMode false
```

## GNOME

- [GNOME Shell Extensions](https://extensions.gnome.org/)

## Browser

- [Chrome](http://www.ubuntuupdates.org/ppa/google_chrome?dist=stable)
- [Fix ‘Failed To Fetch’ Apt Error on Ubuntu](http://www.omgubuntu.co.uk/2016/03/fix-failed-to-fetch-google-chrome-apt-error-ubuntu)

## Themes, Icons

- [Arc Theme](https://github.com/horst3180/Arc-theme)
- [Vertex Theme](https://github.com/horst3180/vertex-theme)
- [Ambiance & Radiance Flat](http://www.ravefinity.com/p/download-ambiance-radiance-flat-colors.html)

### Numix Theme

``` bash
sudo add-apt-repository ppa:numix/ppa
sudo apt-get update
sudo apt-get install numix-*
```

- [Numix Hardcoded Icon Fixer](https://github.com/Foggalong/hardcode-fixer)


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

### Brackets

``` bash
sudo add-apt-repository -y ppa:webupd8team/brackets
sudo apt-get update
sudo apt-get install brackets
```

### PhpStorm

- [PhpStorm Download Page](https://www.jetbrains.com/phpstorm/)

#### PhpStorm Plugins

- [Php Inspections (EA Extended)](https://plugins.jetbrains.com/plugin/7622?pr=idea)
- [GitHub markdown](https://plugins.jetbrains.com/search/index?pr=idea&search=Gfm)
- [Apache config (.htaccess) support](https://plugins.jetbrains.com/plugin/6834?pr=idea)
- [EditorConfig](https://plugins.jetbrains.com/plugin/7294?pr=idea)
- [.ignore](https://plugins.jetbrains.com/plugin/7495?pr=idea)

## Developer Tools

### Composer

- [Composer Download Page](https://getcomposer.org/download/)
- [Composer Global Installation](https://getcomposer.org/doc/00-intro.md#globally)

### Node.js & npm

``` bash
sudo apt-get install git nodejs
sudo ln -s /usr/bin/nodejs /usr/bin/node
sudo apt-get install npm
sudo npm install npm -g
```
