HAP-NodeJS - Weaved Edition
=============
***FYIs:*** **Weaved SmartPlug must be configured to have a static IP of 10.0.1.12!**  *Server also does not start at boot, command must be run at boot. To auto-start at boot on Raspberry Pi, follow this tutorial: https://youtu.be/j6NfB1omsrQ*

HAP-NodeJS is a Node.js implementation of HomeKit Accessory Server.

With this project, you can convert the Weaved SmartPlug to be compatible with iOS HomeKit, giving it the ability to be controlled by Siri. 

The implementation may not 100% follow the HAP MFi Specification since MFi program doesn't allow individual developer to join. 

Remember to run `npm install` before actually running the server.

You can use the following command to start the HAP Server:
  ```js
  sudo forever start Core.js
  ```
After starting the server, pair the Outlet with your iPhone via the Insteon+ app on the App Store: https://appsto.re/us/-oVY2.i 

***Installation Instructions are in the Wiki!***

Special thanks to [KhaosT](https://github.com/KhaosT), who created this server software, and  [Alex Skalozub](https://twitter.com/pieceofsummer), who reverse engineered the server side HAP. ~~You can find his research at [here](https://gist.github.com/pieceofsummer/13272bf76ac1d6b58a30).~~ (Sadly, on Nov 4, Apple sent the [DMCA](https://github.com/github/dmca/blob/master/2014-11-04-Apple.md) request to Github to remove the research.)

