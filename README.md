---
layout: default
title: README
---
# Getting Started with the Linden Scripting Language
## Introduction
This is an introduction to the [Linden Scripting Language](http://wiki.secondlife.com/wiki/A_Basic_LSL_Tutorial) and how to use it on [Second Life](https://secondlife.com/). Second Life is a massive multiplayer online game that allows users to program elements of the game while in game! This allows users to create objects or scripts and then sell them on the [Second Life Marketplace](https://marketplace.secondlife.com/) for in-game currency called Linden Dollars (L$). Those Linden dollars can be exchanged for US Dollars (USD) and thus be a great way to both practice programming skills and make some money! This introduction assumes that you have minimal programming experience, with at least some knowledge about the keywords: *constants*, *events*, *flow control (i.e. if, while, return statements)*, *functions (also called methods)*, *operators*, *states*, *types*, *variables*, and *errors*.

## Materials Needed
To start scripting on Second Life you will need a Viewer and an account on Second Life, that's it! A Viewer is the application that allows you to play the game, there are two popular choices with links to the download listed under the Viewer section. You can optinally download a text editor to write in the Linden Scripting Language while offline.

- [Second Life Account](https://join.secondlife.com/)
- [Viewer](#viewers)
- [Text editor (optional)](#recommended-text-editors)
- [Linden Scripting Language Documentation](http://wiki.secondlife.com/wiki/LSL_Portal)

Download either Viewer (I recommend Firestorm) and then make an account to get started.

## Start Coding In Second Life
Every script in Second Life works with or on created objects. You can make a script that can be placed inside many different kinds of objects, or tailor your object to work for your script specifically. Before beginning to script it is necessary to travel to a place that allows you to start scripting. Since you start in a tutorial, you will need to try it out until you can move around and work the third-person camera. Then travel to a place that allows you to make scripts. Since scripts can be malicious to other users in extreme cases and can take up a lot of the memory used by the simulation, they are often relegated to places that will contain the script functionality to prevent server issues. One of the most popular places to do this is the [Happy Hippo Building School (G Rated)](http://maps.secondlife.com/secondlife/Pandorus/96/129/30)

After arriving and finding a good place to start working, create an object. In my case, I made a cube. Every object should contain the following code example, but you should also try out setting up the [other examples](#examples-of-my-code) provided in this tutorial.


## Code Example
The best beginner coding examples can be found on the [Linden Scripting Language Wiki (LSL Wiki)](http://wiki.secondlife.com/wiki/A_Basic_LSL_Tutorial). This wiki is the definitive source for all of the Linden Scripting Language, and should be referenced as your comprehensive resource after this tutorial. 

The following code is one of the most basic examples of a script from the LSL Wiki.

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


## Installation instructions

### A Viewer is required to log in to SecondLife, choose either of these Viewers to get started with programming!

#### Viewers
- [Firestorm Viewer](https://www.firestormviewer.org/os/)
- [SecondLife Viewer](https://secondlife.com/support/downloads/)

Return to [Description of Materials](#description-of-materials)

### A text editor is helpful for scripting outside of SecondLife

#### Recommended Text Editors

- [LSLEditor](https://sourceforge.net/projects/lsleditor/)

- [Notepad++ LSL keyword import](https://pastebin.com/maYqDNxT)

## Examples of my Code

[Basic payment script](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/code-examples/allowPayment)
This script will allow you to store an object within another object, then when another user clicks the ```Pay``` action, they will send you money to receive the item. Like a vending machine that never runs out of stock, but only carries one item!

[Basic Head up display](https://github.com/t9605tripp/linden-scripting-tutorial/blob/main/code-examples/basicHUD)
This script uses three different objects to display a button that when clicked will make another button to send a message.

## FAQs

- **Q:** *Does it matter where I go to test scripts?*
- **A:** The only differences will be the ratings approved for the sim. There are three different content levels called general, mature, and adult which changes what you are allowed to see and show while in that place. Otherwise, there are no differences between where you pick to start scripting.

- **Q:** *How do I get to a place where I can start scripting?*
- **A:** You need to search for Happy Hippo Building School and teleport there to start building your first object and script.

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

