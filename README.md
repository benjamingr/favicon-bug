# favicon-bug

This repository demonstrates that browsers will download huge favicon and touch-icon files to the point that they crash and/or bring the computer to a halt - all in the background with no indication to the user that any form of download or networking is happening.

(no spinner)

I originally tested this with Chrome. People have pointed [Firefox](http://i.imgur.com/3zkPKD7.png) and [Safari](https://i.imgur.com/B2LeRy4.png) do this too, [IE](https://github.com/benjamingr/favicon-bug/issues/5)  does not appear to be affected.

[Chrome bug 500639](https://code.google.com/p/chromium/issues/detail?id=500639) [Firefox bug 1174811](https://bugzilla.mozilla.org/show_bug.cgi?id=1174811)

This is what it looks like before crashing on my computer (currently testing on travel laptop with 4gb ram):

![](http://i.imgur.com/J16lwjF.png)


Inspired by [a tweet](https://twitter.com/a_de_pasquale/status/608997818913665024) by [a_de_pasquale](https://twitter.com/a_de_pasquale).

### Running it

 1. Install [io.js](http://www.iojs.org) (NodeJS works too)
 2. Run: `node exploit.js`
 3. Test your browser by visiting http://localhost:3000  (or if you have `process.env.PORT` set then that port)
      
### Running it for Apple Touch Icon

 1. Install [io.js](http://www.iojs.org) (NodeJS works too)
 2. Run: `node exploit-ios.js`
 3. Test on iOS by visiting http://ip-of-computer:3000 and tapping on the share icon (or if you have `process.env.PORT` set then that port)
