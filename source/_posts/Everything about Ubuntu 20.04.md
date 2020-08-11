---
title: Everything about Ubuntu 20.04
tags: ["Education", "Linux"] 
categories: ["Linux"]
---

# Some good software to have


## Email
<ins>__Thunderbird Mail__</ins>  
This is where you send emails. For Ubuntu 20.04, it is installed automatically. You just need to log in with your credentials. 

## Keyboard
<ins>__Google Pinyin__</ins>  
I am using Chinese to write some things so wanted to download one. This can be done by the following steps in terminal.

`sudo apt install fcitx-bin`

`sudo apt install fcitx-googlepinyin`

*In region and language, choose fcitx instead of ibus.*

`fcitx-configtool`

*Add Google Pinyin from the list.*

Now you are set! You can see all uninstalled keyboards at the top right corner. Press `ctrl+space` to switch keyboard!


## Screen Recorder
<ins>__Kazam__</ins>  
This is a screen recorder with screenshot functions. You can record the whole screen and partial screen.

`sudo apt-get update`

`sudo apt install kazam`  

Now you will be able to see it in "Show Applications".

## Screenshot
<ins>__Flameshot__</ins>   
I use it as a Linux substitute for Windows Snipping Tool. You can also edit the screenshots.

`sudo apt install flameshot`

## Gamers
<ins>__Steam__</ins>  
Most PC games can be found here. You can download it from the Steam website. [Click here.](https://store.steampowered.com/about/) After you download, click on the downloaded file. Click install. Then you are good to go.

<ins>__Winetricks__</ins>  
Winetricks is a helper script to download and install various redistributable runtime libraries needed to run some programs in Wine.  

__What is Wine?__  
Wine is a free and open-source compatibility layer that aims to allow software developed for Microsoft Windows to run on Unix-like operating systems. Wine also provides a software library, known as Winelib, against which developers can compile Windows applications to help port them to Unix-like systems.

<ins>__Lutris__</ins>    
Open source gaming platform. Refer to its website for specific information. [Click here.](https://lutris.net/) 
 
## Text Editor
<ins>__Texmaker__</ins>  
This is a free text editor. [Click here to download the file](https://www.xm1math.net/texmaker/download.html).  

<ins>__Sublime__</ins> 
This is a paid text editor.  

1. Install the GPG key:

`wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -`  

2. Ensure apt is set up to work with https sources:  
`sudo apt-get install apt-transport-https`   

3. Select the channel to use:  

Stable (I selected this)  
`echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list`  
Dev  
`echo "deb https://download.sublimetext.com/ apt/dev/" | sudo tee /etc/apt/sources.list.d/sublime-text.list`  

4. Update apt sources and install Sublime Text   

`sudo apt-get update`   

`sudo apt-get install sublime-text`  

## Communications
<ins>__Slack__</ins>  
Commuincating software used for work.
Download from [here](https://slack.com/intl/en-ca/downloads/linux). Click the file to install. 

<ins>__Discord__</ins>  
Chatting and streaming software. 
Download from [here](https://discord.com/). Click the file to install. 

## System Optimizers/Task Managers
<ins>__Stacer__</ins>  
This is like a Linux version of task manager with a beautiful interface. You can view CPU usage, memory usage and disk usage. You can also terminate some unwanted programs.
You can install by typing this in the terminal: 

`sudo apt install stacer`


## IDEs
<ins>__Visual Studio Code__</ins>  
The IDE for web developers.
Download it from the official website and click the deb file to install.

<ins>__PyCharm__</ins>  
This is a Python IDE by JetBrains. Before you install this, you need to get the latest version of Python as well. This should be automatically installed in your Ubuntu. Check by typing `python3 -V`. Some output should be like `Python 3.8.2`.

Now, install PyCharm by typing the following in the terminal:

`sudo snap install [pycharm-professional|pycharm-community] --classic`


<ins>__Eclipse__</ins>
I use it as Java IDE. Install by typing the following:

`sudo apt install default-jre`

`sudo snap install --classic eclipse`

## Hacking
<ins>__Ettercap__</ins>  
It is a tool for Man in the Middle Attacks. Used for APR poisoning.

`sudo apt-get update -y`   

`sudo apt-get install -y ettercap-graphical`   

--- 
v.1 2020.8  

