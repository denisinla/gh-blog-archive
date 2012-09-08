---
layout: post
title: MacVim Configuration
tags: macvim - mvim - osx
---

So brew makes life so much easier when installing packages locally(So long MacPorts, I despise you !). So In a perfect world a ``$ brew install package-name`` should get you up and running with said package-name. But I'm not going to go into details about brew, instead I'll be talking about macvim and configuring it to a tasteful degree(perhaps maybe half assed ? ... je ne sais pas) and integrate mvim into your terminal. o.O

After trying to install macvim via brew I kept on getting build errors(and I wasn't the only one either - theres a ticket for it as well). So I opted to install the traditional way; Grabbing a snapshop from [GitHub](https://github.com/b4winckler/macvim/downloads). So here is my small experience installing the non-conventional, simple, stupid effing easy way ... what ever.

**Installation**

Downloaded MacVim via [GitHub](https://github.com/b4winckler/macvim/downloads).  
Installed the traditional way(moved **MacVim** app and **mvim** into _/Applications_)     
You should now have both the **MacVim** app and **mvim** placed inside of _/Applications_.

**PATH Configuration** 
 
Since my shell of choice is **zsh** my $PATH configuration happens in **~/.zshrc**.  
Typed the following: ``$ export PATH=/Applications:$PATH``   
_this added **/Applications** directory where **mvim** resides into my PATH._


**Launch mvim from terminal**  
CD into your directory of choice and initiate mvim by typing ``mvim .``


