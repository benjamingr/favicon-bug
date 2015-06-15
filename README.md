# favicon-bug

This repository demonstrates that Chrome will download huge favicon files to the point that they crash Chrome and bring the computer to a halt - all in the background with no indication to the user that any form of download or networking is happening.

(no spinner)

As people have pointed Firefox [does this too](http://i.imgur.com/3zkPKD7.png). Safari is also affected and will make the computer unresponsive and then crash (on my OSX 10.10).

[Chrome bug 500639](https://code.google.com/p/chromium/issues/detail?id=500639) [Firefox bug 1174811](https://bugzilla.mozilla.org/show_bug.cgi?id=1174811)

This is what it looks like before crashing on my computer (currently testing on travel laptop with 4gb ram):

![](http://i.imgur.com/J16lwjF.png)


Inspired by a tweet by https://twitter.com/a_de_pasquale https://twitter.com/a_de_pasquale/status/608997818913665024

### Running it

 1. Install [io.js](http://www.iojs.org) (NodeJS works too)
 2. Run: `node exploit.js`
 3. Test your browser by visiting http://localhost:3000  (or if you have `process.env.PORT` set then that port)
            
    
