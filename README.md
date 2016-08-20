![Ubuntu](http://i.imgur.com/YcPevAu.jpg)
![Linux](http://i.imgur.com/y7tCjqG.jpg)

# Ubuntu Web Developer Setup

My ubuntu setup guide, configuration snippets and scripts.

## Commands

### Update everything macro

Update package list, upgrades them and removes all unnecessary pacakges

``` bash
sudo apt update && sudo apt -y upgrade && sudo apt -y autoremove && sudo apt autoclean && sudo apt -y dist-upgrade 
```

### Import MySQL database dump using command line

``` bash
mysql -u username -p database_name < file.sql
```

### Ignore file permission changes in git root

``` bash
git config core.fileMode false
```

### Optimize Composer autoload

``` bash
composer dump-autoload -o
```

## System

- [GNOME Shell Extensions](https://extensions.gnome.org/)
- [Redshift](https://github.com/jonls/redshift)
- [Redshift geoclue2 Fix](https://github.com/jonls/redshift/issues/158)
- [Variety Wallpapers](http://peterlevi.com/variety/how-to-install/)
- [TopIcons for GNOME](https://extensions.gnome.org/extension/1031/topicons/)

``` bash
sudo apt install ubuntu-restricted-extras
```

## Terminal, Shell

- [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh)
- [GNOME Solarized](https://github.com/Anthony25/gnome-terminal-colors-solarized)

## Browser

- [Chrome](http://www.ubuntuupdates.org/ppa/google_chrome?dist=stable)
- [Fix ‘Failed To Fetch’ Apt Error on Ubuntu](http://www.omgubuntu.co.uk/2016/03/fix-failed-to-fetch-google-chrome-apt-error-ubuntu)
- [Fix source file for Chrome](http://askubuntu.com/questions/741410/skipping-acquire-of-configured-file-main-binary-i386-packages-as-repository-x)

## Themes, Icons

- [Arc Theme](https://github.com/horst3180/Arc-theme)
- [Vertex Theme](https://github.com/horst3180/vertex-theme)
- [Ambiance & Radiance Flat](http://www.ravefinity.com/p/download-ambiance-radiance-flat-colors.html)

### Numix Theme

``` bash
sudo add-apt-repository ppa:numix/ppa
sudo apt update
sudo apt install numix-*
```

- [Numix Hardcoded Icon Fixer](https://github.com/Foggalong/hardcode-fixer)


## Fonts

``` bash
sudo apt install msttcorefonts ttf-mscorefonts-installer
sudo apt install fonts-cantarell fonts-droid fonts-roboto fonts-noto
```
- [Hack Font](http://sourcefoundry.org/hack/)
- [Source Code Pro](http://askubuntu.com/questions/193072/how-to-use-the-new-adobe-source-code-pro-font)
- [Google Fonts](https://www.google.com/fonts)
- [Fira](https://github.com/mozilla/Fira)
- [Fira Code](https://github.com/tonsky/FiraCode)
 
``` bash
mv *.ttf ~/.fonts
sudo fc-cache -f
```

## Editors

### Atom

``` bash
sudo add-apt-repository -y ppa:webupd8team/atom
sudo apt update
sudo apt install atom
```

### Brackets

``` bash
sudo add-apt-repository -y ppa:webupd8team/brackets
sudo apt update
sudo apt install brackets
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

### [Webmin](http://www.webmin.com/)

### Composer

- [Composer Download Page](https://getcomposer.org/download/)
- [Composer Global Installation](https://getcomposer.org/doc/00-intro.md#globally)

### Node.js & npm

``` bash
sudo apt install git nodejs
sudo ln -s /usr/bin/nodejs /usr/bin/node
sudo apt install npm
sudo npm install npm -g
```

### Compass

- [Compass](http://compass-style.org/install)

### PHP CodeSniffer

- [CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer)

### Vagrant

``` bash
sudo apt install vagrant virtualbox
```
