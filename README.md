Simple-Script
=============

This is a sample game for the [HappyFunTimes party games system](http://greggman.github.io/HappyFunTimes).
It's a clone of the [Simple Example](http://github.com/greggman/hft-simple). The only difference is
this one uses a standard `<script>` tag to get the HappyFunTimes libraries.

Most HappyFunTimes examples use [require.js](http://requirejs.org) style to include JavaScript files.
I really prefer that method as it's much cleaner and lets each module include its own dependencices.
In contrast the traditional `<script>` tag method requires you, the programmer, know all the dependencies
of all your modules are manaully add `<script>` tags to your HTML

Anyway, this sample uses `<script>` tags. The `<script>` tags for HappyFunTimes are automatically
added for you and so is the script tag that includes `scripts/game.js` for your game and
`scripts/controller.js` for your controller. If you need any other scripts, say for
[three.js](http://threejs.org) or [pixi.js](http://www.pixijs.com) add script tags to
either `game.html` or `controller.html`.  The HappyFunTimes libraries will be inserted before
those tags. The `game.js` or `controller.js` will be inserted after.

The important things to note if you'd like to use this style.

*   In your `package.json` the `apiVersion` must be set to `1.3.0` or higher.
*   You must add the setting `happyFunTimes.useScriptTag`. Example

        {
          ...
          "happyFunTimes": {
            ...
            "apiVersion": "1.3.0",
            "useScriptTag": true,
            ...
          }
        }

Cloning
-------

[If you want to clone this follow the instructions here](https://github.com/greggman/HappyFunTimes/blob/master/docs/makinggames.md)




