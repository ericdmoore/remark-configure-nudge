remark-configure-nudge
==================

the remark MD world is amazing...

If you dont understand webpack and you see a js file importing CSS files, or images etc... its a real headscratcher. 
For those on the side of enlightenmrnt, they understand it as extending the inherent language syntax to now support other entities that your project might have real depndencies on.


Right, makes a TON of sense... if you understand webpack. The same would be true of the unifiedjs/remark systems,

This projet aimes to leave a polite little comment at the beginning of the MD file stating that this file really only makes sense to be parsed with remark and configured in a given way.

The beauty of making up your own rule, is that "the game" fits your situation. The problem is that it is not transferable in source form. only output form.

Based on your plugin chain this plugin might leave a comment/note at the beginning or in the front matter.

 ```text
 <!--
 * This is a comment automatically generatedd based on the plugins used to process this file.
 * Since markdown does not have proper fallback support on how to handle various cases, 
 * this comment aims to document the requirements for rendering this MD as intended.
 * 
 * The Author might even add some text here in the premable, 
 * all occurring before the {{ MDConfig }} delimiter.
 * 
 *
 * {{ MDConfig }}
 * preprocessor:
 *   engine:
 *    name: @unified/Remark
 *    npm: remarkjs
 *    link: https://npm.im/remarkjs
 *   config:
 *    name: @federa/remarkPreset2020
 *    npm: [ '@federa/remarkPreset2020' ]
 *    link: http://npm.im/@feder/remarkpreset2020
 -->
```

