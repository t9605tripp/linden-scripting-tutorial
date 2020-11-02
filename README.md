---
layout: default
title: README
---
# Getting Started with the Linden Scripting Language
## Introduction
This is an introduction to the [Linden Scripting Language](http://wiki.secondlife.com/wiki/A_Basic_LSL_Tutorial) and how to use it on [Second Life](https://secondlife.com/). Second Life is a massive multiplayer online game that allows users to program elements of the game while in game! This allows users to create objects or scripts and then sell them on the [Second Life Marketplace](https://marketplace.secondlife.com/) for in-game currency called Linden Dollars (L$). Those Linden dollars can be exchanged for US Dollars (USD) and thus be a great way to both practice programming skills and make some money! This introduction assumes that you have minimal programming experience, with at least some knowledge about the keywords: *constants*, *events*, *flow control (i.e. if, while, return statements)*, *functions (also called methods)*, *operators*, *states*, *types*, *variables*, and *errors*.

## Before Coding Instructions
To start scripting on Second Life you will need a Viewer and an account on Second Life, that's it! A Viewer is the application that allows you to play the game, there are two popular choices with links to the download listed under the Viewer section. You can optinally download a text editor to write in the Linden Scripting Language while offline.

1. First, follow this link to create a [Second Life Account](https://join.secondlife.com/)
1. Next, follow this link and choose the recommended [Viewer](#viewers)
1. Finally, Log in to the Viewer using your new SecondLife account information

### Firestorm Viewer Login Screen
![Login Page](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/images/login_screen.png)

[//]: # (../images/login_screen.png)

## Start Coding In Second Life
Before beginning to script it is necessary to travel to a place that allows you to start scripting. Since scripts can be malicious to other users in extreme cases and can take up a lot of the memory used by the simulation, they are often relegated to places that will contain the script functionality to prevent server issues. A good place to start is the [Happy Hippo Building School (G Rated)](http://maps.secondlife.com/secondlife/Pandorus/96/129/30). Follow these instructions to get there.

- In the top right corner of the window, type in "happy hippo" and hit enter.
- Find the same result as the one in the image then click the Teleport button to go there.

![Travelling](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/images/inked_travel.jpg)

[//]: # (../images/inked_travel.jpg)

- After arriving, walk into the grassy area then click on the Build Button located at the top left of the screen, then select Build from the dropdown.

![Building](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/images/build.png)

[//]: # (../images/build.png)

- Now click anywhere on the ground to create an object, the default build setting will make a cube.

![Object Creation](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/images/object_creation.png)

[//]: # (../images/object_creation.png)

- Then click on the Content tab and select New Script to create a script that is held within the object. 

![New Script](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/images/new_script.png)

[//]: # (../images/new_script.png)

- Continue to the next section to see what the contents of the New Script mean


## Code Example and Breakdown
Every script in Second Life works with or on objects. You can make a script that can be placed inside many different kinds of objects, or tailor your object to work for your script specifically. The New Script that you just created is one of the most basic examples that is default of all new scripts.

```
default
{
    state_entry()
    {
        llSay(0, "Hello, Avatar!");
    }
 
    touch_start(integer total_number)
    {
        llSay(0, "Touched.");
    }
}
``` 

The first keyword ```default``` is a ***state***. To start, you only need to use the ```default``` state which makes the script run whenever the associated object is interacted with by an ***event***. In this example, there are two events. The first, ```state_entry()``` is run when the object enters the ```default``` state. This means that it will run when the script is saved after editing, or is entered by another method changing the script state to default. Throughout this tutorial only the default state will be used. Inside the ```state_entry``` event, there is a ***function*** called ```llSay(integer channel, string message)``` which takes an integer that represents where the message should be sent, and a string containing the message to send.
The next ***event*** is ```touch_start(integer num_detected)``` which runs when the object that the script is in is first touched. Whenever it is touched then it will run the ```llSay()``` function.


## Examples of my Code

To get more in-depth, you should also try out setting up the other examples provided in this tutorial.

[Basic payment script](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/code-examples/allowPayment)
This script will allow you to store an object within another object, then when another user clicks the ```Pay``` action, they will send you money to receive the item. Like a vending machine that never runs out of stock, but only carries one item!

[Basic Head up display](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/code-examples/basicHUD)
This script uses three different objects to display a button that when clicked will make another button to send a message.

## Installation Links

A viewer is required to log in to SecondLife. Choose one of the Viewers to install then follow the website instructions for installation.

#### Viewers
- [Firestorm Viewer](https://www.firestormviewer.org/os/) ***(Recommended)*** 
- [SecondLife Viewer](https://secondlife.com/support/downloads/)

After downloading, you should return to [Before Coding Instructions](#before-coding-instructions)

#### Text Editors

A text editor is optional, this tutorial will not use one, but you may find it helpful if you practice coding after this tutorial.

- [LSLEditor](https://sourceforge.net/projects/lsleditor/)
- [Notepad++ LSL keyword import](https://pastebin.com/maYqDNxT)

## FAQs

**Q:** ***Are there more code examples that I can look at?***

**A:** The best beginner coding examples can be found on the [Linden Scripting Language Wiki (LSL Wiki)](http://wiki.secondlife.com/wiki/A_Basic_LSL_Tutorial). This wiki is the definitive source for all of the Linden Scripting Language, and should be referenced as your comprehensive resource after this tutorial. 

**Q:** ***Does it matter where I go to test scripts?***

**A:** The only differences will be the ratings approved for the sim. There are three different content levels called general, mature, and adult which changes what you are allowed to see and show while in that place. Otherwise, there are no differences between where you pick to start scripting.

**Q:** ***How do I get to a place where I can start scripting?***

**A:** You need to search for Happy Hippo Building School and teleport there to start building your first object and script.

## Troubleshooting

Most issues will be related to installation, so view the provided guides on installation or account creation provided by the website that was linked for more help with those problems.

If there is a problem with your script not running, then it is likely related to the place you are inside because not all places allow scripts to be run by anyone.

If you don't place an object into the world from your inventory or create a new object, then you cannot run it's scripts.

## How to Contribute

Offer some changes on this [GitHub.](https://github.com/t9605tripp/linden-scripting-tutorial)

## Licensing

[MIT License](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/LICENSE)

## Instructions for Use

Hopefully you can use the skills gained from this documentation to start selling scripts on [Second Life!](https://secondlife.com/)

