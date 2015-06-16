# favicon-bug

This repository demonstrates that Chrome will download huge favicon files to the point that they crash Chrome and bring the computer to a halt - all in the background with no indication to the user that any form of download or networking is happening.

(no spinner)

As people have pointed [Firefox](http://i.imgur.com/3zkPKD7.png) and [Safari](https://i.imgur.com/B2LeRy4.png) does this too. Safari is also affected and will make the computer unresponsive and then crash (on my OSX 10.10).

This is what it looks like before crashing on my computer (currently testing on travel laptop with 4gb ram):

![](http://i.imgur.com/J16lwjF.png)


Inspired by a tweet by https://twitter.com/a_de_pasquale https://twitter.com/a_de_pasquale/status/608997818913665024

### Running it

 1. Install [io.js](http://www.iojs.org) (NodeJS works too)
 2. Run: `node exploit.js`
 3. Test your browser by visiting http://localhost:3000  (or if you have `process.env.PORT` set then that port)
      
### Running it for Apple Touch Icon

 1. Install [io.js](http://www.iojs.org) (NodeJS works too)
 2. Run: `node exploit-ios.js`
 3. Test on iOS by visiting http://localhost:3000 and tapping on the share icon (or if you have `process.env.PORT` set then that port)
