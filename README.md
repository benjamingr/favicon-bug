# favicon-bug

This repository demonstrates that Chrome will download huge favicon files to the point that they crash Chrome and bring the computer to a halt - all in the background with no indication to the user that any form of download or networking is happening.

(no spinner)

As people have pointed Firefox [does this too](http://i.imgur.com/3zkPKD7.png).

This is what it looks like before crashing on my computer (currently testing on travel laptop with 4gb ram):

![](http://i.imgur.com/J16lwjF.png)


Inspired by a tweet by https://twitter.com/a_de_pasquale https://twitter.com/a_de_pasquale/status/608997818913665024

###Running it

Install [io.js](http://www.iojs.org) (NodeJS works too)
Run:
    node exploit.js
    
    
